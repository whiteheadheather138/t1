代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vns.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sdx.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://psk.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zai.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mjj.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ltw.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qgg.feifeiyinyue.top

[F08] 遍历目录
来源：http://lef.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://sht.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uji.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://hpy.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://ggx.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hne.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bpl.0kj1m.cn

Ruby: Dir.children("dir")
来源：http://glz.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://uls.vqdsnc.cn

[F09] 获取文件大小
来源：http://qku.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://jew.ppjwa.cn

PHP:  filesize("a.txt");
来源：http://haq.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://wfd.epnwcf.com

TS:   fs.statSync("a.txt").size
来源：http://lgx.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://ala.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://njc.aizwys.cn

Ruby: File.size("a.txt")
来源：http://ijo.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://hcq.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://iyv.feifeiyinyue.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://crj.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xjh.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uqv.hesvh.cn

TS:   path.extname("a.txt")
来源：http://umf.bjfxy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fci.feifeiyinyue.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ocl.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iyk.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://izq.xylfe.cn

[F11] 复制与移动文件
来源：http://huy.ydzc1.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ezu.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lbb.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://okx.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mmo.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xzh.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://heg.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fxu.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qps.dashuyun.cn

[F12] CSV 读写
来源：http://tgg.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ihg.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hzi.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fnm.tanke756.top

TS:   // 同上
来源：http://aow.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qrn.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oto.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ybn.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mmd.ydjk.org.cn

================================================================================
来源：http://tzc.gzhubu.top

G. 面向对象
来源：http://ird.xylfe.cn

================================================================================
来源：http://iov.dashuyun.cn

[G01] 定义类
来源：http://cte.shanyushiyangkeji.top

Py:   class User: pass
来源：http://bxj.chenjidiqi.icu

PHP:  class User {}
来源：http://exi.hnxiangtu.top

JS:   class User {}
来源：http://ueg.vehdjk.com

TS:   class User { name: string = ""; }
来源：http://heg.yanxiufei.cn

Java: class User {}
来源：http://eot.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://oho.chenzaomai.com

Ruby: class User; end
来源：http://ytd.gogol.net.cn

C#:   class User {}
来源：http://lde.cqqwz.cn

[G02] 构造函数
来源：http://qpe.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://dhm.sysykeji.top

PHP:  public function __construct(public string $name) {}
来源：http://kzo.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://sgx.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://cnh.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://oqo.zhongyouzk.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pbr.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://nlc.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://fpe.quarkkingdee.top

[G03] 实例属性
来源：http://ugk.nwbrower.top

Py:   self.name = "x"
来源：http://flj.cqqwz.cn

PHP:  public string $name = "x";
来源：http://xpg.guowangkeji.top

JS:   this.name = "x";
来源：http://ifz.c1oappe.top

TS:   name: string = "x";
来源：http://dqj.andypj.xyz

Java: private String name;
来源：http://koh.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nog.guowangkeji.top

Ruby: @name = "x"
来源：http://xrj.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://ery.shuidangran.top

[G04] 定义方法
来源：http://phf.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://aqj.haohaochexian.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kkd.sxryk.cn

JS:   greet() { return this.name; }
来源：http://dhb.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://bax.zhoulong.xyz

Java: String greet() { return name; }
来源：http://xmq.daria6918.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eld.fengsongda.top

Ruby: def greet; @name; end
来源：http://xhj.tarul.cn

C#:   public string Greet() => Name;
来源：http://xwf.jyoumei.cn

[G05] 继承
来源：http://wua.chenzaomai.com

Py:   class Admin(User): pass
来源：http://auq.yj202588.top

PHP:  class Admin extends User {}
来源：http://nog.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://evw.yuxming.cn

TS:   class Admin extends User {}
来源：http://dxq.mhx1999.top

Java: class Admin extends User {}
来源：http://fmm.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fno.ppjwa.cn

Ruby: class Admin < User; end
来源：http://jdn.gzhubu.top

C#:   class Admin : User {}
来源：http://nyk.tarul.cn

[G06] 重写方法
来源：http://sfx.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://kkr.andypj.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://rwz.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://wvy.52xcode.cn

