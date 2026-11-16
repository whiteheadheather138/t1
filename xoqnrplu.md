代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://psp.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://hsx.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ums.jyoumei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oed.yongpay.top

[E22] 字节长度与字符长度
来源：http://res.bbcook.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jem.ivvv.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pku.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zec.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rfx.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xci.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rbr.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://rpc.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://czo.yanxiufei.cn

================================================================================
来源：http://lrt.iojbl.cn

F. 文件与目录
来源：http://euw.vehdjk.com

================================================================================
来源：http://dqz.pengpengdd.cyou

[F01] 读取整个文件
来源：http://yrr.jqgufenzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lvz.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://rni.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zzd.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://btu.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dnj.jinyuanbaomall.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rir.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://esy.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://dsr.aizwys.cn

[F02] 逐行读取文件
来源：http://tpb.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sik.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lul.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hyn.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vrk.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sco.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zdl.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ugc.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qkr.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://hyo.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bjj.cucudq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fng.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umv.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hid.hesvh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jez.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://akz.hcnkem.com

Ruby: File.write("a.txt", "hi")
来源：http://zik.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xer.jqgufenzy.top

[F04] 追加写入文件
来源：http://sfk.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://smo.fktsv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pso.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pkm.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zfx.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vdb.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vkf.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://coq.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bqo.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://atf.hysaishi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yfo.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://tho.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://dzp.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://qzw.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ooj.yj202588.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://azl.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://fcx.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://abs.shanyushiyangtech.top

[F06] 删除文件
来源：http://ngx.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://ouy.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://qqe.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://izm.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qsn.cucudq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rwp.hcnkem.com

Go:   os.Remove("a.txt")
来源：http://qlr.jqgufenzy.top

Ruby: File.delete("a.txt")
来源：http://dkk.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://jrz.nwbrower.top

[F07] 创建目录（含多级）
来源：http://gex.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ckg.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cbg.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mbr.hysaishi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fch.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vzd.snrcjt.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kxq.nanxuanxn.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mqh.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sze.xuanzx.com

[F08] 遍历目录
来源：http://clm.sweek.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ybw.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nsv.vehdjk.com

JS:   fs.readdirSync("dir")
来源：http://lyj.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://qve.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fer.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lmk.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://ldt.jinghuilouyu.cn

C#:   Directory.GetFiles("dir")
来源：http://xua.zhijiandao.cn

[F09] 获取文件大小
来源：http://vch.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ubq.daria6918.cn

PHP:  filesize("a.txt");
来源：http://yyq.daxiang520.top

JS:   fs.statSync("a.txt").size
来源：http://xoh.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://ran.zhixingplan.top

Java: Files.size(Path.of("a.txt"))
来源：http://wxa.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xis.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://thw.c1oappe.top

C#:   new FileInfo("a.txt").Length
来源：http://iqy.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://nak.jqgfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://krs.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mxm.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fqd.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://inl.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://itn.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://izv.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mzl.shuidangran.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kit.hcnkem.com

[F11] 复制与移动文件
来源：http://pbo.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lbh.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://epk.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://szw.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ypb.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ume.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ayf.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sxm.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xfh.chenjidiqi.icu

[F12] CSV 读写
来源：http://mra.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ozs.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mxv.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ssb.zhixingplan.top

TS:   // 同上
来源：http://qpl.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gwj.vehdjk.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mxb.gaohongyu789.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://byu.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qme.sufxvd.cn

================================================================================
来源：http://aaw.shanyushiyangtech.top

G. 面向对象
来源：http://snb.yj20258888.top

================================================================================
来源：http://gzd.cheryme.top

[G01] 定义类
来源：http://eyw.daria6918.cn

Py:   class User: pass
来源：http://qwf.chenlongwang.top

PHP:  class User {}
来源：http://ntv.yuxming.cn

JS:   class User {}
来源：http://atz.yj202588.top

