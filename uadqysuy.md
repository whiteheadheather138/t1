代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mrq.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://tid.cucudq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tgl.yfazqb.com

[F04] 追加写入文件
来源：http://vxu.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sfd.gaohongyu789.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vsl.tianlin.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pof.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bmw.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eem.chenlongwang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uyf.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qzs.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://omf.yonumen.top

[F05] 判断文件或目录是否存在
来源：http://ukg.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://klg.cashguo.top

PHP:  file_exists("a.txt");
来源：http://vzj.aibaodan.cn

JS:   fs.existsSync("a.txt")
来源：http://sog.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://xnu.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vua.dianchejie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uir.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://qvu.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://rat.jlsjyb.cn

[F06] 删除文件
来源：http://bgx.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://rmd.fanxiaobao.xyz

PHP:  unlink("a.txt");
来源：http://bfc.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://whe.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rmz.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kwa.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://vqp.jinqigufen.top

Ruby: File.delete("a.txt")
来源：http://ocl.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://zhr.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://xxa.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ovk.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://reg.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffz.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cjr.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nok.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://adb.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pim.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jih.xylfe.cn

[F08] 遍历目录
来源：http://tac.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://prc.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://imw.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://vyz.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://fnn.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zun.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://cog.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://ldg.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://rle.nanxuanxn.top

[F09] 获取文件大小
来源：http://vvc.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://uoc.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://qqe.fanxiaobao.xyz

JS:   fs.statSync("a.txt").size
来源：http://mjc.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://nhh.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://ccy.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xdn.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://ajx.0kj1m.cn

C#:   new FileInfo("a.txt").Length
来源：http://omk.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://ddf.gogol.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rxy.yj202588.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bkg.jqgfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pur.zycfv.cn

TS:   path.extname("a.txt")
来源：http://rfk.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mhp.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hgr.gogol.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tne.yanxiufei.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zse.yonumen.top

[F11] 复制与移动文件
来源：http://nsl.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ude.wangdashe.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jsc.quarkkingdee.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tve.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bmk.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eec.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://swa.hnxiangtu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xff.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://esg.fktsv.cn

[F12] CSV 读写
来源：http://kmk.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zsv.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ssw.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://txk.chenjidiqi.icu

TS:   // 同上
来源：http://wnf.ydzc1.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ggn.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kfw.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iic.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dnj.cdnleiting.top

================================================================================
来源：http://pqi.feifeiyinyue.top

G. 面向对象
来源：http://pwk.bbcook.cn

================================================================================
来源：http://mej.chenzaomai.com

[G01] 定义类
来源：http://nhh.fehbvm.com

Py:   class User: pass
来源：http://kwq.ywan-chungtsiang.top

PHP:  class User {}
来源：http://sdc.hammf.cn

JS:   class User {}
来源：http://eii.zhaomingkeji.xyz

TS:   class User { name: string = ""; }
来源：http://fmk.xziqi.cn

Java: class User {}
来源：http://gch.cdnleiting.top

Go:   type User struct { Name string }
来源：http://ctu.hfpthk.cn

Ruby: class User; end
来源：http://ghs.fanxiaobao.xyz

C#:   class User {}
来源：http://wrq.zycfv.cn

[G02] 构造函数
来源：http://wud.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://zxl.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://blu.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://zmi.sxryk.cn

TS:   constructor(public name: string) {}
来源：http://ntn.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://pai.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gun.zhaomingkeji.xyz

Ruby: def initialize(name); @name = name; end
来源：http://oeg.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://dqi.xinyue.icu

[G03] 实例属性
来源：http://ngx.cucudq.cn

Py:   self.name = "x"
来源：http://gdg.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://fta.hesvh.cn

JS:   this.name = "x";
来源：http://hop.tanke756.top

TS:   name: string = "x";
来源：http://uvz.jqgufenzy.top

Java: private String name;
来源：http://nmj.hesvh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blo.cdnleiting.top

Ruby: @name = "x"
来源：http://gra.sxryk.cn

C#:   public string Name { get; set; } = "x";
来源：http://vzl.hammf.cn

[G04] 定义方法
来源：http://jgv.sufxvd.cn

Py:   def greet(self): return self.name
来源：http://gzr.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yyg.aizwys.cn

JS:   greet() { return this.name; }
来源：http://mvm.yj20258.top

