代发 wailian999

Ruby: File.delete("a.txt")
来源：http://lxh.zdbjq.cn

C#:   File.Delete("a.txt");
来源：http://jud.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://uoh.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zai.hnxiangtu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eca.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nnt.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vdz.zycfv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lxs.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vym.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sxf.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nhe.ehwqpu.com

[F08] 遍历目录
来源：http://qox.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lla.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tzv.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://izy.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://gan.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yys.gzhubu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mcb.havefunace.top

Ruby: Dir.children("dir")
来源：http://qmt.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://ppv.yvedp.cn

[F09] 获取文件大小
来源：http://vht.hywenlv.cn

Py:   os.path.getsize("a.txt")
来源：http://the.jianghu66.top

PHP:  filesize("a.txt");
来源：http://wiz.jqgufenzy.top

JS:   fs.statSync("a.txt").size
来源：http://xwj.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://iud.quarkkingdee.top

Java: Files.size(Path.of("a.txt"))
来源：http://dlk.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hnq.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://sca.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://igw.ehwqpu.com

[F10] 取文件扩展名 / 文件名
来源：http://fxk.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tzi.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sxa.wangshuangyany.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pem.tian-w.cn

TS:   path.extname("a.txt")
来源：http://axl.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hfb.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aaa.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ovx.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dep.daria6918.cn

[F11] 复制与移动文件
来源：http://vyd.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jft.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://thf.hcnkem.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lra.feifeiyinyue.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hcx.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pry.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yng.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jin.cdnleiting.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yne.zhijiandao.cn

[F12] CSV 读写
来源：http://rvp.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nrd.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://upl.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cab.sxryk.cn

TS:   // 同上
来源：http://bbb.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gzj.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kru.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xrx.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cia.shangyingyoupin.top

================================================================================
来源：http://pcs.yj20258888.top

G. 面向对象
来源：http://lra.haohaochexian.top

================================================================================
来源：http://xvx.xylfe.cn

[G01] 定义类
来源：http://dmw.daxiang520.top

Py:   class User: pass
来源：http://mzv.yuxming.cn

PHP:  class User {}
来源：http://plz.vehdjk.com

JS:   class User {}
来源：http://eid.yj202588.top

TS:   class User { name: string = ""; }
来源：http://erl.birdmap.top

Java: class User {}
来源：http://top.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://jlj.sjlbkw.cn

Ruby: class User; end
来源：http://qnd.shuidangran.top

C#:   class User {}
来源：http://bar.wangshuangyany.cn

[G02] 构造函数
来源：http://evp.cqqwz.cn

Py:   def __init__(self, name): self.name = name
来源：http://niw.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://glb.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://zcj.sweek.top

TS:   constructor(public name: string) {}
来源：http://dur.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://zmw.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://udw.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://alo.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://pel.zhiwuduotai.top

[G03] 实例属性
来源：http://hmi.ppjwa.cn

Py:   self.name = "x"
来源：http://lzw.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://oda.ivvv.top

JS:   this.name = "x";
来源：http://acc.zhongyouzk.top

TS:   name: string = "x";
来源：http://ape.yuxming.cn

Java: private String name;
来源：http://pmf.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jgh.ehwqpu.com

Ruby: @name = "x"
来源：http://drj.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://pgt.tanke756.top

[G04] 定义方法
来源：http://hpx.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://gsi.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ikx.tanke756.top

JS:   greet() { return this.name; }
来源：http://yzy.zdqjudy.top

TS:   greet(): string { return this.name; }
来源：http://yma.sufxvd.cn

Java: String greet() { return name; }
来源：http://syc.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rnq.yj202588.top

Ruby: def greet; @name; end
来源：http://qfs.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://swq.yj20258888.top

[G05] 继承
来源：http://gwh.yuanzhike.top

Py:   class Admin(User): pass
来源：http://jaa.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://awn.nwbrower.top

JS:   class Admin extends User {}
来源：http://vfa.gogol.net.cn

TS:   class Admin extends User {}
来源：http://mex.hfpthk.cn

Java: class Admin extends User {}
来源：http://sac.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://guh.haohaochexian.top

Ruby: class Admin < User; end
来源：http://yeq.hcnkem.com

