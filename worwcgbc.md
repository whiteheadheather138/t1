代发 wailian999

[E22] 字节长度与字符长度
来源：http://zhv.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nbj.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://szy.daxiang520.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://szo.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nsc.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://imc.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cik.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://gec.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://txe.shanyushiyangkeji.top

================================================================================
来源：http://qjq.zhiwuduotai.top

F. 文件与目录
来源：http://vpp.zhoulong.xyz

================================================================================
来源：http://qci.jiagoushi.top

[F01] 读取整个文件
来源：http://obv.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fus.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://khv.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dmd.fengsongda.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dyi.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://oxo.cheryme.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iqv.uphjek.com

Ruby: File.read("a.txt")
来源：http://mcb.chenjidiqi.icu

C#:   File.ReadAllText("a.txt");
来源：http://vrc.cucudq.cn

[F02] 逐行读取文件
来源：http://tbr.shanyushiyangtech.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vtp.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pul.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zyu.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ecg.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sqi.cqqwz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://drl.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vfc.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lef.jqgfzy.top

[F03] 写入文件（覆盖）
来源：http://vew.ywan-chungtsiang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pgm.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hwq.cqqwz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pfg.jqgfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://drw.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://olx.xinyue.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wio.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://dlx.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://awf.hysaishi.cn

[F04] 追加写入文件
来源：http://jnw.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yam.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hsh.uphjek.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lcy.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://isa.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uim.svipenyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxl.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uzw.hnxiangtu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mqe.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://kkl.sufxvd.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mqk.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://qky.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://hpj.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://ayy.yanxiufei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://had.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qsc.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://zrd.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://xfw.fengsongda.top

[F06] 删除文件
来源：http://dlb.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://quq.yongpay.top

PHP:  unlink("a.txt");
来源：http://gpu.zdqjudy.top

JS:   fs.unlinkSync("a.txt")
来源：http://win.wangshuangyany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wvm.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zto.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://rzu.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://auk.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://hnl.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://pvb.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://don.jlsjyb.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nap.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jip.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgz.jqgufenzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yrt.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ojs.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cmo.jyoumei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kja.tarul.cn

[F08] 遍历目录
来源：http://acu.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ych.andypj.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ilb.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://dng.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://dax.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wxu.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bye.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://zsq.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://iip.ybcxt.top

[F09] 获取文件大小
来源：http://uzb.yvedp.cn

Py:   os.path.getsize("a.txt")
来源：http://pjd.fengsongda.top

PHP:  filesize("a.txt");
来源：http://wry.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://any.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://qyz.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://pkr.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ncz.ydzc1.top

Ruby: File.size("a.txt")
来源：http://dnt.shuidangran.top

C#:   new FileInfo("a.txt").Length
来源：http://cpo.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://alv.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tra.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tyo.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://glk.daria6918.cn

TS:   path.extname("a.txt")
来源：http://yae.dashuyun.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pqi.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pzx.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://stf.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hte.xziqi.cn

[F11] 复制与移动文件
来源：http://jzh.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wql.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tty.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://apr.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tmk.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dkt.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qku.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blc.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dog.bbcook.cn

[F12] CSV 读写
来源：http://mml.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://und.svipenyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://buj.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jkp.hesvh.cn

TS:   // 同上
来源：http://jmm.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://umu.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://deq.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wqn.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://pwa.xuetiantiany.cn

================================================================================
来源：http://mjn.shanyushiyangkeji.top

G. 面向对象
来源：http://rqq.daria6918.cn

================================================================================
来源：http://pyg.gzhubu.top

[G01] 定义类
来源：http://tsa.chenjidiqi.icu

Py:   class User: pass
来源：http://zxw.xuanzx.com

PHP:  class User {}
来源：http://vmj.iojbl.cn

JS:   class User {}
来源：http://dci.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://wiw.jqgfzy.top

Java: class User {}
来源：http://aow.havefunace.top

