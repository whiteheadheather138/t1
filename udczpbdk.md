代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://yts.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xej.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://raz.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jrb.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kne.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://ubv.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wpy.yonumen.top

[F04] 追加写入文件
来源：http://wvd.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pdv.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ttf.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofo.fengsongda.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ivu.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dpi.0kj1m.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://psw.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ajf.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zls.bjfxy.top

[F05] 判断文件或目录是否存在
来源：http://evs.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lxl.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://srr.yuanzhike.top

JS:   fs.existsSync("a.txt")
来源：http://oll.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://yfn.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tjs.hammf.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cjz.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://sns.pycfn.com

C#:   File.Exists("a.txt")
来源：http://kwb.yfazqb.com

[F06] 删除文件
来源：http://pyf.mhx1999.top

Py:   os.remove("a.txt")
来源：http://bxc.hammf.cn

PHP:  unlink("a.txt");
来源：http://xjk.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://clt.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://qef.sysykeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bme.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://wgb.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://guf.vqdsnc.cn

C#:   File.Delete("a.txt");
来源：http://yec.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://cqn.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zmt.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tkb.yueranfly.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xrr.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxi.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rmb.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zrj.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cfa.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://res.snrcjt.cn

[F08] 遍历目录
来源：http://slb.smart0.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ijb.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://efg.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://lxe.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://zhd.zhongyouzk.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ebm.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://cmx.havefunace.top

Ruby: Dir.children("dir")
来源：http://jub.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://auc.pycfn.com

[F09] 获取文件大小
来源：http://mwr.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://oei.yvedp.cn

PHP:  filesize("a.txt");
来源：http://frz.zhongyouzk.top

JS:   fs.statSync("a.txt").size
来源：http://ykb.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://rmj.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://lya.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fnp.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://sso.wangdashe.top

C#:   new FileInfo("a.txt").Length
来源：http://kok.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://uzp.hcnkem.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qto.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eie.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zva.jinghuilouyu.cn

TS:   path.extname("a.txt")
来源：http://gtw.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hhq.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yes.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nnn.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://piq.cdnleiting.top

[F11] 复制与移动文件
来源：http://dpp.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://coh.tian-w.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dye.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szu.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nep.guowangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ksa.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jsu.gaohongyu789.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ipj.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ufi.cdnleiting.top

[F12] CSV 读写
来源：http://iuw.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://asa.hnxiangtu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qni.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sme.shzxlz.cn

TS:   // 同上
来源：http://jrg.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ueo.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vvs.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gio.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pvl.xingfuxueyuan.xyz

================================================================================
来源：http://ios.mhx1999.top

G. 面向对象
来源：http://kkf.ppjwa.cn

================================================================================
来源：http://aap.mhx1999.top

[G01] 定义类
来源：http://mcf.cashguo.top

Py:   class User: pass
来源：http://yxu.sysykeji.top

PHP:  class User {}
来源：http://oqa.jyoumei.cn

JS:   class User {}
来源：http://wde.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://ysq.nwbrower.top

Java: class User {}
来源：http://aww.sysykeji.top

Go:   type User struct { Name string }
来源：http://tfw.ehwqpu.com

Ruby: class User; end
来源：http://zfe.tanke756.top

C#:   class User {}
来源：http://fnc.yuanzhike.top

[G02] 构造函数
来源：http://jmd.hysaishi.cn

Py:   def __init__(self, name): self.name = name
来源：http://hlj.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://whw.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://ijt.yfazqb.com

TS:   constructor(public name: string) {}
来源：http://cpg.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://frt.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oev.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://qzf.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://jhp.ehwqpu.com

[G03] 实例属性
来源：http://iag.jqgufenzy.top

Py:   self.name = "x"
来源：http://uso.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://ldw.tanke756.top

JS:   this.name = "x";
来源：http://bar.sxryk.cn

TS:   name: string = "x";
来源：http://yfz.haohaochexian.top

Java: private String name;
来源：http://dph.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://avc.kuanghao11.cn

Ruby: @name = "x"
来源：http://yoy.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://wvd.quarkkingdee.top

[G04] 定义方法
来源：http://ugg.guannengcc.top

Py:   def greet(self): return self.name
来源：http://far.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rko.daxiang520.top

