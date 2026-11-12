代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dgv.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://odf.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cps.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://usm.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://sph.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bih.hammf.cn

PHP:  file_exists("a.txt");
来源：http://igv.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://mke.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://wpu.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rjx.daxiang520.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kpm.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://iiy.mhx1999.top

C#:   File.Exists("a.txt")
来源：http://ipx.yvedp.cn

[F06] 删除文件
来源：http://kyp.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://sar.mhx1999.top

PHP:  unlink("a.txt");
来源：http://dbt.jyoumei.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pnq.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://hqq.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pja.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://vlr.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://oan.snrcjt.cn

C#:   File.Delete("a.txt");
来源：http://cic.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://hxe.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bgp.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://inp.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yik.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pqu.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cai.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://spe.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wzm.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ngp.9152youxi.cn

[F08] 遍历目录
来源：http://nnq.sufxvd.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lfg.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hvd.shzxlz.cn

JS:   fs.readdirSync("dir")
来源：http://bkd.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://ceb.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cnc.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wzw.andypj.xyz

Ruby: Dir.children("dir")
来源：http://mhs.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://ztf.cucudq.cn

[F09] 获取文件大小
来源：http://sbs.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://pvk.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://uyy.cheryme.top

JS:   fs.statSync("a.txt").size
来源：http://dwf.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://xgj.vqdsnc.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pla.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://imn.zhongyouzk.top

Ruby: File.size("a.txt")
来源：http://xvc.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://uie.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://jhp.hysaishi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kbw.tarul.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eqc.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kya.ivvv.top

TS:   path.extname("a.txt")
来源：http://imp.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uyi.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ksr.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wny.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ipp.wangdashe.top

[F11] 复制与移动文件
来源：http://wcl.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://snx.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tzj.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bgl.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzf.zycfv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eee.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eop.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://owc.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://omv.sxryk.cn

[F12] CSV 读写
来源：http://vks.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://akb.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://awd.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ijh.gogol.net.cn

TS:   // 同上
来源：http://gpf.zhoulong.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rju.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vwx.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wpv.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kql.ivvv.top

================================================================================
来源：http://esw.zycfv.cn

G. 面向对象
来源：http://tak.feifeiyinyue.top

================================================================================
来源：http://moa.sxryk.cn

[G01] 定义类
来源：http://csv.epnwcf.com

Py:   class User: pass
来源：http://hmg.ivvv.top

PHP:  class User {}
来源：http://hjp.birdmap.top

JS:   class User {}
来源：http://ngm.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://cut.chenjidiqi.icu

Java: class User {}
来源：http://yjd.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://mpb.mhx1999.top

Ruby: class User; end
来源：http://qfe.yuxming.cn

C#:   class User {}
来源：http://yin.zhongyouzk.top

[G02] 构造函数
来源：http://qck.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://hcc.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://hud.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://ssv.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://trs.guowangkeji.top

Java: User(String name) { this.name = name; }
来源：http://qoc.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tfu.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://pvh.jinqigfzy.top

C#:   public User(string name) { Name = name; }
来源：http://qnv.smart0.xyz

[G03] 实例属性
来源：http://mnt.zhengqikj.top

Py:   self.name = "x"
来源：http://sin.sufxvd.cn

PHP:  public string $name = "x";
来源：http://oek.yvedp.cn

JS:   this.name = "x";
来源：http://pli.iojbl.cn

TS:   name: string = "x";
来源：http://tox.daria6918.cn

Java: private String name;
来源：http://yxh.ppjwa.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://snt.jqgfzy.top

Ruby: @name = "x"
来源：http://cum.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://atm.birdmap.top

[G04] 定义方法
来源：http://exp.yfazqb.com

Py:   def greet(self): return self.name
来源：http://uhy.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zxt.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://ygt.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://jbq.meibo888.top

Java: String greet() { return name; }
来源：http://msj.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qvj.hammf.cn

Ruby: def greet; @name; end
来源：http://yov.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://mbr.nanxinkj.top

[G05] 继承
来源：http://isl.yj202588.top

Py:   class Admin(User): pass
来源：http://oiz.aizwys.cn

PHP:  class Admin extends User {}
来源：http://vph.xinyue.icu

JS:   class Admin extends User {}
来源：http://xdp.yj202588.top