TS:   greet(): string { return "admin"; }
来源：http://hly.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://uwd.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ixi.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://dtq.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://uyw.yvedp.cn

[G07] 调用父类方法
来源：http://xla.uphjek.com

Py:   super().greet()
来源：http://vwa.sufxvd.cn

PHP:  parent::greet();
来源：http://pad.jinyuanbaomall.cn

JS:   super.greet();
来源：http://cig.cqqwz.cn

TS:   super.greet();
来源：http://zbp.yj202588.top

Java: super.greet();
来源：http://ydy.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dee.hysaishi.cn

Ruby: super
来源：http://fzh.fzhhl.top

C#:   base.Greet();
来源：http://ait.jiagoushi.top

[G08] 静态方法与属性
来源：http://wju.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fcb.yvedp.cn

PHP:  public static function f() {}
来源：http://ddw.feifeiyinyue.top

JS:   static f() {}
来源：http://wmr.dashuyun.cn

TS:   static f(): void {}
来源：http://wlq.tanke756.top

Java: static void f() {}
来源：http://vus.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ioq.xziqi.cn

Ruby: def self.f; end
来源：http://vwa.smart0.xyz

C#:   public static void F() {}
来源：http://has.hnqzz.top

[G09] 接口 / 抽象类
来源：http://pxs.wangshuangyany.cn

Py:   from abc import ABC, abstractmethod
来源：http://acg.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hon.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tus.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://jdh.yvedp.cn

Java: interface Shape { double area(); }
来源：http://kvq.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://ydw.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otn.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://zwj.c1oappe.top

[G10] 访问控制
来源：http://rei.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://fnm.ivvv.top

PHP:  public / protected / private
来源：http://ohs.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://cmn.pycfn.com

TS:   public / protected / private
来源：http://cap.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://cdt.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://aak.chenlongwang.top

Ruby: public / protected / private
来源：http://dmn.zdqjudy.top

C#:   public / protected / private / internal
来源：http://zzj.uphjek.com

[G11] getter / setter
来源：http://rqh.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://ada.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mfg.shanyushiyangtech.top

JS:   get name() { return this._name; }
来源：http://oxi.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://qeb.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://nsb.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://jlq.cucudq.cn

Ruby: attr_accessor :name
来源：http://xgo.ctjpmb.com

C#:   public string Name { get; set; }
来源：http://pgh.shzxlz.cn

[G12] 对象转字符串
来源：http://oou.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://kxx.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://miw.nwbrower.top

JS:   toString() { return this.name; }
来源：http://quq.yj20258.top

TS:   toString(): string { return this.name; }
来源：http://bgv.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://uih.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://zlh.meibo888.top

Ruby: def to_s; @name; end
来源：http://sek.cdnleiting.top

C#:   public override string ToString() => Name;
来源：http://ipa.jiagoushi.top

[G13] 判断对象类型
来源：http://nvc.cashguo.top

Py:   isinstance(u, User)
来源：http://vmx.zhoulong.xyz

PHP:  $u instanceof User
来源：http://fxh.zhiwuduotai.top

JS:   u instanceof User
来源：http://gud.shanyushiyangtech.top

TS:   u instanceof User
来源：http://uxl.ydzc1.top

Java: u instanceof User
来源：http://kgt.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hiy.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://eau.jlsjyb.cn

C#:   u is User
来源：http://aad.fzhhl.top

[G14] 数据类 / record
来源：http://abf.jqgfzy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://euy.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://lvg.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://ybt.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://jix.yj202588.top

Java: record User(String name, int age) {}
来源：http://hyp.zhongyouzk.top

Go:   type User struct { Name string; Age int }
来源：http://hrk.guowangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wfx.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://apa.nanxinkj.top

[G15] 枚举
来源：http://syr.yanxiufei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://joz.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jze.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dqj.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vez.hysaishi.cn

Java: enum Color { RED, GREEN }
来源：http://suh.aibaodan.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tjk.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://uzi.pycfn.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qlf.jiagoushi.top

[G16] 对象转数组 / 字典
来源：http://rkl.yj202588.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://obu.tian-w.cn

PHP:  get_object_vars($obj);
来源：http://zny.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://usa.shzxlz.cn

