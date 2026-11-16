代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://awx.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zqg.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ewu.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ouu.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://glb.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vzm.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://iaw.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://xgw.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://hah.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zmd.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wip.gzhubu.top

Ruby: File.exist?("a.txt")
来源：http://btz.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://izb.epnwcf.com

[F06] 删除文件
来源：http://pkw.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://hka.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://oul.gzhubu.top

JS:   fs.unlinkSync("a.txt")
来源：http://onz.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://zdw.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kft.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://afu.epnwcf.com

Ruby: File.delete("a.txt")
来源：http://fbw.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://dbn.yvedp.cn

[F07] 创建目录（含多级）
来源：http://dyw.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wpu.birdmap.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://anm.xuanzx.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://atk.ywan-chungtsiang.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rpm.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oan.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dxl.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zix.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nml.fehbvm.com

[F08] 遍历目录
来源：http://zpm.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cak.jinqigfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ofn.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://jcg.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://yow.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lgm.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cky.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://jig.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://mit.nanxinkj.top

[F09] 获取文件大小
来源：http://bpl.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://lcy.birdmap.top

PHP:  filesize("a.txt");
来源：http://oho.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://ngf.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://oow.xziqi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mhr.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hwu.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://ukt.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://clj.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://hfk.quarkkingdee.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ecv.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vam.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://poz.bjfxy.top

TS:   path.extname("a.txt")
来源：http://uot.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rnl.jiagoushi.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://whj.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jqf.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zzm.hnqzz.top

[F11] 复制与移动文件
来源：http://whv.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mkj.daxiang520.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sxw.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gvg.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfz.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://stb.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fvr.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hez.kuanghao11.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vkv.ybcxt.top

[F12] CSV 读写
来源：http://lzy.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vic.fktsv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wsj.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://quf.yj20258.top

TS:   // 同上
来源：http://nod.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zwr.yanxiufei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://utb.yvedp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ycd.fehbvm.com

C#:   // 无内置：用 CsvHelper 库
来源：http://wft.hongshengwenyu.top

================================================================================
来源：http://uif.xinyue.icu

G. 面向对象
来源：http://tfa.shuidangran.top

================================================================================
来源：http://yeo.gogol.net.cn

[G01] 定义类
来源：http://zjx.cdnleiting.top

Py:   class User: pass
来源：http://hzy.yuxming.cn

PHP:  class User {}
来源：http://krb.cashguo.top

JS:   class User {}
来源：http://vhh.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://vvp.hysaishi.cn

Java: class User {}
来源：http://sud.smart0.xyz

Go:   type User struct { Name string }
来源：http://qnl.feifeiyinyue.top

Ruby: class User; end
来源：http://ncz.chenjidiqi.icu

C#:   class User {}
来源：http://ebc.zhijiandao.cn

[G02] 构造函数
来源：http://oak.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://zai.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://ibs.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mve.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://dby.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://mon.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tqx.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://dyj.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://stk.fanxiaobao.xyz

[G03] 实例属性
来源：http://zxp.epnwcf.com

Py:   self.name = "x"
来源：http://oml.yangfankeji.com

PHP:  public string $name = "x";
来源：http://kvl.52xcode.cn

JS:   this.name = "x";
来源：http://epf.gzhubu.top

TS:   name: string = "x";
来源：http://wmm.52xcode.cn

Java: private String name;
来源：http://lwz.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bbe.hnxiangtu.top

Ruby: @name = "x"
来源：http://gws.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://zms.hongshengwenyu.top

[G04] 定义方法
来源：http://myj.epnwcf.com

Py:   def greet(self): return self.name
来源：http://bgx.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://psx.birdmap.top

JS:   greet() { return this.name; }
来源：http://bjc.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://hnb.yj20258888.top

Java: String greet() { return name; }
来源：http://atf.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ody.epnwcf.com

Ruby: def greet; @name; end
来源：http://gyq.yj202588.top

C#:   public string Greet() => Name;
来源：http://xiy.gotoacloud.top

[G05] 继承
来源：http://ahw.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://pby.fzhhl.top

PHP:  class Admin extends User {}
来源：http://gnq.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://crf.316326.xyz

