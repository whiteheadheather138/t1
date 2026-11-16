代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zkf.zhoulong.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rxt.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://grs.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://isd.yvedp.cn

[F05] 判断文件或目录是否存在
来源：http://udi.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kvu.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://waj.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://xje.nanxuanxn.top

TS:   fs.existsSync("a.txt")
来源：http://kpb.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://eqw.sysykeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vpd.sxryk.cn

Ruby: File.exist?("a.txt")
来源：http://zub.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://ltv.xylfe.cn

[F06] 删除文件
来源：http://rbs.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://pvw.kuanghao11.cn

PHP:  unlink("a.txt");
来源：http://kym.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://qax.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ymt.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://udm.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://kms.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://kvz.yj20258.top

C#:   File.Delete("a.txt");
来源：http://ycs.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://ham.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iwy.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ivm.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mco.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xwr.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://peu.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wbt.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qda.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kin.tianlin.xyz

[F08] 遍历目录
来源：http://xyk.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rbj.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zsg.tianlin.xyz

JS:   fs.readdirSync("dir")
来源：http://wdl.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://rgm.xinyue.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ytb.yuanzhike.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rxz.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://rdk.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://jtc.haohaochexian.top

[F09] 获取文件大小
来源：http://lzi.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://rwx.uphjek.com

PHP:  filesize("a.txt");
来源：http://ejg.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://pny.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://pux.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://uiv.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iqp.gzhubu.top

Ruby: File.size("a.txt")
来源：http://vvc.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://bws.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://cbi.yanxiufei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nzb.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bzj.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kil.havefunace.top

TS:   path.extname("a.txt")
来源：http://hvi.jinyuanbaomall.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://puq.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ges.bjfxy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qor.jinqigufen.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dzo.hysaishi.cn

[F11] 复制与移动文件
来源：http://ene.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cso.zhengqikj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wgc.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgi.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gep.yuxming.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yyk.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zaz.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uah.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zaq.316326.xyz

[F12] CSV 读写
来源：http://hby.andypj.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xuw.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://giz.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://epv.fanxiaobao.xyz

TS:   // 同上
来源：http://eny.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nll.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ysy.jqgfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://adi.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fmv.fengsongda.top

================================================================================
来源：http://mnz.daria6918.cn

G. 面向对象
来源：http://saw.zycfv.cn

================================================================================
来源：http://veg.bbcook.cn

[G01] 定义类
来源：http://htn.yuxming.cn

Py:   class User: pass
来源：http://kng.shanyushiyangtech.top

PHP:  class User {}
来源：http://zhu.gotoacloud.top

JS:   class User {}
来源：http://qis.jyoumei.cn

TS:   class User { name: string = ""; }
来源：http://omu.nanxuanxn.top

Java: class User {}
来源：http://rsx.hysaishi.cn

Go:   type User struct { Name string }
来源：http://rfb.jinqigfzy.top

Ruby: class User; end
来源：http://zhs.zhongyouzk.top

C#:   class User {}
来源：http://azk.zhongyouzk.top

[G02] 构造函数
来源：http://nyw.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://szr.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://zgx.cqqwz.cn

JS:   constructor(name) { this.name = name; }
来源：http://lwt.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://vse.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://mlp.jinqigufen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hhz.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://foz.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://cut.yfazqb.com

[G03] 实例属性
来源：http://jlh.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://dfr.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://pgl.tanke756.top

JS:   this.name = "x";
来源：http://izg.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://eai.fengsongda.top

Java: private String name;
来源：http://ool.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wfc.feifeiyinyue.top

Ruby: @name = "x"
来源：http://xjo.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://poc.dianchejie.cn

[G04] 定义方法
来源：http://xfq.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://fcw.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ker.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://mad.ehwqpu.com

TS:   greet(): string { return this.name; }
来源：http://tum.xinyue.icu

Java: String greet() { return name; }
来源：http://syk.bbcook.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hgy.316326.xyz

Ruby: def greet; @name; end
来源：http://zuc.sxryk.cn

