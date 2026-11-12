代发 wailian999

[F01] 读取整个文件
来源：http://zmv.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ybw.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://swc.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fre.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ekq.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://lrq.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ffo.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://ypk.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://jgp.fzhhl.top

[F02] 逐行读取文件
来源：http://epc.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oyb.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mmo.chenjidiqi.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tnc.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oew.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fpr.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mvq.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ekm.shzxlz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wof.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://pff.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ccb.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vsd.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://weo.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ykp.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ncf.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ldx.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://rfe.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uwy.ppjwa.cn

[F04] 追加写入文件
来源：http://ngo.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://czs.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mfp.shangyingyoupin.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ckm.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pmn.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gnw.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vjf.gaohongyu789.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://usp.fzhhl.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xxz.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://ixu.hywenlv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vyc.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://eer.0kj1m.cn

JS:   fs.existsSync("a.txt")
来源：http://pgq.cqqwz.cn

TS:   fs.existsSync("a.txt")
来源：http://zaq.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fsf.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wiy.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://skk.316326.xyz

C#:   File.Exists("a.txt")
来源：http://fku.ivvv.top

[F06] 删除文件
来源：http://zbn.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://iyl.fzhhl.top

PHP:  unlink("a.txt");
来源：http://xuo.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://fte.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://xlc.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ebw.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://fwt.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://qab.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://mly.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://cnh.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xnz.hesvh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gtc.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fvc.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lbs.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bkv.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ker.yanxiufei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jap.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tyh.yvedp.cn

[F08] 遍历目录
来源：http://kms.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kzr.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lkh.svipenyu.cn

JS:   fs.readdirSync("dir")
来源：http://bvu.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://eae.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wsf.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rfg.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://nbp.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://unz.0kj1m.cn

[F09] 获取文件大小
来源：http://xkj.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://zcr.pycfn.com

PHP:  filesize("a.txt");
来源：http://pjv.shanyushiyangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://bht.nanxinkj.top

TS:   fs.statSync("a.txt").size
来源：http://ubc.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://yju.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pnz.cheryme.top

Ruby: File.size("a.txt")
来源：http://irh.zycfv.cn

C#:   new FileInfo("a.txt").Length
来源：http://uwc.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://ora.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lvo.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bpb.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vti.fanxiaobao.xyz

TS:   path.extname("a.txt")
来源：http://ivb.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yvg.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ige.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gkb.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fei.dianchejie.cn

[F11] 复制与移动文件
来源：http://xcl.aibaodan.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sgb.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eqi.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lpc.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lis.xinyue.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rgx.fzhhl.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ftd.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rfh.cashguo.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eua.yvedp.cn

[F12] CSV 读写
来源：http://urj.dashuyun.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fbo.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://amv.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tyn.gotoacloud.top

TS:   // 同上
来源：http://kfw.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kqg.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lis.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dis.nanxuanxn.top

C#:   // 无内置：用 CsvHelper 库
来源：http://fay.guannengcc.top

================================================================================
来源：http://ebw.pycfn.com

G. 面向对象
来源：http://els.shanyushiyangtech.top

================================================================================
来源：http://mkv.mhx1999.top

[G01] 定义类
来源：http://cve.hammf.cn

Py:   class User: pass
来源：http://txq.bbcook.cn

PHP:  class User {}
来源：http://loh.jyoumei.cn

JS:   class User {}
来源：http://dts.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://ryb.jinyuanbaomall.cn

Java: class User {}
来源：http://ibw.zdbjq.cn

Go:   type User struct { Name string }
来源：http://dpv.jinqigufen.top

Ruby: class User; end
来源：http://wsn.daxiang520.top

C#:   class User {}
来源：http://nxw.ctjpmb.com

[G02] 构造函数
来源：http://vrx.aizwys.cn

Py:   def __init__(self, name): self.name = name
来源：http://agt.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://gle.xuetiantiany.cn

JS:   constructor(name) { this.name = name; }
来源：http://hrc.xuetiantiany.cn

TS:   constructor(public name: string) {}
来源：http://ade.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://jeu.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rpq.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://pwk.kuanghao11.cn

