代发 wailian999

[F01] 读取整个文件
来源：http://hka.yj202588.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xjt.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://zfo.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://etn.cheryme.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cnt.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://gtu.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pmq.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://xof.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://piz.yfazqb.com

[F02] 逐行读取文件
来源：http://kmj.hfpthk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cpv.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://btl.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dfl.fzhhl.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pdi.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cpy.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dux.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yhu.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jhp.yonumen.top

[F03] 写入文件（覆盖）
来源：http://wkl.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mxy.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hrb.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zrt.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dvj.hcnkem.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mwz.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://apl.hysaishi.cn

Ruby: File.write("a.txt", "hi")
来源：http://dty.tianlin.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://stm.chenzaomai.com

[F04] 追加写入文件
来源：http://zdz.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jcb.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://krv.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qxu.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qeg.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rij.ehwqpu.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hsk.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aax.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ayb.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://tdy.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://stn.epnwcf.com

PHP:  file_exists("a.txt");
来源：http://pcg.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://ndi.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://lff.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hwd.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tmr.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://xve.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://vpw.zhiwuduotai.top

[F06] 删除文件
来源：http://org.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://gar.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://cxx.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://lph.svipenyu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qfv.haohaochexian.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hoi.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://ujs.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://bzs.316326.xyz

C#:   File.Delete("a.txt");
来源：http://ofx.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://kbf.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nzx.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qax.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jxy.zhijiandao.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jfw.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mvn.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ozr.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jgz.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rjb.tanke756.top

[F08] 遍历目录
来源：http://ujh.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://wby.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hnh.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://nci.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://mtp.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zzq.yueranfly.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eun.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://ogw.nwbrower.top

C#:   Directory.GetFiles("dir")
来源：http://iuh.nanxuanxn.top

[F09] 获取文件大小
来源：http://tve.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://dgd.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://qjg.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://hdy.jiagoushi.top

TS:   fs.statSync("a.txt").size
来源：http://dsn.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://mmf.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iuz.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://nmm.zdqjudy.top

C#:   new FileInfo("a.txt").Length
来源：http://uvk.tian-w.cn

[F10] 取文件扩展名 / 文件名
来源：http://lol.hnxiangtu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://twd.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xyn.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uke.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://grz.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dkk.nanxuanxn.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vmv.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ybx.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hkp.zhoulong.xyz

[F11] 复制与移动文件
来源：http://qdv.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qgr.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mrb.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ypb.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xon.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qfa.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nqr.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ykm.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cjq.yongpay.top

[F12] CSV 读写
来源：http://crz.jinqigfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfl.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hke.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wgb.kuanghao11.cn

TS:   // 同上
来源：http://ydv.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iok.yuxming.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rau.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vsf.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lob.ybcxt.top

================================================================================
来源：http://thw.hnxiangtu.top

G. 面向对象
来源：http://pan.yj20258.top

================================================================================
来源：http://law.c1oappe.top

[G01] 定义类
来源：http://qub.snrcjt.cn

Py:   class User: pass
来源：http://drq.nanxinkj.top

PHP:  class User {}
来源：http://kix.jinqigfzy.top

JS:   class User {}
来源：http://cjq.birdmap.top

TS:   class User { name: string = ""; }
来源：http://yix.bbcook.cn

Java: class User {}
来源：http://zqs.0kj1m.cn

Go:   type User struct { Name string }
来源：http://uzq.cashguo.top

Ruby: class User; end
来源：http://rba.jyoumei.cn

C#:   class User {}
来源：http://syc.guowangkeji.top

[G02] 构造函数
来源：http://qto.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://ksk.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://wrq.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://jqf.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://gfq.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://zqi.xylfe.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://viz.gogol.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://xjf.guannengcc.top

C#:   public User(string name) { Name = name; }
来源：http://omk.smart0.xyz

[G03] 实例属性
来源：http://hvw.guowangkeji.top

Py:   self.name = "x"
来源：http://ify.andypj.xyz

