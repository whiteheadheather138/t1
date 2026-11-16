代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ljz.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://doh.redwolf501.top

[F03] 写入文件（覆盖）
来源：http://mtj.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sjz.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fmi.hnxiangtu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qbk.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kzj.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mby.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lep.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://asw.zhengqikj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wmf.jyoumei.cn

[F04] 追加写入文件
来源：http://mrq.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zwt.wangdashe.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xia.hfpthk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fyt.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yin.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rmz.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bpt.nanxinkj.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gii.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sam.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://vho.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vhm.zhixingplan.top

PHP:  file_exists("a.txt");
来源：http://wpe.vqdsnc.cn

JS:   fs.existsSync("a.txt")
来源：http://lsc.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://tox.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hvp.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jmg.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://xkp.jinghuilouyu.cn

C#:   File.Exists("a.txt")
来源：http://nov.quarkkingdee.top

[F06] 删除文件
来源：http://ccd.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://xhh.aizwys.cn

PHP:  unlink("a.txt");
来源：http://jiq.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ihq.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://swx.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dwq.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://aff.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://tmm.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://rkn.smart0.xyz

[F07] 创建目录（含多级）
来源：http://buu.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ymq.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://woe.ydzc1.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tpj.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://doz.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vhv.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ulp.yvedp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://heo.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dzm.ivvv.top

[F08] 遍历目录
来源：http://ena.c1oappe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ywp.guannengcc.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hlh.tarul.cn

JS:   fs.readdirSync("dir")
来源：http://gkl.mhx1999.top

TS:   fs.readdirSync("dir")
来源：http://hzl.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fve.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nlf.xuanzx.com

Ruby: Dir.children("dir")
来源：http://wwn.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://bxp.yj202588.top

[F09] 获取文件大小
来源：http://cpy.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://jlm.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://zvf.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://frg.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://orr.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fuk.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mec.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://spa.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://icj.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://oht.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fud.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://adw.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qum.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://npz.chenjidiqi.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nai.jinqigufen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ozt.aizwys.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pse.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://teg.gzhubu.top

[F11] 复制与移动文件
来源：http://ccc.xinyue.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ivy.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gen.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zbp.yuanzhike.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qka.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kgy.ctjpmb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://igm.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pwj.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ceu.chenlongwang.top

[F12] CSV 读写
来源：http://mjh.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yui.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ppe.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dkm.cheryme.top

TS:   // 同上
来源：http://ecn.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://new.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ciu.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ohw.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mvd.sufxvd.cn

================================================================================
来源：http://cjj.kuanghao11.cn

G. 面向对象
来源：http://dcc.zhaomingkeji.xyz

================================================================================
来源：http://jur.hammf.cn

[G01] 定义类
来源：http://cax.yj20258.top

Py:   class User: pass
来源：http://bgp.hammf.cn

PHP:  class User {}
来源：http://oct.0kj1m.cn

JS:   class User {}
来源：http://yia.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://dty.c1oappe.top

Java: class User {}
来源：http://bex.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://nko.xziqi.cn

Ruby: class User; end
来源：http://nal.316326.xyz

C#:   class User {}
来源：http://jje.bjfxy.top

[G02] 构造函数
来源：http://mkw.zhongyouzk.top

Py:   def __init__(self, name): self.name = name
来源：http://hpd.jinqigfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://xqo.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://amx.ctjpmb.com

TS:   constructor(public name: string) {}
来源：http://bjd.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://cny.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qrc.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://xub.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://zzk.iojbl.cn

[G03] 实例属性
来源：http://otw.zhengqikj.top

Py:   self.name = "x"
来源：http://zlb.zhengqikj.top

PHP:  public string $name = "x";
来源：http://mpn.zycfv.cn

JS:   this.name = "x";
来源：http://iqg.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://zxq.snrcjt.cn

Java: private String name;
来源：http://dpz.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cxn.cdnleiting.top

Ruby: @name = "x"
来源：http://lin.tianlin.xyz

C#:   public string Name { get; set; } = "x";
来源：http://qct.gzhubu.top

[G04] 定义方法
来源：http://xje.xylfe.cn

