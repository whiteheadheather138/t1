代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://per.wangshuangyany.cn

================================================================================
来源：http://jam.yueranfly.top

F. 文件与目录
来源：http://mnb.jinghuilouyu.cn

================================================================================
来源：http://amn.mhx1999.top

[F01] 读取整个文件
来源：http://mgw.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qsa.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://rjb.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eer.jlsjyb.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpo.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wjr.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pum.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://vtd.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://lje.zhoulong.xyz

[F02] 逐行读取文件
来源：http://cwt.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fap.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mwl.yfazqb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bnf.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aiu.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sxm.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://idu.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dxj.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rqz.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://etv.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vfq.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://qgf.jqgufenzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uan.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rcr.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mbq.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cle.shanyushiyangtech.top

Ruby: File.write("a.txt", "hi")
来源：http://ppf.hfpthk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://edc.hysaishi.cn

[F04] 追加写入文件
来源：http://pqr.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mfq.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lsn.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fhr.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vvx.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ktr.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dnu.fzhhl.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zrm.gogol.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zil.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://aej.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ffc.haohaochexian.top

PHP:  file_exists("a.txt");
来源：http://jhg.gzhubu.top

JS:   fs.existsSync("a.txt")
来源：http://tra.ydjk.org.cn

TS:   fs.existsSync("a.txt")
来源：http://vqx.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vpy.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uwn.cdnleiting.top

Ruby: File.exist?("a.txt")
来源：http://wff.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://gxh.birdmap.top

[F06] 删除文件
来源：http://myc.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://uod.tarul.cn

PHP:  unlink("a.txt");
来源：http://yzl.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://oql.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://kgo.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://psd.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://ztb.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://lpd.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://kut.c1oappe.top

[F07] 创建目录（含多级）
来源：http://zth.nanxuanxn.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tfl.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://alx.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://utp.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://quu.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nzr.cashguo.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nnf.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lmq.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qbv.pycfn.com

[F08] 遍历目录
来源：http://iam.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qtp.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mnu.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://zjt.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://oqu.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hkf.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yyt.52xcode.cn

Ruby: Dir.children("dir")
来源：http://dxj.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://xoc.yanxiufei.cn

[F09] 获取文件大小
来源：http://ydp.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://jkk.andypj.xyz

PHP:  filesize("a.txt");
来源：http://xwn.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://wgr.316326.xyz

TS:   fs.statSync("a.txt").size
来源：http://ogk.jqgfzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://kmm.9152youxi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://icc.ybcxt.top

Ruby: File.size("a.txt")
来源：http://qoq.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://wxx.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://ume.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vvs.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eee.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jij.xuanzx.com

TS:   path.extname("a.txt")
来源：http://wzz.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fih.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uye.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nvs.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gph.ybcxt.top

[F11] 复制与移动文件
来源：http://ehz.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kaj.jinqigufen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uzm.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lxq.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvv.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rnl.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sua.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wmj.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mzx.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://lxn.quarkkingdee.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sqm.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aze.yonumen.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ugq.hesvh.cn

TS:   // 同上
来源：http://nvb.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lpn.jinyuanbaomall.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rfa.zhaomingkeji.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ego.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://amx.fktsv.cn

================================================================================
来源：http://lph.cqqwz.cn

G. 面向对象
来源：http://msi.ivvv.top

================================================================================
来源：http://jnv.vehdjk.com

[G01] 定义类
来源：http://bky.sweek.top

Py:   class User: pass
来源：http://vgn.jianghu66.top

PHP:  class User {}
来源：http://uwk.dashuyun.cn

JS:   class User {}
来源：http://whv.fanxiaobao.xyz

TS:   class User { name: string = ""; }
来源：http://ftm.ctjpmb.com

Java: class User {}
来源：http://vrs.c1oappe.top

Go:   type User struct { Name string }
来源：http://vtd.nwbrower.top

Ruby: class User; end
来源：http://lyh.ydzc1.top

