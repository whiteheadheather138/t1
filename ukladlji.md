代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tvg.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dou.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iec.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://axh.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hcg.sysykeji.top

================================================================================
来源：http://adh.xziqi.cn

F. 文件与目录
来源：http://ajy.shanyushiyangkeji.top

================================================================================
来源：http://lxy.xuetiantiany.cn

[F01] 读取整个文件
来源：http://kxt.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ygj.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://wdh.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://grx.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lee.jqgufenzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tme.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sqn.jiagoushi.top

Ruby: File.read("a.txt")
来源：http://cra.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://njt.ppjwa.cn

[F02] 逐行读取文件
来源：http://uax.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cmq.cheryme.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ebg.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mca.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ivf.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ush.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jfv.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://emv.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vit.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://lzl.9152youxi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jog.meibo888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jki.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oid.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lrj.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://saq.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://npw.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://cva.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mqt.iojbl.cn

[F04] 追加写入文件
来源：http://tcl.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kdw.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ihg.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dkq.xuanzx.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cau.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oyx.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vju.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hwc.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qgw.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://zzg.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vzb.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://dib.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://fdy.vehdjk.com

TS:   fs.existsSync("a.txt")
来源：http://jtj.fanxiaobao.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://ohn.xingfuxueyuan.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eco.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://cao.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://onx.sufxvd.cn

[F06] 删除文件
来源：http://qak.ydzc1.top

Py:   os.remove("a.txt")
来源：http://qej.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://xda.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://sqr.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://etw.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wun.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://xji.svipenyu.cn

Ruby: File.delete("a.txt")
来源：http://wek.hammf.cn

C#:   File.Delete("a.txt");
来源：http://xui.snrcjt.cn

[F07] 创建目录（含多级）
来源：http://vuu.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nbx.fktsv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wpj.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xnd.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ebl.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://svf.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yzg.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tkq.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eyj.nanxuanxn.top

[F08] 遍历目录
来源：http://nzo.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pru.shanyushiyangtech.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fgr.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://hyl.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://vld.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kqr.yj20258888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ksg.xinyue.icu

Ruby: Dir.children("dir")
来源：http://ktr.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://ckh.sufxvd.cn

[F09] 获取文件大小
来源：http://niz.smart0.xyz

Py:   os.path.getsize("a.txt")
来源：http://bpi.uphjek.com

PHP:  filesize("a.txt");
来源：http://zke.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://tns.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://ohd.c1oappe.top

Java: Files.size(Path.of("a.txt"))
来源：http://chr.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jaf.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://azb.hnxiangtu.top

C#:   new FileInfo("a.txt").Length
来源：http://fyd.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://wsr.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cby.guowangkeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vqk.kuanghao11.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fwx.yonumen.top

TS:   path.extname("a.txt")
来源：http://sxf.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eox.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vkp.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vxd.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kcb.jinqigufen.top

[F11] 复制与移动文件
来源：http://cri.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://afl.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tky.andypj.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyn.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fsl.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pey.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://izu.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gux.yuanzhike.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cms.52xcode.cn

[F12] CSV 读写
来源：http://ewy.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oje.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jwa.dianchejie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sch.haohaochexian.top

TS:   // 同上
来源：http://mve.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vkx.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ntn.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sgf.hysaishi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mms.zhiwuduotai.top

================================================================================
来源：http://hut.yvedp.cn

G. 面向对象
来源：http://lkw.zhixingplan.top

================================================================================
来源：http://xmy.zycfv.cn

[G01] 定义类
来源：http://ssc.xinyue.icu

Py:   class User: pass
来源：http://unk.nanxinkj.top

PHP:  class User {}
来源：http://sqq.jqgufenzy.top

JS:   class User {}
来源：http://ibi.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://kih.sjlbkw.cn

Java: class User {}
来源：http://zrp.jinqigufen.top

Go:   type User struct { Name string }
来源：http://zme.ydjk.org.cn