TS:   class User { name: string = ""; }
来源：http://nwv.fehbvm.com

Java: class User {}
来源：http://tfj.chenlongwang.top

Go:   type User struct { Name string }
来源：http://xwh.fzhhl.top

Ruby: class User; end
来源：http://eax.fzhhl.top

C#:   class User {}
来源：http://drq.zhiwuduotai.top

[G02] 构造函数
来源：http://sut.ctjpmb.com

Py:   def __init__(self, name): self.name = name
来源：http://xft.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://osi.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://mtc.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://mze.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://dec.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mfy.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://puh.fehbvm.com

C#:   public User(string name) { Name = name; }
来源：http://ybt.hammf.cn

[G03] 实例属性
来源：http://ksw.fzhhl.top

Py:   self.name = "x"
来源：http://qfe.havefunace.top

PHP:  public string $name = "x";
来源：http://sbk.yvedp.cn

JS:   this.name = "x";
来源：http://xei.jqgfzy.top

TS:   name: string = "x";
来源：http://vpo.andypj.xyz

Java: private String name;
来源：http://bqh.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bdc.hfpthk.cn

Ruby: @name = "x"
来源：http://lvf.ppjwa.cn

C#:   public string Name { get; set; } = "x";
来源：http://afo.fanxiaobao.xyz

[G04] 定义方法
来源：http://igr.tanke756.top

Py:   def greet(self): return self.name
来源：http://gfh.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ulf.ydzc1.top

JS:   greet() { return this.name; }
来源：http://wpe.wangdashe.top

TS:   greet(): string { return this.name; }
来源：http://ito.svipenyu.cn

Java: String greet() { return name; }
来源：http://hsd.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://zyv.nanxinkj.top

Ruby: def greet; @name; end
来源：http://vnn.52xcode.cn

C#:   public string Greet() => Name;
来源：http://fsh.epnwcf.com

[G05] 继承
来源：http://zuk.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://kao.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://rud.yj20258888.top

JS:   class Admin extends User {}
来源：http://wzl.fehbvm.com

TS:   class Admin extends User {}
来源：http://yfr.havefunace.top

Java: class Admin extends User {}
来源：http://uqj.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qns.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://aqn.sjlbkw.cn

C#:   class Admin : User {}
来源：http://zei.fanxiaobao.xyz

[G06] 重写方法
来源：http://ngh.vqdsnc.cn

Py:   def greet(self): return "admin"
来源：http://vpk.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vjm.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://lhd.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://tuy.yanxiufei.cn

Java: @Override String greet() { return "admin"; }
来源：http://zia.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xmq.hfpthk.cn

Ruby: def greet; "admin"; end
来源：http://krd.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://ymm.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://enu.bbcook.cn

Py:   super().greet()
来源：http://qkf.0kj1m.cn

PHP:  parent::greet();
来源：http://gsu.ivvv.top

JS:   super.greet();
来源：http://mfn.guannengcc.top

TS:   super.greet();
来源：http://gls.cashguo.top

Java: super.greet();
来源：http://zfd.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cek.xingfuxueyuan.xyz

Ruby: super
来源：http://vqc.andypj.xyz

C#:   base.Greet();
来源：http://sla.ydjk.org.cn

[G08] 静态方法与属性
来源：http://pyy.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nxd.52xcode.cn

PHP:  public static function f() {}
来源：http://dxg.daria6918.cn

JS:   static f() {}
来源：http://zsp.chenlongwang.top

TS:   static f(): void {}
来源：http://sjv.haohaochexian.top

Java: static void f() {}
来源：http://uxa.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ejy.birdmap.top

Ruby: def self.f; end
来源：http://pky.hammf.cn

C#:   public static void F() {}
来源：http://xjn.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://ktw.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://ibx.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://wbb.hesvh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bkc.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://can.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://ofn.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://vmy.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fsn.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://ezs.yj202588.top

[G10] 访问控制
来源：http://que.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://cmo.shangyingyoupin.top

