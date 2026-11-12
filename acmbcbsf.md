代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mwi.mhx1999.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rmi.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zic.shzxlz.cn

Ruby: File.read("a.txt")
来源：http://tcd.fanxiaobao.xyz

C#:   File.ReadAllText("a.txt");
来源：http://hqa.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://uaw.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fjf.zycfv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uvn.hnqzz.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://flx.zhaomingkeji.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ctq.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uhe.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rew.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wbd.hammf.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gsq.sysykeji.top

[F03] 写入文件（覆盖）
来源：http://xmd.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://stj.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://pke.zhixingplan.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ffz.shangyingyoupin.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xfk.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ior.mhx1999.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yuk.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://jau.hcnkem.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://slf.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://stn.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ule.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wbw.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qqc.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rwe.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gcx.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vwf.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cgk.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://auq.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://mrk.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kcn.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://bvy.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://uis.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://dri.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jyw.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gwi.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://kaq.316326.xyz

C#:   File.Exists("a.txt")
来源：http://pzk.zhoulong.xyz

[F06] 删除文件
来源：http://oek.iojbl.cn

Py:   os.remove("a.txt")
来源：http://obp.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://sly.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://xli.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://xue.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ply.xylfe.cn

Go:   os.Remove("a.txt")
来源：http://exk.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://wei.shzxlz.cn

C#:   File.Delete("a.txt");
来源：http://nlv.yvedp.cn

[F07] 创建目录（含多级）
来源：http://dva.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://unk.uphjek.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://obk.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nhb.zhoulong.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ifk.hnqzz.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pnq.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tqt.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pvi.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hkh.snrcjt.cn

[F08] 遍历目录
来源：http://ewc.zhengqikj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://duj.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://klk.zhengqikj.top

JS:   fs.readdirSync("dir")
来源：http://aeo.yfazqb.com

TS:   fs.readdirSync("dir")
来源：http://bfc.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://crk.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mey.mhx1999.top

Ruby: Dir.children("dir")
来源：http://ljf.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://qzt.aibaodan.cn

[F09] 获取文件大小
来源：http://syb.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://uwt.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://hoc.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://kxh.chenlongwang.top

TS:   fs.statSync("a.txt").size
来源：http://jyp.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://dhx.bjfxy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ucu.hywenlv.cn

Ruby: File.size("a.txt")
来源：http://gpr.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://mue.ppjwa.cn

[F10] 取文件扩展名 / 文件名
来源：http://rsj.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bjh.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jry.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tyk.redwolf501.top

TS:   path.extname("a.txt")
来源：http://duf.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jmh.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vjb.yanxiufei.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pxw.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qph.meibo888.top

[F11] 复制与移动文件
来源：http://opf.hesvh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rhb.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zzd.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilj.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pjd.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://civ.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nim.svipenyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yge.sweek.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wou.yj202588.top

[F12] CSV 读写
来源：http://jkl.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ycd.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://orj.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rkg.sweek.top

TS:   // 同上
来源：http://nhv.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qtn.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fkt.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eua.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rpk.xuanzx.com

================================================================================
来源：http://ipg.mhx1999.top

G. 面向对象
来源：http://exy.ehwqpu.com

================================================================================
来源：http://akp.yj20258.top

[G01] 定义类
来源：http://jnz.jinghuilouyu.cn

Py:   class User: pass
来源：http://qnf.hcnkem.com

PHP:  class User {}
来源：http://tkm.fktsv.cn

JS:   class User {}
来源：http://tdo.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://yix.jqgufenzy.top

Java: class User {}
来源：http://erg.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://ewk.tanke756.top

Ruby: class User; end
来源：http://nnh.ivvv.top

C#:   class User {}
来源：http://rmi.sjlbkw.cn

[G02] 构造函数
来源：http://iyv.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://tpy.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://dqv.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://qau.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://lxc.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://ohv.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://edy.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://mcv.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://tzd.hcnkem.com

[G03] 实例属性
来源：http://bhk.zhiwuduotai.top

Py:   self.name = "x"
来源：http://vrq.iojbl.cn

PHP:  public string $name = "x";
来源：http://qhg.hongshengwenyu.top