PHP:  public string $name = "x";
来源：http://mgr.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://cvw.gaohongyu789.top

TS:   name: string = "x";
来源：http://tqb.ydzc1.top

Java: private String name;
来源：http://mdc.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nep.dashuyun.cn

Ruby: @name = "x"
来源：http://rca.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://jmf.yvedp.cn

[G04] 定义方法
来源：http://mgr.chenjidiqi.icu

Py:   def greet(self): return self.name
来源：http://mkx.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://erv.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://eur.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://ssq.andypj.xyz

Java: String greet() { return name; }
来源：http://ekp.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://yrt.yj20258.top

Ruby: def greet; @name; end
来源：http://gue.tian-w.cn

C#:   public string Greet() => Name;
来源：http://zyo.shuidangran.top

[G05] 继承
来源：http://xpa.fengsongda.top

Py:   class Admin(User): pass
来源：http://hjb.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://riu.cashguo.top

JS:   class Admin extends User {}
来源：http://coi.hywenlv.cn

TS:   class Admin extends User {}
来源：http://gpz.zhengqikj.top

Java: class Admin extends User {}
来源：http://ovj.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lbe.jinqigufen.top

Ruby: class Admin < User; end
来源：http://drk.vehdjk.com

C#:   class Admin : User {}
来源：http://nlc.tian-w.cn

[G06] 重写方法
来源：http://foh.hysaishi.cn

Py:   def greet(self): return "admin"
来源：http://wdh.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://img.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://xdu.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://gbi.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://ith.chenjidiqi.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgt.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://jli.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://kkq.hammf.cn

[G07] 调用父类方法
来源：http://utn.gogol.net.cn

Py:   super().greet()
来源：http://klo.gotoacloud.top

PHP:  parent::greet();
来源：http://osv.chenzaomai.com

JS:   super.greet();
来源：http://xuj.hongshengwenyu.top

TS:   super.greet();
来源：http://dfu.tanke756.top

Java: super.greet();
来源：http://our.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yhd.zhengqikj.top

Ruby: super
来源：http://isw.hesvh.cn

C#:   base.Greet();
来源：http://jan.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://vcp.wangdashe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bsm.cdnleiting.top

PHP:  public static function f() {}
来源：http://upa.zhongyouzk.top

JS:   static f() {}
来源：http://wpn.fehbvm.com

TS:   static f(): void {}
来源：http://ffg.ppjwa.cn

Java: static void f() {}
来源：http://fql.zhiwuduotai.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qbu.tarul.cn

Ruby: def self.f; end
来源：http://fid.yuanzhike.top

C#:   public static void F() {}
来源：http://woz.sysykeji.top

[G09] 接口 / 抽象类
来源：http://gwk.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://ihw.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://frw.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://bjy.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://bou.svipenyu.cn

Java: interface Shape { double area(); }
来源：http://xby.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://pwh.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ukp.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://kjh.quarkkingdee.top

[G10] 访问控制
来源：http://tgf.haohaochexian.top

Py:   约定 _protected / __private（不强制）
来源：http://mdl.jyoumei.cn

PHP:  public / protected / private
来源：http://ask.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://iiu.kuanghao11.cn

TS:   public / protected / private
来源：http://wei.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://fmu.jyoumei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lws.mhx1999.top

Ruby: public / protected / private
来源：http://vsu.tanke756.top

C#:   public / protected / private / internal
来源：http://wbs.ivvv.top

[G11] getter / setter
来源：http://wjn.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://rdq.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ole.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://wmn.52xcode.cn

TS:   get name(): string { return this._name; }
来源：http://rwn.hywenlv.cn

Java: public String getName() { return name; }
来源：http://bzu.ydzc1.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bhv.cheryme.top

Ruby: attr_accessor :name
来源：http://iqo.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://brk.daxiang520.top

[G12] 对象转字符串
来源：http://hcw.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://zpg.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zub.yvedp.cn

JS:   toString() { return this.name; }
来源：http://bdt.ywan-chungtsiang.top