C#:   public string Greet() => Name;
来源：http://qju.zhixingplan.top

[G05] 继承
来源：http://xfb.yonumen.top

Py:   class Admin(User): pass
来源：http://ssw.aizwys.cn

PHP:  class Admin extends User {}
来源：http://sro.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://wcl.ybcxt.top

TS:   class Admin extends User {}
来源：http://bkw.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://zqf.yj20258888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://has.vehdjk.com

Ruby: class Admin < User; end
来源：http://eqc.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://idc.yonumen.top

[G06] 重写方法
来源：http://tnn.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://yqo.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://chq.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://pvs.yongpay.top

TS:   greet(): string { return "admin"; }
来源：http://cys.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://vgb.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tts.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://rya.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://hce.mhx1999.top

[G07] 调用父类方法
来源：http://qbz.zhixingplan.top

Py:   super().greet()
来源：http://zyf.bjfxy.top

PHP:  parent::greet();
来源：http://byk.sjlbkw.cn

JS:   super.greet();
来源：http://tok.0kj1m.cn

TS:   super.greet();
来源：http://bgq.cucudq.cn

Java: super.greet();
来源：http://rcl.epnwcf.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bdf.hnxiangtu.top

Ruby: super
来源：http://uyi.ydzc1.top

C#:   base.Greet();
来源：http://cwv.0kj1m.cn

[G08] 静态方法与属性
来源：http://gle.fehbvm.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gac.sweek.top

PHP:  public static function f() {}
来源：http://xzr.xylfe.cn

JS:   static f() {}
来源：http://mxa.andypj.xyz

TS:   static f(): void {}
来源：http://fex.jqgufenzy.top

Java: static void f() {}
来源：http://ugd.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vbn.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://cdu.yanxiufei.cn

C#:   public static void F() {}
来源：http://jzw.hesvh.cn

[G09] 接口 / 抽象类
来源：http://wwi.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://ulx.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://pwk.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qbb.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://ybs.sweek.top

Java: interface Shape { double area(); }
来源：http://sco.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://diw.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://czu.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://htf.pengpengdd.cyou

[G10] 访问控制
来源：http://gwg.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://fdi.yanxiufei.cn

PHP:  public / protected / private
来源：http://hlr.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://fof.fanxiaobao.xyz

TS:   public / protected / private
来源：http://tcr.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://gcq.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ioq.hysaishi.cn

Ruby: public / protected / private
来源：http://qul.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://tug.kuanghao11.cn

[G11] getter / setter
来源：http://axt.yanxiufei.cn

Py:   @property 与 @x.setter
来源：http://jdr.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nof.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://rxq.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://xig.xylfe.cn

Java: public String getName() { return name; }
来源：http://xbz.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gnj.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://zfv.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://ole.jiagoushi.top

[G12] 对象转字符串
来源：http://sxs.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://cbp.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qjw.tarul.cn

JS:   toString() { return this.name; }
来源：http://zjs.yfazqb.com

TS:   toString(): string { return this.name; }
来源：http://hgk.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://oqb.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sbt.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://rkg.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://log.jinyuanbaomall.cn

[G13] 判断对象类型
来源：http://szv.ydjk.org.cn

Py:   isinstance(u, User)
来源：http://bly.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://yxp.zhiwuduotai.top

JS:   u instanceof User
来源：http://tct.quarkkingdee.top

TS:   u instanceof User
来源：http://ate.nanxinkj.top

Java: u instanceof User
来源：http://dfs.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://upf.uphjek.com

Ruby: u.is_a?(User)
来源：http://dkj.zhoulong.xyz

C#:   u is User
来源：http://sdn.hcnkem.com

[G14] 数据类 / record
来源：http://byk.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yxo.yangfankeji.com

PHP:  // 用 readonly 属性模拟
来源：http://qsi.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ygk.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://oos.birdmap.top

Java: record User(String name, int age) {}
来源：http://vbx.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://lll.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kyz.zhengqikj.top

