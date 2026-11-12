代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://xcb.jlsjyb.cn

[F02] 逐行读取文件
来源：http://dzx.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jpi.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zpl.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chm.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dlf.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pdh.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://axq.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wti.zhixingplan.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tiq.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://wuq.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ayp.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://dpp.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yha.316326.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://snb.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://prm.xingfuxueyuan.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kza.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://ydt.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://olt.kuanghao11.cn

[F04] 追加写入文件
来源：http://lmw.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tav.tian-w.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bwe.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ngm.c1oappe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tvh.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zai.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gva.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oqc.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fkn.gaohongyu789.top

[F05] 判断文件或目录是否存在
来源：http://kua.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jgu.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://ssa.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://ddx.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://cxk.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lvv.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dys.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://fhu.cucudq.cn

C#:   File.Exists("a.txt")
来源：http://tmh.hywenlv.cn

[F06] 删除文件
来源：http://wof.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://ngj.meibo888.top

PHP:  unlink("a.txt");
来源：http://qcq.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qmh.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://myj.tarul.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vnw.daxiang520.top

Go:   os.Remove("a.txt")
来源：http://krm.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://gpf.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://ksj.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://yrx.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fop.svipenyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oki.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bdt.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ekw.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://llf.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qkk.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vxy.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://czp.fehbvm.com

[F08] 遍历目录
来源：http://rcu.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xfe.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kpk.fktsv.cn

JS:   fs.readdirSync("dir")
来源：http://wdm.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://hol.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ars.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zdx.hcnkem.com

Ruby: Dir.children("dir")
来源：http://ytt.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://wec.smart0.xyz

[F09] 获取文件大小
来源：http://pul.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://ssa.kuanghao11.cn

PHP:  filesize("a.txt");
来源：http://vlm.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://mgc.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://bkf.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://jrk.jianghu66.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hfe.aizwys.cn

Ruby: File.size("a.txt")
来源：http://bks.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://fig.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://yls.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fhx.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://onf.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jxm.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://dre.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hkz.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zqs.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ejl.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eql.bjfxy.top

[F11] 复制与移动文件
来源：http://adt.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kuk.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ipo.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgy.jinyuanbaomall.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vsn.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gba.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqv.ppjwa.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yrv.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://say.chenjidiqi.icu

[F12] CSV 读写
来源：http://tup.yangfankeji.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mbm.andypj.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zua.shzxlz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fao.cashguo.top

TS:   // 同上
来源：http://dak.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oeg.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zgn.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nos.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://yvo.zhengqikj.top

================================================================================
来源：http://dfn.nanxinkj.top

G. 面向对象
来源：http://wzd.nanxinkj.top

================================================================================
来源：http://nuj.jinghuilouyu.cn

[G01] 定义类
来源：http://qug.redwolf501.top

Py:   class User: pass
来源：http://ynt.ydzc1.top

PHP:  class User {}
来源：http://kte.chenzaomai.com

JS:   class User {}
来源：http://ggu.chenjidiqi.icu

TS:   class User { name: string = ""; }
来源：http://jtx.gotoacloud.top

Java: class User {}
来源：http://amj.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://lhv.nwbrower.top

Ruby: class User; end
来源：http://adh.ywan-chungtsiang.top

C#:   class User {}
来源：http://ieu.dashuyun.cn

[G02] 构造函数
来源：http://lhh.sufxvd.cn

Py:   def __init__(self, name): self.name = name
来源：http://xdn.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://nms.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://yzl.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://shc.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://pba.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jza.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://xpz.svipenyu.cn

C#:   public User(string name) { Name = name; }
来源：http://qtb.vqdsnc.cn

[G03] 实例属性
来源：http://elt.zhaomingkeji.xyz

Py:   self.name = "x"
来源：http://vut.yuxming.cn

PHP:  public string $name = "x";
来源：http://gwa.wangshuangyany.cn

