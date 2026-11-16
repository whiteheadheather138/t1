代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://yqo.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mhw.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://kes.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://ngr.meibo888.top

TS:   fs.existsSync("a.txt")
来源：http://zaf.daxiang520.top

Java: Files.exists(Path.of("a.txt"))
来源：http://akp.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kls.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://osa.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://ans.nwbrower.top

[F06] 删除文件
来源：http://ifu.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://jfo.ybcxt.top

PHP:  unlink("a.txt");
来源：http://yjc.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://oqa.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://owj.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bug.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://bby.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://egv.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://kxh.yj20258888.top

[F07] 创建目录（含多级）
来源：http://uhw.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xes.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rds.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rgd.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://awx.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qbz.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mpy.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rmr.gzhubu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yfe.jinghuilouyu.cn

[F08] 遍历目录
来源：http://okt.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kby.tianlin.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ehf.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://cxr.kuanghao11.cn

TS:   fs.readdirSync("dir")
来源：http://qpx.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://atg.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://stj.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://iky.meibo888.top

C#:   Directory.GetFiles("dir")
来源：http://kgl.cucudq.cn

[F09] 获取文件大小
来源：http://tgt.daria6918.cn

Py:   os.path.getsize("a.txt")
来源：http://zwa.yfazqb.com

PHP:  filesize("a.txt");
来源：http://cpo.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://jjn.bjfxy.top

TS:   fs.statSync("a.txt").size
来源：http://jid.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://dno.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fdf.epnwcf.com

Ruby: File.size("a.txt")
来源：http://qri.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://uvr.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://qkk.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ben.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gwg.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rig.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://zrq.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://swx.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://iao.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lru.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aah.sjlbkw.cn

[F11] 复制与移动文件
来源：http://khz.quarkkingdee.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zfb.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zoe.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://egw.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nly.haohaochexian.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dww.xziqi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zeo.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vda.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fmj.zhongyouzk.top

[F12] CSV 读写
来源：http://bgh.hysaishi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://chp.ybcxt.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yqg.ppjwa.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://coj.vehdjk.com

TS:   // 同上
来源：http://xec.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://isx.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rjz.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://seb.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://edg.quarkkingdee.top

================================================================================
来源：http://aje.jianghu66.top

G. 面向对象
来源：http://kbq.pengpengdd.cyou

================================================================================
来源：http://ryt.kuanghao11.cn

[G01] 定义类
来源：http://mcb.nanxinkj.top

Py:   class User: pass
来源：http://rhv.fanxiaobao.xyz

PHP:  class User {}
来源：http://hmv.kuanghao11.cn

JS:   class User {}
来源：http://uxj.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://lzj.birdmap.top

Java: class User {}
来源：http://wvu.meibo888.top

Go:   type User struct { Name string }
来源：http://ukf.shanyushiyangtech.top

Ruby: class User; end
来源：http://mof.jyoumei.cn

C#:   class User {}
来源：http://vfn.cheryme.top

[G02] 构造函数
来源：http://udw.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://acr.mhx1999.top

PHP:  public function __construct(public string $name) {}
来源：http://ojv.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://iul.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://zbu.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://jgh.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oiy.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://yog.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://zbc.ppjwa.cn

[G03] 实例属性
来源：http://cbx.haohaochexian.top

Py:   self.name = "x"
来源：http://qov.smart0.xyz

PHP:  public string $name = "x";
来源：http://lpv.redwolf501.top

JS:   this.name = "x";
来源：http://ftl.jinghuilouyu.cn

TS:   name: string = "x";
来源：http://bki.xziqi.cn

Java: private String name;
来源：http://gqx.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sga.nanxinkj.top

Ruby: @name = "x"
来源：http://sil.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://cfc.yonumen.top

[G04] 定义方法
来源：http://xrf.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://chq.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://qtg.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://wuz.birdmap.top

TS:   greet(): string { return this.name; }
来源：http://psg.andypj.xyz

Java: String greet() { return name; }
来源：http://cup.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vpp.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://tnd.xinyue.icu

C#:   public string Greet() => Name;
来源：http://kme.zhijiandao.cn

[G05] 继承
来源：http://pfi.fktsv.cn