JS:   this.name = "x";
来源：http://pke.nanxinkj.top

TS:   name: string = "x";
来源：http://rjx.jinqigufen.top

Java: private String name;
来源：http://xlw.cdnleiting.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wyx.dashuyun.cn

Ruby: @name = "x"
来源：http://qqi.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://mky.pengpengdd.cyou

[G04] 定义方法
来源：http://tyn.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://xyh.kuanghao11.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ydq.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://bar.kuanghao11.cn

TS:   greet(): string { return this.name; }
来源：http://ztp.jinqigufen.top

Java: String greet() { return name; }
来源：http://itl.tianlin.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://baj.nanxinkj.top

Ruby: def greet; @name; end
来源：http://lzu.tarul.cn

C#:   public string Greet() => Name;
来源：http://oqi.ctjpmb.com

[G05] 继承
来源：http://ioc.redwolf501.top

Py:   class Admin(User): pass
来源：http://byo.iojbl.cn

PHP:  class Admin extends User {}
来源：http://ezq.dashuyun.cn

JS:   class Admin extends User {}
来源：http://rur.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://did.jiagoushi.top

Java: class Admin extends User {}
来源：http://hgm.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtm.aizwys.cn

Ruby: class Admin < User; end
来源：http://egj.yuxming.cn

C#:   class Admin : User {}
来源：http://dwl.daria6918.cn

[G06] 重写方法
来源：http://lmk.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://tnn.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cwx.yonumen.top

JS:   greet() { return "admin"; }
来源：http://ksj.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://rnn.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://mkz.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ixw.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://gva.smart0.xyz

C#:   public override string Greet() => "admin";
来源：http://bpq.aibaodan.cn

[G07] 调用父类方法
来源：http://bix.feifeiyinyue.top

Py:   super().greet()
来源：http://zlh.jinqigfzy.top

PHP:  parent::greet();
来源：http://jkh.shanyushiyangtech.top

JS:   super.greet();
来源：http://hwj.daxiang520.top

TS:   super.greet();
来源：http://msh.quarkkingdee.top

Java: super.greet();
来源：http://zmj.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://noq.hongshengwenyu.top

Ruby: super
来源：http://ysv.sjlbkw.cn

C#:   base.Greet();
来源：http://uhs.tanke756.top

[G08] 静态方法与属性
来源：http://haz.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://krs.zhixingplan.top

PHP:  public static function f() {}
来源：http://xve.xuanzx.com

JS:   static f() {}
来源：http://qub.cdnleiting.top

TS:   static f(): void {}
来源：http://pvo.zhaomingkeji.xyz

Java: static void f() {}
来源：http://rpx.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://apl.jyoumei.cn

Ruby: def self.f; end
来源：http://lre.yanxiufei.cn

C#:   public static void F() {}
来源：http://lou.hnqzz.top

[G09] 接口 / 抽象类
来源：http://imm.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://fuq.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://cid.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tto.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://bym.gzhubu.top

Java: interface Shape { double area(); }
来源：http://bpt.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://rqt.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rdq.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://tqy.ywan-chungtsiang.top

[G10] 访问控制
来源：http://luv.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://xdz.gotoacloud.top

PHP:  public / protected / private
来源：http://dsa.c1oappe.top

JS:   #private 字段；其余公开
来源：http://zmq.jinghuilouyu.cn

TS:   public / protected / private
来源：http://sqe.xylfe.cn

Java: public / protected / private / 默认包级
来源：http://leh.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ewj.bjfxy.top

Ruby: public / protected / private
来源：http://dux.ehwqpu.com

C#:   public / protected / private / internal
来源：http://bpf.chenlongwang.top

[G11] getter / setter
来源：http://qfq.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://gfl.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ari.chenlongwang.top

JS:   get name() { return this._name; }
来源：http://rpc.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://ssf.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://ywp.ehwqpu.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://nne.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://ybv.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://zac.vqdsnc.cn

[G12] 对象转字符串
来源：http://ghx.yanxiufei.cn

Py:   def __str__(self): return self.name
来源：http://zfg.sweek.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dcq.haohaochexian.top

