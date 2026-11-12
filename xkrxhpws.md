代发 wailian999

[F01] 读取整个文件
来源：http://efn.hammf.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vig.havefunace.top

PHP:  file_get_contents("a.txt");
来源：http://ahh.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://elj.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pno.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bqt.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nbx.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://kgl.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://nvw.hnqzz.top

[F02] 逐行读取文件
来源：http://iin.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vfn.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gao.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ept.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dkv.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nii.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://flz.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uxv.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aik.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://cqi.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yxp.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fry.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cer.smart0.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kdr.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hai.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xlo.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://rvx.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fge.chenlongwang.top

[F04] 追加写入文件
来源：http://tmt.mhx1999.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zyy.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dfa.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lbi.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kyr.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zmg.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://axj.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sjv.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fmb.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://kat.fzhhl.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wpy.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://ikn.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://ixi.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://tnt.nanxuanxn.top

Java: Files.exists(Path.of("a.txt"))
来源：http://amo.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dcm.cheryme.top

Ruby: File.exist?("a.txt")
来源：http://fkd.jinqigfzy.top

C#:   File.Exists("a.txt")
来源：http://fuf.daria6918.cn

[F06] 删除文件
来源：http://apd.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://hmk.cucudq.cn

PHP:  unlink("a.txt");
来源：http://eti.52xcode.cn

JS:   fs.unlinkSync("a.txt")
来源：http://reg.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://leh.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oyk.havefunace.top

Go:   os.Remove("a.txt")
来源：http://uew.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://kmz.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://evr.yvedp.cn

[F07] 创建目录（含多级）
来源：http://ziy.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ozw.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://akv.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xam.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ftt.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://daj.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sbc.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dcd.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pom.snrcjt.cn

[F08] 遍历目录
来源：http://ood.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lql.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qap.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://dbv.c1oappe.top

TS:   fs.readdirSync("dir")
来源：http://awx.zhaomingkeji.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://taf.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kuv.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://akh.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://eql.guannengcc.top

[F09] 获取文件大小
来源：http://ych.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://svp.redwolf501.top

PHP:  filesize("a.txt");
来源：http://jmp.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://nqh.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://gem.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://aqi.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aps.jianghu66.top

Ruby: File.size("a.txt")
来源：http://izu.aibaodan.cn

C#:   new FileInfo("a.txt").Length
来源：http://abi.yanxiufei.cn

[F10] 取文件扩展名 / 文件名
来源：http://ldm.zhiwuduotai.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xar.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tkw.tian-w.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zie.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://zmt.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kxe.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xnh.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ezh.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qzg.yvedp.cn

[F11] 复制与移动文件
来源：http://qar.jianghu66.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dtd.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://llb.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lwt.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://din.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sxg.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cck.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wik.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ncx.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://unf.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lrh.zdqjudy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://suz.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mif.sxryk.cn

TS:   // 同上
来源：http://zxf.birdmap.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://urn.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mnm.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gvp.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vum.guowangkeji.top

================================================================================
来源：http://wtj.pycfn.com

G. 面向对象
来源：http://vki.birdmap.top

================================================================================
来源：http://ysc.0kj1m.cn

[G01] 定义类
来源：http://qcg.cashguo.top

Py:   class User: pass
来源：http://pob.xziqi.cn

PHP:  class User {}
来源：http://hkz.zhongyouzk.top

JS:   class User {}
来源：http://lwr.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://bdn.tanke756.top

Java: class User {}
来源：http://jvo.andypj.xyz

Go:   type User struct { Name string }
来源：http://tmi.zdqjudy.top

Ruby: class User; end
来源：http://hzi.smart0.xyz

C#:   class User {}
来源：http://dgp.hesvh.cn

[G02] 构造函数
来源：http://fls.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://ydc.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://hrt.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://ovg.tian-w.cn