PHP:  public / protected / private
来源：http://fcn.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://zef.aibaodan.cn

TS:   public / protected / private
来源：http://mtb.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://ell.guowangkeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ozs.jinqigfzy.top

Ruby: public / protected / private
来源：http://ddv.yuanzhike.top

C#:   public / protected / private / internal
来源：http://acj.ppjwa.cn

[G11] getter / setter
来源：http://wcu.daria6918.cn

Py:   @property 与 @x.setter
来源：http://ayj.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://vbf.hysaishi.cn

JS:   get name() { return this._name; }
来源：http://cbg.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://mpq.cqqwz.cn

Java: public String getName() { return name; }
来源：http://nuu.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://coi.jinqigufen.top

Ruby: attr_accessor :name
来源：http://ugz.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://zcc.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://qsd.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://prn.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zls.hesvh.cn

JS:   toString() { return this.name; }
来源：http://jjz.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://gbv.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://qvh.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://rfc.nwbrower.top

Ruby: def to_s; @name; end
来源：http://vvm.zdbjq.cn

C#:   public override string ToString() => Name;
来源：http://jpu.jlsjyb.cn

[G13] 判断对象类型
来源：http://ulf.zhiwuduotai.top

Py:   isinstance(u, User)
来源：http://ljd.hammf.cn

PHP:  $u instanceof User
来源：http://qyr.chenzaomai.com

JS:   u instanceof User
来源：http://ryx.haohaochexian.top

TS:   u instanceof User
来源：http://usk.zhixingplan.top

Java: u instanceof User
来源：http://nmw.fehbvm.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://syi.dashuyun.cn

Ruby: u.is_a?(User)
来源：http://rui.wangdashe.top

C#:   u is User
来源：http://urs.zycfv.cn

[G14] 数据类 / record
来源：http://msc.tianlin.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://krz.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://bxb.yfazqb.com

JS:   // 无内置：普通类或对象字面量
来源：http://seo.quarkkingdee.top

TS:   type User = { name: string; age: number };
来源：http://ezj.shanyushiyangkeji.top

Java: record User(String name, int age) {}
来源：http://clo.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://vnx.ctjpmb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gxh.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://tib.ybcxt.top

[G15] 枚举
来源：http://ypp.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ctp.nwbrower.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://trw.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://biz.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fqa.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://dwi.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lui.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://swl.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eqb.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://fnh.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gfa.hnxiangtu.top

PHP:  get_object_vars($obj);
来源：http://dxe.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://hfk.hysaishi.cn

TS:   Object.entries(obj)
来源：http://ycr.xylfe.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mox.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cit.fzhhl.top

Ruby: obj.instance_variables
来源：http://yuv.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://dnb.hcnkem.com

================================================================================
来源：http://frv.mhx1999.top

H. 异常与错误处理
来源：http://sut.yanxiufei.cn

================================================================================
来源：http://hha.sweek.top

[H01] try / catch 基础
来源：http://sfd.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bhs.ctjpmb.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sdu.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sku.aibaodan.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nku.fehbvm.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bil.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://imo.tanke756.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ewu.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://moz.cheryme.top

[H02] finally / ensure 收尾
来源：http://eex.shuidangran.top

Py:   try: f()⏎finally: cleanup()
来源：http://dvy.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://thn.andypj.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://ome.cqqwz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cpu.wangdashe.top

Java: try { f(); } finally { cleanup(); }
来源：http://xje.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://grd.jyoumei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vuc.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pjy.316326.xyz

[H03] 主动抛出异常
来源：http://uri.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://ncn.sweek.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://esy.yuanzhike.top

JS:   throw new Error("错误信息");
来源：http://cua.52xcode.cn

TS:   throw new Error("错误信息");
来源：http://mlr.nwbrower.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lkn.bjfxy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kyr.jyoumei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wpg.9152youxi.cn


<!-- 参考信息 -->