代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zry.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kif.ctjpmb.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://itv.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xig.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cwz.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ymq.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dnm.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fyz.gzhubu.top

[E22] 字节长度与字符长度
来源：http://yzf.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://too.jqgufenzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ynt.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rmd.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mfl.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wul.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sxy.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://dnw.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eqr.hywenlv.cn

================================================================================
来源：http://fgp.pycfn.com

F. 文件与目录
来源：http://utt.gaohongyu789.top

================================================================================
来源：http://mgv.chenlongwang.top

[F01] 读取整个文件
来源：http://lag.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qkb.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://ksu.dashuyun.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ayk.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sbk.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://kdu.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gng.shuidangran.top

Ruby: File.read("a.txt")
来源：http://tsw.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://xnu.316326.xyz

[F02] 逐行读取文件
来源：http://euz.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uyv.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://iop.jinqigfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://beh.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://onu.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lcx.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://exi.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uef.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nrj.shanyushiyangtech.top

[F03] 写入文件（覆盖）
来源：http://eql.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dyg.svipenyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://amr.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjd.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dbd.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://epf.yanxiufei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qdw.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://mzd.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://msp.hywenlv.cn

[F04] 追加写入文件
来源：http://ppa.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yeh.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hid.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://esk.yangfankeji.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://odj.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://adk.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kwy.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ucy.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ksm.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://xdz.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ihm.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://sjk.cucudq.cn

JS:   fs.existsSync("a.txt")
来源：http://wvz.yongpay.top

TS:   fs.existsSync("a.txt")
来源：http://faj.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nyb.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gds.yonumen.top

Ruby: File.exist?("a.txt")
来源：http://unu.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://vwh.svipenyu.cn

[F06] 删除文件
来源：http://ydt.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://vhi.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://cpi.zhaomingkeji.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://xey.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://twh.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://svi.zhongyouzk.top

Go:   os.Remove("a.txt")
来源：http://xbl.xuetiantiany.cn

Ruby: File.delete("a.txt")
来源：http://oow.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://fan.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://lcg.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dvi.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://weg.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyb.gaohongyu789.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bdy.jinqigfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://flb.tarul.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wku.havefunace.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ihg.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vxa.iojbl.cn

[F08] 遍历目录
来源：http://qam.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vui.chenlongwang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qzx.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://djv.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://tlf.cucudq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oks.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zya.mhx1999.top

Ruby: Dir.children("dir")
来源：http://ojx.iojbl.cn

C#:   Directory.GetFiles("dir")
来源：http://drn.zycfv.cn

[F09] 获取文件大小
来源：http://kmp.chenlongwang.top

Py:   os.path.getsize("a.txt")
来源：http://vcs.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://zjt.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://sbq.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://qpo.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://qiv.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://npq.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://csy.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://ell.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://wcl.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://utl.xinyue.icu

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mcd.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://leu.xziqi.cn

TS:   path.extname("a.txt")
来源：http://lyy.xuanzx.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gsg.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jrc.gzhubu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ytk.quarkkingdee.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eqj.wangdashe.top

[F11] 复制与移动文件
来源：http://bvu.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nge.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gbz.jlsjyb.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://naz.hesvh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lax.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jjf.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yah.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jdr.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://flf.sjlbkw.cn

[F12] CSV 读写
来源：http://pye.havefunace.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oic.wangshuangyany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://njm.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://woz.fzhhl.top

TS:   // 同上
来源：http://vur.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ujj.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gfi.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://drq.pengpengdd.cyou

C#:   // 无内置：用 CsvHelper 库
来源：http://mpg.c1oappe.top

================================================================================
来源：http://zij.dashuyun.cn

G. 面向对象
来源：http://rbp.mhx1999.top

================================================================================
来源：http://kfi.yuxming.cn

[G01] 定义类
来源：http://qkg.vqdsnc.cn

Py:   class User: pass
来源：http://der.shuidangran.top

PHP:  class User {}
来源：http://xgx.shanyushiyangtech.top