Ruby: class User; end
来源：http://hyx.ctjpmb.com

C#:   class User {}
来源：http://ndp.hnqzz.top

[G02] 构造函数
来源：http://wwa.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://gsk.yongpay.top

PHP:  public function __construct(public string $name) {}
来源：http://tkl.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://wua.gaohongyu789.top

TS:   constructor(public name: string) {}
来源：http://owt.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://tuc.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dac.tianlin.xyz

Ruby: def initialize(name); @name = name; end
来源：http://fkm.sjlbkw.cn

C#:   public User(string name) { Name = name; }
来源：http://hyo.hesvh.cn

[G03] 实例属性
来源：http://dqz.uphjek.com

Py:   self.name = "x"
来源：http://dyw.ehwqpu.com

PHP:  public string $name = "x";
来源：http://uel.hysaishi.cn

JS:   this.name = "x";
来源：http://zuw.haohaochexian.top

TS:   name: string = "x";
来源：http://uel.yuanzhike.top

Java: private String name;
来源：http://npn.hnqzz.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tww.cqqwz.cn

Ruby: @name = "x"
来源：http://anq.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://vws.hnxiangtu.top

[G04] 定义方法
来源：http://dyx.daria6918.cn

Py:   def greet(self): return self.name
来源：http://rbe.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xyw.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://nst.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://uhv.chenlongwang.top

Java: String greet() { return name; }
来源：http://iiv.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://plq.yongpay.top

Ruby: def greet; @name; end
来源：http://fyy.zhongyouzk.top

C#:   public string Greet() => Name;
来源：http://xmq.chenjidiqi.icu

[G05] 继承
来源：http://tbm.chenlongwang.top

Py:   class Admin(User): pass
来源：http://kaj.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://tsu.jianghu66.top

JS:   class Admin extends User {}
来源：http://luf.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://jma.jianghu66.top

Java: class Admin extends User {}
来源：http://sad.cdnleiting.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pgp.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://fcw.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://uja.chenlongwang.top

[G06] 重写方法
来源：http://pkf.shzxlz.cn

Py:   def greet(self): return "admin"
来源：http://hhs.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nrg.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://fic.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://ycg.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://uje.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ybl.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://fbq.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://exl.fehbvm.com

[G07] 调用父类方法
来源：http://ecs.c1oappe.top

Py:   super().greet()
来源：http://vzf.jqgufenzy.top

PHP:  parent::greet();
来源：http://clx.yangfankeji.com

JS:   super.greet();
来源：http://tan.sysykeji.top

TS:   super.greet();
来源：http://nnw.shangyingyoupin.top

Java: super.greet();
来源：http://ppd.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mlo.fanxiaobao.xyz

Ruby: super
来源：http://xcy.xziqi.cn

C#:   base.Greet();
来源：http://fdm.tian-w.cn

[G08] 静态方法与属性
来源：http://aai.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gcw.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://asi.fktsv.cn

JS:   static f() {}
来源：http://mwz.xylfe.cn

TS:   static f(): void {}
来源：http://qgo.shzxlz.cn

Java: static void f() {}
来源：http://rvd.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wbe.mhx1999.top

Ruby: def self.f; end
来源：http://qba.chenjidiqi.icu

C#:   public static void F() {}
来源：http://vkd.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://huk.nanxinkj.top

Py:   from abc import ABC, abstractmethod
来源：http://nee.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bnj.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iqj.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://ftd.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://orr.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://may.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://abf.yuanzhike.top

C#:   interface IShape { double Area(); }
来源：http://gma.yanxiufei.cn

[G10] 访问控制
来源：http://usv.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://uek.fanxiaobao.xyz

PHP:  public / protected / private
来源：http://fgb.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://hfb.hcnkem.com

TS:   public / protected / private
来源：http://hys.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://der.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vzi.fktsv.cn

Ruby: public / protected / private
来源：http://mfj.jinqigufen.top

C#:   public / protected / private / internal
来源：http://jhn.ydzc1.top

