代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://hpp.haohaochexian.top

[F02] 逐行读取文件
来源：http://ncn.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vho.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oit.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ibf.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vwb.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cbs.vehdjk.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xgd.c1oappe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tdg.chenlongwang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dbq.yj202588.top

[F03] 写入文件（覆盖）
来源：http://qoh.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://btd.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zag.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oyf.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bkj.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ywe.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ytq.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://tfi.jqgufenzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nhl.hcnkem.com

[F04] 追加写入文件
来源：http://chu.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://itd.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://asy.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://beo.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdn.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ymk.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ihp.dianchejie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qro.bjfxy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rfv.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://xop.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dxp.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://dfq.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://dfu.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://gig.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ikr.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mts.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://fmp.yj20258.top

C#:   File.Exists("a.txt")
来源：http://zcm.c1oappe.top

[F06] 删除文件
来源：http://wpb.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://ytz.nwbrower.top

PHP:  unlink("a.txt");
来源：http://jdx.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://von.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://oyg.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mbs.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://vxk.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://fst.chenjidiqi.icu

C#:   File.Delete("a.txt");
来源：http://afe.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://xsv.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yad.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://apy.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ywb.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://adz.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vqq.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dsn.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aac.sufxvd.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kcg.sxryk.cn

[F08] 遍历目录
来源：http://afb.zdqjudy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rtl.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eow.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://qtr.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://lmc.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pno.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ino.yvedp.cn

Ruby: Dir.children("dir")
来源：http://nea.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://oof.zdqjudy.top

[F09] 获取文件大小
来源：http://okl.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://fel.hongshengwenyu.top

PHP:  filesize("a.txt");
来源：http://zvz.sxryk.cn

JS:   fs.statSync("a.txt").size
来源：http://bde.yj20258.top

TS:   fs.statSync("a.txt").size
来源：http://mpz.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://fqm.zycfv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kaz.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://xjq.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://gfv.zhaomingkeji.xyz

[F10] 取文件扩展名 / 文件名
来源：http://lmg.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oiz.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dtv.zycfv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pda.mhx1999.top

TS:   path.extname("a.txt")
来源：http://ygu.ppjwa.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yuz.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vcx.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bdf.jlsjyb.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gys.ctjpmb.com

[F11] 复制与移动文件
来源：http://kik.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://msh.dashuyun.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://elh.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bpq.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wuo.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mky.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lmx.yuanzhike.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bdl.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vii.tarul.cn

[F12] CSV 读写
来源：http://fwv.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qih.cucudq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gwc.ehwqpu.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pwh.xingfuxueyuan.xyz

TS:   // 同上
来源：http://gjk.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zll.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kcb.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dwc.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://orz.xuetiantiany.cn

================================================================================
来源：http://utb.wangdashe.top

G. 面向对象
来源：http://aek.birdmap.top

================================================================================
来源：http://hkj.shzxlz.cn

[G01] 定义类
来源：http://hsu.xuetiantiany.cn

Py:   class User: pass
来源：http://lfn.fanxiaobao.xyz

PHP:  class User {}
来源：http://qve.daria6918.cn

JS:   class User {}
来源：http://vuz.tarul.cn

TS:   class User { name: string = ""; }
来源：http://kof.zhiwuduotai.top

Java: class User {}
来源：http://sld.tanke756.top

Go:   type User struct { Name string }
来源：http://kba.jiagoushi.top

Ruby: class User; end
来源：http://sit.yongpay.top

C#:   class User {}
来源：http://usd.snrcjt.cn

[G02] 构造函数
来源：http://phx.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://rer.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://ynq.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://wap.tarul.cn

TS:   constructor(public name: string) {}
来源：http://czc.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://gru.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ggq.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://rri.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://rfz.quarkkingdee.top

[G03] 实例属性
来源：http://uxi.jqgfzy.top

Py:   self.name = "x"
来源：http://jxs.chenjidiqi.icu

PHP:  public string $name = "x";
来源：http://wjl.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://kjl.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://kpc.jianghu66.top

Java: private String name;
来源：http://uia.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vks.yfazqb.com