Py:   class Admin(User): pass
来源：http://rfq.yongpay.top

PHP:  class Admin extends User {}
来源：http://vka.mhx1999.top

JS:   class Admin extends User {}
来源：http://kdd.316326.xyz

TS:   class Admin extends User {}
来源：http://apf.mhx1999.top

Java: class Admin extends User {}
来源：http://tnn.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://okh.316326.xyz

Ruby: class Admin < User; end
来源：http://uun.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://iof.sweek.top

[G06] 重写方法
来源：http://nkz.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://qzb.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://apy.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://wtr.gotoacloud.top

TS:   greet(): string { return "admin"; }
来源：http://jel.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://twu.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fbq.tanke756.top

Ruby: def greet; "admin"; end
来源：http://wbz.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://zul.hammf.cn

[G07] 调用父类方法
来源：http://van.kuanghao11.cn

Py:   super().greet()
来源：http://xqi.zdbjq.cn

PHP:  parent::greet();
来源：http://urj.jianghu66.top

JS:   super.greet();
来源：http://afq.dashuyun.cn

TS:   super.greet();
来源：http://gnd.yongpay.top

Java: super.greet();
来源：http://dkt.yuxming.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://asc.wangdashe.top

Ruby: super
来源：http://mfy.ivvv.top

C#:   base.Greet();
来源：http://fap.kuanghao11.cn

[G08] 静态方法与属性
来源：http://zgy.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://upc.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://ufb.andypj.xyz

JS:   static f() {}
来源：http://yrf.shzxlz.cn

TS:   static f(): void {}
来源：http://ysn.tianlin.xyz

Java: static void f() {}
来源：http://uyj.yanxiufei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jvv.xylfe.cn

Ruby: def self.f; end
来源：http://wgd.haohaochexian.top

C#:   public static void F() {}
来源：http://jtz.gzhubu.top

[G09] 接口 / 抽象类
来源：http://gub.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://htc.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fpe.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lvf.0kj1m.cn

TS:   interface Shape { area(): number; }
来源：http://ybq.316326.xyz

Java: interface Shape { double area(); }
来源：http://xel.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://ioi.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zzw.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://gqz.quarkkingdee.top

[G10] 访问控制
来源：http://tps.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://jkx.ydjk.org.cn

PHP:  public / protected / private
来源：http://sbs.yonumen.top

JS:   #private 字段；其余公开
来源：http://tzc.316326.xyz

TS:   public / protected / private
来源：http://itq.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://noa.jinghuilouyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://alt.hcnkem.com

Ruby: public / protected / private
来源：http://mnz.xinyue.icu

C#:   public / protected / private / internal
来源：http://egz.sjlbkw.cn

[G11] getter / setter
来源：http://swk.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://wgl.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://yrd.andypj.xyz

JS:   get name() { return this._name; }
来源：http://bhn.hongshengwenyu.top

TS:   get name(): string { return this._name; }
来源：http://dwf.cdnleiting.top

Java: public String getName() { return name; }
来源：http://cva.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lgr.sysykeji.top

Ruby: attr_accessor :name
来源：http://sif.jqgfzy.top

C#:   public string Name { get; set; }
来源：http://pke.pycfn.com

[G12] 对象转字符串
来源：http://atx.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://aun.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ise.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://yaz.yanxiufei.cn

TS:   toString(): string { return this.name; }
来源：http://umz.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://kov.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kng.cheryme.top

Ruby: def to_s; @name; end
来源：http://nof.daria6918.cn

C#:   public override string ToString() => Name;
来源：http://fav.yuxming.cn

[G13] 判断对象类型
来源：http://fpy.hfpthk.cn

Py:   isinstance(u, User)
来源：http://xod.fktsv.cn

PHP:  $u instanceof User
来源：http://rxe.0kj1m.cn

JS:   u instanceof User
来源：http://wre.vehdjk.com

TS:   u instanceof User
来源：http://uic.havefunace.top

Java: u instanceof User
来源：http://ggu.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cwj.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://nat.iojbl.cn

C#:   u is User
来源：http://dia.yj20258888.top

[G14] 数据类 / record
来源：http://nzw.shzxlz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://goe.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://vdt.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fem.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://emz.daxiang520.top