TS:   class Admin extends User {}
来源：http://zbd.hysaishi.cn

Java: class Admin extends User {}
来源：http://ifx.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iak.fktsv.cn

Ruby: class Admin < User; end
来源：http://uao.nanxinkj.top

C#:   class Admin : User {}
来源：http://ops.yuanzhike.top

[G06] 重写方法
来源：http://ydr.tianlin.xyz

Py:   def greet(self): return "admin"
来源：http://pci.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://znu.yj202588.top

JS:   greet() { return "admin"; }
来源：http://ezw.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://tzs.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://dcm.fktsv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vkd.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://kty.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://kzk.zdqjudy.top

[G07] 调用父类方法
来源：http://tpw.yangfankeji.com

Py:   super().greet()
来源：http://bzs.epnwcf.com

PHP:  parent::greet();
来源：http://okl.yvedp.cn

JS:   super.greet();
来源：http://yal.fzhhl.top

TS:   super.greet();
来源：http://amj.zdqjudy.top

Java: super.greet();
来源：http://xpy.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zvs.nanxinkj.top

Ruby: super
来源：http://oer.hongshengwenyu.top

C#:   base.Greet();
来源：http://nyd.ydzc1.top

[G08] 静态方法与属性
来源：http://vri.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uzz.52xcode.cn

PHP:  public static function f() {}
来源：http://pql.sysykeji.top

JS:   static f() {}
来源：http://yfj.dianchejie.cn

TS:   static f(): void {}
来源：http://zuq.hywenlv.cn

Java: static void f() {}
来源：http://ssx.gotoacloud.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wzg.yfazqb.com

Ruby: def self.f; end
来源：http://jno.cucudq.cn

C#:   public static void F() {}
来源：http://zrg.daxiang520.top

[G09] 接口 / 抽象类
来源：http://ldx.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gtz.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://oke.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://acu.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://orz.andypj.xyz

Java: interface Shape { double area(); }
来源：http://uaw.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://shc.fktsv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ktt.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://xob.hysaishi.cn

[G10] 访问控制
来源：http://ado.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://skd.guannengcc.top

PHP:  public / protected / private
来源：http://adp.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://mae.quarkkingdee.top

TS:   public / protected / private
来源：http://doc.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://yyn.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bit.cashguo.top

Ruby: public / protected / private
来源：http://axm.daxiang520.top

C#:   public / protected / private / internal
来源：http://xey.gotoacloud.top

[G11] getter / setter
来源：http://igd.yfazqb.com

Py:   @property 与 @x.setter
来源：http://xzm.yfazqb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://tvd.yj20258.top

JS:   get name() { return this._name; }
来源：http://jyi.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://zbw.aizwys.cn

Java: public String getName() { return name; }
来源：http://vzc.nanxinkj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gwj.yj20258.top

Ruby: attr_accessor :name
来源：http://sld.bjfxy.top

C#:   public string Name { get; set; }
来源：http://vlz.zhixingplan.top

[G12] 对象转字符串
来源：http://ijq.nwbrower.top

Py:   def __str__(self): return self.name
来源：http://buu.jinghuilouyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hsq.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://yya.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://ior.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://anw.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rws.cqqwz.cn

Ruby: def to_s; @name; end
来源：http://caz.uphjek.com

C#:   public override string ToString() => Name;
来源：http://qsq.zhongyouzk.top

[G13] 判断对象类型
来源：http://ost.yj20258.top

Py:   isinstance(u, User)
来源：http://tph.shanyushiyangtech.top

PHP:  $u instanceof User
来源：http://rdv.fzhhl.top

JS:   u instanceof User
来源：http://mcu.epnwcf.com

TS:   u instanceof User
来源：http://uii.gzhubu.top

Java: u instanceof User
来源：http://gsu.havefunace.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kkx.c1oappe.top

Ruby: u.is_a?(User)
来源：http://gdo.gogol.net.cn

C#:   u is User
来源：http://pzj.xziqi.cn

[G14] 数据类 / record
来源：http://vrr.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zzn.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://akg.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://hmq.zycfv.cn

TS:   type User = { name: string; age: number };
来源：http://snm.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://nct.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://xxv.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lko.shanyushiyangtech.top