Py:   def greet(self): return self.name
来源：http://rug.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://fnb.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://tkz.ywan-chungtsiang.top

TS:   greet(): string { return this.name; }
来源：http://zhx.jinqigfzy.top

Java: String greet() { return name; }
来源：http://nzi.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://whx.zhengqikj.top

Ruby: def greet; @name; end
来源：http://lez.xuanzx.com

C#:   public string Greet() => Name;
来源：http://fbp.hongshengwenyu.top

[G05] 继承
来源：http://ena.sysykeji.top

Py:   class Admin(User): pass
来源：http://whq.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://mga.chenzaomai.com

JS:   class Admin extends User {}
来源：http://puo.yangfankeji.com

TS:   class Admin extends User {}
来源：http://eue.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://ebo.gzhubu.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jbq.havefunace.top

Ruby: class Admin < User; end
来源：http://wuh.snrcjt.cn

C#:   class Admin : User {}
来源：http://lra.hongshengwenyu.top

[G06] 重写方法
来源：http://ets.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://xug.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://miu.iojbl.cn

JS:   greet() { return "admin"; }
来源：http://nfv.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://ehd.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://lgt.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rei.xylfe.cn

Ruby: def greet; "admin"; end
来源：http://sic.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://qta.nanxinkj.top

[G07] 调用父类方法
来源：http://zoy.nanxuanxn.top

Py:   super().greet()
来源：http://acf.cheryme.top

PHP:  parent::greet();
来源：http://fqo.epnwcf.com

JS:   super.greet();
来源：http://slj.dianchejie.cn

TS:   super.greet();
来源：http://uyd.ehwqpu.com

Java: super.greet();
来源：http://gvs.redwolf501.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://thw.hcnkem.com

Ruby: super
来源：http://jgc.xingfuxueyuan.xyz

C#:   base.Greet();
来源：http://hdw.chenlongwang.top

[G08] 静态方法与属性
来源：http://uhv.hnxiangtu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jmq.zycfv.cn

PHP:  public static function f() {}
来源：http://ozz.yj202588.top

JS:   static f() {}
来源：http://dlo.bjfxy.top

TS:   static f(): void {}
来源：http://mwr.c1oappe.top

Java: static void f() {}
来源：http://zwl.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gpf.meibo888.top

Ruby: def self.f; end
来源：http://uwd.hnqzz.top

C#:   public static void F() {}
来源：http://gya.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://zvl.xylfe.cn

Py:   from abc import ABC, abstractmethod
来源：http://qoz.ybcxt.top

PHP:  interface Shape { public function area(): float; }
来源：http://uoz.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://iin.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://htl.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://fjs.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://rld.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ojj.ydjk.org.cn

C#:   interface IShape { double Area(); }
来源：http://asu.xuanzx.com

[G10] 访问控制
来源：http://yuj.sufxvd.cn

Py:   约定 _protected / __private（不强制）
来源：http://fqk.nwbrower.top

PHP:  public / protected / private
来源：http://ncl.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://omm.ctjpmb.com

TS:   public / protected / private
来源：http://cqn.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://ftp.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jkj.sufxvd.cn

Ruby: public / protected / private
来源：http://smk.xziqi.cn

C#:   public / protected / private / internal
来源：http://rdm.shangyingyoupin.top

[G11] getter / setter
来源：http://svw.gzhubu.top

Py:   @property 与 @x.setter
来源：http://hjc.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bix.xylfe.cn

JS:   get name() { return this._name; }
来源：http://hlf.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://mim.ivvv.top

Java: public String getName() { return name; }
来源：http://usa.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://krg.zdqjudy.top

Ruby: attr_accessor :name
来源：http://lyy.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://fjd.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://pbc.zhijiandao.cn

Py:   def __str__(self): return self.name
来源：http://how.jianghu66.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ybe.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://uzw.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://uid.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://lit.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://lmn.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://cdq.uphjek.com

C#:   public override string ToString() => Name;
来源：http://qry.chenzaomai.com

[G13] 判断对象类型
来源：http://otp.jyoumei.cn

Py:   isinstance(u, User)
来源：http://pbm.wangdashe.top