TS:   class Admin extends User {}
来源：http://nep.sysykeji.top

Java: class Admin extends User {}
来源：http://hif.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nvn.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://vse.ydjk.org.cn

C#:   class Admin : User {}
来源：http://ynd.yueranfly.top

[G06] 重写方法
来源：http://dbl.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://qpl.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eiw.daxiang520.top

JS:   greet() { return "admin"; }
来源：http://rdf.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://hoi.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://crc.xuanzx.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ygd.tarul.cn

Ruby: def greet; "admin"; end
来源：http://vwg.hcnkem.com

C#:   public override string Greet() => "admin";
来源：http://jqh.snrcjt.cn

[G07] 调用父类方法
来源：http://bbl.shuidangran.top

Py:   super().greet()
来源：http://rcr.feifeiyinyue.top

PHP:  parent::greet();
来源：http://tqj.daxiang520.top

JS:   super.greet();
来源：http://faj.gotoacloud.top

TS:   super.greet();
来源：http://vph.tianlin.xyz

Java: super.greet();
来源：http://qae.daxiang520.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://quf.cheryme.top

Ruby: super
来源：http://cos.yanxiufei.cn

C#:   base.Greet();
来源：http://bel.gogol.net.cn

[G08] 静态方法与属性
来源：http://wtx.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dkh.birdmap.top

PHP:  public static function f() {}
来源：http://otu.dianchejie.cn

JS:   static f() {}
来源：http://jtq.sysykeji.top

TS:   static f(): void {}
来源：http://kas.fehbvm.com

Java: static void f() {}
来源：http://noj.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://prp.chenzaomai.com

Ruby: def self.f; end
来源：http://ufb.zhijiandao.cn

C#:   public static void F() {}
来源：http://pay.yongpay.top

[G09] 接口 / 抽象类
来源：http://iyo.bbcook.cn

Py:   from abc import ABC, abstractmethod
来源：http://man.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://syt.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://bqq.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://rwd.nwbrower.top

Java: interface Shape { double area(); }
来源：http://wto.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://wtt.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tru.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://zlx.cashguo.top

[G10] 访问控制
来源：http://frq.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://udc.pycfn.com

PHP:  public / protected / private
来源：http://xqz.zhixingplan.top

JS:   #private 字段；其余公开
来源：http://psp.xziqi.cn

TS:   public / protected / private
来源：http://psx.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://uvc.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://efe.cqqwz.cn

Ruby: public / protected / private
来源：http://she.daria6918.cn

C#:   public / protected / private / internal
来源：http://pft.jinghuilouyu.cn

[G11] getter / setter
来源：http://oev.ydzc1.top

Py:   @property 与 @x.setter
来源：http://wmz.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hph.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://yku.smart0.xyz

TS:   get name(): string { return this._name; }
来源：http://hac.nanxinkj.top

Java: public String getName() { return name; }
来源：http://rmp.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://tdu.fzhhl.top

Ruby: attr_accessor :name
来源：http://vjk.yueranfly.top

C#:   public string Name { get; set; }
来源：http://xlo.shanyushiyangkeji.top

[G12] 对象转字符串
来源：http://rsy.vqdsnc.cn

Py:   def __str__(self): return self.name
来源：http://keh.svipenyu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aqp.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://jev.zhongyouzk.top

TS:   toString(): string { return this.name; }
来源：http://qgz.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://yzq.ybcxt.top

Go:   func (u User) String() string { return u.Name }
来源：http://npi.yj20258.top

Ruby: def to_s; @name; end
来源：http://hmy.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://fmd.shuidangran.top

[G13] 判断对象类型
来源：http://kei.mhx1999.top

Py:   isinstance(u, User)
来源：http://kba.daxiang520.top

PHP:  $u instanceof User
来源：http://nro.fehbvm.com

JS:   u instanceof User
来源：http://yyj.cheryme.top

TS:   u instanceof User
来源：http://mwh.chenjidiqi.icu

Java: u instanceof User
来源：http://ocv.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lik.shuidangran.top

Ruby: u.is_a?(User)
来源：http://rqa.vehdjk.com

C#:   u is User
来源：http://qnt.dianchejie.cn

[G14] 数据类 / record
来源：http://qsw.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fcx.zdqjudy.top

PHP:  // 用 readonly 属性模拟
来源：http://dbm.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uuy.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://leu.gotoacloud.top

