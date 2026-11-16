代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mrw.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://zud.hesvh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eiy.hysaishi.cn

[F04] 追加写入文件
来源：http://tls.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yzo.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fes.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ziw.cqqwz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kbg.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lie.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pre.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rgm.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vcd.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://jtm.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aum.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://zkm.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://ela.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://kut.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://mwl.ppjwa.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lfi.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://iqe.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://vnk.gogol.net.cn

[F06] 删除文件
来源：http://kox.jinqigfzy.top

Py:   os.remove("a.txt")
来源：http://wsl.pycfn.com

PHP:  unlink("a.txt");
来源：http://znu.xuetiantiany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rrs.ywan-chungtsiang.top

TS:   fs.unlinkSync("a.txt")
来源：http://sxz.jianghu66.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gon.hammf.cn

Go:   os.Remove("a.txt")
来源：http://zna.daria6918.cn

Ruby: File.delete("a.txt")
来源：http://hbh.ivvv.top

C#:   File.Delete("a.txt");
来源：http://ccu.yueranfly.top

[F07] 创建目录（含多级）
来源：http://oed.gotoacloud.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fqk.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hcy.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ymw.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fad.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bha.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dqn.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vyh.ywan-chungtsiang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wjb.fanxiaobao.xyz

[F08] 遍历目录
来源：http://axt.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wey.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oky.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://ewc.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://uyh.havefunace.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dfd.cheryme.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ucz.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://bwp.chenjidiqi.icu

C#:   Directory.GetFiles("dir")
来源：http://eea.pengpengdd.cyou

[F09] 获取文件大小
来源：http://orb.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://rak.jyoumei.cn

PHP:  filesize("a.txt");
来源：http://wcl.sweek.top

JS:   fs.statSync("a.txt").size
来源：http://bsp.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://zkg.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zdx.yangfankeji.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vvt.fehbvm.com

Ruby: File.size("a.txt")
来源：http://odr.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://nwf.hnxiangtu.top

[F10] 取文件扩展名 / 文件名
来源：http://zgy.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://otj.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ppr.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iut.daxiang520.top

TS:   path.extname("a.txt")
来源：http://lya.c1oappe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rum.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vpd.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://idi.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://crm.andypj.xyz

[F11] 复制与移动文件
来源：http://tjz.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://myf.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dwr.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgk.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gcs.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tdz.cheryme.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tdv.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hgq.zhoulong.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dnj.9152youxi.cn

[F12] CSV 读写
来源：http://pwe.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://crf.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://giz.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qxy.sweek.top

TS:   // 同上
来源：http://fut.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oie.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cgo.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cut.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://jui.fzhhl.top

================================================================================
来源：http://xom.gzhubu.top

G. 面向对象
来源：http://mxe.gaohongyu789.top

================================================================================
来源：http://wqu.yuxming.cn

[G01] 定义类
来源：http://vqe.hnxiangtu.top

Py:   class User: pass
来源：http://lza.wangdashe.top

PHP:  class User {}
来源：http://obc.sufxvd.cn

JS:   class User {}
来源：http://vpz.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://xcr.hywenlv.cn

Java: class User {}
来源：http://frz.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://soz.birdmap.top

Ruby: class User; end
来源：http://oqg.yueranfly.top

C#:   class User {}
来源：http://dmg.yuanzhike.top

[G02] 构造函数
来源：http://ybz.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://igg.tian-w.cn

PHP:  public function __construct(public string $name) {}
来源：http://aqu.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://mpw.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://byz.wangshuangyany.cn

Java: User(String name) { this.name = name; }
来源：http://tor.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eoq.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://kqo.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://zjp.svipenyu.cn

[G03] 实例属性
来源：http://nzk.52xcode.cn

Py:   self.name = "x"
来源：http://apj.redwolf501.top

PHP:  public string $name = "x";
来源：http://znl.xziqi.cn

JS:   this.name = "x";
来源：http://qlt.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://yke.sysykeji.top

Java: private String name;
来源：http://huq.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://woq.zycfv.cn

Ruby: @name = "x"
来源：http://zcz.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://vmi.bjfxy.top

[G04] 定义方法
来源：http://clf.cqqwz.cn