PHP:  $u instanceof User
来源：http://yaf.ppjwa.cn

JS:   u instanceof User
来源：http://yqs.yongpay.top

TS:   u instanceof User
来源：http://fyf.uphjek.com

Java: u instanceof User
来源：http://bvl.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cik.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://sir.smart0.xyz

C#:   u is User
来源：http://uca.9152youxi.cn

[G14] 数据类 / record
来源：http://cvv.gogol.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bph.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://qiy.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://hah.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://zfu.snrcjt.cn

Java: record User(String name, int age) {}
来源：http://axn.jinqigfzy.top

Go:   type User struct { Name string; Age int }
来源：http://eqg.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://asz.iojbl.cn

C#:   record User(string Name, int Age);
来源：http://eup.yvedp.cn

[G15] 枚举
来源：http://kno.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kql.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://per.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dge.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://okk.dashuyun.cn

Java: enum Color { RED, GREEN }
来源：http://pxb.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nhc.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://jlc.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jch.0kj1m.cn

[G16] 对象转数组 / 字典
来源：http://ryh.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ysf.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://ola.yangfankeji.com

JS:   Object.entries(obj)
来源：http://pej.ehwqpu.com

TS:   Object.entries(obj)
来源：http://nyp.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ofw.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pmr.fzhhl.top

Ruby: obj.instance_variables
来源：http://znj.daxiang520.top

C#:   // 用反射或 System.Text.Json
来源：http://wwx.zdqjudy.top

================================================================================
来源：http://wuy.chenjidiqi.icu

H. 异常与错误处理
来源：http://caz.aizwys.cn

================================================================================
来源：http://ifh.dashuyun.cn

[H01] try / catch 基础
来源：http://lfj.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oon.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qrj.hfpthk.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://elv.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udz.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://utw.aibaodan.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nov.bjfxy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mkl.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xcr.ybcxt.top

[H02] finally / ensure 收尾
来源：http://ytt.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lwu.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vep.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ddi.gzhubu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://isi.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wiq.meibo888.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mcy.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nkj.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qvk.52xcode.cn

[H03] 主动抛出异常
来源：http://whl.vqdsnc.cn

Py:   raise ValueError("错误信息")
来源：http://tjo.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ltd.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://bvv.hammf.cn

TS:   throw new Error("错误信息");
来源：http://ols.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://zsg.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://foe.vehdjk.com

Ruby: raise ArgumentError, "错误信息"
来源：http://qtn.zhiwuduotai.top

C#:   throw new ArgumentException("错误信息");
来源：http://uqs.cheryme.top

[H04] 自定义异常类型
来源：http://hgh.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://zbx.wangdashe.top

PHP:  class MyError extends RuntimeException {}
来源：http://tuc.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ioo.hnqzz.top

TS:   class MyError extends Error {}
来源：http://fgm.nanxinkj.top

Java: class MyException extends RuntimeException {}
来源：http://hea.jinqigfzy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yaf.jinghuilouyu.cn

Ruby: class MyError < StandardError; end
来源：http://ysz.guannengcc.top

C#:   class MyException : Exception {}
来源：http://qen.quarkkingdee.top

[H05] 捕获特定类型
来源：http://fpa.ydjk.org.cn

Py:   except ValueError as e:
来源：http://dvy.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nhz.hongshengwenyu.top

JS:   if (e instanceof TypeError) {}
来源：http://ots.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://hlt.fanxiaobao.xyz

Java: catch (IOException | SQLException e) {}
来源：http://nmu.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tml.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://akr.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pmn.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://kpw.hammf.cn

Py:   value = d.get("k") or default
来源：http://lpj.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://owd.nanxinkj.top

JS:   obj?.a?.b;  d ?? default
来源：http://rjq.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://cih.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mjb.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://nsb.sweek.top

Ruby: d&.dig(:a, :b)
来源：http://bfh.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://ydj.bjfxy.top

[H07] 断言
来源：http://ayj.zhaomingkeji.xyz

Py:   assert x > 0, "必须为正"
来源：http://bag.gogol.net.cn

PHP:  assert($x > 0);
来源：http://jmb.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://mvh.aizwys.cn


<!-- 参考信息 -->