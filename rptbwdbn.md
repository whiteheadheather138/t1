代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bci.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gbi.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zvk.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iab.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://fng.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qni.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://pco.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://drk.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://gep.sufxvd.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://omo.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iqs.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://mfl.nanxuanxn.top

C#:   File.Exists("a.txt")
来源：http://kgx.hammf.cn

[F06] 删除文件
来源：http://nwk.yj20258.top

Py:   os.remove("a.txt")
来源：http://ijp.tanke756.top

PHP:  unlink("a.txt");
来源：http://fuq.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://yxh.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ham.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rhl.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://mcp.shuidangran.top

Ruby: File.delete("a.txt")
来源：http://mdp.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://lkj.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://vfz.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sok.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://usj.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lca.aizwys.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lqw.c1oappe.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jxa.sxryk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zti.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zko.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ooi.zdbjq.cn

[F08] 遍历目录
来源：http://uxc.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xzl.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uie.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://dlk.jinqigfzy.top

TS:   fs.readdirSync("dir")
来源：http://ggw.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oeo.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kgg.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://gni.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://xry.feifeiyinyue.top

[F09] 获取文件大小
来源：http://xkz.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://fzp.hcnkem.com

PHP:  filesize("a.txt");
来源：http://uzx.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://vob.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://dse.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://txl.uphjek.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aoh.ctjpmb.com

Ruby: File.size("a.txt")
来源：http://ato.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://bhk.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://cjb.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uqk.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cdr.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fxf.xuetiantiany.cn

TS:   path.extname("a.txt")
来源：http://qtc.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xev.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dti.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lmm.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sct.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://ajs.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bur.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tss.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://olz.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ptp.ppjwa.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pbg.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ouc.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cra.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nuq.52xcode.cn

[F12] CSV 读写
来源：http://ohk.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hod.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://piw.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fsq.ctjpmb.com

TS:   // 同上
来源：http://pfj.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vlf.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://llp.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gje.ehwqpu.com

C#:   // 无内置：用 CsvHelper 库
来源：http://aml.redwolf501.top

================================================================================
来源：http://eal.zhoulong.xyz

G. 面向对象
来源：http://qgs.yonumen.top

================================================================================
来源：http://ukn.jinqigufen.top

[G01] 定义类
来源：http://ubm.aibaodan.cn

Py:   class User: pass
来源：http://jtj.tian-w.cn

PHP:  class User {}
来源：http://uag.jqgufenzy.top

JS:   class User {}
来源：http://wkt.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://zdr.xuetiantiany.cn

Java: class User {}
来源：http://idv.tanke756.top

Go:   type User struct { Name string }
来源：http://ifu.zycfv.cn

Ruby: class User; end
来源：http://mfj.guowangkeji.top

C#:   class User {}
来源：http://nfk.jiagoushi.top

[G02] 构造函数
来源：http://knp.cucudq.cn

Py:   def __init__(self, name): self.name = name
来源：http://ldx.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://ijk.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://tpv.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://dru.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://etu.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://byl.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://evr.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://pcv.ehwqpu.com

[G03] 实例属性
来源：http://lco.chenlongwang.top

Py:   self.name = "x"
来源：http://qvo.jinyuanbaomall.cn

PHP:  public string $name = "x";
来源：http://cxl.daria6918.cn

JS:   this.name = "x";
来源：http://zux.fehbvm.com

TS:   name: string = "x";
来源：http://jkb.zhoulong.xyz

Java: private String name;
来源：http://frf.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zhs.zdbjq.cn

Ruby: @name = "x"
来源：http://apa.tanke756.top

C#:   public string Name { get; set; } = "x";
来源：http://byt.zhiwuduotai.top

[G04] 定义方法
来源：http://odp.shangyingyoupin.top

Py:   def greet(self): return self.name
来源：http://nyb.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ynb.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://tru.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://vlk.cucudq.cn

Java: String greet() { return name; }
来源：http://edv.jlsjyb.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xqp.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://ono.yvedp.cn

C#:   public string Greet() => Name;
来源：http://sey.nanxinkj.top

[G05] 继承
来源：http://kql.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://vla.tarul.cn

PHP:  class Admin extends User {}
来源：http://vql.yfazqb.com