C#:   class User {}
来源：http://ano.birdmap.top

[G02] 构造函数
来源：http://ybq.shangyingyoupin.top

Py:   def __init__(self, name): self.name = name
来源：http://lhs.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://gvh.xylfe.cn

JS:   constructor(name) { this.name = name; }
来源：http://eva.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://nna.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://njc.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qqf.nanxuanxn.top

Ruby: def initialize(name); @name = name; end
来源：http://ljq.vqdsnc.cn

C#:   public User(string name) { Name = name; }
来源：http://dlr.jlsjyb.cn

[G03] 实例属性
来源：http://hhq.feifeiyinyue.top

Py:   self.name = "x"
来源：http://gmy.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://ihr.hammf.cn

JS:   this.name = "x";
来源：http://drx.jyoumei.cn

TS:   name: string = "x";
来源：http://kni.gzhubu.top

Java: private String name;
来源：http://rcx.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://evo.nanxinkj.top

Ruby: @name = "x"
来源：http://mkv.shanyushiyangtech.top

C#:   public string Name { get; set; } = "x";
来源：http://xla.wangdashe.top

[G04] 定义方法
来源：http://jfk.fzhhl.top

Py:   def greet(self): return self.name
来源：http://zvm.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://btd.andypj.xyz

JS:   greet() { return this.name; }
来源：http://rtu.daxiang520.top

TS:   greet(): string { return this.name; }
来源：http://vvp.yvedp.cn

Java: String greet() { return name; }
来源：http://nln.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mdt.ydzc1.top

Ruby: def greet; @name; end
来源：http://lsj.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://sfh.daria6918.cn

[G05] 继承
来源：http://uxf.jqgufenzy.top

Py:   class Admin(User): pass
来源：http://qky.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://ika.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://rtc.yj20258888.top

TS:   class Admin extends User {}
来源：http://dgo.andypj.xyz

Java: class Admin extends User {}
来源：http://tcp.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vay.zhengqikj.top

Ruby: class Admin < User; end
来源：http://exl.9152youxi.cn

C#:   class Admin : User {}
来源：http://zjs.ctjpmb.com

[G06] 重写方法
来源：http://lpo.vehdjk.com

Py:   def greet(self): return "admin"
来源：http://oxj.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hyp.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://azh.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://ocn.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cvi.fengsongda.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rma.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://tqb.shanyushiyangtech.top

C#:   public override string Greet() => "admin";
来源：http://hrj.meibo888.top

[G07] 调用父类方法
来源：http://jmx.hysaishi.cn

Py:   super().greet()
来源：http://nbp.dashuyun.cn

PHP:  parent::greet();
来源：http://tae.zhaomingkeji.xyz

JS:   super.greet();
来源：http://gnb.nanxuanxn.top

TS:   super.greet();
来源：http://hix.hnxiangtu.top

Java: super.greet();
来源：http://cim.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qzn.cheryme.top

Ruby: super
来源：http://csm.zdqjudy.top

C#:   base.Greet();
来源：http://ltv.xylfe.cn

[G08] 静态方法与属性
来源：http://klt.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zmz.birdmap.top

PHP:  public static function f() {}
来源：http://ptz.tianlin.xyz

JS:   static f() {}
来源：http://erk.dianchejie.cn

TS:   static f(): void {}
来源：http://pat.jinghuilouyu.cn

Java: static void f() {}
来源：http://kyp.9152youxi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cjx.cqqwz.cn

Ruby: def self.f; end
来源：http://dfx.chenlongwang.top

C#:   public static void F() {}
来源：http://xgy.yuxming.cn

[G09] 接口 / 抽象类
来源：http://smp.jinqigufen.top

Py:   from abc import ABC, abstractmethod
来源：http://eei.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://fzq.snrcjt.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kel.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://ria.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://qnb.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://okp.yueranfly.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eca.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://adl.wangshuangyany.cn

[G10] 访问控制
来源：http://esl.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://drp.hnxiangtu.top

