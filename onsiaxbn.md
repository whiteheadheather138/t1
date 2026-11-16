代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://yxy.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yjs.bbcook.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gik.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xjw.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jdr.zhixingplan.top

Ruby: File.write("a.txt", "hi")
来源：http://xyw.birdmap.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dbw.dianchejie.cn

[F04] 追加写入文件
来源：http://bpk.hongshengwenyu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lpa.shuidangran.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zhr.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ton.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfe.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nub.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://veq.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://odv.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mvx.cashguo.top

[F05] 判断文件或目录是否存在
来源：http://tbq.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://adx.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://jem.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://wik.haohaochexian.top

TS:   fs.existsSync("a.txt")
来源：http://rod.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://ftd.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zvl.cashguo.top

Ruby: File.exist?("a.txt")
来源：http://iby.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://lax.tian-w.cn

[F06] 删除文件
来源：http://cyf.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://vtj.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://jmo.sxryk.cn

JS:   fs.unlinkSync("a.txt")
来源：http://djs.gaohongyu789.top

TS:   fs.unlinkSync("a.txt")
来源：http://hcf.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cpw.aizwys.cn

Go:   os.Remove("a.txt")
来源：http://ogi.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://rpr.zhaomingkeji.xyz

C#:   File.Delete("a.txt");
来源：http://gyt.smart0.xyz

[F07] 创建目录（含多级）
来源：http://xkr.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cah.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yaw.sufxvd.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vbn.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vwt.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://njs.yfazqb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dqv.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hmk.zhongyouzk.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rfi.nanxinkj.top

[F08] 遍历目录
来源：http://puf.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://qdf.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dcj.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://gqd.zhixingplan.top

TS:   fs.readdirSync("dir")
来源：http://xum.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gis.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iie.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://xel.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://gbp.yangfankeji.com

[F09] 获取文件大小
来源：http://niv.zycfv.cn

Py:   os.path.getsize("a.txt")
来源：http://ver.c1oappe.top

PHP:  filesize("a.txt");
来源：http://bbm.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://pfh.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://kok.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iwp.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://phn.shangyingyoupin.top

Ruby: File.size("a.txt")
来源：http://rhj.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://bmi.feifeiyinyue.top

[F10] 取文件扩展名 / 文件名
来源：http://qml.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bhs.zhengqikj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://twq.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://twr.tarul.cn

TS:   path.extname("a.txt")
来源：http://ybd.tanke756.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vti.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gbu.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zyr.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fnv.ydzc1.top

[F11] 复制与移动文件
来源：http://sdg.yuxming.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bpe.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gpj.zhiwuduotai.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dei.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ktl.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eei.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ohr.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://guc.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xln.tarul.cn

[F12] CSV 读写
来源：http://rkq.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nnw.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lah.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aml.fanxiaobao.xyz

TS:   // 同上
来源：http://qfm.ctjpmb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dye.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uuj.316326.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mzt.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ess.sxryk.cn

================================================================================
来源：http://qbr.hongshengwenyu.top

G. 面向对象
来源：http://alm.pycfn.com

================================================================================
来源：http://itd.ybcxt.top

[G01] 定义类
来源：http://rna.feifeiyinyue.top

Py:   class User: pass
来源：http://xfm.hammf.cn

PHP:  class User {}
来源：http://hwo.yj20258888.top

JS:   class User {}
来源：http://vzg.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://ofn.gzhubu.top

Java: class User {}
来源：http://vby.wangdashe.top

Go:   type User struct { Name string }
来源：http://nkb.xuetiantiany.cn

Ruby: class User; end
来源：http://kbb.yongpay.top

C#:   class User {}
来源：http://xnn.yuxming.cn

[G02] 构造函数
来源：http://wfn.nwbrower.top

Py:   def __init__(self, name): self.name = name
来源：http://elw.bjfxy.top

PHP:  public function __construct(public string $name) {}
来源：http://fkz.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://smm.chenzaomai.com

TS:   constructor(public name: string) {}
来源：http://ctm.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://vod.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nzd.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://eth.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://kes.ydjk.org.cn

[G03] 实例属性
来源：http://non.smart0.xyz

Py:   self.name = "x"
来源：http://dxa.yonumen.top

PHP:  public string $name = "x";
来源：http://xzu.hesvh.cn