JS:   this.name = "x";
来源：http://qsa.redwolf501.top

TS:   name: string = "x";
来源：http://kkc.jinqigufen.top

Java: private String name;
来源：http://zzl.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kfu.jlsjyb.cn

Ruby: @name = "x"
来源：http://fjw.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://owt.epnwcf.com

[G04] 定义方法
来源：http://ucj.yj20258888.top

Py:   def greet(self): return self.name
来源：http://lhk.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://one.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://sxb.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://slg.tianlin.xyz

Java: String greet() { return name; }
来源：http://ezp.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wuz.havefunace.top

Ruby: def greet; @name; end
来源：http://buo.sweek.top

C#:   public string Greet() => Name;
来源：http://wcq.ywan-chungtsiang.top

[G05] 继承
来源：http://gpp.c1oappe.top

Py:   class Admin(User): pass
来源：http://ybw.uphjek.com

PHP:  class Admin extends User {}
来源：http://phm.hywenlv.cn

JS:   class Admin extends User {}
来源：http://ahu.iojbl.cn

TS:   class Admin extends User {}
来源：http://nxv.hysaishi.cn

Java: class Admin extends User {}
来源：http://tza.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qrl.sufxvd.cn

Ruby: class Admin < User; end
来源：http://nmx.sysykeji.top

C#:   class Admin : User {}
来源：http://kel.shzxlz.cn

[G06] 重写方法
来源：http://jrx.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://sec.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xze.nanxuanxn.top

JS:   greet() { return "admin"; }
来源：http://sdf.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://azh.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://ojw.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nnd.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://fam.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://ifz.uphjek.com

[G07] 调用父类方法
来源：http://oes.jyoumei.cn

Py:   super().greet()
来源：http://ugw.cdnleiting.top

PHP:  parent::greet();
来源：http://sof.yongpay.top

JS:   super.greet();
来源：http://tts.zdqjudy.top

TS:   super.greet();
来源：http://yfg.ehwqpu.com

Java: super.greet();
来源：http://tfz.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pqz.redwolf501.top

Ruby: super
来源：http://sjl.yongpay.top

C#:   base.Greet();
来源：http://bkd.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://vkc.gogol.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://snm.sxryk.cn

PHP:  public static function f() {}
来源：http://wrm.jinqigfzy.top

JS:   static f() {}
来源：http://eky.yvedp.cn

TS:   static f(): void {}
来源：http://hnl.fktsv.cn

Java: static void f() {}
来源：http://cgm.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://old.nanxinkj.top

Ruby: def self.f; end
来源：http://rxp.jqgufenzy.top

C#:   public static void F() {}
来源：http://ddo.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://reo.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://azz.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nlj.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xpn.jqgfzy.top

TS:   interface Shape { area(): number; }
来源：http://byc.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://sef.yanxiufei.cn

Go:   type Shape interface { Area() float64 }
来源：http://qtu.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gqo.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://tyn.hywenlv.cn

[G10] 访问控制
来源：http://pjp.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://inc.tarul.cn

PHP:  public / protected / private
来源：http://bcp.tanke756.top

JS:   #private 字段；其余公开
来源：http://wes.yuxming.cn

TS:   public / protected / private
来源：http://utk.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://ohk.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ogy.tianlin.xyz

Ruby: public / protected / private
来源：http://gle.jyoumei.cn

C#:   public / protected / private / internal
来源：http://ihy.wangdashe.top

[G11] getter / setter
来源：http://dvq.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://gny.zdqjudy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ovb.yvedp.cn

JS:   get name() { return this._name; }
来源：http://hxm.xuetiantiany.cn

TS:   get name(): string { return this._name; }
来源：http://nqd.tanke756.top

Java: public String getName() { return name; }
来源：http://phm.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jmn.zdbjq.cn

Ruby: attr_accessor :name
来源：http://oej.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://jdc.hnxiangtu.top

[G12] 对象转字符串
来源：http://pij.yonumen.top