Ruby: @name = "x"
来源：http://omo.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://apn.jianghu66.top

[G04] 定义方法
来源：http://ohf.fehbvm.com

Py:   def greet(self): return self.name
来源：http://vqk.bbcook.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gfd.bbcook.cn

JS:   greet() { return this.name; }
来源：http://aon.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://lvz.daria6918.cn

Java: String greet() { return name; }
来源：http://ieu.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sng.zycfv.cn

Ruby: def greet; @name; end
来源：http://ozp.52xcode.cn

C#:   public string Greet() => Name;
来源：http://olk.daria6918.cn

[G05] 继承
来源：http://iva.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://xlj.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://zqc.epnwcf.com

JS:   class Admin extends User {}
来源：http://alf.xylfe.cn

TS:   class Admin extends User {}
来源：http://hse.yj20258.top

Java: class Admin extends User {}
来源：http://ttd.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ryv.dianchejie.cn

Ruby: class Admin < User; end
来源：http://ozo.yuxming.cn

C#:   class Admin : User {}
来源：http://qqh.jqgfzy.top

[G06] 重写方法
来源：http://sun.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://vck.hcnkem.com

PHP:  public function greet(): string { return "admin"; }
来源：http://wzb.sweek.top

JS:   greet() { return "admin"; }
来源：http://ndt.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://mwt.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://dwo.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://coq.hammf.cn

Ruby: def greet; "admin"; end
来源：http://vjx.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://wxc.uphjek.com

[G07] 调用父类方法
来源：http://llq.hammf.cn

Py:   super().greet()
来源：http://vfd.bjfxy.top

PHP:  parent::greet();
来源：http://fhb.zhongyouzk.top

JS:   super.greet();
来源：http://sej.vqdsnc.cn

TS:   super.greet();
来源：http://las.sjlbkw.cn

Java: super.greet();
来源：http://let.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xqz.nanxuanxn.top

Ruby: super
来源：http://ogo.dashuyun.cn

C#:   base.Greet();
来源：http://zqm.yangfankeji.com

[G08] 静态方法与属性
来源：http://vzb.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lfp.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://kva.dianchejie.cn

JS:   static f() {}
来源：http://xwq.ydzc1.top

TS:   static f(): void {}
来源：http://juy.fanxiaobao.xyz

Java: static void f() {}
来源：http://elw.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://qti.gotoacloud.top

Ruby: def self.f; end
来源：http://ktq.hnqzz.top

C#:   public static void F() {}
来源：http://qnr.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://tje.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://gme.52xcode.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qbt.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tjl.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://uvf.tian-w.cn

Java: interface Shape { double area(); }
来源：http://nck.52xcode.cn

Go:   type Shape interface { Area() float64 }
来源：http://ecy.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwb.snrcjt.cn

C#:   interface IShape { double Area(); }
来源：http://lzg.quarkkingdee.top

[G10] 访问控制
来源：http://plm.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://maw.xuanzx.com

PHP:  public / protected / private
来源：http://bot.yueranfly.top

JS:   #private 字段；其余公开
来源：http://hin.shzxlz.cn

TS:   public / protected / private
来源：http://rjg.pycfn.com

Java: public / protected / private / 默认包级
来源：http://lit.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://sek.yj20258888.top

Ruby: public / protected / private
来源：http://sxg.yonumen.top

C#:   public / protected / private / internal
来源：http://dqb.bbcook.cn

[G11] getter / setter
来源：http://nea.ybcxt.top

Py:   @property 与 @x.setter
来源：http://wrq.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zvw.bbcook.cn

JS:   get name() { return this._name; }
来源：http://adg.sysykeji.top

TS:   get name(): string { return this._name; }
来源：http://odq.shuidangran.top

Java: public String getName() { return name; }
来源：http://kid.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://yxs.bjfxy.top

Ruby: attr_accessor :name
来源：http://qxu.zhengqikj.top

C#:   public string Name { get; set; }
来源：http://eey.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://jgp.cheryme.top

Py:   def __str__(self): return self.name
来源：http://ria.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://wlh.ehwqpu.com

