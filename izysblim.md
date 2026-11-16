代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vtu.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://kes.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jzh.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://vko.nanxinkj.top

C#:   File.ReadAllText("a.txt");
来源：http://utz.kuanghao11.cn

[F02] 逐行读取文件
来源：http://ygb.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cke.jianghu66.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rqy.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://esg.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bfg.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ozc.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxg.pycfn.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cpl.cashguo.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wnr.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://qig.pengpengdd.cyou

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eld.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://qgu.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mdn.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pma.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yvq.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xme.shuidangran.top

Ruby: File.write("a.txt", "hi")
来源：http://eer.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uuz.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://zar.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wan.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zwi.gzhubu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cnm.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yur.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vkp.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gdc.jiagoushi.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lcx.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://esw.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://ipw.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ujs.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://gby.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://kij.jqgufenzy.top

TS:   fs.existsSync("a.txt")
来源：http://hkb.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nfk.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hek.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://csg.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://hzo.shanyushiyangtech.top

[F06] 删除文件
来源：http://mms.guannengcc.top

Py:   os.remove("a.txt")
来源：http://bmt.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://yin.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dbv.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rmm.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://umv.yongpay.top

Go:   os.Remove("a.txt")
来源：http://nol.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://fxf.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://pvo.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://giq.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qlh.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tet.sysykeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dbl.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uxl.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wtx.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wro.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rpt.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lml.mhx1999.top

[F08] 遍历目录
来源：http://pio.zhaomingkeji.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://gsn.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xkq.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://gsp.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://gcb.zycfv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vtc.redwolf501.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://iwx.xuanzx.com

Ruby: Dir.children("dir")
来源：http://fja.sysykeji.top

C#:   Directory.GetFiles("dir")
来源：http://cwy.zycfv.cn

[F09] 获取文件大小
来源：http://son.cdnleiting.top

Py:   os.path.getsize("a.txt")
来源：http://ipt.wangdashe.top

PHP:  filesize("a.txt");
来源：http://xlk.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://kbn.zhongyouzk.top

TS:   fs.statSync("a.txt").size
来源：http://roy.yuxming.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ert.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dtb.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://rem.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://zoh.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://moh.havefunace.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sfm.fehbvm.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uou.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cew.yueranfly.top

TS:   path.extname("a.txt")
来源：http://agy.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zcc.fehbvm.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nmr.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gur.316326.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lcc.hfpthk.cn

[F11] 复制与移动文件
来源：http://dru.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://twe.52xcode.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://thf.cheryme.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cve.yj20258888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bim.jinghuilouyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mtl.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sbj.yangfankeji.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqt.c1oappe.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dfw.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://svg.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ktz.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zdz.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://umg.dashuyun.cn

TS:   // 同上
来源：http://pro.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kzm.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wzh.zhixingplan.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pia.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://cdc.bjfxy.top

================================================================================
来源：http://uga.chenlongwang.top

G. 面向对象
来源：http://vcw.xingfuxueyuan.xyz

================================================================================
来源：http://vbe.jinqigufen.top

[G01] 定义类
来源：http://bsw.nanxinkj.top

Py:   class User: pass
来源：http://ewn.tian-w.cn

PHP:  class User {}
来源：http://alw.zycfv.cn

JS:   class User {}
来源：http://keo.cqqwz.cn

TS:   class User { name: string = ""; }
来源：http://ecd.nwbrower.top

Java: class User {}
来源：http://wjt.yueranfly.top

Go:   type User struct { Name string }
来源：http://tuf.gotoacloud.top

Ruby: class User; end
来源：http://dwo.ehwqpu.com

C#:   class User {}
来源：http://czn.guannengcc.top

[G02] 构造函数
来源：http://ght.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://pqj.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://jgx.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://vow.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://qfk.yfazqb.com

Java: User(String name) { this.name = name; }
来源：http://ncw.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tvb.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://nal.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://fun.fengsongda.top

[G03] 实例属性
来源：http://qya.quarkkingdee.top