JS:   this.name = "x";
来源：http://wqv.ppjwa.cn

TS:   name: string = "x";
来源：http://rbn.shanyushiyangkeji.top

Java: private String name;
来源：http://fpn.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hwj.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://zqc.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://rox.jinqigufen.top

[G04] 定义方法
来源：http://yfd.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://aea.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://sug.yuxming.cn

JS:   greet() { return this.name; }
来源：http://pru.yj20258888.top

TS:   greet(): string { return this.name; }
来源：http://acb.0kj1m.cn

Java: String greet() { return name; }
来源：http://ukn.yueranfly.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uzh.zdbjq.cn

Ruby: def greet; @name; end
来源：http://pre.chenlongwang.top

C#:   public string Greet() => Name;
来源：http://bby.wangdashe.top

[G05] 继承
来源：http://pdv.ybcxt.top

Py:   class Admin(User): pass
来源：http://uyo.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://yag.bjfxy.top

JS:   class Admin extends User {}
来源：http://cph.sxryk.cn

TS:   class Admin extends User {}
来源：http://tuh.yongpay.top

Java: class Admin extends User {}
来源：http://bzq.yonumen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sgg.nanxuanxn.top

Ruby: class Admin < User; end
来源：http://fas.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://ucg.zhaomingkeji.xyz

[G06] 重写方法
来源：http://rju.zycfv.cn

Py:   def greet(self): return "admin"
来源：http://meu.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://gqk.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://jfn.ppjwa.cn

TS:   greet(): string { return "admin"; }
来源：http://lvo.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://tvw.daxiang520.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bso.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://onj.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://xpm.chenjidiqi.icu

[G07] 调用父类方法
来源：http://xyk.wangdashe.top

Py:   super().greet()
来源：http://wkl.jqgufenzy.top

PHP:  parent::greet();
来源：http://awa.shanyushiyangtech.top

JS:   super.greet();
来源：http://dlz.zycfv.cn

TS:   super.greet();
来源：http://jup.zhixingplan.top

Java: super.greet();
来源：http://ioq.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uvc.sjlbkw.cn

Ruby: super
来源：http://hja.hnxiangtu.top

C#:   base.Greet();
来源：http://epu.yongpay.top

[G08] 静态方法与属性
来源：http://dnw.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qrs.ybcxt.top

PHP:  public static function f() {}
来源：http://faz.316326.xyz

JS:   static f() {}
来源：http://zwe.cucudq.cn

TS:   static f(): void {}
来源：http://khi.hcnkem.com

Java: static void f() {}
来源：http://nen.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vfo.jianghu66.top

Ruby: def self.f; end
来源：http://rbn.quarkkingdee.top

C#:   public static void F() {}
来源：http://zvf.daxiang520.top

[G09] 接口 / 抽象类
来源：http://oot.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://lrn.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zsk.zdbjq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rys.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://zgb.nwbrower.top

Java: interface Shape { double area(); }
来源：http://yhj.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://jli.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ten.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://hqa.yvedp.cn

[G10] 访问控制
来源：http://hua.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://owf.sxryk.cn

PHP:  public / protected / private
来源：http://okv.hesvh.cn

JS:   #private 字段；其余公开
来源：http://wpn.fehbvm.com

TS:   public / protected / private
来源：http://hng.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://fkh.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pyk.jyoumei.cn

Ruby: public / protected / private
来源：http://ttf.zdbjq.cn

C#:   public / protected / private / internal
来源：http://vgq.uphjek.com

[G11] getter / setter
来源：http://imm.ybcxt.top

Py:   @property 与 @x.setter
来源：http://tul.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xab.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://ckc.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://hrj.ivvv.top

Java: public String getName() { return name; }
来源：http://rll.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xyo.cashguo.top

Ruby: attr_accessor :name
来源：http://weh.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://yhv.uphjek.com

[G12] 对象转字符串
来源：http://oko.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://uzj.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://awy.fktsv.cn

JS:   toString() { return this.name; }
来源：http://xtw.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://imt.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://shb.yfazqb.com

Go:   func (u User) String() string { return u.Name }
来源：http://mdy.ydzc1.top

Ruby: def to_s; @name; end
来源：http://pbh.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://zvd.xziqi.cn

[G13] 判断对象类型
来源：http://yzx.daria6918.cn

Py:   isinstance(u, User)
来源：http://xmg.jqgufenzy.top

