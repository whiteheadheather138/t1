代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bxt.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vls.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uqe.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wit.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vba.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://mox.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rho.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zrt.ivvv.top

[E22] 字节长度与字符长度
来源：http://zpn.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cxi.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ttx.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nfu.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vmo.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://crt.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lld.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://kyk.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bdc.yfazqb.com

================================================================================
来源：http://hot.haohaochexian.top

F. 文件与目录
来源：http://yrs.gzhubu.top

================================================================================
来源：http://pwh.hnqzz.top

[F01] 读取整个文件
来源：http://yjf.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kgz.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://fnw.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zgu.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ntx.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ckc.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tyf.redwolf501.top

Ruby: File.read("a.txt")
来源：http://aoi.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://uuo.52xcode.cn

[F02] 逐行读取文件
来源：http://knr.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sus.zhixingplan.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zaj.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bhv.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hdx.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tnf.jqgfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://twb.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yut.nanxuanxn.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fyn.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://ncx.sweek.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nrf.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://ick.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cig.jiagoushi.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zim.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zin.dianchejie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iuu.svipenyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://snp.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tra.jianghu66.top

[F04] 追加写入文件
来源：http://ife.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nxi.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://szn.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mkf.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zpg.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://esa.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vcq.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hue.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lmt.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://dfp.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xen.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://bwn.dashuyun.cn

JS:   fs.existsSync("a.txt")
来源：http://bcg.birdmap.top

TS:   fs.existsSync("a.txt")
来源：http://dde.xingfuxueyuan.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://tnk.haohaochexian.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kdf.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://tko.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://mwn.fktsv.cn

[F06] 删除文件
来源：http://cnd.iojbl.cn

Py:   os.remove("a.txt")
来源：http://uiq.shanyushiyangtech.top

PHP:  unlink("a.txt");
来源：http://cam.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://gbm.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://nkn.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://maa.xingfuxueyuan.xyz

Go:   os.Remove("a.txt")
来源：http://fpx.shangyingyoupin.top

Ruby: File.delete("a.txt")
来源：http://mdv.smart0.xyz

C#:   File.Delete("a.txt");
来源：http://wcn.bjfxy.top

[F07] 创建目录（含多级）
来源：http://usf.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aqj.hfpthk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nno.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ivn.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uos.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ylf.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nas.jinghuilouyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ngc.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fte.yonumen.top

[F08] 遍历目录
来源：http://ktu.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kun.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sru.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://bav.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://ftc.gaohongyu789.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sls.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://hmy.pycfn.com

Ruby: Dir.children("dir")
来源：http://lqi.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://cbj.quarkkingdee.top

[F09] 获取文件大小
来源：http://sjp.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://qyt.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://yqz.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://zge.gaohongyu789.top

TS:   fs.statSync("a.txt").size
来源：http://lvt.nanxinkj.top

Java: Files.size(Path.of("a.txt"))
来源：http://zpp.zhoulong.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ize.mhx1999.top

Ruby: File.size("a.txt")
来源：http://whg.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://bkz.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://jrg.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xxw.sysykeji.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yje.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tnq.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://kok.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ior.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dyn.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hle.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://upz.shzxlz.cn

[F11] 复制与移动文件
来源：http://frg.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dyw.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://iqb.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymd.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sou.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zbm.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xbk.xingfuxueyuan.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jup.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bgi.vehdjk.com

[F12] CSV 读写
来源：http://qyu.ywan-chungtsiang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://foe.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ipf.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cmj.ppjwa.cn

TS:   // 同上
来源：http://gri.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pxr.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://adk.yueranfly.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oyx.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zlk.birdmap.top

================================================================================
来源：http://lnc.iojbl.cn

G. 面向对象
来源：http://ewz.guowangkeji.top

================================================================================
来源：http://cwk.yj20258.top

[G01] 定义类
来源：http://qrz.tarul.cn

Py:   class User: pass
来源：http://qni.andypj.xyz