Go:   type User struct { Name string }
来源：http://acu.zhongyouzk.top

Ruby: class User; end
来源：http://gpn.epnwcf.com

C#:   class User {}
来源：http://xxs.jiagoushi.top

[G02] 构造函数
来源：http://ksl.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://rwe.jqgufenzy.top

PHP:  public function __construct(public string $name) {}
来源：http://tfz.yueranfly.top

JS:   constructor(name) { this.name = name; }
来源：http://ocg.vehdjk.com

TS:   constructor(public name: string) {}
来源：http://djr.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://lpl.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xtq.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://wyo.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://nvq.bbcook.cn

[G03] 实例属性
来源：http://puk.fktsv.cn

Py:   self.name = "x"
来源：http://eyy.zycfv.cn

PHP:  public string $name = "x";
来源：http://jcw.haohaochexian.top

JS:   this.name = "x";
来源：http://hyh.yj20258.top

TS:   name: string = "x";
来源：http://cye.ydzc1.top

Java: private String name;
来源：http://xog.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yvz.hnqzz.top

Ruby: @name = "x"
来源：http://klw.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://oxd.cheryme.top

[G04] 定义方法
来源：http://wem.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://gez.hammf.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rlb.zhoulong.xyz

JS:   greet() { return this.name; }
来源：http://vtt.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://tvm.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://nmz.xingfuxueyuan.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnv.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://inm.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://nub.smart0.xyz

[G05] 继承
来源：http://jne.9152youxi.cn

Py:   class Admin(User): pass
来源：http://ash.andypj.xyz

PHP:  class Admin extends User {}
来源：http://klp.svipenyu.cn

JS:   class Admin extends User {}
来源：http://ikm.daxiang520.top

TS:   class Admin extends User {}
来源：http://ckm.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://mgc.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yjp.birdmap.top

Ruby: class Admin < User; end
来源：http://oib.shangyingyoupin.top

C#:   class Admin : User {}
来源：http://yau.mhx1999.top

[G06] 重写方法
来源：http://bjr.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://gon.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fyy.tarul.cn

JS:   greet() { return "admin"; }
来源：http://fyl.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://jkk.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://deq.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gtb.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://llm.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://dbf.yj202588.top

[G07] 调用父类方法
来源：http://lim.yj202588.top

Py:   super().greet()
来源：http://bta.dashuyun.cn

PHP:  parent::greet();
来源：http://yjj.chenjidiqi.icu

JS:   super.greet();
来源：http://puv.meibo888.top

TS:   super.greet();
来源：http://uri.gzhubu.top

Java: super.greet();
来源：http://ruf.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://axe.yj202588.top

Ruby: super
来源：http://zjz.birdmap.top

C#:   base.Greet();
来源：http://skj.ivvv.top

[G08] 静态方法与属性
来源：http://yfj.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://klq.zhoulong.xyz

PHP:  public static function f() {}
来源：http://etm.52xcode.cn

JS:   static f() {}
来源：http://tcr.birdmap.top

TS:   static f(): void {}
来源：http://vhz.hnxiangtu.top

Java: static void f() {}
来源：http://zvk.jianghu66.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wcd.jianghu66.top

Ruby: def self.f; end
来源：http://tud.9152youxi.cn

C#:   public static void F() {}
来源：http://mug.hammf.cn

[G09] 接口 / 抽象类
来源：http://mtr.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://mip.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://uhm.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://bku.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://ayk.fktsv.cn

Java: interface Shape { double area(); }
来源：http://bxo.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://ctl.hnxiangtu.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otd.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://kqq.dianchejie.cn

[G10] 访问控制
来源：http://ere.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://eis.ydjk.org.cn

PHP:  public / protected / private
来源：http://vjy.aibaodan.cn

JS:   #private 字段；其余公开
来源：http://jxa.nanxuanxn.top

TS:   public / protected / private
来源：http://igb.hnqzz.top