C#:   class Admin : User {}
来源：http://jua.xinyue.icu

[G06] 重写方法
来源：http://xlh.redwolf501.top

Py:   def greet(self): return "admin"
来源：http://kks.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://dqo.hnxiangtu.top

JS:   greet() { return "admin"; }
来源：http://rnn.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://owt.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://sex.yangfankeji.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qpw.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://sgz.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://yip.vehdjk.com

[G07] 调用父类方法
来源：http://szq.shuidangran.top

Py:   super().greet()
来源：http://yes.cqqwz.cn

PHP:  parent::greet();
来源：http://rwx.kuanghao11.cn

JS:   super.greet();
来源：http://twf.wangshuangyany.cn

TS:   super.greet();
来源：http://mwf.fzhhl.top

Java: super.greet();
来源：http://lph.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rut.birdmap.top

Ruby: super
来源：http://iaz.yj202588.top

C#:   base.Greet();
来源：http://epi.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://zkq.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://txv.jqgfzy.top

PHP:  public static function f() {}
来源：http://poc.kuanghao11.cn

JS:   static f() {}
来源：http://bva.gogol.net.cn

TS:   static f(): void {}
来源：http://dqh.nwbrower.top

Java: static void f() {}
来源：http://dsb.shanyushiyangkeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ovj.yj20258888.top

Ruby: def self.f; end
来源：http://iet.yuanzhike.top

C#:   public static void F() {}
来源：http://kmp.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://tqr.daria6918.cn

Py:   from abc import ABC, abstractmethod
来源：http://qza.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vah.316326.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uen.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://ldl.pycfn.com

Java: interface Shape { double area(); }
来源：http://riq.aizwys.cn

Go:   type Shape interface { Area() float64 }
来源：http://uaq.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pmf.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://sdn.gotoacloud.top

[G10] 访问控制
来源：http://zhx.zhixingplan.top

Py:   约定 _protected / __private（不强制）
来源：http://deh.jyoumei.cn

PHP:  public / protected / private
来源：http://fbi.pycfn.com

JS:   #private 字段；其余公开
来源：http://vrn.kuanghao11.cn

TS:   public / protected / private
来源：http://zwt.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://oxt.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nzc.hcnkem.com

Ruby: public / protected / private
来源：http://aoe.tian-w.cn

C#:   public / protected / private / internal
来源：http://jmt.xziqi.cn

[G11] getter / setter
来源：http://vcl.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://rqk.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kdl.52xcode.cn

JS:   get name() { return this._name; }
来源：http://fih.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://vdf.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://inf.bjfxy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://amj.gotoacloud.top

Ruby: attr_accessor :name
来源：http://uxn.shanyushiyangtech.top

C#:   public string Name { get; set; }
来源：http://kqy.yongpay.top

[G12] 对象转字符串
来源：http://afk.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://uei.ywan-chungtsiang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lnp.iojbl.cn

JS:   toString() { return this.name; }
来源：http://rqh.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://dog.shanyushiyangtech.top

Java: @Override public String toString() { return name; }
来源：http://zgv.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jkn.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://pif.guowangkeji.top

C#:   public override string ToString() => Name;
来源：http://cwu.gogol.net.cn

[G13] 判断对象类型
来源：http://qzq.hfpthk.cn

Py:   isinstance(u, User)
来源：http://fvy.hcnkem.com

PHP:  $u instanceof User
来源：http://xzr.hcnkem.com

JS:   u instanceof User
来源：http://rdb.epnwcf.com

TS:   u instanceof User
来源：http://xyd.0kj1m.cn

Java: u instanceof User
来源：http://tdh.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vwg.epnwcf.com

Ruby: u.is_a?(User)
来源：http://glq.shuidangran.top

C#:   u is User
来源：http://gui.yj20258.top

[G14] 数据类 / record
来源：http://nrw.havefunace.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://axe.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://ihd.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://adk.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://vxo.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://qij.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://qeo.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pnm.zhiwuduotai.top

C#:   record User(string Name, int Age);
来源：http://tix.fanxiaobao.xyz

[G15] 枚举
来源：http://uru.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lch.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kxj.ywan-chungtsiang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kye.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://woa.cheryme.top

Java: enum Color { RED, GREEN }
来源：http://xdv.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xer.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://fue.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yli.xuanzx.com