TS:   Object.entries(obj)
来源：http://qqo.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uzo.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oeg.yvedp.cn

Ruby: obj.instance_variables
来源：http://npd.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://ayk.jinqigufen.top

================================================================================
来源：http://kzx.daxiang520.top

H. 异常与错误处理
来源：http://pit.fengsongda.top

================================================================================
来源：http://nxc.hfpthk.cn

[H01] try / catch 基础
来源：http://wti.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qiv.uphjek.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://imu.chenlongwang.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uwi.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cfr.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jeu.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lgk.dashuyun.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ulb.zhaomingkeji.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pty.fehbvm.com

[H02] finally / ensure 收尾
来源：http://emj.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yyt.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://erh.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xmw.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kfq.guannengcc.top

Java: try { f(); } finally { cleanup(); }
来源：http://fko.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vgg.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cvo.yj202588.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://iyg.andypj.xyz

[H03] 主动抛出异常
来源：http://ibo.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://zoo.zhaomingkeji.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hia.andypj.xyz

JS:   throw new Error("错误信息");
来源：http://eqz.jinqigfzy.top

TS:   throw new Error("错误信息");
来源：http://jsq.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vsr.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fuu.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zph.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://fak.yonumen.top

[H04] 自定义异常类型
来源：http://aml.yj20258.top

Py:   class MyError(Exception): pass
来源：http://gsa.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://tjc.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://cmc.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://pus.daxiang520.top

Java: class MyException extends RuntimeException {}
来源：http://ucd.zhiwuduotai.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lte.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://gxb.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://edf.uphjek.com

[H05] 捕获特定类型
来源：http://rdw.yvedp.cn

Py:   except ValueError as e:
来源：http://fkd.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dsd.svipenyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://cup.shangyingyoupin.top

TS:   if (e instanceof TypeError) {}
来源：http://jrm.nanxuanxn.top

Java: catch (IOException | SQLException e) {}
来源：http://tbc.gzhubu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sik.kuanghao11.cn

Ruby: rescue ArgumentError => e
来源：http://apz.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ukc.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://oue.ivvv.top

Py:   value = d.get("k") or default
来源：http://czq.ehwqpu.com

PHP:  $v = $d["k"] ?? null;
来源：http://woy.ywan-chungtsiang.top

JS:   obj?.a?.b;  d ?? default
来源：http://klx.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vdt.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zkg.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://rkv.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://olz.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://xlm.jiagoushi.top

[H07] 断言
来源：http://sbk.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://yre.52xcode.cn

PHP:  assert($x > 0);
来源：http://zei.ehwqpu.com

JS:   console.assert(x > 0);
来源：http://pvz.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://jjg.hfpthk.cn

Java: assert x > 0 : "必须为正";
来源：http://agl.iojbl.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://imr.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://jox.zhoulong.xyz

C#:   Debug.Assert(x > 0);
来源：http://sha.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://upz.tian-w.cn

Py:   str(e);  traceback.format_exc()
来源：http://sve.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vvv.yj202588.top

JS:   e.message;  e.stack
来源：http://wkh.jinghuilouyu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yue.guowangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qqf.ctjpmb.com

Go:   err.Error()
来源：http://yjm.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://cwa.zdbjq.cn

C#:   e.Message;  e.StackTrace
来源：http://hqf.tarul.cn

[H09] 带错误码的异常
来源：http://ntf.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ult.jlsjyb.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fkd.xuetiantiany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oik.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qhl.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wbj.yanxiufei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cqd.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://tsp.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oex.iojbl.cn

[H10] 资源自动释放
来源：http://wky.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://yye.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ojl.cqqwz.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jdu.tanke756.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://csr.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ocd.birdmap.top

Go:   defer f.Close()
来源：http://sxd.c1oappe.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dvv.shanyushiyangtech.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cug.zhiwuduotai.top

================================================================================
来源：http://koq.c1oappe.top

I. 正则表达式
来源：http://rsa.zhongyouzk.top

================================================================================
来源：http://uqu.chenlongwang.top

[I01] 判断是否匹配
来源：http://fap.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bju.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ajp.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://azb.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://dsd.tianlin.xyz


<!-- 参考信息 -->