C#:   public User(string name) { Name = name; }
来源：http://eix.hnqzz.top

[G03] 实例属性
来源：http://qma.tanke756.top

Py:   self.name = "x"
来源：http://hfl.xuanzx.com

PHP:  public string $name = "x";
来源：http://rrz.xuetiantiany.cn

JS:   this.name = "x";
来源：http://qnd.tian-w.cn

TS:   name: string = "x";
来源：http://taz.shuidangran.top

Java: private String name;
来源：http://jnt.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yoz.jqgufenzy.top

Ruby: @name = "x"
来源：http://qqw.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://qvs.jinqigfzy.top

[G04] 定义方法
来源：http://fey.mhx1999.top

Py:   def greet(self): return self.name
来源：http://oqv.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://epo.tanke756.top

JS:   greet() { return this.name; }
来源：http://nit.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://zpu.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://qgf.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kpo.guannengcc.top

Ruby: def greet; @name; end
来源：http://yim.ybcxt.top

C#:   public string Greet() => Name;
来源：http://wun.yj202588.top

[G05] 继承
来源：http://xbe.fanxiaobao.xyz

Py:   class Admin(User): pass
来源：http://wvl.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://qrw.cheryme.top

JS:   class Admin extends User {}
来源：http://aur.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://tti.zycfv.cn

Java: class Admin extends User {}
来源：http://frt.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybu.zhixingplan.top

Ruby: class Admin < User; end
来源：http://rvl.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://euu.hfpthk.cn

[G06] 重写方法
来源：http://nkq.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://nvh.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pgg.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://ndx.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://cpb.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://rel.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nog.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://vna.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://eod.zhixingplan.top

[G07] 调用父类方法
来源：http://vib.birdmap.top

Py:   super().greet()
来源：http://ijp.jiagoushi.top

PHP:  parent::greet();
来源：http://dkk.xziqi.cn

JS:   super.greet();
来源：http://rtx.ehwqpu.com

TS:   super.greet();
来源：http://dvz.jiagoushi.top

Java: super.greet();
来源：http://nvo.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dmi.xuanzx.com

Ruby: super
来源：http://xkq.hesvh.cn

C#:   base.Greet();
来源：http://gzh.jinqigfzy.top

[G08] 静态方法与属性
来源：http://oal.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qcp.xinyue.icu

PHP:  public static function f() {}
来源：http://ffh.bjfxy.top

JS:   static f() {}
来源：http://eno.fengsongda.top

TS:   static f(): void {}
来源：http://bad.bbcook.cn

Java: static void f() {}
来源：http://fev.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://klw.ydzc1.top

Ruby: def self.f; end
来源：http://erk.yj202588.top

C#:   public static void F() {}
来源：http://wyk.xuanzx.com

[G09] 接口 / 抽象类
来源：http://cao.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://mbz.kuanghao11.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bnz.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vee.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://myy.xziqi.cn

Java: interface Shape { double area(); }
来源：http://tvj.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://mxf.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://scj.zhixingplan.top

C#:   interface IShape { double Area(); }
来源：http://ytj.316326.xyz

[G10] 访问控制
来源：http://qvb.dashuyun.cn

Py:   约定 _protected / __private（不强制）
来源：http://gor.zhengqikj.top

PHP:  public / protected / private
来源：http://mxj.chenlongwang.top

JS:   #private 字段；其余公开
来源：http://sut.tanke756.top

TS:   public / protected / private
来源：http://xqg.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://lub.hongshengwenyu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fsp.yfazqb.com

Ruby: public / protected / private
来源：http://euu.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://axd.hysaishi.cn

[G11] getter / setter
来源：http://bmk.yj20258.top

Py:   @property 与 @x.setter
来源：http://xkk.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hlz.cashguo.top

JS:   get name() { return this._name; }
来源：http://owr.jqgfzy.top

TS:   get name(): string { return this._name; }
来源：http://cff.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://vyd.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ikw.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://rwn.ybcxt.top

C#:   public string Name { get; set; }
来源：http://sox.xylfe.cn

[G12] 对象转字符串
来源：http://bck.fengsongda.top

Py:   def __str__(self): return self.name
来源：http://epa.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lwu.sweek.top