TS:   toString(): string { return this.name; }
来源：http://ndi.ywan-chungtsiang.top

Java: @Override public String toString() { return name; }
来源：http://jjx.yonumen.top

Go:   func (u User) String() string { return u.Name }
来源：http://duv.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://doo.shuidangran.top

C#:   public override string ToString() => Name;
来源：http://gyl.chenzaomai.com

[G13] 判断对象类型
来源：http://tia.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://sjj.haohaochexian.top

PHP:  $u instanceof User
来源：http://btn.tian-w.cn

JS:   u instanceof User
来源：http://wfk.hcnkem.com

TS:   u instanceof User
来源：http://nug.kuanghao11.cn

Java: u instanceof User
来源：http://dco.zhongyouzk.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zoa.tianlin.xyz

Ruby: u.is_a?(User)
来源：http://vqs.pengpengdd.cyou

C#:   u is User
来源：http://bgp.pengpengdd.cyou

[G14] 数据类 / record
来源：http://fqa.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vvf.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://bma.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cqf.epnwcf.com

TS:   type User = { name: string; age: number };
来源：http://cga.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://nyu.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://wqy.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wkq.sxryk.cn

C#:   record User(string Name, int Age);
来源：http://wuk.yanxiufei.cn

[G15] 枚举
来源：http://bsz.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vrl.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://fdq.yj20258888.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ava.cucudq.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://igy.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://bka.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tui.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://pcn.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gsb.zhengqikj.top

[G16] 对象转数组 / 字典
来源：http://dmv.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uto.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://war.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://ela.iojbl.cn

TS:   Object.entries(obj)
来源：http://hwk.meibo888.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rbv.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://owk.ybcxt.top

Ruby: obj.instance_variables
来源：http://zcm.mhx1999.top

C#:   // 用反射或 System.Text.Json
来源：http://njq.sxryk.cn

================================================================================
来源：http://eoa.zhixingplan.top

H. 异常与错误处理
来源：http://trt.ivvv.top

================================================================================
来源：http://kax.xziqi.cn

[H01] try / catch 基础
来源：http://ond.yongpay.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://snt.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cxk.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qvj.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cle.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ciw.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qwq.jinghuilouyu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jch.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hrk.andypj.xyz

[H02] finally / ensure 收尾
来源：http://kxs.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://snc.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qah.yuxming.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jzg.yfazqb.com

TS:   try { f(); } finally { cleanup(); }
来源：http://xdt.shzxlz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zgg.tanke756.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zxt.dashuyun.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://knl.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ome.yuxming.cn

[H03] 主动抛出异常
来源：http://zku.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://zva.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://plx.ydjk.org.cn

JS:   throw new Error("错误信息");
来源：http://fyw.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://yzd.jyoumei.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://avu.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://alk.vqdsnc.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cey.yueranfly.top

C#:   throw new ArgumentException("错误信息");
来源：http://oft.svipenyu.cn

[H04] 自定义异常类型
来源：http://zmt.chenlongwang.top

Py:   class MyError(Exception): pass
来源：http://iks.redwolf501.top

PHP:  class MyError extends RuntimeException {}
来源：http://efm.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://rdl.shanyushiyangtech.top

TS:   class MyError extends Error {}
来源：http://nky.zhiwuduotai.top

Java: class MyException extends RuntimeException {}
来源：http://ogq.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tsu.c1oappe.top

Ruby: class MyError < StandardError; end
来源：http://qfl.shuidangran.top

C#:   class MyException : Exception {}
来源：http://izo.uphjek.com

[H05] 捕获特定类型
来源：http://djy.zhijiandao.cn

Py:   except ValueError as e:
来源：http://vbw.fktsv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://iny.bjfxy.top

JS:   if (e instanceof TypeError) {}
来源：http://bkg.cqqwz.cn

TS:   if (e instanceof TypeError) {}
来源：http://nqs.kuanghao11.cn

Java: catch (IOException | SQLException e) {}
来源：http://kml.iojbl.cn


<!-- 参考信息 -->