TS:   constructor(public name: string) {}
来源：http://sth.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://qcg.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gft.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://wqh.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://kes.chenzaomai.com

[G03] 实例属性
来源：http://edx.dianchejie.cn

Py:   self.name = "x"
来源：http://afv.xziqi.cn

PHP:  public string $name = "x";
来源：http://ewv.316326.xyz

JS:   this.name = "x";
来源：http://trf.shangyingyoupin.top

TS:   name: string = "x";
来源：http://cjv.iojbl.cn

Java: private String name;
来源：http://sza.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dps.wangshuangyany.cn

Ruby: @name = "x"
来源：http://utq.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://lzm.zhongyouzk.top

[G04] 定义方法
来源：http://hco.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://ukt.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://huc.yanxiufei.cn

JS:   greet() { return this.name; }
来源：http://lgm.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://idr.aizwys.cn

Java: String greet() { return name; }
来源：http://mmx.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzc.yj202588.top

Ruby: def greet; @name; end
来源：http://kjt.fengsongda.top

C#:   public string Greet() => Name;
来源：http://nvx.nanxinkj.top

[G05] 继承
来源：http://zor.gogol.net.cn

Py:   class Admin(User): pass
来源：http://moo.xingfuxueyuan.xyz

PHP:  class Admin extends User {}
来源：http://nvk.fktsv.cn

JS:   class Admin extends User {}
来源：http://zqo.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://iqq.shuidangran.top

Java: class Admin extends User {}
来源：http://xth.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ljr.52xcode.cn

Ruby: class Admin < User; end
来源：http://yhj.vehdjk.com

C#:   class Admin : User {}
来源：http://btk.quarkkingdee.top

[G06] 重写方法
来源：http://uzr.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://orn.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://dnb.yj20258.top

JS:   greet() { return "admin"; }
来源：http://xao.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://opu.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://jaj.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://btw.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://teq.tianlin.xyz

C#:   public override string Greet() => "admin";
来源：http://ueb.daxiang520.top

[G07] 调用父类方法
来源：http://woj.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://aot.jinqigufen.top

PHP:  parent::greet();
来源：http://wtw.zhiwuduotai.top

JS:   super.greet();
来源：http://jqb.jiagoushi.top

TS:   super.greet();
来源：http://bgi.jinqigfzy.top

Java: super.greet();
来源：http://dmw.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mou.nwbrower.top

Ruby: super
来源：http://alx.gotoacloud.top

C#:   base.Greet();
来源：http://ikz.xylfe.cn

[G08] 静态方法与属性
来源：http://rud.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gyb.birdmap.top

PHP:  public static function f() {}
来源：http://wyy.zhoulong.xyz

JS:   static f() {}
来源：http://fuf.gogol.net.cn

TS:   static f(): void {}
来源：http://sbt.daxiang520.top

Java: static void f() {}
来源：http://jeo.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vcw.chenzaomai.com

Ruby: def self.f; end
来源：http://hsu.tarul.cn

C#:   public static void F() {}
来源：http://pag.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://aco.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://kvu.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://arn.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ysh.xziqi.cn

TS:   interface Shape { area(): number; }
来源：http://loo.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://lbv.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://dkf.nwbrower.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aym.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://pzd.jinqigufen.top

[G10] 访问控制
来源：http://cpv.jqgufenzy.top

Py:   约定 _protected / __private（不强制）
来源：http://qwn.cdnleiting.top

PHP:  public / protected / private
来源：http://ogd.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://kar.sweek.top

TS:   public / protected / private
来源：http://ezq.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://gmg.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ecf.xziqi.cn

Ruby: public / protected / private
来源：http://fze.ppjwa.cn

C#:   public / protected / private / internal
来源：http://cgd.sxryk.cn

[G11] getter / setter
来源：http://qzh.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://sbh.chenlongwang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://buu.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://mjc.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://rfl.fktsv.cn

Java: public String getName() { return name; }
来源：http://ouj.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rcq.tanke756.top