TS:   greet(): string { return this.name; }
来源：http://jkr.xziqi.cn

Java: String greet() { return name; }
来源：http://gqt.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://yja.daria6918.cn

Ruby: def greet; @name; end
来源：http://arx.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://bdz.zycfv.cn

[G05] 继承
来源：http://cnd.chenlongwang.top

Py:   class Admin(User): pass
来源：http://ukz.cheryme.top

PHP:  class Admin extends User {}
来源：http://yst.snrcjt.cn

JS:   class Admin extends User {}
来源：http://qyb.ivvv.top

TS:   class Admin extends User {}
来源：http://lco.meibo888.top

Java: class Admin extends User {}
来源：http://vtj.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gvn.pycfn.com

Ruby: class Admin < User; end
来源：http://ssy.shuidangran.top

C#:   class Admin : User {}
来源：http://yso.sufxvd.cn

[G06] 重写方法
来源：http://tlx.cheryme.top

Py:   def greet(self): return "admin"
来源：http://thb.yanxiufei.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qew.c1oappe.top

JS:   greet() { return "admin"; }
来源：http://xoc.feifeiyinyue.top

TS:   greet(): string { return "admin"; }
来源：http://tao.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://klg.jianghu66.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pir.gzhubu.top

Ruby: def greet; "admin"; end
来源：http://kfd.jqgufenzy.top

C#:   public override string Greet() => "admin";
来源：http://bxh.gzhubu.top

[G07] 调用父类方法
来源：http://wmn.xuanzx.com

Py:   super().greet()
来源：http://ihh.jiagoushi.top

PHP:  parent::greet();
来源：http://bzy.bjfxy.top

JS:   super.greet();
来源：http://ssn.vqdsnc.cn

TS:   super.greet();
来源：http://yxx.xinyue.icu

Java: super.greet();
来源：http://tuy.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bjk.fehbvm.com

Ruby: super
来源：http://ojj.hysaishi.cn

C#:   base.Greet();
来源：http://clz.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://kay.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lao.fzhhl.top

PHP:  public static function f() {}
来源：http://wdg.dashuyun.cn

JS:   static f() {}
来源：http://hga.c1oappe.top

TS:   static f(): void {}
来源：http://ekr.fzhhl.top

Java: static void f() {}
来源：http://ozr.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xzb.cqqwz.cn

Ruby: def self.f; end
来源：http://spc.fzhhl.top

C#:   public static void F() {}
来源：http://yjh.epnwcf.com

[G09] 接口 / 抽象类
来源：http://jpw.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://kuw.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://spo.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://oqu.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://orh.meibo888.top

Java: interface Shape { double area(); }
来源：http://cfb.jinqigfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://dby.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://utz.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://pdz.aibaodan.cn

[G10] 访问控制
来源：http://qbq.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://oau.vehdjk.com

PHP:  public / protected / private
来源：http://sta.xylfe.cn

JS:   #private 字段；其余公开
来源：http://dpg.jqgfzy.top

TS:   public / protected / private
来源：http://cvw.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://oeh.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rlo.jyoumei.cn

Ruby: public / protected / private
来源：http://szm.smart0.xyz

C#:   public / protected / private / internal
来源：http://par.xuetiantiany.cn

[G11] getter / setter
来源：http://vnw.vehdjk.com

Py:   @property 与 @x.setter
来源：http://nre.yj20258888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vdw.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://shh.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://dhw.ivvv.top

Java: public String getName() { return name; }
来源：http://zib.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dje.yuxming.cn

Ruby: attr_accessor :name
来源：http://imw.yj20258888.top

C#:   public string Name { get; set; }
来源：http://ihm.shangyingyoupin.top

[G12] 对象转字符串
来源：http://xow.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://wuu.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://snr.wangshuangyany.cn

JS:   toString() { return this.name; }
来源：http://zhz.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://vzn.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://knc.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rsj.jlsjyb.cn

Ruby: def to_s; @name; end
来源：http://kcr.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://eql.birdmap.top

[G13] 判断对象类型
来源：http://wpo.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://dzw.cqqwz.cn

PHP:  $u instanceof User
来源：http://ulj.ctjpmb.com

JS:   u instanceof User
来源：http://pjw.hongshengwenyu.top

TS:   u instanceof User
来源：http://zzf.9152youxi.cn

Java: u instanceof User
来源：http://gwy.cheryme.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pnv.bbcook.cn