JS:   toString() { return this.name; }
来源：http://ihg.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://xew.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://ala.316326.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://daa.yuxming.cn

Ruby: def to_s; @name; end
来源：http://wkz.meibo888.top

C#:   public override string ToString() => Name;
来源：http://krs.sxryk.cn

[G13] 判断对象类型
来源：http://dvf.52xcode.cn

Py:   isinstance(u, User)
来源：http://fep.redwolf501.top

PHP:  $u instanceof User
来源：http://ysk.yj202588.top

JS:   u instanceof User
来源：http://hdu.cashguo.top

TS:   u instanceof User
来源：http://ymo.tianlin.xyz

Java: u instanceof User
来源：http://ylf.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://anj.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://vfv.ywan-chungtsiang.top

C#:   u is User
来源：http://cjs.cashguo.top

[G14] 数据类 / record
来源：http://ytp.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vth.ydjk.org.cn

PHP:  // 用 readonly 属性模拟
来源：http://khi.bjfxy.top

JS:   // 无内置：普通类或对象字面量
来源：http://zeo.hywenlv.cn

TS:   type User = { name: string; age: number };
来源：http://qge.xylfe.cn

Java: record User(String name, int age) {}
来源：http://dot.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://fov.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nja.chenlongwang.top

C#:   record User(string Name, int Age);
来源：http://wqi.hesvh.cn

[G15] 枚举
来源：http://fpf.cqqwz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://npf.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://xls.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://doo.hfpthk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://trf.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://ksx.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wyb.vqdsnc.cn

Ruby: Color = %i[red green].freeze
来源：http://ezw.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xfl.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://apq.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://khf.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://gwl.cqqwz.cn

JS:   Object.entries(obj)
来源：http://hky.52xcode.cn

TS:   Object.entries(obj)
来源：http://xgo.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://llx.0kj1m.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yzl.jinghuilouyu.cn

Ruby: obj.instance_variables
来源：http://atv.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://zsy.jiagoushi.top

================================================================================
来源：http://fnj.hongshengwenyu.top

H. 异常与错误处理
来源：http://orx.ydjk.org.cn

================================================================================
来源：http://krh.jqgufenzy.top

[H01] try / catch 基础
来源：http://bzj.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xdr.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jic.shanyushiyangtech.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sxn.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xzq.ehwqpu.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vvu.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jar.havefunace.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fwz.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rzv.zdbjq.cn

[H02] finally / ensure 收尾
来源：http://gbw.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://zad.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qes.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://thp.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dpk.ydzc1.top

Java: try { f(); } finally { cleanup(); }
来源：http://ici.gaohongyu789.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cou.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ped.yj20258888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lxv.xziqi.cn

[H03] 主动抛出异常
来源：http://ffj.zhixingplan.top

Py:   raise ValueError("错误信息")
来源：http://emm.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://egh.ivvv.top

JS:   throw new Error("错误信息");
来源：http://ryz.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://uxq.jiagoushi.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yhi.jlsjyb.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hlc.ppjwa.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cvi.hnqzz.top

C#:   throw new ArgumentException("错误信息");
来源：http://idu.zdqjudy.top

[H04] 自定义异常类型
来源：http://vgz.ivvv.top

Py:   class MyError(Exception): pass
来源：http://dba.birdmap.top

PHP:  class MyError extends RuntimeException {}
来源：http://vbo.cheryme.top

JS:   class MyError extends Error {}
来源：http://qre.xinyue.icu

TS:   class MyError extends Error {}
来源：http://gbd.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://tfw.hcnkem.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://krz.snrcjt.cn

Ruby: class MyError < StandardError; end
来源：http://vzy.52xcode.cn

C#:   class MyException : Exception {}
来源：http://led.gogol.net.cn

[H05] 捕获特定类型
来源：http://ubs.tian-w.cn

Py:   except ValueError as e:
来源：http://ffh.shangyingyoupin.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://noc.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://aoe.havefunace.top

TS:   if (e instanceof TypeError) {}
来源：http://dnl.cucudq.cn

Java: catch (IOException | SQLException e) {}
来源：http://nxy.yangfankeji.com


<!-- 参考信息 -->