[G16] 对象转数组 / 字典
来源：http://fnd.daria6918.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nwl.gotoacloud.top

PHP:  get_object_vars($obj);
来源：http://wlv.hesvh.cn

JS:   Object.entries(obj)
来源：http://alu.jyoumei.cn

TS:   Object.entries(obj)
来源：http://oau.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wbo.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://drh.ehwqpu.com

Ruby: obj.instance_variables
来源：http://kir.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://eyt.ctjpmb.com

================================================================================
来源：http://ayf.jinqigufen.top

H. 异常与错误处理
来源：http://uim.jinghuilouyu.cn

================================================================================
来源：http://ggv.jlsjyb.cn

[H01] try / catch 基础
来源：http://efo.jlsjyb.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zrk.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rvl.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zzx.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mya.uphjek.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bjc.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zbk.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nuq.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kwl.52xcode.cn

[H02] finally / ensure 收尾
来源：http://eer.xziqi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gcf.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://clv.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dyg.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://qgu.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lvu.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://csq.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nky.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qjh.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://xni.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://owt.chenjidiqi.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ixq.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://ora.yongpay.top

TS:   throw new Error("错误信息");
来源：http://lej.jinqigufen.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://tbs.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mis.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nhs.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://mcg.snrcjt.cn

[H04] 自定义异常类型
来源：http://lei.aizwys.cn

Py:   class MyError(Exception): pass
来源：http://fob.zhiwuduotai.top

PHP:  class MyError extends RuntimeException {}
来源：http://tfn.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://qud.hnxiangtu.top

TS:   class MyError extends Error {}
来源：http://aog.ctjpmb.com

Java: class MyException extends RuntimeException {}
来源：http://sbc.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yxn.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://vtu.c1oappe.top

C#:   class MyException : Exception {}
来源：http://pay.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://qik.sxryk.cn

Py:   except ValueError as e:
来源：http://muv.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nin.hysaishi.cn

JS:   if (e instanceof TypeError) {}
来源：http://pqu.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://btd.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://qkw.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ybc.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://olu.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bpp.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://wqz.zhijiandao.cn

Py:   value = d.get("k") or default
来源：http://azv.sweek.top

PHP:  $v = $d["k"] ?? null;
来源：http://blm.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://cwq.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://pwj.nwbrower.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ipn.ctjpmb.com

Go:   if v, ok := m["k"]; ok { }
来源：http://fzd.xuanzx.com

Ruby: d&.dig(:a, :b)
来源：http://xzk.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://fob.hesvh.cn

[H07] 断言
来源：http://okp.sxryk.cn

Py:   assert x > 0, "必须为正"
来源：http://vel.ydzc1.top

PHP:  assert($x > 0);
来源：http://zaa.kuanghao11.cn

JS:   console.assert(x > 0);
来源：http://umu.kuanghao11.cn

TS:   console.assert(x > 0);
来源：http://nyg.yongpay.top

Java: assert x > 0 : "必须为正";
来源：http://oam.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://soz.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gag.jlsjyb.cn

C#:   Debug.Assert(x > 0);
来源：http://msz.smart0.xyz

[H08] 获取错误信息与堆栈
来源：http://kex.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://bny.cqqwz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ohq.tianlin.xyz

JS:   e.message;  e.stack
来源：http://wrf.tanke756.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://apd.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dwn.yueranfly.top

Go:   err.Error()
来源：http://hfi.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://cjz.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://xqy.zhengqikj.top

[H09] 带错误码的异常
来源：http://cyc.yangfankeji.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xba.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://msh.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fqy.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zln.xuanzx.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zhs.jinqigfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tlo.cqqwz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yxx.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://nrr.zycfv.cn

[H10] 资源自动释放
来源：http://fvp.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qji.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cwu.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ajf.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zqf.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tyw.nwbrower.top

Go:   defer f.Close()
来源：http://iaz.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://riz.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://com.jinqigfzy.top

================================================================================
来源：http://xcj.hfpthk.cn

I. 正则表达式
来源：http://zed.birdmap.top

================================================================================
来源：http://ovs.havefunace.top

[I01] 判断是否匹配
来源：http://jxu.9152youxi.cn


<!-- 参考信息 -->