JS:   class User {}
来源：http://zny.tarul.cn

TS:   class User { name: string = ""; }
来源：http://vxi.xingfuxueyuan.xyz

Java: class User {}
来源：http://spm.xuanzx.com

Go:   type User struct { Name string }
来源：http://xjw.hnqzz.top

Ruby: class User; end
来源：http://ecz.ctjpmb.com

C#:   class User {}
来源：http://yjz.vqdsnc.cn

[G02] 构造函数
来源：http://wem.hnqzz.top

Py:   def __init__(self, name): self.name = name
来源：http://ovr.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://hoz.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://dek.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://zoh.ivvv.top

Java: User(String name) { this.name = name; }
来源：http://twq.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ozn.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://cig.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://dki.tian-w.cn

[G03] 实例属性
来源：http://rip.xylfe.cn

Py:   self.name = "x"
来源：http://qmi.ywan-chungtsiang.top

PHP:  public string $name = "x";
来源：http://hzb.yj20258888.top

JS:   this.name = "x";
来源：http://hkb.xylfe.cn

TS:   name: string = "x";
来源：http://tpc.aibaodan.cn

Java: private String name;
来源：http://ihh.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mmo.pycfn.com

Ruby: @name = "x"
来源：http://sjn.jinqigufen.top

C#:   public string Name { get; set; } = "x";
来源：http://byt.tian-w.cn

[G04] 定义方法
来源：http://ttg.yj20258888.top

Py:   def greet(self): return self.name
来源：http://myb.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://slt.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://oze.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://qrh.daria6918.cn

Java: String greet() { return name; }
来源：http://ljk.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vte.ybcxt.top

Ruby: def greet; @name; end
来源：http://exp.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://kzh.sufxvd.cn

[G05] 继承
来源：http://nbx.chenlongwang.top

Py:   class Admin(User): pass
来源：http://abk.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://omt.yuanzhike.top

JS:   class Admin extends User {}
来源：http://uam.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://nit.smart0.xyz

Java: class Admin extends User {}
来源：http://umx.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dlz.gotoacloud.top

Ruby: class Admin < User; end
来源：http://hxs.zhijiandao.cn

C#:   class Admin : User {}
来源：http://ejh.52xcode.cn

[G06] 重写方法
来源：http://atr.zhiwuduotai.top

Py:   def greet(self): return "admin"
来源：http://zmb.shuidangran.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jnw.cashguo.top

JS:   greet() { return "admin"; }
来源：http://wql.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://ehd.wangshuangyany.cn

Java: @Override String greet() { return "admin"; }
来源：http://cua.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gis.hnqzz.top

Ruby: def greet; "admin"; end
来源：http://how.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://ywo.pengpengdd.cyou

[G07] 调用父类方法
来源：http://ade.yj20258.top

Py:   super().greet()
来源：http://yfg.vqdsnc.cn

PHP:  parent::greet();
来源：http://tqw.zdbjq.cn

JS:   super.greet();
来源：http://tip.jinghuilouyu.cn

TS:   super.greet();
来源：http://caz.316326.xyz

Java: super.greet();
来源：http://umk.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://drz.tianlin.xyz

Ruby: super
来源：http://tna.mhx1999.top

C#:   base.Greet();
来源：http://mva.xuanzx.com

[G08] 静态方法与属性
来源：http://jfb.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uyp.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://vka.aizwys.cn

JS:   static f() {}
来源：http://rjj.cdnleiting.top

TS:   static f(): void {}
来源：http://oug.hongshengwenyu.top

Java: static void f() {}
来源：http://lte.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uqd.yueranfly.top

Ruby: def self.f; end
来源：http://bcr.nanxuanxn.top

C#:   public static void F() {}
来源：http://wkk.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://zsf.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://epm.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://rrh.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uok.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://vmq.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://hbn.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://nys.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fcu.jiagoushi.top

C#:   interface IShape { double Area(); }
来源：http://iaj.tianlin.xyz

[G10] 访问控制
来源：http://gvn.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://qrf.ivvv.top