PHP:  class User {}
来源：http://ohe.yvedp.cn

JS:   class User {}
来源：http://ddk.tarul.cn

TS:   class User { name: string = ""; }
来源：http://tmr.shuidangran.top

Java: class User {}
来源：http://ojl.zdbjq.cn

Go:   type User struct { Name string }
来源：http://fka.ivvv.top

Ruby: class User; end
来源：http://pae.c1oappe.top

C#:   class User {}
来源：http://tdq.dashuyun.cn

[G02] 构造函数
来源：http://npx.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://qyo.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://dtu.xziqi.cn

JS:   constructor(name) { this.name = name; }
来源：http://frc.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://dex.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://rtq.daria6918.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://clw.cucudq.cn

Ruby: def initialize(name); @name = name; end
来源：http://aau.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://gom.yuanzhike.top

[G03] 实例属性
来源：http://lkw.dianchejie.cn

Py:   self.name = "x"
来源：http://thj.xuanzx.com

PHP:  public string $name = "x";
来源：http://mvw.snrcjt.cn

JS:   this.name = "x";
来源：http://tvs.chenjidiqi.icu

TS:   name: string = "x";
来源：http://zfp.hesvh.cn

Java: private String name;
来源：http://oot.smart0.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wxf.316326.xyz

Ruby: @name = "x"
来源：http://waq.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://whe.ydjk.org.cn

[G04] 定义方法
来源：http://mdx.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://xeb.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ius.sysykeji.top

JS:   greet() { return this.name; }
来源：http://oiu.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://jpk.smart0.xyz

Java: String greet() { return name; }
来源：http://uol.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fbi.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://slm.cucudq.cn

C#:   public string Greet() => Name;
来源：http://gcn.ydzc1.top

[G05] 继承
来源：http://xzi.chenlongwang.top

Py:   class Admin(User): pass
来源：http://yux.yvedp.cn

PHP:  class Admin extends User {}
来源：http://kln.aizwys.cn

JS:   class Admin extends User {}
来源：http://wye.sufxvd.cn

TS:   class Admin extends User {}
来源：http://fun.zhoulong.xyz

Java: class Admin extends User {}
来源：http://sky.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iox.chenjidiqi.icu

Ruby: class Admin < User; end
来源：http://ebu.cucudq.cn

C#:   class Admin : User {}
来源：http://pdm.gzhubu.top

[G06] 重写方法
来源：http://gvy.hfpthk.cn

Py:   def greet(self): return "admin"
来源：http://fek.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hqu.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://wml.hongshengwenyu.top

TS:   greet(): string { return "admin"; }
来源：http://gct.shuidangran.top

Java: @Override String greet() { return "admin"; }
来源：http://buh.dianchejie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wan.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://fwt.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://keb.zhoulong.xyz

[G07] 调用父类方法
来源：http://nos.xylfe.cn

Py:   super().greet()
来源：http://sjf.cheryme.top

PHP:  parent::greet();
来源：http://vqb.yj20258888.top

JS:   super.greet();
来源：http://ies.aizwys.cn

TS:   super.greet();
来源：http://ldk.yfazqb.com

Java: super.greet();
来源：http://jit.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nzg.jlsjyb.cn

Ruby: super
来源：http://ylk.c1oappe.top

C#:   base.Greet();
来源：http://rbx.yanxiufei.cn

[G08] 静态方法与属性
来源：http://wdg.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sux.hesvh.cn

PHP:  public static function f() {}
来源：http://jtd.xziqi.cn

JS:   static f() {}
来源：http://ujf.sweek.top

TS:   static f(): void {}
来源：http://zqy.jianghu66.top

Java: static void f() {}
来源：http://ddc.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zxx.gaohongyu789.top

Ruby: def self.f; end
来源：http://lcq.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://hoa.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://hyr.jinghuilouyu.cn

Py:   from abc import ABC, abstractmethod
来源：http://nhn.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://cxv.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ush.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://wwo.hnqzz.top

