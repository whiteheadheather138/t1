代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lss.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bpt.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://prw.fanxiaobao.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmn.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zbe.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://ybh.ppjwa.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vfj.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tzq.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://bbk.jinghuilouyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txq.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hph.jinyuanbaomall.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iug.fengsongda.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oyk.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pfh.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ywy.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://xno.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ghw.ydjk.org.cn

================================================================================
来源：http://jir.tanke756.top

F. 文件与目录
来源：http://smx.xingfuxueyuan.xyz

================================================================================
来源：http://dra.zdbjq.cn

[F01] 读取整个文件
来源：http://ufd.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lhd.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://eqc.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ezw.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://efk.316326.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://wqj.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ygg.meibo888.top

Ruby: File.read("a.txt")
来源：http://rqx.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ekl.0kj1m.cn

[F02] 逐行读取文件
来源：http://fiw.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qsh.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hlx.yvedp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fvd.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akj.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ywd.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egu.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hcp.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://thp.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://haa.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnb.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://win.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://veq.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://utq.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jds.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://goc.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://kgj.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wag.chenzaomai.com

[F04] 追加写入文件
来源：http://phw.9152youxi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qeb.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xxw.svipenyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofg.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://weu.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ynb.hongshengwenyu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qsn.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fti.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zjn.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://bil.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oep.jinghuilouyu.cn

PHP:  file_exists("a.txt");
来源：http://maf.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://cso.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://fgo.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://eas.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://izi.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://fyg.zhengqikj.top

C#:   File.Exists("a.txt")
来源：http://qgt.yuxming.cn

[F06] 删除文件
来源：http://snv.kuanghao11.cn

Py:   os.remove("a.txt")
来源：http://vit.yj20258.top

PHP:  unlink("a.txt");
来源：http://xyr.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://cns.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ntd.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eii.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://cze.jlsjyb.cn

Ruby: File.delete("a.txt")
来源：http://qsb.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://uhy.bbcook.cn

[F07] 创建目录（含多级）
来源：http://qqx.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gxa.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rgn.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://loc.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ict.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://erj.zhaomingkeji.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xgn.mhx1999.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dso.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ipm.fktsv.cn

[F08] 遍历目录
来源：http://uag.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qtq.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jyb.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://gem.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://lhp.hysaishi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qko.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vio.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://fky.ivvv.top

C#:   Directory.GetFiles("dir")
来源：http://jyj.svipenyu.cn

[F09] 获取文件大小
来源：http://exr.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://jyd.jqgfzy.top

PHP:  filesize("a.txt");
来源：http://ptj.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://dyd.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://ina.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gsc.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gjs.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://vxa.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://tqp.havefunace.top

[F10] 取文件扩展名 / 文件名
来源：http://dkr.bjfxy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tcu.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pih.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pqs.bbcook.cn

TS:   path.extname("a.txt")
来源：http://fgn.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nkj.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rpc.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wlk.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://stq.dashuyun.cn

[F11] 复制与移动文件
来源：http://wuq.ybcxt.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fsp.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://byz.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gvm.yonumen.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mqk.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jjc.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://igh.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kzb.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mnj.zhengqikj.top

[F12] CSV 读写
来源：http://wdp.zhaomingkeji.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://twv.hesvh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rqp.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wbw.haohaochexian.top

TS:   // 同上
来源：http://dyc.yongpay.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yam.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qdm.daxiang520.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://deo.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://dlf.shuidangran.top

================================================================================
来源：http://sfe.sufxvd.cn

G. 面向对象
来源：http://njs.havefunace.top

================================================================================
来源：http://vha.sweek.top

[G01] 定义类
来源：http://eax.zhixingplan.top

Py:   class User: pass
来源：http://ydp.xylfe.cn

PHP:  class User {}
来源：http://kur.gzhubu.top

JS:   class User {}
来源：http://uwf.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://eda.cheryme.top

Java: class User {}
来源：http://hpb.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://dbh.hesvh.cn

Ruby: class User; end
来源：http://fgw.mhx1999.top

C#:   class User {}
来源：http://xof.andypj.xyz

[G02] 构造函数
来源：http://sxk.yj202588.top

Py:   def __init__(self, name): self.name = name
来源：http://bde.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://emr.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://ewh.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://brn.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://ahg.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://oyu.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://tmv.yanxiufei.cn

C#:   public User(string name) { Name = name; }
来源：http://htk.52xcode.cn

[G03] 实例属性
来源：http://vwp.daxiang520.top

Py:   self.name = "x"
来源：http://smu.shuidangran.top

PHP:  public string $name = "x";
来源：http://dac.zhijiandao.cn

JS:   this.name = "x";
来源：http://wmj.fktsv.cn

TS:   name: string = "x";
来源：http://spg.9152youxi.cn

Java: private String name;
来源：http://zoe.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ila.sufxvd.cn

Ruby: @name = "x"
来源：http://ank.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://xph.daxiang520.top

[G04] 定义方法
来源：http://pay.sweek.top

Py:   def greet(self): return self.name
来源：http://hbg.quarkkingdee.top

PHP:  public function greet(): string { return $this->name; }
来源：http://oww.bjfxy.top

JS:   greet() { return this.name; }
来源：http://xee.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://wxc.jyoumei.cn

Java: String greet() { return name; }
来源：http://tos.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://rvb.yvedp.cn

Ruby: def greet; @name; end
来源：http://wnm.redwolf501.top

C#:   public string Greet() => Name;
来源：http://ejq.yonumen.top

[G05] 继承
来源：http://xyg.meibo888.top

Py:   class Admin(User): pass
来源：http://kup.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://orl.birdmap.top

JS:   class Admin extends User {}
来源：http://otx.tian-w.cn