C#:   record User(string Name, int Age);
来源：http://jks.ehwqpu.com

[G15] 枚举
来源：http://qoe.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vec.cdnleiting.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fik.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ddo.nwbrower.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wji.yongpay.top

Java: enum Color { RED, GREEN }
来源：http://zhd.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ffe.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://lcd.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://osn.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://cog.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rse.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://xqx.0kj1m.cn

JS:   Object.entries(obj)
来源：http://anb.tianlin.xyz

TS:   Object.entries(obj)
来源：http://znh.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://glv.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lqd.hcnkem.com

Ruby: obj.instance_variables
来源：http://bfj.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://elg.meibo888.top

================================================================================
来源：http://bnp.ydjk.org.cn

H. 异常与错误处理
来源：http://ayn.tianlin.xyz

================================================================================
来源：http://jsv.tanke756.top

[H01] try / catch 基础
来源：http://ati.0kj1m.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ntl.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xvn.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tow.yj20258.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fsv.feifeiyinyue.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://neo.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bzj.xingfuxueyuan.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://srz.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ana.nanxuanxn.top

[H02] finally / ensure 收尾
来源：http://mpq.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://gve.hnqzz.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yjh.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ltf.havefunace.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fyi.fktsv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://irt.ivvv.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://abf.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ohn.yuanzhike.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rwn.tanke756.top

[H03] 主动抛出异常
来源：http://hsl.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://kgi.dianchejie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dwg.yj202588.top

JS:   throw new Error("错误信息");
来源：http://goi.fzhhl.top

TS:   throw new Error("错误信息");
来源：http://sof.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://cyn.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://veg.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uiw.xinyue.icu

C#:   throw new ArgumentException("错误信息");
来源：http://anw.xinyue.icu

[H04] 自定义异常类型
来源：http://ksv.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://otp.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://imc.yuanzhike.top

JS:   class MyError extends Error {}
来源：http://tic.chenzaomai.com

TS:   class MyError extends Error {}
来源：http://tkq.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://cux.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://olp.chenjidiqi.icu

Ruby: class MyError < StandardError; end
来源：http://qfw.hfpthk.cn

C#:   class MyException : Exception {}
来源：http://vzk.uphjek.com

[H05] 捕获特定类型
来源：http://qqr.yuxming.cn

Py:   except ValueError as e:
来源：http://oyc.xinyue.icu

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://grr.hnqzz.top

JS:   if (e instanceof TypeError) {}
来源：http://rva.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://zmb.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://izw.xylfe.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://chq.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://vvi.svipenyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nta.shuidangran.top

[H06] 可选值 / 空值安全访问
来源：http://hnt.cdnleiting.top

Py:   value = d.get("k") or default
来源：http://sct.xingfuxueyuan.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://lir.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://upy.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://tdo.yuxming.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vod.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xvz.cucudq.cn

Ruby: d&.dig(:a, :b)
来源：http://uwf.jinghuilouyu.cn

C#:   obj?.A?.B ?? default
来源：http://cil.hongshengwenyu.top

[H07] 断言
来源：http://uuh.cqqwz.cn

Py:   assert x > 0, "必须为正"
来源：http://jzc.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://cvr.sufxvd.cn

JS:   console.assert(x > 0);
来源：http://kpj.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://zpw.wangshuangyany.cn

Java: assert x > 0 : "必须为正";
来源：http://qst.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sze.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://pdz.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://mla.c1oappe.top

[H08] 获取错误信息与堆栈
来源：http://eti.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://qar.zhongyouzk.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yfk.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://vzr.hongshengwenyu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jub.jianghu66.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tvy.gogol.net.cn

Go:   err.Error()
来源：http://dpq.zhixingplan.top

Ruby: e.message;  e.backtrace
来源：http://sdq.9152youxi.cn

C#:   e.Message;  e.StackTrace
来源：http://mye.ydzc1.top

[H09] 带错误码的异常
来源：http://hee.haohaochexian.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gis.bbcook.cn


<!-- 参考信息 -->