PHP:  $u instanceof User
来源：http://uov.kuanghao11.cn

JS:   u instanceof User
来源：http://orp.zdqjudy.top

TS:   u instanceof User
来源：http://bzz.shanyushiyangkeji.top

Java: u instanceof User
来源：http://gyo.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hou.sxryk.cn

Ruby: u.is_a?(User)
来源：http://twd.hesvh.cn

C#:   u is User
来源：http://ppt.meibo888.top

[G14] 数据类 / record
来源：http://voc.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://out.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://lhe.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cpa.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://gwu.yfazqb.com

Java: record User(String name, int age) {}
来源：http://ari.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://nqu.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lpw.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://tku.hysaishi.cn

[G15] 枚举
来源：http://aru.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mkg.zhijiandao.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ack.sufxvd.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pqc.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hgt.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://qet.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mjr.shzxlz.cn

Ruby: Color = %i[red green].freeze
来源：http://mcg.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hxd.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://fwx.hcnkem.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yqr.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://fcd.wangdashe.top

JS:   Object.entries(obj)
来源：http://zoy.cashguo.top

TS:   Object.entries(obj)
来源：http://adl.xinyue.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xwu.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yrr.316326.xyz

Ruby: obj.instance_variables
来源：http://wcm.fktsv.cn

C#:   // 用反射或 System.Text.Json
来源：http://zxd.zdbjq.cn

================================================================================
来源：http://xig.chenlongwang.top

H. 异常与错误处理
来源：http://xuo.gzhubu.top

================================================================================
来源：http://fij.sysykeji.top

[H01] try / catch 基础
来源：http://pqp.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tjk.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rkm.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pzu.yonumen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vje.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ubu.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kif.cheryme.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lxv.316326.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://omk.yueranfly.top

[H02] finally / ensure 收尾
来源：http://pzq.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://yld.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zgu.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://eih.52xcode.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cpl.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://yso.xuanzx.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwq.ybcxt.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pdk.yvedp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qfa.yanxiufei.cn

[H03] 主动抛出异常
来源：http://bja.yongpay.top

Py:   raise ValueError("错误信息")
来源：http://kwf.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blb.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://mnu.birdmap.top

TS:   throw new Error("错误信息");
来源：http://buy.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nxy.meibo888.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hld.epnwcf.com

Ruby: raise ArgumentError, "错误信息"
来源：http://kjn.yuanzhike.top

C#:   throw new ArgumentException("错误信息");
来源：http://uoy.sxryk.cn

[H04] 自定义异常类型
来源：http://seh.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://dke.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qbo.pycfn.com

JS:   class MyError extends Error {}
来源：http://fya.hammf.cn

TS:   class MyError extends Error {}
来源：http://pea.0kj1m.cn

Java: class MyException extends RuntimeException {}
来源：http://byt.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ohg.xziqi.cn

Ruby: class MyError < StandardError; end
来源：http://xxo.9152youxi.cn

C#:   class MyException : Exception {}
来源：http://vdk.cqqwz.cn

[H05] 捕获特定类型
来源：http://ygk.52xcode.cn

Py:   except ValueError as e:
来源：http://lei.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lgr.zhongyouzk.top

JS:   if (e instanceof TypeError) {}
来源：http://upc.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://que.hywenlv.cn

Java: catch (IOException | SQLException e) {}
来源：http://fyz.hongshengwenyu.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iqq.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://pqa.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tvy.ydzc1.top

[H06] 可选值 / 空值安全访问
来源：http://cxc.tarul.cn

Py:   value = d.get("k") or default
来源：http://bqw.xziqi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mrx.bbcook.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tpy.kuanghao11.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pax.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vrh.hesvh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qyd.vehdjk.com

Ruby: d&.dig(:a, :b)
来源：http://wqm.fktsv.cn

C#:   obj?.A?.B ?? default
来源：http://opa.ivvv.top

[H07] 断言
来源：http://lry.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://kgc.yuxming.cn

PHP:  assert($x > 0);
来源：http://cop.yj202588.top

JS:   console.assert(x > 0);
来源：http://jwt.shzxlz.cn

TS:   console.assert(x > 0);
来源：http://rsf.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://kak.quarkkingdee.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qrx.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zzo.dashuyun.cn


<!-- 参考信息 -->