TS:   class Admin extends User {}
来源：http://itk.bbcook.cn

Java: class Admin extends User {}
来源：http://dui.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mdq.tarul.cn

Ruby: class Admin < User; end
来源：http://yya.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://kaz.feifeiyinyue.top

[G06] 重写方法
来源：http://mzr.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://wvl.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://xno.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://hev.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://rmg.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://idd.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mql.hammf.cn

Ruby: def greet; "admin"; end
来源：http://cbm.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://ojv.shzxlz.cn

[G07] 调用父类方法
来源：http://lwg.smart0.xyz

Py:   super().greet()
来源：http://uum.shangyingyoupin.top

PHP:  parent::greet();
来源：http://qnd.quarkkingdee.top

JS:   super.greet();
来源：http://brp.0kj1m.cn

TS:   super.greet();
来源：http://ihw.shzxlz.cn

Java: super.greet();
来源：http://opi.sweek.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lat.fanxiaobao.xyz

Ruby: super
来源：http://kuc.yuanzhike.top

C#:   base.Greet();
来源：http://hwi.aizwys.cn

[G08] 静态方法与属性
来源：http://ghn.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hqv.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://dei.c1oappe.top

JS:   static f() {}
来源：http://gkz.sysykeji.top

TS:   static f(): void {}
来源：http://pre.9152youxi.cn

Java: static void f() {}
来源：http://mjy.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zuy.pengpengdd.cyou

Ruby: def self.f; end
来源：http://sia.jinqigufen.top

C#:   public static void F() {}
来源：http://cpw.yfazqb.com

[G09] 接口 / 抽象类
来源：http://oea.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pxu.aibaodan.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dxd.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cab.jiagoushi.top

TS:   interface Shape { area(): number; }
来源：http://eyn.bjfxy.top

Java: interface Shape { double area(); }
来源：http://bkv.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://eag.vehdjk.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ply.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://vlp.gogol.net.cn

[G10] 访问控制
来源：http://vgv.jyoumei.cn

Py:   约定 _protected / __private（不强制）
来源：http://zoy.sufxvd.cn

PHP:  public / protected / private
来源：http://xbm.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://nan.shanyushiyangkeji.top

TS:   public / protected / private
来源：http://xfw.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://lqw.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uuv.birdmap.top

Ruby: public / protected / private
来源：http://izx.hongshengwenyu.top

C#:   public / protected / private / internal
来源：http://ckx.ywan-chungtsiang.top

[G11] getter / setter
来源：http://lxy.meibo888.top

Py:   @property 与 @x.setter
来源：http://hzp.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://soe.fengsongda.top

JS:   get name() { return this._name; }
来源：http://gfk.zhongyouzk.top

TS:   get name(): string { return this._name; }
来源：http://orw.redwolf501.top

Java: public String getName() { return name; }
来源：http://oqw.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mek.pycfn.com

Ruby: attr_accessor :name
来源：http://vmg.zycfv.cn

C#:   public string Name { get; set; }
来源：http://izl.uphjek.com

[G12] 对象转字符串
来源：http://zea.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://zvj.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cuo.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://pmw.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://qtu.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://abb.fehbvm.com

Go:   func (u User) String() string { return u.Name }
来源：http://flq.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://tfp.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://ntg.chenzaomai.com

[G13] 判断对象类型
来源：http://zfr.daxiang520.top

Py:   isinstance(u, User)
来源：http://iqt.havefunace.top

PHP:  $u instanceof User
来源：http://xxj.sysykeji.top

JS:   u instanceof User
来源：http://qaw.yonumen.top

TS:   u instanceof User
来源：http://nkl.jianghu66.top

Java: u instanceof User
来源：http://xod.chenjidiqi.icu

Go:   u, ok := v.(User)            // 类型断言
来源：http://fix.tanke756.top

Ruby: u.is_a?(User)
来源：http://ebe.yj20258.top

C#:   u is User
来源：http://zmz.ydzc1.top

[G14] 数据类 / record
来源：http://mvs.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vkr.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://xow.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cqz.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://aus.cucudq.cn

Java: record User(String name, int age) {}
来源：http://dne.ybcxt.top

Go:   type User struct { Name string; Age int }
来源：http://qzj.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bno.ctjpmb.com

C#:   record User(string Name, int Age);
来源：http://btj.hysaishi.cn

[G15] 枚举
来源：http://obq.zhoulong.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://khc.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vne.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vyt.jinqigfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fxo.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://kdm.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pvw.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://dna.vqdsnc.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zps.tianlin.xyz

[G16] 对象转数组 / 字典
来源：http://sed.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fqv.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://jiw.svipenyu.cn

JS:   Object.entries(obj)
来源：http://daj.guowangkeji.top

TS:   Object.entries(obj)
来源：http://uvq.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dms.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nfj.yueranfly.top

Ruby: obj.instance_variables
来源：http://lsd.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://fpc.yj202588.top

================================================================================
来源：http://vxd.fanxiaobao.xyz

H. 异常与错误处理
来源：http://bgk.xinyue.icu

================================================================================
来源：http://pnp.yj20258888.top

[H01] try / catch 基础
来源：http://eey.hysaishi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tmo.sysykeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jjd.c1oappe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ljb.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bgj.zdqjudy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gow.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xuu.fengsongda.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zvt.meibo888.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://czh.yonumen.top

[H02] finally / ensure 收尾
来源：http://evt.guowangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://qpt.jyoumei.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://har.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tgx.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bvs.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://wkp.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://afv.svipenyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hsy.xuetiantiany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lth.yvedp.cn

[H03] 主动抛出异常
来源：http://xit.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://mlx.xinyue.icu

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ptz.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://rsu.shzxlz.cn


<!-- 参考信息 -->