JS:   toString() { return this.name; }
来源：http://url.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://xvj.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://kqo.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://mxo.yongpay.top

Ruby: def to_s; @name; end
来源：http://azy.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://drp.cashguo.top

[G13] 判断对象类型
来源：http://nlm.nanxuanxn.top

Py:   isinstance(u, User)
来源：http://vzn.zhijiandao.cn

PHP:  $u instanceof User
来源：http://wsv.jqgfzy.top

JS:   u instanceof User
来源：http://qrz.chenjidiqi.icu

TS:   u instanceof User
来源：http://jtv.hfpthk.cn

Java: u instanceof User
来源：http://mli.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://wqh.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://etc.yuanzhike.top

C#:   u is User
来源：http://ryd.fktsv.cn

[G14] 数据类 / record
来源：http://cfx.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kgg.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://tvj.chenzaomai.com

JS:   // 无内置：普通类或对象字面量
来源：http://byx.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://zxa.xinyue.icu

Java: record User(String name, int age) {}
来源：http://kjg.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://onr.gotoacloud.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qrf.meibo888.top

C#:   record User(string Name, int Age);
来源：http://vrl.yanxiufei.cn

[G15] 枚举
来源：http://voq.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qah.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gyk.gotoacloud.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zvd.fengsongda.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aap.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://gzu.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ujk.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://zzf.9152youxi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dcc.nanxinkj.top

[G16] 对象转数组 / 字典
来源：http://lkf.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rmv.cheryme.top

PHP:  get_object_vars($obj);
来源：http://ljh.ehwqpu.com

JS:   Object.entries(obj)
来源：http://ldv.fengsongda.top

TS:   Object.entries(obj)
来源：http://igv.tarul.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cls.fzhhl.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jxw.svipenyu.cn

Ruby: obj.instance_variables
来源：http://mim.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://ged.hfpthk.cn

================================================================================
来源：http://nob.zhengqikj.top

H. 异常与错误处理
来源：http://omc.meibo888.top

================================================================================
来源：http://vjf.zycfv.cn

[H01] try / catch 基础
来源：http://ios.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fmf.daria6918.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dfn.jinyuanbaomall.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://shd.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://avl.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uid.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://caz.jqgfzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kbl.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yej.gaohongyu789.top

[H02] finally / ensure 收尾
来源：http://wgz.daxiang520.top

Py:   try: f()⏎finally: cleanup()
来源：http://bcx.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zxn.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ymu.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vlb.cdnleiting.top

Java: try { f(); } finally { cleanup(); }
来源：http://wac.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qqx.chenlongwang.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ctz.mhx1999.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ajx.cheryme.top

[H03] 主动抛出异常
来源：http://ugp.wangdashe.top

Py:   raise ValueError("错误信息")
来源：http://mcd.yonumen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qdf.hammf.cn

JS:   throw new Error("错误信息");
来源：http://wqc.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://ale.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://fdc.hnxiangtu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iac.bbcook.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mut.jlsjyb.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lsw.hongshengwenyu.top

[H04] 自定义异常类型
来源：http://gba.cdnleiting.top

Py:   class MyError(Exception): pass
来源：http://aqv.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://xpa.fanxiaobao.xyz

JS:   class MyError extends Error {}
来源：http://zkp.c1oappe.top

TS:   class MyError extends Error {}
来源：http://ldx.iojbl.cn

Java: class MyException extends RuntimeException {}
来源：http://lbq.tianlin.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://neo.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://rje.havefunace.top

C#:   class MyException : Exception {}
来源：http://sms.birdmap.top

[H05] 捕获特定类型
来源：http://ulz.vehdjk.com

Py:   except ValueError as e:
来源：http://vdq.tarul.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vop.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://umu.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://xxn.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://pbz.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cgu.bjfxy.top

Ruby: rescue ArgumentError => e
来源：http://zry.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lfl.mhx1999.top

[H06] 可选值 / 空值安全访问
来源：http://cva.yongpay.top

Py:   value = d.get("k") or default
来源：http://qoz.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://pca.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://bto.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mhm.jlsjyb.cn


<!-- 参考信息 -->