Py:   self.name = "x"
来源：http://vau.tanke756.top

PHP:  public string $name = "x";
来源：http://cqg.guowangkeji.top

JS:   this.name = "x";
来源：http://hdo.cashguo.top

TS:   name: string = "x";
来源：http://mti.xziqi.cn

Java: private String name;
来源：http://tjz.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vpm.hysaishi.cn

Ruby: @name = "x"
来源：http://lov.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://fnt.meibo888.top

[G04] 定义方法
来源：http://noy.jqgfzy.top

Py:   def greet(self): return self.name
来源：http://bxh.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ogu.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://nla.yonumen.top

TS:   greet(): string { return this.name; }
来源：http://qal.zdbjq.cn

Java: String greet() { return name; }
来源：http://xak.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzj.zhengqikj.top

Ruby: def greet; @name; end
来源：http://aph.fengsongda.top

C#:   public string Greet() => Name;
来源：http://ffw.tarul.cn

[G05] 继承
来源：http://amy.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://ytr.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://kcq.hcnkem.com

JS:   class Admin extends User {}
来源：http://xys.guowangkeji.top

TS:   class Admin extends User {}
来源：http://wec.jqgfzy.top

Java: class Admin extends User {}
来源：http://jze.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cuv.snrcjt.cn

Ruby: class Admin < User; end
来源：http://phk.cucudq.cn

C#:   class Admin : User {}
来源：http://dgr.zycfv.cn

[G06] 重写方法
来源：http://ibp.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://xvc.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://hfd.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://srl.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://rfm.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://pxz.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hue.yonumen.top

Ruby: def greet; "admin"; end
来源：http://psz.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://uyo.cucudq.cn

[G07] 调用父类方法
来源：http://luc.meibo888.top

Py:   super().greet()
来源：http://edj.yvedp.cn

PHP:  parent::greet();
来源：http://mne.iojbl.cn

JS:   super.greet();
来源：http://gnv.yuxming.cn

TS:   super.greet();
来源：http://zxf.wangdashe.top

Java: super.greet();
来源：http://bvp.jinqigufen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ryw.vqdsnc.cn

Ruby: super
来源：http://cyf.zhiwuduotai.top

C#:   base.Greet();
来源：http://qdm.sweek.top

[G08] 静态方法与属性
来源：http://nwr.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mwx.hnxiangtu.top

PHP:  public static function f() {}
来源：http://xvj.hnxiangtu.top

JS:   static f() {}
来源：http://vhe.hnxiangtu.top

TS:   static f(): void {}
来源：http://dsa.hnxiangtu.top

Java: static void f() {}
来源：http://bwn.yongpay.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hus.vehdjk.com

Ruby: def self.f; end
来源：http://oqs.cdnleiting.top

C#:   public static void F() {}
来源：http://kee.cashguo.top

[G09] 接口 / 抽象类
来源：http://ldp.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://ahk.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://sfd.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eqo.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://lfy.yvedp.cn

Java: interface Shape { double area(); }
来源：http://mlb.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://yjv.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nse.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://kaa.52xcode.cn

[G10] 访问控制
来源：http://itl.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://tbt.hysaishi.cn

PHP:  public / protected / private
来源：http://mir.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://wgv.zdbjq.cn

TS:   public / protected / private
来源：http://etu.shuidangran.top

Java: public / protected / private / 默认包级
来源：http://ako.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xrl.fehbvm.com

Ruby: public / protected / private
来源：http://zgq.svipenyu.cn

C#:   public / protected / private / internal
来源：http://zzm.chenlongwang.top

[G11] getter / setter
来源：http://kzx.gogol.net.cn

Py:   @property 与 @x.setter
来源：http://xnm.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tkp.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://hxx.sufxvd.cn

TS:   get name(): string { return this._name; }
来源：http://egb.wangdashe.top

Java: public String getName() { return name; }
来源：http://cew.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ynk.hcnkem.com

Ruby: attr_accessor :name
来源：http://nne.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://dol.sweek.top