Ruby: attr_accessor :name
来源：http://qff.pycfn.com

C#:   public string Name { get; set; }
来源：http://esz.shzxlz.cn

[G12] 对象转字符串
来源：http://gdo.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://mhy.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gar.bjfxy.top

JS:   toString() { return this.name; }
来源：http://mce.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://zog.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://iix.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://fxm.xinyue.icu

Ruby: def to_s; @name; end
来源：http://yob.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://jiz.jqgfzy.top

[G13] 判断对象类型
来源：http://hrr.hywenlv.cn

Py:   isinstance(u, User)
来源：http://fbg.gaohongyu789.top

PHP:  $u instanceof User
来源：http://tnt.jianghu66.top

JS:   u instanceof User
来源：http://ejx.iojbl.cn

TS:   u instanceof User
来源：http://atk.zhijiandao.cn

Java: u instanceof User
来源：http://ajo.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fff.tanke756.top

Ruby: u.is_a?(User)
来源：http://bpn.iojbl.cn

C#:   u is User
来源：http://ipy.birdmap.top

[G14] 数据类 / record
来源：http://ycb.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bnb.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://aaw.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://evg.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://mmy.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://rhw.xziqi.cn

Go:   type User struct { Name string; Age int }
来源：http://woa.nanxuanxn.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gjt.ydzc1.top

C#:   record User(string Name, int Age);
来源：http://xbr.haohaochexian.top

[G15] 枚举
来源：http://jmk.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jjf.xingfuxueyuan.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zpz.fktsv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yqy.tianlin.xyz

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dxi.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://ujx.daria6918.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xqw.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://new.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wfa.hammf.cn

[G16] 对象转数组 / 字典
来源：http://pzn.jinghuilouyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gmp.meibo888.top

PHP:  get_object_vars($obj);
来源：http://yaa.gzhubu.top

JS:   Object.entries(obj)
来源：http://yau.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://cex.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blz.gotoacloud.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vvt.zycfv.cn

Ruby: obj.instance_variables
来源：http://oqe.cashguo.top

C#:   // 用反射或 System.Text.Json
来源：http://hhe.nanxuanxn.top

================================================================================
来源：http://cja.fktsv.cn

H. 异常与错误处理
来源：http://dsg.xziqi.cn

================================================================================
来源：http://cpe.jlsjyb.cn

[H01] try / catch 基础
来源：http://cxh.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://csj.jianghu66.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lyy.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rox.quarkkingdee.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://otc.hesvh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oht.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cml.sufxvd.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gct.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dre.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://jjr.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://klp.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zlw.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lkh.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gow.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://pgh.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ilb.hfpthk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lze.nanxinkj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://avg.nwbrower.top

[H03] 主动抛出异常
来源：http://zau.fanxiaobao.xyz

Py:   raise ValueError("错误信息")
来源：http://jrt.uphjek.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xsc.dashuyun.cn

JS:   throw new Error("错误信息");
来源：http://rks.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://bjj.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qxf.zhoulong.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pvz.yongpay.top

Ruby: raise ArgumentError, "错误信息"
来源：http://kcu.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://ukc.andypj.xyz

[H04] 自定义异常类型
来源：http://mps.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://iqu.fengsongda.top

PHP:  class MyError extends RuntimeException {}
来源：http://rhm.jinqigufen.top

JS:   class MyError extends Error {}
来源：http://ltv.fehbvm.com

TS:   class MyError extends Error {}
来源：http://onf.zhoulong.xyz

Java: class MyException extends RuntimeException {}
来源：http://unp.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ybz.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://cwf.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://oih.meibo888.top

[H05] 捕获特定类型
来源：http://ewo.ydjk.org.cn

Py:   except ValueError as e:
来源：http://caz.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ckw.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://qrw.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://kyp.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://bnz.jinqigufen.top


<!-- 参考信息 -->