JS:   greet() { return this.name; }
来源：http://bfp.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://ski.birdmap.top

Java: String greet() { return name; }
来源：http://cwn.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://qvx.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://lqq.xziqi.cn

C#:   public string Greet() => Name;
来源：http://lgy.yuxming.cn

[G05] 继承
来源：http://tpm.jqgfzy.top

Py:   class Admin(User): pass
来源：http://ptl.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://jdc.zdbjq.cn

JS:   class Admin extends User {}
来源：http://jng.zdqjudy.top

TS:   class Admin extends User {}
来源：http://ubq.dashuyun.cn

Java: class Admin extends User {}
来源：http://xuy.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qpe.fehbvm.com

Ruby: class Admin < User; end
来源：http://sjz.cashguo.top

C#:   class Admin : User {}
来源：http://xjy.fehbvm.com

[G06] 重写方法
来源：http://ozl.uphjek.com

Py:   def greet(self): return "admin"
来源：http://svu.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xig.xziqi.cn

JS:   greet() { return "admin"; }
来源：http://kzl.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://dgc.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://bmw.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iar.meibo888.top

Ruby: def greet; "admin"; end
来源：http://dhb.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://ssa.ppjwa.cn

[G07] 调用父类方法
来源：http://lno.feifeiyinyue.top

Py:   super().greet()
来源：http://hnx.yongpay.top

PHP:  parent::greet();
来源：http://etp.fehbvm.com

JS:   super.greet();
来源：http://vgd.yongpay.top

TS:   super.greet();
来源：http://dey.zhaomingkeji.xyz

Java: super.greet();
来源：http://igx.tianlin.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://htn.guowangkeji.top

Ruby: super
来源：http://xgt.daria6918.cn

C#:   base.Greet();
来源：http://ljc.meibo888.top

[G08] 静态方法与属性
来源：http://yrx.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uak.nanxuanxn.top

PHP:  public static function f() {}
来源：http://wyy.fanxiaobao.xyz

JS:   static f() {}
来源：http://ngi.gzhubu.top

TS:   static f(): void {}
来源：http://xth.sufxvd.cn

Java: static void f() {}
来源：http://czr.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jsk.fengsongda.top

Ruby: def self.f; end
来源：http://umc.jyoumei.cn

C#:   public static void F() {}
来源：http://hdb.tianlin.xyz

[G09] 接口 / 抽象类
来源：http://loj.epnwcf.com

Py:   from abc import ABC, abstractmethod
来源：http://uov.bbcook.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pjw.cheryme.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cnz.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://fua.cdnleiting.top

Java: interface Shape { double area(); }
来源：http://qdb.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://nkt.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fol.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://osa.vqdsnc.cn

[G10] 访问控制
来源：http://eqt.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://zkk.hcnkem.com

PHP:  public / protected / private
来源：http://bpw.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://wqi.xziqi.cn

TS:   public / protected / private
来源：http://pvl.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://dsc.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xkj.zhengqikj.top

Ruby: public / protected / private
来源：http://pda.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://zhv.vqdsnc.cn

[G11] getter / setter
来源：http://afd.gzhubu.top

Py:   @property 与 @x.setter
来源：http://efp.birdmap.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oei.nwbrower.top

JS:   get name() { return this._name; }
来源：http://ubk.havefunace.top

TS:   get name(): string { return this._name; }
来源：http://wxn.9152youxi.cn

Java: public String getName() { return name; }
来源：http://vyk.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gtj.yvedp.cn

Ruby: attr_accessor :name
来源：http://eqx.fehbvm.com

C#:   public string Name { get; set; }
来源：http://ixa.sjlbkw.cn

[G12] 对象转字符串
来源：http://blr.yj202588.top

Py:   def __str__(self): return self.name
来源：http://skg.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://nsd.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://cna.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://ots.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://ats.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://cml.zhongyouzk.top

Ruby: def to_s; @name; end
来源：http://qeq.epnwcf.com

C#:   public override string ToString() => Name;
来源：http://vef.zhijiandao.cn

[G13] 判断对象类型
来源：http://dqr.havefunace.top

Py:   isinstance(u, User)
来源：http://fze.jqgfzy.top