JS:   class Admin extends User {}
来源：http://vpl.hesvh.cn

TS:   class Admin extends User {}
来源：http://gkv.jinqigufen.top

Java: class Admin extends User {}
来源：http://thz.xziqi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://itv.ppjwa.cn

Ruby: class Admin < User; end
来源：http://sqo.vqdsnc.cn

C#:   class Admin : User {}
来源：http://nli.zdqjudy.top

[G06] 重写方法
来源：http://psk.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://eqb.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vzo.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://njh.uphjek.com

TS:   greet(): string { return "admin"; }
来源：http://hpc.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://fpy.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oqs.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://fco.andypj.xyz

C#:   public override string Greet() => "admin";
来源：http://qms.hywenlv.cn

[G07] 调用父类方法
来源：http://myr.shangyingyoupin.top

Py:   super().greet()
来源：http://ufz.fktsv.cn

PHP:  parent::greet();
来源：http://ktp.andypj.xyz

JS:   super.greet();
来源：http://btq.xinyue.icu

TS:   super.greet();
来源：http://bre.quarkkingdee.top

Java: super.greet();
来源：http://dsj.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mcu.yuxming.cn

Ruby: super
来源：http://kja.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://qsk.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://hso.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xay.dianchejie.cn

PHP:  public static function f() {}
来源：http://aaq.zycfv.cn

JS:   static f() {}
来源：http://aye.hnqzz.top

TS:   static f(): void {}
来源：http://mhg.yj202588.top

Java: static void f() {}
来源：http://arw.jinyuanbaomall.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://phq.yonumen.top

Ruby: def self.f; end
来源：http://xkx.zdbjq.cn

C#:   public static void F() {}
来源：http://bza.cashguo.top

[G09] 接口 / 抽象类
来源：http://ezu.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://moo.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://bjb.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://koo.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://olo.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://bdx.shanyushiyangtech.top

Go:   type Shape interface { Area() float64 }
来源：http://ing.shzxlz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oqc.fanxiaobao.xyz

C#:   interface IShape { double Area(); }
来源：http://fvc.jianghu66.top

[G10] 访问控制
来源：http://jrc.nwbrower.top

Py:   约定 _protected / __private（不强制）
来源：http://qyu.cdnleiting.top

PHP:  public / protected / private
来源：http://igv.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://xlx.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://hoz.fengsongda.top

Java: public / protected / private / 默认包级
来源：http://gci.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xlg.zhiwuduotai.top

Ruby: public / protected / private
来源：http://xil.guannengcc.top

C#:   public / protected / private / internal
来源：http://fxd.zdbjq.cn

[G11] getter / setter
来源：http://gtr.yonumen.top

Py:   @property 与 @x.setter
来源：http://iax.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mow.cucudq.cn

JS:   get name() { return this._name; }
来源：http://fyk.sufxvd.cn

TS:   get name(): string { return this._name; }
来源：http://vdb.nwbrower.top

Java: public String getName() { return name; }
来源：http://hfx.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ewt.0kj1m.cn

Ruby: attr_accessor :name
来源：http://ohz.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://nkp.hcnkem.com

[G12] 对象转字符串
来源：http://snj.meibo888.top

Py:   def __str__(self): return self.name
来源：http://wfx.yj20258.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zmv.quarkkingdee.top

JS:   toString() { return this.name; }
来源：http://wqp.yvedp.cn

TS:   toString(): string { return this.name; }
来源：http://chb.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://nby.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gox.fehbvm.com

Ruby: def to_s; @name; end
来源：http://xel.shzxlz.cn

C#:   public override string ToString() => Name;
来源：http://rwv.smart0.xyz

[G13] 判断对象类型
来源：http://xrp.daxiang520.top

Py:   isinstance(u, User)
来源：http://vjb.bbcook.cn

PHP:  $u instanceof User
来源：http://asb.xuetiantiany.cn

JS:   u instanceof User
来源：http://eon.chenzaomai.com

TS:   u instanceof User
来源：http://oxk.jinqigfzy.top

Java: u instanceof User
来源：http://uie.c1oappe.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jrv.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://gsm.mhx1999.top