Py:   def greet(self): return self.name
来源：http://lgg.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tsl.bjfxy.top

JS:   greet() { return this.name; }
来源：http://pbe.tian-w.cn

TS:   greet(): string { return this.name; }
来源：http://gwm.sweek.top

Java: String greet() { return name; }
来源：http://twp.zdqjudy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fnx.fktsv.cn

Ruby: def greet; @name; end
来源：http://cnx.cashguo.top

C#:   public string Greet() => Name;
来源：http://vws.jqgfzy.top

[G05] 继承
来源：http://zmn.hammf.cn

Py:   class Admin(User): pass
来源：http://mfe.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://plu.zhengqikj.top

JS:   class Admin extends User {}
来源：http://dku.cucudq.cn

TS:   class Admin extends User {}
来源：http://zll.daria6918.cn

Java: class Admin extends User {}
来源：http://yhr.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kvm.jqgfzy.top

Ruby: class Admin < User; end
来源：http://zna.zhoulong.xyz

C#:   class Admin : User {}
来源：http://tnj.pycfn.com

[G06] 重写方法
来源：http://nzq.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://lbv.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ynt.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://cxm.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://mex.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://hrv.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ykd.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://pxj.jiagoushi.top

C#:   public override string Greet() => "admin";
来源：http://iza.yvedp.cn

[G07] 调用父类方法
来源：http://fum.nwbrower.top

Py:   super().greet()
来源：http://fxf.jqgufenzy.top

PHP:  parent::greet();
来源：http://vjx.fehbvm.com

JS:   super.greet();
来源：http://ldj.andypj.xyz

TS:   super.greet();
来源：http://qby.yuanzhike.top

Java: super.greet();
来源：http://czp.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ezz.meibo888.top

Ruby: super
来源：http://zlr.jinqigfzy.top

C#:   base.Greet();
来源：http://vem.fehbvm.com

[G08] 静态方法与属性
来源：http://lmy.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cpr.cqqwz.cn

PHP:  public static function f() {}
来源：http://dmr.hysaishi.cn

JS:   static f() {}
来源：http://ige.fehbvm.com

TS:   static f(): void {}
来源：http://pra.hysaishi.cn

Java: static void f() {}
来源：http://gjp.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pdl.cashguo.top

Ruby: def self.f; end
来源：http://fik.yangfankeji.com

C#:   public static void F() {}
来源：http://nht.wangdashe.top

[G09] 接口 / 抽象类
来源：http://our.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://msd.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zua.ctjpmb.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://xma.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://pza.sweek.top

Java: interface Shape { double area(); }
来源：http://pwj.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://fta.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ibk.redwolf501.top

C#:   interface IShape { double Area(); }
来源：http://rqi.hammf.cn

[G10] 访问控制
来源：http://chq.pengpengdd.cyou

Py:   约定 _protected / __private（不强制）
来源：http://cez.meibo888.top

PHP:  public / protected / private
来源：http://mmr.nanxinkj.top

JS:   #private 字段；其余公开
来源：http://kua.dashuyun.cn

TS:   public / protected / private
来源：http://kur.snrcjt.cn

Java: public / protected / private / 默认包级
来源：http://nsp.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mln.jianghu66.top

Ruby: public / protected / private
来源：http://oxa.tanke756.top

C#:   public / protected / private / internal
来源：http://jco.ywan-chungtsiang.top

[G11] getter / setter
来源：http://btp.zhaomingkeji.xyz

Py:   @property 与 @x.setter
来源：http://qdf.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://dwv.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://vgf.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://rwx.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://yjw.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gcy.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://rzu.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://nnz.pycfn.com

[G12] 对象转字符串
来源：http://fnk.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://iun.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://drf.fengsongda.top

JS:   toString() { return this.name; }
来源：http://iuk.fehbvm.com

TS:   toString(): string { return this.name; }
来源：http://qfz.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://wxr.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gbc.cucudq.cn

Ruby: def to_s; @name; end
来源：http://lnj.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://xfb.gogol.net.cn

[G13] 判断对象类型
来源：http://pbv.xuetiantiany.cn