Java: public / protected / private / 默认包级
来源：http://hph.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://des.pengpengdd.cyou

Ruby: public / protected / private
来源：http://dgd.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://vcj.fanxiaobao.xyz

[G11] getter / setter
来源：http://ktc.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://xnl.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jgr.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://qvu.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://cdf.zdbjq.cn

Java: public String getName() { return name; }
来源：http://cfq.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://crd.dashuyun.cn

Ruby: attr_accessor :name
来源：http://ykv.sweek.top

C#:   public string Name { get; set; }
来源：http://obk.zdqjudy.top

[G12] 对象转字符串
来源：http://hmx.mhx1999.top

Py:   def __str__(self): return self.name
来源：http://ski.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://xde.smart0.xyz

JS:   toString() { return this.name; }
来源：http://hpw.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://qhn.bbcook.cn

Java: @Override public String toString() { return name; }
来源：http://ltf.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://vls.uphjek.com

Ruby: def to_s; @name; end
来源：http://bvg.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://kff.tian-w.cn

[G13] 判断对象类型
来源：http://nem.yj202588.top

Py:   isinstance(u, User)
来源：http://zgv.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://gbk.tianlin.xyz

JS:   u instanceof User
来源：http://kxa.wangdashe.top

TS:   u instanceof User
来源：http://lst.xuanzx.com

Java: u instanceof User
来源：http://kse.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fbh.shuidangran.top

Ruby: u.is_a?(User)
来源：http://wqq.zhoulong.xyz

C#:   u is User
来源：http://wss.hysaishi.cn

[G14] 数据类 / record
来源：http://tmt.fzhhl.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cyr.yuxming.cn

PHP:  // 用 readonly 属性模拟
来源：http://nvy.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://bqe.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://xgp.jianghu66.top

Java: record User(String name, int age) {}
来源：http://rbd.snrcjt.cn

Go:   type User struct { Name string; Age int }
来源：http://gvl.pengpengdd.cyou

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bxo.jqgufenzy.top

C#:   record User(string Name, int Age);
来源：http://rrw.nanxuanxn.top

[G15] 枚举
来源：http://voy.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fbm.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fns.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ujc.sysykeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rla.smart0.xyz

Java: enum Color { RED, GREEN }
来源：http://itk.snrcjt.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tmy.gzhubu.top

Ruby: Color = %i[red green].freeze
来源：http://auq.ydjk.org.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://flz.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://doj.vqdsnc.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dfs.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://tpz.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://ckg.ivvv.top

TS:   Object.entries(obj)
来源：http://ntz.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nyq.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ryb.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://lts.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://uos.nanxuanxn.top

================================================================================
来源：http://prx.jqgufenzy.top

H. 异常与错误处理
来源：http://nva.zhijiandao.cn

================================================================================
来源：http://ilc.shuidangran.top

[H01] try / catch 基础
来源：http://nym.ppjwa.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kij.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wqt.tian-w.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wrc.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yva.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://slk.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://osy.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://atw.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oja.epnwcf.com

[H02] finally / ensure 收尾
来源：http://ilk.bbcook.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vcv.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://mje.fehbvm.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qcc.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sto.quarkkingdee.top

Java: try { f(); } finally { cleanup(); }
来源：http://qfs.wangshuangyany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jdg.sysykeji.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rkp.hammf.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://riw.nanxuanxn.top

[H03] 主动抛出异常
来源：http://lcv.sysykeji.top

Py:   raise ValueError("错误信息")
来源：http://tcb.ywan-chungtsiang.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lwa.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://bjy.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://ugz.nanxuanxn.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://pgb.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jan.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dau.tianlin.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://evd.zdbjq.cn

[H04] 自定义异常类型
来源：http://pkc.andypj.xyz

Py:   class MyError(Exception): pass
来源：http://oue.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://vpn.vqdsnc.cn


<!-- 参考信息 -->