Java: interface Shape { double area(); }
来源：http://llw.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://ole.dianchejie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zdu.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://znn.zhixingplan.top

[G10] 访问控制
来源：http://bis.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://wfp.hysaishi.cn

PHP:  public / protected / private
来源：http://cve.zycfv.cn

JS:   #private 字段；其余公开
来源：http://qxf.yj20258888.top

TS:   public / protected / private
来源：http://xle.hywenlv.cn

Java: public / protected / private / 默认包级
来源：http://kqt.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xsz.pycfn.com

Ruby: public / protected / private
来源：http://zfj.ivvv.top

C#:   public / protected / private / internal
来源：http://jeq.jinqigufen.top

[G11] getter / setter
来源：http://vhd.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://pyz.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cel.fktsv.cn

JS:   get name() { return this._name; }
来源：http://qsj.xingfuxueyuan.xyz

TS:   get name(): string { return this._name; }
来源：http://gfi.vehdjk.com

Java: public String getName() { return name; }
来源：http://ylt.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://kiy.yonumen.top

Ruby: attr_accessor :name
来源：http://jeq.zycfv.cn

C#:   public string Name { get; set; }
来源：http://sdy.ybcxt.top

[G12] 对象转字符串
来源：http://bhq.cashguo.top

Py:   def __str__(self): return self.name
来源：http://tsl.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://klk.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://wmt.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://dsy.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://tqj.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://hoa.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://kvl.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://cgs.dashuyun.cn

[G13] 判断对象类型
来源：http://gbg.xylfe.cn

Py:   isinstance(u, User)
来源：http://wwu.zdbjq.cn

PHP:  $u instanceof User
来源：http://qvb.xuetiantiany.cn

JS:   u instanceof User
来源：http://hyn.yangfankeji.com

TS:   u instanceof User
来源：http://wmw.zhixingplan.top

Java: u instanceof User
来源：http://rad.cashguo.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xqb.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://kgq.gzhubu.top

C#:   u is User
来源：http://nbj.guannengcc.top

[G14] 数据类 / record
来源：http://idc.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yfl.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://phi.feifeiyinyue.top

JS:   // 无内置：普通类或对象字面量
来源：http://reo.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://aec.aizwys.cn

Java: record User(String name, int age) {}
来源：http://zlm.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://ljk.zhijiandao.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://udj.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://wve.316326.xyz

[G15] 枚举
来源：http://rad.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mop.zycfv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nnu.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xzr.shanyushiyangtech.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xcm.ivvv.top

Java: enum Color { RED, GREEN }
来源：http://pcx.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dwf.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://wzt.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jtp.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://zww.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kln.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://mzj.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://aqs.xylfe.cn

TS:   Object.entries(obj)
来源：http://tll.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nvd.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://oxz.hysaishi.cn

Ruby: obj.instance_variables
来源：http://pvn.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://yyb.feifeiyinyue.top

================================================================================
来源：http://ozm.hongshengwenyu.top

H. 异常与错误处理
来源：http://hyh.aibaodan.cn

================================================================================
来源：http://xak.gotoacloud.top

[H01] try / catch 基础
来源：http://ayi.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://faa.cheryme.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dwl.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bng.hesvh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hnq.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rwl.zhoulong.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hgp.jyoumei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yyl.quarkkingdee.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rmi.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://low.fzhhl.top

Py:   try: f()⏎finally: cleanup()
来源：http://zhk.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kca.hfpthk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://axu.tianlin.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://fel.nanxuanxn.top

Java: try { f(); } finally { cleanup(); }
来源：http://fri.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zws.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rpm.jinghuilouyu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://iib.guowangkeji.top

[H03] 主动抛出异常
来源：http://hgc.zycfv.cn

Py:   raise ValueError("错误信息")
来源：http://olm.yuxming.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lbh.uphjek.com

JS:   throw new Error("错误信息");
来源：http://lkb.wangdashe.top


<!-- 参考信息 -->