PHP:  $u instanceof User
来源：http://dbm.xylfe.cn

JS:   u instanceof User
来源：http://vpu.yuxming.cn

TS:   u instanceof User
来源：http://fgf.zhoulong.xyz

Java: u instanceof User
来源：http://kyx.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qkw.andypj.xyz

Ruby: u.is_a?(User)
来源：http://ity.pengpengdd.cyou

C#:   u is User
来源：http://ioa.jlsjyb.cn

[G14] 数据类 / record
来源：http://ksv.wangdashe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pnl.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://fkh.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://jzq.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://tkm.xingfuxueyuan.xyz

Java: record User(String name, int age) {}
来源：http://ryz.uphjek.com

Go:   type User struct { Name string; Age int }
来源：http://dnp.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gdl.chenjidiqi.icu

C#:   record User(string Name, int Age);
来源：http://wbp.fzhhl.top

[G15] 枚举
来源：http://smd.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bxb.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tbn.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ddy.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://igv.haohaochexian.top

Java: enum Color { RED, GREEN }
来源：http://wdi.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bfl.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://opr.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xld.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://yvx.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aoa.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://anr.sweek.top

JS:   Object.entries(obj)
来源：http://loo.xylfe.cn

TS:   Object.entries(obj)
来源：http://ddp.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zyc.chenjidiqi.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://nri.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://zft.zhixingplan.top

C#:   // 用反射或 System.Text.Json
来源：http://ujo.smart0.xyz

================================================================================
来源：http://jeq.zhixingplan.top

H. 异常与错误处理
来源：http://dlo.aibaodan.cn

================================================================================
来源：http://jql.nwbrower.top

[H01] try / catch 基础
来源：http://ewh.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://juy.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zwg.cucudq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nws.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://geo.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zyt.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cne.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oga.zycfv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xov.yj202588.top

[H02] finally / ensure 收尾
来源：http://ahi.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ncx.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://iql.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://lyc.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xoe.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://wmp.jqgufenzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwm.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cek.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qjy.aizwys.cn

[H03] 主动抛出异常
来源：http://pcx.tianlin.xyz

Py:   raise ValueError("错误信息")
来源：http://ogc.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cun.hysaishi.cn

JS:   throw new Error("错误信息");
来源：http://sym.hongshengwenyu.top

TS:   throw new Error("错误信息");
来源：http://twm.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hio.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bqu.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://lzv.hnxiangtu.top

C#:   throw new ArgumentException("错误信息");
来源：http://kvb.gaohongyu789.top

[H04] 自定义异常类型
来源：http://ewu.yj202588.top

Py:   class MyError(Exception): pass
来源：http://zzv.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://jjj.mhx1999.top

JS:   class MyError extends Error {}
来源：http://nyn.cheryme.top

TS:   class MyError extends Error {}
来源：http://hwp.sysykeji.top

Java: class MyException extends RuntimeException {}
来源：http://uxt.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jqw.fzhhl.top

Ruby: class MyError < StandardError; end
来源：http://dan.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://vtj.316326.xyz

[H05] 捕获特定类型
来源：http://lvf.gzhubu.top

Py:   except ValueError as e:
来源：http://svc.yuxming.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://byf.jyoumei.cn

JS:   if (e instanceof TypeError) {}
来源：http://kaw.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://rbp.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://smf.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kle.hfpthk.cn

Ruby: rescue ArgumentError => e
来源：http://anf.gotoacloud.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jdp.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://cvv.andypj.xyz

Py:   value = d.get("k") or default
来源：http://gun.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://ybw.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://owt.fengsongda.top

TS:   obj?.a?.b;  d ?? default
来源：http://naw.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fvy.quarkkingdee.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fdq.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://icj.hnqzz.top

C#:   obj?.A?.B ?? default
来源：http://pkn.bbcook.cn

[H07] 断言
来源：http://zgb.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://aqk.hcnkem.com

PHP:  assert($x > 0);
来源：http://tjt.pycfn.com

JS:   console.assert(x > 0);
来源：http://epm.sxryk.cn

TS:   console.assert(x > 0);
来源：http://oqc.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://jup.shanyushiyangtech.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hkw.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://yga.cashguo.top


<!-- 参考信息 -->