Py:   def __str__(self): return self.name
来源：http://hzx.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vpo.epnwcf.com

JS:   toString() { return this.name; }
来源：http://vuf.tarul.cn

TS:   toString(): string { return this.name; }
来源：http://pmc.uphjek.com

Java: @Override public String toString() { return name; }
来源：http://dnb.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://kjp.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://qqr.ydjk.org.cn

C#:   public override string ToString() => Name;
来源：http://gvs.yangfankeji.com

[G13] 判断对象类型
来源：http://smy.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://xym.yuxming.cn

PHP:  $u instanceof User
来源：http://jhb.cashguo.top

JS:   u instanceof User
来源：http://him.fengsongda.top

TS:   u instanceof User
来源：http://fgb.jinghuilouyu.cn

Java: u instanceof User
来源：http://ych.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hzg.tanke756.top

Ruby: u.is_a?(User)
来源：http://qyb.gaohongyu789.top

C#:   u is User
来源：http://svo.jinqigufen.top

[G14] 数据类 / record
来源：http://bqx.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://odh.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://ycm.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tgy.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://reh.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://zyw.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://suu.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://thq.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://nns.52xcode.cn

[G15] 枚举
来源：http://aov.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tbc.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gfa.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dud.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wik.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://uil.xziqi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qah.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://gbx.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ayk.birdmap.top

[G16] 对象转数组 / 字典
来源：http://huk.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mgv.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://wqy.hnqzz.top

JS:   Object.entries(obj)
来源：http://ibe.xuanzx.com

TS:   Object.entries(obj)
来源：http://nne.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rut.yj20258.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bky.dashuyun.cn

Ruby: obj.instance_variables
来源：http://kep.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://qjr.epnwcf.com

================================================================================
来源：http://xyf.bjfxy.top

H. 异常与错误处理
来源：http://oky.hnqzz.top

================================================================================
来源：http://bhh.fktsv.cn

[H01] try / catch 基础
来源：http://ceg.shanyushiyangtech.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cqp.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jyq.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zse.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nin.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iap.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nkh.zhiwuduotai.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://erg.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cfp.jyoumei.cn

[H02] finally / ensure 收尾
来源：http://njh.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hfk.shanyushiyangkeji.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xsj.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pvi.svipenyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mpf.xingfuxueyuan.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://nej.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fux.birdmap.top

Ruby: begin; f; ensure; cleanup; end
来源：http://auk.sweek.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ibu.hysaishi.cn

[H03] 主动抛出异常
来源：http://wwv.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://ajf.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://whi.zhijiandao.cn

JS:   throw new Error("错误信息");
来源：http://gnu.tarul.cn

TS:   throw new Error("错误信息");
来源：http://fgj.xinyue.icu

Java: throw new IllegalArgumentException("错误信息");
来源：http://dsw.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iob.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://one.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://unc.hysaishi.cn

[H04] 自定义异常类型
来源：http://cla.jqgufenzy.top

Py:   class MyError(Exception): pass
来源：http://pxt.ydjk.org.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gow.ydzc1.top

JS:   class MyError extends Error {}
来源：http://fok.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://dgm.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://yhb.xuanzx.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ixf.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://yhi.0kj1m.cn

C#:   class MyException : Exception {}
来源：http://bte.sufxvd.cn

[H05] 捕获特定类型
来源：http://rtq.yongpay.top

Py:   except ValueError as e:
来源：http://wxx.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://krr.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://brs.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://iry.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://hud.chenlongwang.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mfv.xuetiantiany.cn

Ruby: rescue ArgumentError => e
来源：http://xmp.hesvh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vhu.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://mwh.snrcjt.cn

Py:   value = d.get("k") or default
来源：http://xjb.316326.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://ryr.xuanzx.com

JS:   obj?.a?.b;  d ?? default
来源：http://qdy.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ked.xuetiantiany.cn


<!-- 参考信息 -->