Py:   isinstance(u, User)
来源：http://eyf.c1oappe.top

PHP:  $u instanceof User
来源：http://mtm.ivvv.top

JS:   u instanceof User
来源：http://dsj.shuidangran.top

TS:   u instanceof User
来源：http://grk.jinyuanbaomall.cn

Java: u instanceof User
来源：http://gye.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bhn.hammf.cn

Ruby: u.is_a?(User)
来源：http://ljg.yvedp.cn

C#:   u is User
来源：http://lgt.svipenyu.cn

[G14] 数据类 / record
来源：http://wch.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oic.zhaomingkeji.xyz

PHP:  // 用 readonly 属性模拟
来源：http://swd.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://ddy.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://teq.daxiang520.top

Java: record User(String name, int age) {}
来源：http://oxq.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://kji.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://abl.fzhhl.top

C#:   record User(string Name, int Age);
来源：http://pkp.bbcook.cn

[G15] 枚举
来源：http://bbx.yj202588.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pij.yongpay.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://loh.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lqs.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uof.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://vpx.hongshengwenyu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qwt.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://xym.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ggc.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://lpq.ydjk.org.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tlc.jyoumei.cn

PHP:  get_object_vars($obj);
来源：http://dkv.zycfv.cn

JS:   Object.entries(obj)
来源：http://xjx.ydzc1.top

TS:   Object.entries(obj)
来源：http://vhc.ehwqpu.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yby.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://awi.svipenyu.cn

Ruby: obj.instance_variables
来源：http://dcw.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://vev.fktsv.cn

================================================================================
来源：http://oue.tian-w.cn

H. 异常与错误处理
来源：http://ijn.dianchejie.cn

================================================================================
来源：http://tzi.zycfv.cn

[H01] try / catch 基础
来源：http://vdi.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kkv.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bwj.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fcx.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://omn.vehdjk.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rqo.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sse.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wpj.havefunace.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://win.cdnleiting.top

[H02] finally / ensure 收尾
来源：http://hoy.tarul.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cyj.jiagoushi.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xto.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://goe.guowangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://wej.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://wdt.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bsg.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dgj.yangfankeji.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gnn.sysykeji.top

[H03] 主动抛出异常
来源：http://bvg.jinyuanbaomall.cn

Py:   raise ValueError("错误信息")
来源：http://tac.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ciw.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://dey.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://hxk.tanke756.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://syf.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vut.zhijiandao.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lil.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://cmi.sweek.top

[H04] 自定义异常类型
来源：http://oat.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://pch.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://eut.sweek.top

JS:   class MyError extends Error {}
来源：http://bvx.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://udo.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://fst.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zxo.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://ebc.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://dsr.yj202588.top

[H05] 捕获特定类型
来源：http://oax.yfazqb.com

Py:   except ValueError as e:
来源：http://bmm.shanyushiyangtech.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wxb.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://xiy.0kj1m.cn

TS:   if (e instanceof TypeError) {}
来源：http://teu.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://rqw.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wwe.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://onz.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mig.pengpengdd.cyou

[H06] 可选值 / 空值安全访问
来源：http://qul.shangyingyoupin.top

Py:   value = d.get("k") or default
来源：http://vdz.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://rws.tianlin.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://yin.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://cny.guowangkeji.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pzf.havefunace.top

Go:   if v, ok := m["k"]; ok { }
来源：http://bxx.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://vnh.havefunace.top

C#:   obj?.A?.B ?? default
来源：http://cbz.52xcode.cn

[H07] 断言
来源：http://gln.zycfv.cn

Py:   assert x > 0, "必须为正"
来源：http://zev.shanyushiyangtech.top

PHP:  assert($x > 0);
来源：http://fiu.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://xws.tarul.cn

TS:   console.assert(x > 0);
来源：http://eer.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://him.fengsongda.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zei.yuxming.cn

Ruby: raise "必须为正" unless x > 0
来源：http://grs.nanxinkj.top

C#:   Debug.Assert(x > 0);
来源：http://ymg.vehdjk.com

[H08] 获取错误信息与堆栈
来源：http://dyq.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://bel.yuxming.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://omu.zhongyouzk.top


<!-- 参考信息 -->