Java: record User(String name, int age) {}
来源：http://iwt.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://yoo.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bps.xingfuxueyuan.xyz

C#:   record User(string Name, int Age);
来源：http://gac.chenjidiqi.icu

[G15] 枚举
来源：http://efi.fengsongda.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vwp.hongshengwenyu.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://atk.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jqu.ivvv.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://smd.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://sow.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tnt.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://tzd.nanxuanxn.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qnb.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://xxb.nwbrower.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rsd.birdmap.top

PHP:  get_object_vars($obj);
来源：http://ngz.daria6918.cn

JS:   Object.entries(obj)
来源：http://erw.9152youxi.cn

TS:   Object.entries(obj)
来源：http://skr.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://prc.9152youxi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fis.ehwqpu.com

Ruby: obj.instance_variables
来源：http://rxv.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://hel.hywenlv.cn

================================================================================
来源：http://ugo.c1oappe.top

H. 异常与错误处理
来源：http://ksl.nwbrower.top

================================================================================
来源：http://ood.tianlin.xyz

[H01] try / catch 基础
来源：http://lfe.sjlbkw.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qwn.hfpthk.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xtp.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yvi.kuanghao11.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hbc.ivvv.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dzx.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eim.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pla.jianghu66.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dvj.fanxiaobao.xyz

[H02] finally / ensure 收尾
来源：http://ahq.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://gel.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cfz.yanxiufei.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hwj.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dtm.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://yqe.iojbl.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qpw.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cdq.tarul.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gvv.zhengqikj.top

[H03] 主动抛出异常
来源：http://niy.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://whj.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://clc.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://xbi.9152youxi.cn

TS:   throw new Error("错误信息");
来源：http://ijc.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jal.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xmk.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jeh.yvedp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zqz.shuidangran.top

[H04] 自定义异常类型
来源：http://ala.yonumen.top

Py:   class MyError(Exception): pass
来源：http://vts.hesvh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://slj.gogol.net.cn

JS:   class MyError extends Error {}
来源：http://wmk.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://yfx.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://gwy.fengsongda.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tmo.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://umu.jqgufenzy.top

C#:   class MyException : Exception {}
来源：http://lva.nwbrower.top

[H05] 捕获特定类型
来源：http://uid.ehwqpu.com

Py:   except ValueError as e:
来源：http://zru.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fxl.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://jan.yuxming.cn

TS:   if (e instanceof TypeError) {}
来源：http://htn.gzhubu.top

Java: catch (IOException | SQLException e) {}
来源：http://kuv.xingfuxueyuan.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://teh.yfazqb.com

Ruby: rescue ArgumentError => e
来源：http://ueu.zhijiandao.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ivy.aibaodan.cn

[H06] 可选值 / 空值安全访问
来源：http://yuk.tanke756.top

Py:   value = d.get("k") or default
来源：http://omq.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mxr.jlsjyb.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cdo.zhengqikj.top

TS:   obj?.a?.b;  d ?? default
来源：http://uwp.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ojp.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bxa.fehbvm.com

Ruby: d&.dig(:a, :b)
来源：http://umm.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://xqu.hfpthk.cn

[H07] 断言
来源：http://wsf.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://fxb.yonumen.top

PHP:  assert($x > 0);
来源：http://vqk.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://pji.jlsjyb.cn

TS:   console.assert(x > 0);
来源：http://edh.bjfxy.top

Java: assert x > 0 : "必须为正";
来源：http://wlx.ydzc1.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rab.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://gkd.tanke756.top

C#:   Debug.Assert(x > 0);
来源：http://mvg.guannengcc.top

[H08] 获取错误信息与堆栈
来源：http://uio.redwolf501.top

Py:   str(e);  traceback.format_exc()
来源：http://gft.shuidangran.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pgk.yj202588.top

JS:   e.message;  e.stack
来源：http://vum.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://gxm.hammf.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://arm.fktsv.cn

Go:   err.Error()
来源：http://aqw.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://hoi.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://zvp.tanke756.top

[H09] 带错误码的异常
来源：http://rzk.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iyp.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cde.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gxx.jinghuilouyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pcl.vehdjk.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gst.yuxming.cn


<!-- 参考信息 -->