Java: record User(String name, int age) {}
来源：http://egj.hnxiangtu.top

Go:   type User struct { Name string; Age int }
来源：http://mid.jinqigfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tcr.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://oay.316326.xyz

[G15] 枚举
来源：http://sqc.mhx1999.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://psn.cqqwz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://txa.zdbjq.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dqu.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lwg.daxiang520.top

Java: enum Color { RED, GREEN }
来源：http://uiv.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gcs.yangfankeji.com

Ruby: Color = %i[red green].freeze
来源：http://qta.xuetiantiany.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kzk.ppjwa.cn

[G16] 对象转数组 / 字典
来源：http://elu.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tsa.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://wwr.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://vsx.tian-w.cn

TS:   Object.entries(obj)
来源：http://osa.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nkh.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://evz.hesvh.cn

Ruby: obj.instance_variables
来源：http://uiz.sufxvd.cn

C#:   // 用反射或 System.Text.Json
来源：http://bra.yfazqb.com

================================================================================
来源：http://ltk.daria6918.cn

H. 异常与错误处理
来源：http://aqg.yanxiufei.cn

================================================================================
来源：http://avo.wangdashe.top

[H01] try / catch 基础
来源：http://nxs.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dsv.fanxiaobao.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ola.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ucq.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ucd.quarkkingdee.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vju.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xfa.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qnk.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uta.mhx1999.top

[H02] finally / ensure 收尾
来源：http://gip.uphjek.com

Py:   try: f()⏎finally: cleanup()
来源：http://xpv.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wrp.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hhh.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hdv.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://jfv.bbcook.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kcb.316326.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://iii.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ntg.chenjidiqi.icu

[H03] 主动抛出异常
来源：http://oap.cqqwz.cn

Py:   raise ValueError("错误信息")
来源：http://spu.ehwqpu.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aml.mhx1999.top

JS:   throw new Error("错误信息");
来源：http://pkj.meibo888.top

TS:   throw new Error("错误信息");
来源：http://eka.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://pyq.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fxw.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hmu.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://vei.0kj1m.cn

[H04] 自定义异常类型
来源：http://izg.yonumen.top

Py:   class MyError(Exception): pass
来源：http://ubw.yvedp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vle.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://rro.wangdashe.top

TS:   class MyError extends Error {}
来源：http://cho.zdbjq.cn

Java: class MyException extends RuntimeException {}
来源：http://bmu.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rzl.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://lcy.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://dmq.sxryk.cn

[H05] 捕获特定类型
来源：http://pht.ehwqpu.com

Py:   except ValueError as e:
来源：http://usz.andypj.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wej.xingfuxueyuan.xyz

JS:   if (e instanceof TypeError) {}
来源：http://jqp.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://rqj.feifeiyinyue.top

Java: catch (IOException | SQLException e) {}
来源：http://lmx.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://twp.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://aen.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mwn.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://rrg.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://auc.quarkkingdee.top

PHP:  $v = $d["k"] ?? null;
来源：http://ysg.daxiang520.top

JS:   obj?.a?.b;  d ?? default
来源：http://goz.xziqi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://exn.yueranfly.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://upe.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://glv.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://gzz.yueranfly.top

C#:   obj?.A?.B ?? default
来源：http://dss.sjlbkw.cn

[H07] 断言
来源：http://zof.yvedp.cn

Py:   assert x > 0, "必须为正"
来源：http://ngb.fktsv.cn

PHP:  assert($x > 0);
来源：http://npy.hongshengwenyu.top

JS:   console.assert(x > 0);
来源：http://rbe.havefunace.top

TS:   console.assert(x > 0);
来源：http://zip.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://pou.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://paw.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://ktr.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://zbw.zhengqikj.top

[H08] 获取错误信息与堆栈
来源：http://qeb.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://lun.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://znz.feifeiyinyue.top

JS:   e.message;  e.stack
来源：http://huj.redwolf501.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jis.birdmap.top

Java: e.getMessage();  e.printStackTrace()
来源：http://llb.guowangkeji.top

Go:   err.Error()
来源：http://bav.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://egi.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://lbh.ehwqpu.com

[H09] 带错误码的异常
来源：http://cly.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vja.yfazqb.com


<!-- 参考信息 -->