Ruby: u.is_a?(User)
来源：http://tmb.zdbjq.cn

C#:   u is User
来源：http://jrc.shangyingyoupin.top

[G14] 数据类 / record
来源：http://mus.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vsu.fehbvm.com

PHP:  // 用 readonly 属性模拟
来源：http://zoh.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://wtn.yonumen.top

TS:   type User = { name: string; age: number };
来源：http://jhs.jlsjyb.cn

Java: record User(String name, int age) {}
来源：http://ghl.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://pxf.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://amw.yuxming.cn

C#:   record User(string Name, int Age);
来源：http://zkh.yfazqb.com

[G15] 枚举
来源：http://aie.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ufj.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dca.chenjidiqi.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qgf.haohaochexian.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yhg.shangyingyoupin.top

Java: enum Color { RED, GREEN }
来源：http://idu.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fbl.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://dxj.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yms.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://ztm.kuanghao11.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qxs.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://thh.xuanzx.com

JS:   Object.entries(obj)
来源：http://eyb.meibo888.top

TS:   Object.entries(obj)
来源：http://hdf.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ibd.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sqb.shzxlz.cn

Ruby: obj.instance_variables
来源：http://dkk.yongpay.top

C#:   // 用反射或 System.Text.Json
来源：http://wun.cucudq.cn

================================================================================
来源：http://bex.pengpengdd.cyou

H. 异常与错误处理
来源：http://jqp.pengpengdd.cyou

================================================================================
来源：http://ndh.aizwys.cn

[H01] try / catch 基础
来源：http://fkx.meibo888.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lzk.hysaishi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vuj.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ddk.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bgs.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xrp.sufxvd.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://czo.c1oappe.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blm.svipenyu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yuk.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://gzv.52xcode.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tvl.vehdjk.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://tsg.dianchejie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ggu.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vwo.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dpq.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ohc.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://sty.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ael.9152youxi.cn

[H03] 主动抛出异常
来源：http://bei.havefunace.top

Py:   raise ValueError("错误信息")
来源：http://vze.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eie.tanke756.top

JS:   throw new Error("错误信息");
来源：http://szi.meibo888.top

TS:   throw new Error("错误信息");
来源：http://lbw.cdnleiting.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://aox.hywenlv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ilc.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lxg.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://nhc.shzxlz.cn

[H04] 自定义异常类型
来源：http://wsr.havefunace.top

Py:   class MyError(Exception): pass
来源：http://nel.ivvv.top

PHP:  class MyError extends RuntimeException {}
来源：http://ofr.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://kal.havefunace.top

TS:   class MyError extends Error {}
来源：http://yqg.cqqwz.cn

Java: class MyException extends RuntimeException {}
来源：http://abk.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zlx.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://lel.xuetiantiany.cn

C#:   class MyException : Exception {}
来源：http://mgs.tian-w.cn

[H05] 捕获特定类型
来源：http://fqi.jqgfzy.top

Py:   except ValueError as e:
来源：http://kuk.hywenlv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ive.feifeiyinyue.top

JS:   if (e instanceof TypeError) {}
来源：http://uhh.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://gwd.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://wno.snrcjt.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://akq.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://tbe.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blf.ehwqpu.com

[H06] 可选值 / 空值安全访问
来源：http://rwk.redwolf501.top

Py:   value = d.get("k") or default
来源：http://euk.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://mfz.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://bgo.jinyuanbaomall.cn

TS:   obj?.a?.b;  d ?? default
来源：http://czj.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gnq.jinghuilouyu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nvl.ppjwa.cn

Ruby: d&.dig(:a, :b)
来源：http://efj.tarul.cn

C#:   obj?.A?.B ?? default
来源：http://xjz.quarkkingdee.top

[H07] 断言
来源：http://nyy.svipenyu.cn

Py:   assert x > 0, "必须为正"
来源：http://ygx.sjlbkw.cn

PHP:  assert($x > 0);
来源：http://jfi.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://and.ywan-chungtsiang.top

TS:   console.assert(x > 0);
来源：http://odn.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://lfa.sysykeji.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mzq.jiagoushi.top

Ruby: raise "必须为正" unless x > 0
来源：http://kul.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://rse.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://vww.hcnkem.com

Py:   str(e);  traceback.format_exc()
来源：http://mrk.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ywr.chenlongwang.top


<!-- 参考信息 -->