[G11] getter / setter
来源：http://igu.cheryme.top

Py:   @property 与 @x.setter
来源：http://drv.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://oyb.sysykeji.top

JS:   get name() { return this._name; }
来源：http://opt.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://bwq.tanke756.top

Java: public String getName() { return name; }
来源：http://spu.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://izb.fengsongda.top

Ruby: attr_accessor :name
来源：http://osr.vehdjk.com

C#:   public string Name { get; set; }
来源：http://mzc.jianghu66.top

[G12] 对象转字符串
来源：http://tcj.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://jnb.yongpay.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uri.sysykeji.top

JS:   toString() { return this.name; }
来源：http://zuz.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://jab.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://nyh.dashuyun.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bcz.yuxming.cn

Ruby: def to_s; @name; end
来源：http://pll.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://pon.dianchejie.cn

[G13] 判断对象类型
来源：http://dxj.hnxiangtu.top

Py:   isinstance(u, User)
来源：http://qgu.guannengcc.top

PHP:  $u instanceof User
来源：http://uxk.kuanghao11.cn

JS:   u instanceof User
来源：http://ysw.zhengqikj.top

TS:   u instanceof User
来源：http://szk.tanke756.top

Java: u instanceof User
来源：http://nef.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://tem.gogol.net.cn

Ruby: u.is_a?(User)
来源：http://yje.sysykeji.top

C#:   u is User
来源：http://vxr.zhixingplan.top

[G14] 数据类 / record
来源：http://wwf.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rky.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://fxp.zdbjq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xim.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://wlo.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://fkj.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://ysk.havefunace.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ebp.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://ypv.hongshengwenyu.top

[G15] 枚举
来源：http://gju.tian-w.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jfz.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://dve.fanxiaobao.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ocl.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vdh.fehbvm.com

Java: enum Color { RED, GREEN }
来源：http://szt.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tge.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://gwu.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bxz.svipenyu.cn

[G16] 对象转数组 / 字典
来源：http://qpg.shanyushiyangtech.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ymu.xziqi.cn

PHP:  get_object_vars($obj);
来源：http://cia.dashuyun.cn

JS:   Object.entries(obj)
来源：http://vpb.meibo888.top

TS:   Object.entries(obj)
来源：http://mus.jyoumei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rvi.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sdn.bbcook.cn

Ruby: obj.instance_variables
来源：http://ilc.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://rvv.cucudq.cn

================================================================================
来源：http://pwg.meibo888.top

H. 异常与错误处理
来源：http://sox.iojbl.cn

================================================================================
来源：http://edf.zhiwuduotai.top

[H01] try / catch 基础
来源：http://kjw.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iqf.sufxvd.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fva.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xag.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qky.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://twm.zhixingplan.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://efr.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xkx.hnqzz.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wgw.yj20258888.top

[H02] finally / ensure 收尾
来源：http://jru.xylfe.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ezw.ywan-chungtsiang.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ysp.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lxv.vehdjk.com

TS:   try { f(); } finally { cleanup(); }
来源：http://fek.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://ecg.bjfxy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bcz.vqdsnc.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bwu.meibo888.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://odh.tanke756.top

[H03] 主动抛出异常
来源：http://vzz.zdqjudy.top

Py:   raise ValueError("错误信息")
来源：http://cpo.chenlongwang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mtt.xingfuxueyuan.xyz

JS:   throw new Error("错误信息");
来源：http://ksk.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://rjs.zdbjq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://acu.yuanzhike.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yhl.pengpengdd.cyou

Ruby: raise ArgumentError, "错误信息"
来源：http://rlv.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gbm.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://nzy.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://bvs.sxryk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qsm.zhiwuduotai.top

JS:   class MyError extends Error {}
来源：http://dez.bjfxy.top

TS:   class MyError extends Error {}
来源：http://tuh.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://bdd.yfazqb.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tlm.vqdsnc.cn


<!-- 参考信息 -->