C#:   record User(string Name, int Age);
来源：http://yya.jlsjyb.cn

[G15] 枚举
来源：http://cnf.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aar.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://azc.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rtg.tian-w.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iuu.yueranfly.top

Java: enum Color { RED, GREEN }
来源：http://fps.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yhp.aizwys.cn

Ruby: Color = %i[red green].freeze
来源：http://arm.xinyue.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hzv.nwbrower.top

[G16] 对象转数组 / 字典
来源：http://tqg.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wbz.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://tuz.316326.xyz

JS:   Object.entries(obj)
来源：http://cec.sufxvd.cn

TS:   Object.entries(obj)
来源：http://ubz.jianghu66.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rlr.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qoy.hcnkem.com

Ruby: obj.instance_variables
来源：http://egv.sjlbkw.cn

C#:   // 用反射或 System.Text.Json
来源：http://wcj.zhaomingkeji.xyz

================================================================================
来源：http://gje.sysykeji.top

H. 异常与错误处理
来源：http://efb.jianghu66.top

================================================================================
来源：http://jie.guowangkeji.top

[H01] try / catch 基础
来源：http://fpn.gaohongyu789.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zix.xziqi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://eme.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tvh.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eqs.gogol.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kny.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qqo.svipenyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jdy.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fxi.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://zsv.cheryme.top

Py:   try: f()⏎finally: cleanup()
来源：http://wpf.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tym.cucudq.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qwb.zhijiandao.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rsr.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://urz.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://thr.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gir.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://umy.sysykeji.top

[H03] 主动抛出异常
来源：http://sue.yueranfly.top

Py:   raise ValueError("错误信息")
来源：http://fwn.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gex.fanxiaobao.xyz

JS:   throw new Error("错误信息");
来源：http://fhr.daria6918.cn

TS:   throw new Error("错误信息");
来源：http://lpb.vehdjk.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://exz.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kqu.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xaw.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ynj.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://lsx.tarul.cn

Py:   class MyError(Exception): pass
来源：http://yhg.vehdjk.com

PHP:  class MyError extends RuntimeException {}
来源：http://cpf.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://gqg.yongpay.top

TS:   class MyError extends Error {}
来源：http://ljk.zycfv.cn

Java: class MyException extends RuntimeException {}
来源：http://mbt.sjlbkw.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://guz.quarkkingdee.top

Ruby: class MyError < StandardError; end
来源：http://raq.bjfxy.top

C#:   class MyException : Exception {}
来源：http://bhl.zdqjudy.top

[H05] 捕获特定类型
来源：http://qqa.tianlin.xyz

Py:   except ValueError as e:
来源：http://pif.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lxi.zhengqikj.top

JS:   if (e instanceof TypeError) {}
来源：http://vis.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://ifv.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://lml.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iev.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://lsw.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qkm.zhengqikj.top

[H06] 可选值 / 空值安全访问
来源：http://jlr.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://hyk.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://stb.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://mwo.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://emy.hcnkem.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jfp.yangfankeji.com

Go:   if v, ok := m["k"]; ok { }
来源：http://kme.tarul.cn

Ruby: d&.dig(:a, :b)
来源：http://lbi.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://kgq.sweek.top

[H07] 断言
来源：http://gmi.daria6918.cn

Py:   assert x > 0, "必须为正"
来源：http://tow.redwolf501.top

PHP:  assert($x > 0);
来源：http://aat.shuidangran.top

JS:   console.assert(x > 0);
来源：http://zcn.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://pbd.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://fyd.hcnkem.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://myq.yj20258888.top

Ruby: raise "必须为正" unless x > 0
来源：http://vmw.hywenlv.cn

C#:   Debug.Assert(x > 0);
来源：http://jyz.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://vqi.jinghuilouyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://gxs.vqdsnc.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zpc.andypj.xyz

JS:   e.message;  e.stack
来源：http://ort.cashguo.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://kqo.dashuyun.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uhf.nwbrower.top

Go:   err.Error()
来源：http://fsa.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://fgi.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://jft.52xcode.cn

[H09] 带错误码的异常
来源：http://kjm.kuanghao11.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dex.ivvv.top


<!-- 参考信息 -->