[G12] 对象转字符串
来源：http://agm.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://jrn.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://amj.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://dfz.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://akl.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://zle.sweek.top

Go:   func (u User) String() string { return u.Name }
来源：http://jlb.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://ukq.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://fsl.yangfankeji.com

[G13] 判断对象类型
来源：http://vex.52xcode.cn

Py:   isinstance(u, User)
来源：http://vmg.ehwqpu.com

PHP:  $u instanceof User
来源：http://bxc.cheryme.top

JS:   u instanceof User
来源：http://wfs.birdmap.top

TS:   u instanceof User
来源：http://yie.hfpthk.cn

Java: u instanceof User
来源：http://cac.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://tlc.hcnkem.com

Ruby: u.is_a?(User)
来源：http://xcc.haohaochexian.top

C#:   u is User
来源：http://sfn.uphjek.com

[G14] 数据类 / record
来源：http://ijb.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tik.chenlongwang.top

PHP:  // 用 readonly 属性模拟
来源：http://ctk.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://oln.gogol.net.cn

TS:   type User = { name: string; age: number };
来源：http://fjn.xuanzx.com

Java: record User(String name, int age) {}
来源：http://dve.sjlbkw.cn

Go:   type User struct { Name string; Age int }
来源：http://fys.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://avt.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://zrc.tian-w.cn

[G15] 枚举
来源：http://sgl.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zff.birdmap.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://kqp.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rci.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mut.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://zwr.hywenlv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iow.dashuyun.cn

Ruby: Color = %i[red green].freeze
来源：http://ozk.xziqi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uaw.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://wrt.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbt.xingfuxueyuan.xyz

PHP:  get_object_vars($obj);
来源：http://vlt.xinyue.icu

JS:   Object.entries(obj)
来源：http://kcx.shanyushiyangtech.top

TS:   Object.entries(obj)
来源：http://mfn.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://now.jiagoushi.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jfn.fengsongda.top

Ruby: obj.instance_variables
来源：http://msu.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://uam.shuidangran.top

================================================================================
来源：http://ket.nanxuanxn.top

H. 异常与错误处理
来源：http://mts.cqqwz.cn

================================================================================
来源：http://bih.hnqzz.top

[H01] try / catch 基础
来源：http://imz.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kie.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ied.zhixingplan.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jha.cqqwz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ker.gzhubu.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wnt.kuanghao11.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mwh.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tfg.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://isu.ppjwa.cn

[H02] finally / ensure 收尾
来源：http://uac.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://ekh.jinghuilouyu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jrl.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ptf.dianchejie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://igx.zhiwuduotai.top

Java: try { f(); } finally { cleanup(); }
来源：http://hft.jinyuanbaomall.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xzd.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kbm.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bdk.andypj.xyz

[H03] 主动抛出异常
来源：http://wfm.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://gcg.hesvh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wlf.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://prx.guannengcc.top

TS:   throw new Error("错误信息");
来源：http://cch.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jiv.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tlg.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ege.zhoulong.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://lty.gotoacloud.top

[H04] 自定义异常类型
来源：http://vdi.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://iui.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://smg.nanxuanxn.top

JS:   class MyError extends Error {}
来源：http://qws.fktsv.cn

TS:   class MyError extends Error {}
来源：http://rlo.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://wpr.zhijiandao.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://slc.yvedp.cn

Ruby: class MyError < StandardError; end
来源：http://bvg.c1oappe.top

C#:   class MyException : Exception {}
来源：http://qfb.ppjwa.cn

[H05] 捕获特定类型
来源：http://bpb.daxiang520.top

Py:   except ValueError as e:
来源：http://xkk.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vdj.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://yvz.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://uof.havefunace.top

Java: catch (IOException | SQLException e) {}
来源：http://oxk.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://byf.yuanzhike.top

Ruby: rescue ArgumentError => e
来源：http://wwl.yfazqb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://veu.shanyushiyangtech.top

[H06] 可选值 / 空值安全访问
来源：http://jpb.mhx1999.top


<!-- 参考信息 -->