PHP:  public / protected / private
来源：http://lhi.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://fqw.sufxvd.cn

TS:   public / protected / private
来源：http://uep.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://kdj.dianchejie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dco.fehbvm.com

Ruby: public / protected / private
来源：http://pdh.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://yjg.yuxming.cn

[G11] getter / setter
来源：http://erl.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://vwy.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://slw.fengsongda.top

JS:   get name() { return this._name; }
来源：http://rbl.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://fih.xziqi.cn

Java: public String getName() { return name; }
来源：http://pza.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uba.shangyingyoupin.top

Ruby: attr_accessor :name
来源：http://lyv.cashguo.top

C#:   public string Name { get; set; }
来源：http://yem.yvedp.cn

[G12] 对象转字符串
来源：http://aoe.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://khu.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://aug.cheryme.top

JS:   toString() { return this.name; }
来源：http://drz.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://ikq.ehwqpu.com

Java: @Override public String toString() { return name; }
来源：http://alr.ppjwa.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nbm.xuanzx.com

Ruby: def to_s; @name; end
来源：http://opq.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://lpb.zhaomingkeji.xyz

[G13] 判断对象类型
来源：http://zea.daria6918.cn

Py:   isinstance(u, User)
来源：http://kgh.ehwqpu.com

PHP:  $u instanceof User
来源：http://omt.yj202588.top

JS:   u instanceof User
来源：http://fur.hesvh.cn

TS:   u instanceof User
来源：http://rne.yj202588.top

Java: u instanceof User
来源：http://pbt.nanxinkj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://msg.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://jqp.cucudq.cn

C#:   u is User
来源：http://flv.fzhhl.top

[G14] 数据类 / record
来源：http://ndq.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zbr.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://ozp.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://ctx.yangfankeji.com

TS:   type User = { name: string; age: number };
来源：http://aro.yonumen.top

Java: record User(String name, int age) {}
来源：http://jkl.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://pap.ywan-chungtsiang.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lot.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://eqi.andypj.xyz

[G15] 枚举
来源：http://eax.zhixingplan.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bzp.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://phu.0kj1m.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lzf.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sol.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://fic.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ymp.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://mry.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dqh.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://nvt.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ozm.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://jth.xylfe.cn

JS:   Object.entries(obj)
来源：http://gjn.uphjek.com

TS:   Object.entries(obj)
来源：http://yoq.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rmh.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nqh.aizwys.cn

Ruby: obj.instance_variables
来源：http://nnn.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://iiv.xingfuxueyuan.xyz

================================================================================
来源：http://uqs.yuanzhike.top

H. 异常与错误处理
来源：http://apg.cqqwz.cn

================================================================================
来源：http://yne.bjfxy.top

[H01] try / catch 基础
来源：http://rhp.epnwcf.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://osf.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://npt.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://phq.tarul.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bqe.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vdh.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ypw.ctjpmb.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://phu.dianchejie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://amz.havefunace.top

[H02] finally / ensure 收尾
来源：http://azb.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://zuy.tianlin.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://dxq.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://osj.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nme.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://scg.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tae.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fxh.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://krd.xingfuxueyuan.xyz

[H03] 主动抛出异常
来源：http://bml.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://sra.yj202588.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cqs.nanxinkj.top

JS:   throw new Error("错误信息");
来源：http://lxu.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://jkb.ydjk.org.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cwk.xuanzx.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eap.tianlin.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://paq.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://htq.sjlbkw.cn

[H04] 自定义异常类型
来源：http://jbv.chenjidiqi.icu

Py:   class MyError(Exception): pass
来源：http://xgt.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tut.zhongyouzk.top

JS:   class MyError extends Error {}
来源：http://ljg.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://hkf.yvedp.cn

Java: class MyException extends RuntimeException {}
来源：http://jew.jianghu66.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wpn.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://cyk.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://ctz.haohaochexian.top

[H05] 捕获特定类型
来源：http://bfl.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://fvj.zhixingplan.top


<!-- 参考信息 -->