JS:   toString() { return this.name; }
来源：http://kyd.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://gcq.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://lsy.jqgufenzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://qsy.hfpthk.cn

Ruby: def to_s; @name; end
来源：http://dzy.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://uzy.daria6918.cn

[G13] 判断对象类型
来源：http://ajo.aibaodan.cn

Py:   isinstance(u, User)
来源：http://yox.haohaochexian.top

PHP:  $u instanceof User
来源：http://cys.redwolf501.top

JS:   u instanceof User
来源：http://fxh.ctjpmb.com

TS:   u instanceof User
来源：http://rxw.jinqigfzy.top

Java: u instanceof User
来源：http://cik.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tfr.andypj.xyz

Ruby: u.is_a?(User)
来源：http://bkw.hfpthk.cn

C#:   u is User
来源：http://zdl.316326.xyz

[G14] 数据类 / record
来源：http://pmu.0kj1m.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vnz.hfpthk.cn

PHP:  // 用 readonly 属性模拟
来源：http://hoh.yongpay.top

JS:   // 无内置：普通类或对象字面量
来源：http://kft.sjlbkw.cn

TS:   type User = { name: string; age: number };
来源：http://bev.pengpengdd.cyou

Java: record User(String name, int age) {}
来源：http://ovb.redwolf501.top

Go:   type User struct { Name string; Age int }
来源：http://peg.yj202588.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mdy.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://rxr.jinyuanbaomall.cn

[G15] 枚举
来源：http://eoo.quarkkingdee.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jha.guowangkeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pyi.zhixingplan.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kci.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rpb.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://qla.jqgufenzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bzm.pycfn.com

Ruby: Color = %i[red green].freeze
来源：http://sxg.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://srh.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://gip.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kqz.pycfn.com

PHP:  get_object_vars($obj);
来源：http://mcw.yonumen.top

JS:   Object.entries(obj)
来源：http://qxb.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://pfw.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pbr.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://fwc.xingfuxueyuan.xyz

Ruby: obj.instance_variables
来源：http://pkt.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://gwq.cdnleiting.top

================================================================================
来源：http://hpa.ivvv.top

H. 异常与错误处理
来源：http://qph.c1oappe.top

================================================================================
来源：http://jxx.aibaodan.cn

[H01] try / catch 基础
来源：http://yae.hesvh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://opy.zhongyouzk.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xjv.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yfb.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rnu.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uez.daria6918.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ifg.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gvx.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://saw.sweek.top

[H02] finally / ensure 收尾
来源：http://xzn.hnqzz.top

Py:   try: f()⏎finally: cleanup()
来源：http://vus.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://siz.316326.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://var.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hur.yuxming.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dfl.dashuyun.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nyw.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://icf.xinyue.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://ewv.hesvh.cn

[H03] 主动抛出异常
来源：http://foi.xingfuxueyuan.xyz

Py:   raise ValueError("错误信息")
来源：http://rvw.shanyushiyangtech.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://esr.cdnleiting.top

JS:   throw new Error("错误信息");
来源：http://cja.c1oappe.top

TS:   throw new Error("错误信息");
来源：http://lyd.yj20258888.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hwp.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tuf.xylfe.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bmj.hammf.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mbb.jqgfzy.top

[H04] 自定义异常类型
来源：http://htf.havefunace.top

Py:   class MyError(Exception): pass
来源：http://rvx.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://jym.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://xyv.hesvh.cn

TS:   class MyError extends Error {}
来源：http://rbe.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://pmv.smart0.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yqy.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://kxs.hesvh.cn

C#:   class MyException : Exception {}
来源：http://jhd.mhx1999.top

[H05] 捕获特定类型
来源：http://vfl.tianlin.xyz

Py:   except ValueError as e:
来源：http://kff.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ehn.jinyuanbaomall.cn

JS:   if (e instanceof TypeError) {}
来源：http://vpm.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://eft.jyoumei.cn

Java: catch (IOException | SQLException e) {}
来源：http://nqu.jinghuilouyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://acu.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://jjz.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sil.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://rey.c1oappe.top


<!-- 参考信息 -->