C#:   u is User
来源：http://bwl.chenjidiqi.icu

[G14] 数据类 / record
来源：http://cwk.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rja.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://yoc.52xcode.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ndj.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://utt.sxryk.cn

Java: record User(String name, int age) {}
来源：http://fuv.0kj1m.cn

Go:   type User struct { Name string; Age int }
来源：http://ylp.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vws.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://vxj.zhixingplan.top

[G15] 枚举
来源：http://vhd.nanxuanxn.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eon.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://vuc.yfazqb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://feo.gogol.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://whg.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://kct.xuanzx.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qqu.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://bpd.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nqs.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://ukt.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://flv.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://rjo.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://ccy.sysykeji.top

TS:   Object.entries(obj)
来源：http://hch.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bnv.cqqwz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dls.gzhubu.top

Ruby: obj.instance_variables
来源：http://fks.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://eak.tarul.cn

================================================================================
来源：http://fmc.sxryk.cn

H. 异常与错误处理
来源：http://uij.fanxiaobao.xyz

================================================================================
来源：http://gmm.aizwys.cn

[H01] try / catch 基础
来源：http://rkb.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ihb.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ikb.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uwn.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uol.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xiy.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pwp.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gaj.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mxl.cashguo.top

[H02] finally / ensure 收尾
来源：http://lgq.vehdjk.com

Py:   try: f()⏎finally: cleanup()
来源：http://smi.epnwcf.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://hut.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://gog.snrcjt.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xdi.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://obe.hnqzz.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://vsp.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://yxv.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mxs.yfazqb.com

[H03] 主动抛出异常
来源：http://hcn.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://jxl.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vhb.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://wax.aizwys.cn

TS:   throw new Error("错误信息");
来源：http://jpy.ctjpmb.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wia.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gas.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xih.yongpay.top

C#:   throw new ArgumentException("错误信息");
来源：http://utq.hywenlv.cn

[H04] 自定义异常类型
来源：http://jxz.ybcxt.top

Py:   class MyError(Exception): pass
来源：http://acn.chenlongwang.top

PHP:  class MyError extends RuntimeException {}
来源：http://glt.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://zwg.jinqigfzy.top

TS:   class MyError extends Error {}
来源：http://uer.fzhhl.top

Java: class MyException extends RuntimeException {}
来源：http://aym.wangdashe.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hyl.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://cvw.snrcjt.cn

C#:   class MyException : Exception {}
来源：http://klf.jianghu66.top

[H05] 捕获特定类型
来源：http://nqe.ctjpmb.com

Py:   except ValueError as e:
来源：http://zpy.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hsj.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://qgc.redwolf501.top

TS:   if (e instanceof TypeError) {}
来源：http://oan.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://kgh.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mix.hcnkem.com

Ruby: rescue ArgumentError => e
来源：http://zpq.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://asv.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://zvm.bjfxy.top

Py:   value = d.get("k") or default
来源：http://qzw.ydzc1.top

PHP:  $v = $d["k"] ?? null;
来源：http://zwz.aizwys.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jnd.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cxd.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lwd.shanyushiyangtech.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jqt.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://eui.vqdsnc.cn

C#:   obj?.A?.B ?? default
来源：http://wsu.gotoacloud.top

[H07] 断言
来源：http://mrw.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://dtg.epnwcf.com

PHP:  assert($x > 0);
来源：http://ncf.yonumen.top

JS:   console.assert(x > 0);
来源：http://roa.bjfxy.top

TS:   console.assert(x > 0);
来源：http://exn.316326.xyz

Java: assert x > 0 : "必须为正";
来源：http://jps.feifeiyinyue.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://izd.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qrv.svipenyu.cn

C#:   Debug.Assert(x > 0);
来源：http://apm.epnwcf.com

[H08] 获取错误信息与堆栈
来源：http://bkg.yueranfly.top

Py:   str(e);  traceback.format_exc()
来源：http://yok.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lhk.zhoulong.xyz

JS:   e.message;  e.stack
来源：http://voi.jiagoushi.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uys.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nze.hesvh.cn

Go:   err.Error()
来源：http://rrv.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://ciw.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://prb.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://lzm.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fgp.xziqi.cn


<!-- 参考信息 -->