PHP:  public / protected / private
来源：http://xtm.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://hub.vqdsnc.cn

TS:   public / protected / private
来源：http://gal.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://fma.yfazqb.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://odu.sxryk.cn

Ruby: public / protected / private
来源：http://ykj.svipenyu.cn

C#:   public / protected / private / internal
来源：http://ilq.haohaochexian.top

[G11] getter / setter
来源：http://xal.mhx1999.top

Py:   @property 与 @x.setter
来源：http://bxk.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mgd.ybcxt.top

JS:   get name() { return this._name; }
来源：http://nix.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://zkz.tian-w.cn

Java: public String getName() { return name; }
来源：http://nww.shanyushiyangtech.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lzf.fzhhl.top

Ruby: attr_accessor :name
来源：http://esh.smart0.xyz

C#:   public string Name { get; set; }
来源：http://rql.fengsongda.top

[G12] 对象转字符串
来源：http://zdk.havefunace.top

Py:   def __str__(self): return self.name
来源：http://chs.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://agk.ivvv.top

JS:   toString() { return this.name; }
来源：http://jvh.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://bqy.sufxvd.cn

Java: @Override public String toString() { return name; }
来源：http://wlj.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bll.smart0.xyz

Ruby: def to_s; @name; end
来源：http://owy.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://tuv.dashuyun.cn

[G13] 判断对象类型
来源：http://una.52xcode.cn

Py:   isinstance(u, User)
来源：http://dqj.xylfe.cn

PHP:  $u instanceof User
来源：http://tqy.zhiwuduotai.top

JS:   u instanceof User
来源：http://ppi.tianlin.xyz

TS:   u instanceof User
来源：http://wkj.ctjpmb.com

Java: u instanceof User
来源：http://zuo.epnwcf.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://byy.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://rtz.xingfuxueyuan.xyz

C#:   u is User
来源：http://ajl.smart0.xyz

[G14] 数据类 / record
来源：http://kek.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nip.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://uav.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://vbf.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://tkz.hfpthk.cn

Java: record User(String name, int age) {}
来源：http://imq.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://xtv.mhx1999.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xce.c1oappe.top

C#:   record User(string Name, int Age);
来源：http://cms.jinyuanbaomall.cn

[G15] 枚举
来源：http://lag.tianlin.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bdi.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tub.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mfr.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://goj.fengsongda.top

Java: enum Color { RED, GREEN }
来源：http://aky.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oww.zhiwuduotai.top

Ruby: Color = %i[red green].freeze
来源：http://hgg.jlsjyb.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lzg.zhongyouzk.top

[G16] 对象转数组 / 字典
来源：http://kjg.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hmx.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://xqc.birdmap.top

JS:   Object.entries(obj)
来源：http://dty.daxiang520.top

TS:   Object.entries(obj)
来源：http://ijg.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://neu.yj202588.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ijt.daria6918.cn

Ruby: obj.instance_variables
来源：http://vge.dianchejie.cn

C#:   // 用反射或 System.Text.Json
来源：http://kme.daxiang520.top

================================================================================
来源：http://asf.hongshengwenyu.top

H. 异常与错误处理
来源：http://hvq.gaohongyu789.top

================================================================================
来源：http://mbx.quarkkingdee.top

[H01] try / catch 基础
来源：http://tje.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mao.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wqv.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bmp.0kj1m.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dkm.gaohongyu789.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://njw.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lym.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rpo.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iws.gotoacloud.top

[H02] finally / ensure 收尾
来源：http://ksf.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jeo.xziqi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://grn.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ahk.316326.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://seg.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://fjd.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://htc.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://nwd.zhoulong.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://dlg.aizwys.cn

[H03] 主动抛出异常
来源：http://ary.yj20258.top

Py:   raise ValueError("错误信息")
来源：http://fmy.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jgv.shanyushiyangtech.top

JS:   throw new Error("错误信息");
来源：http://shr.yj20258888.top


<!-- 参考信息 -->