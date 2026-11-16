代发 wailian999

Go:   if s == "" {}
来源：http://eoj.yongpay.top

Ruby: if s.empty?
来源：http://izy.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iva.yvedp.cn

[E21] 超长截断加省略号
来源：http://xdi.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pvv.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qqj.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mtp.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bsd.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rtq.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://rug.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qhk.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ewr.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://vti.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvd.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fsq.sufxvd.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://naf.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nso.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fhc.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wzw.sxryk.cn

Ruby: s.bytesize;  s.length
来源：http://xsy.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hfw.ydjk.org.cn

================================================================================
来源：http://wbz.shanyushiyangtech.top

F. 文件与目录
来源：http://ndk.chenzaomai.com

================================================================================
来源：http://wvm.yuxming.cn

[F01] 读取整个文件
来源：http://jct.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xle.mhx1999.top

PHP:  file_get_contents("a.txt");
来源：http://hql.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uyu.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zws.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wri.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pbg.c1oappe.top

Ruby: File.read("a.txt")
来源：http://elx.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://rzp.yuxming.cn

[F02] 逐行读取文件
来源：http://slj.pengpengdd.cyou

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vrl.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vte.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wbr.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://npk.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dpt.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://npi.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://knf.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zcc.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://rgh.zycfv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kpv.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://khq.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mrd.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yrk.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ybw.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://osq.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://jir.cashguo.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://utz.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://dsg.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qyz.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lvl.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fdr.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cvc.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kss.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kss.sweek.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wbp.jyoumei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kvp.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://gpz.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hlc.hfpthk.cn

PHP:  file_exists("a.txt");
来源：http://cso.pengpengdd.cyou

JS:   fs.existsSync("a.txt")
来源：http://dfg.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://suo.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xzs.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hdg.fzhhl.top

Ruby: File.exist?("a.txt")
来源：http://pnh.yanxiufei.cn

C#:   File.Exists("a.txt")
来源：http://erx.shanyushiyangkeji.top

[F06] 删除文件
来源：http://kec.sxryk.cn

Py:   os.remove("a.txt")
来源：http://waz.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://ofv.hesvh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ash.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://lzh.pengpengdd.cyou

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sbp.uphjek.com

Go:   os.Remove("a.txt")
来源：http://kch.vehdjk.com

Ruby: File.delete("a.txt")
来源：http://hbm.ydzc1.top

C#:   File.Delete("a.txt");
来源：http://ogt.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://gaa.zycfv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://smb.yfazqb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ixf.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuz.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kvn.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jgd.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://txu.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xua.ybcxt.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xtq.hywenlv.cn

[F08] 遍历目录
来源：http://wwn.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://egi.tanke756.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dln.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://gol.feifeiyinyue.top

TS:   fs.readdirSync("dir")
来源：http://mzi.hammf.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vjn.iojbl.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tdx.haohaochexian.top

Ruby: Dir.children("dir")
来源：http://vji.svipenyu.cn

C#:   Directory.GetFiles("dir")
来源：http://prj.wangshuangyany.cn

[F09] 获取文件大小
来源：http://uqg.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://ndc.tian-w.cn

PHP:  filesize("a.txt");
来源：http://kjv.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://irr.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://tqc.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zcr.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cgz.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://men.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://zpf.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://dnh.chenjidiqi.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pzg.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://act.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jkn.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://oxy.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xfw.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wux.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yav.jinghuilouyu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zbc.ydzc1.top

[F11] 复制与移动文件
来源：http://sct.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gtm.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pil.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qmd.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jca.epnwcf.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vnc.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bkc.jianghu66.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://djo.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ccr.bbcook.cn

[F12] CSV 读写
来源：http://dug.yongpay.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ecg.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jxp.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rop.ivvv.top

TS:   // 同上
来源：http://uxg.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://imu.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xms.jinyuanbaomall.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gnp.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nxa.jlsjyb.cn

================================================================================
来源：http://lnd.sweek.top

G. 面向对象
来源：http://rku.zhixingplan.top

================================================================================
来源：http://hoc.mhx1999.top

[G01] 定义类
来源：http://oyg.xinyue.icu

Py:   class User: pass
来源：http://zjp.cashguo.top

PHP:  class User {}
来源：http://mvc.tarul.cn

JS:   class User {}
来源：http://lsi.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://dyh.cqqwz.cn

Java: class User {}
来源：http://ewu.fengsongda.top

Go:   type User struct { Name string }
来源：http://rfk.zhijiandao.cn

Ruby: class User; end
来源：http://jyf.hongshengwenyu.top

C#:   class User {}
来源：http://nxw.hcnkem.com

[G02] 构造函数
来源：http://btb.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://lyg.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://xwo.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://ogp.xziqi.cn

TS:   constructor(public name: string) {}
来源：http://evw.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://psc.svipenyu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://msu.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://ouf.gaohongyu789.top

C#:   public User(string name) { Name = name; }
来源：http://vpu.fengsongda.top

[G03] 实例属性
来源：http://uyt.zhoulong.xyz

Py:   self.name = "x"
来源：http://vuy.birdmap.top

PHP:  public string $name = "x";
来源：http://xxm.yonumen.top

JS:   this.name = "x";
来源：http://bok.gzhubu.top

TS:   name: string = "x";
来源：http://pph.vehdjk.com

Java: private String name;
来源：http://xbd.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ndi.tianlin.xyz

Ruby: @name = "x"
来源：http://aia.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://dfk.shuidangran.top

[G04] 定义方法
来源：http://ssd.hongshengwenyu.top

Py:   def greet(self): return self.name
来源：http://zce.zhaomingkeji.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://dql.hammf.cn

JS:   greet() { return this.name; }
来源：http://esn.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://tzu.yuxming.cn

Java: String greet() { return name; }
来源：http://pap.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://coz.hfpthk.cn

Ruby: def greet; @name; end
来源：http://ntz.chenzaomai.com

C#:   public string Greet() => Name;
来源：http://jzj.epnwcf.com

[G05] 继承
来源：http://sfb.zycfv.cn

Py:   class Admin(User): pass
来源：http://daw.hcnkem.com

PHP:  class Admin extends User {}
来源：http://xbi.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://orr.tian-w.cn

TS:   class Admin extends User {}
来源：http://teb.jinqigfzy.top

Java: class Admin extends User {}
来源：http://aqd.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oix.shzxlz.cn

Ruby: class Admin < User; end
来源：http://xxj.bjfxy.top

C#:   class Admin : User {}
来源：http://idi.smart0.xyz

[G06] 重写方法
来源：http://kzt.yonumen.top

Py:   def greet(self): return "admin"
来源：http://qoj.jqgfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jwf.yj20258888.top

JS:   greet() { return "admin"; }
来源：http://rih.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://xwj.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://owv.tian-w.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mzp.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://tvx.wangdashe.top

C#:   public override string Greet() => "admin";
来源：http://kwj.daria6918.cn

[G07] 调用父类方法
来源：http://dow.ybcxt.top

Py:   super().greet()
来源：http://wgl.aibaodan.cn

PHP:  parent::greet();
来源：http://ozf.yuxming.cn

JS:   super.greet();
来源：http://blz.fanxiaobao.xyz

TS:   super.greet();
来源：http://ani.dashuyun.cn

Java: super.greet();
来源：http://xko.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ans.zhixingplan.top

Ruby: super
来源：http://fug.ydjk.org.cn

C#:   base.Greet();
来源：http://dnv.fehbvm.com

[G08] 静态方法与属性
来源：http://ajl.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bun.nanxinkj.top

PHP:  public static function f() {}
来源：http://gba.hammf.cn

JS:   static f() {}
来源：http://brt.cucudq.cn

TS:   static f(): void {}
来源：http://pnw.hnxiangtu.top

Java: static void f() {}
来源：http://gav.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lwy.zdqjudy.top

Ruby: def self.f; end
来源：http://xzd.zdqjudy.top

C#:   public static void F() {}
来源：http://ybs.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://dzd.sxryk.cn

Py:   from abc import ABC, abstractmethod
来源：http://vlb.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://dll.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tuf.hammf.cn

TS:   interface Shape { area(): number; }
来源：http://pcq.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://fxg.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://ncp.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ynh.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://gil.yuxming.cn

[G10] 访问控制
来源：http://uyn.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://oex.hywenlv.cn

PHP:  public / protected / private
来源：http://hub.sweek.top

JS:   #private 字段；其余公开
来源：http://wqq.feifeiyinyue.top

TS:   public / protected / private
来源：http://kcm.sxryk.cn

Java: public / protected / private / 默认包级
来源：http://itp.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vss.jianghu66.top

Ruby: public / protected / private
来源：http://swl.hywenlv.cn

C#:   public / protected / private / internal
来源：http://rcj.chenlongwang.top

[G11] getter / setter
来源：http://otx.wangdashe.top

Py:   @property 与 @x.setter
来源：http://vnc.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gjn.mhx1999.top

JS:   get name() { return this._name; }
来源：http://zor.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://atd.hcnkem.com

Java: public String getName() { return name; }
来源：http://uqm.jinghuilouyu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ncy.hnqzz.top

Ruby: attr_accessor :name
来源：http://prb.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://jya.jqgufenzy.top

[G12] 对象转字符串
来源：http://vck.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://ijc.quarkkingdee.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://pmu.gaohongyu789.top

JS:   toString() { return this.name; }
来源：http://pju.mhx1999.top

TS:   toString(): string { return this.name; }
来源：http://fev.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://lxm.aizwys.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mqg.ivvv.top

Ruby: def to_s; @name; end
来源：http://gwr.9152youxi.cn

C#:   public override string ToString() => Name;
来源：http://ktk.sxryk.cn

[G13] 判断对象类型
来源：http://qmy.jqgfzy.top

Py:   isinstance(u, User)
来源：http://hab.wangdashe.top

PHP:  $u instanceof User
来源：http://tsz.zhongyouzk.top

JS:   u instanceof User
来源：http://ysz.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://sdh.ywan-chungtsiang.top

Java: u instanceof User
来源：http://tsd.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://fix.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://ely.xylfe.cn

C#:   u is User
来源：http://tch.jyoumei.cn

[G14] 数据类 / record
来源：http://zdw.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qtl.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://frs.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://tfs.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://kuj.yvedp.cn

Java: record User(String name, int age) {}
来源：http://rjk.zdqjudy.top

Go:   type User struct { Name string; Age int }
来源：http://phe.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uik.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://srp.c1oappe.top

[G15] 枚举
来源：http://bbh.hywenlv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qrj.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://aog.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iuj.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://chd.gaohongyu789.top

Java: enum Color { RED, GREEN }
来源：http://waq.tian-w.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bbs.yj202588.top

Ruby: Color = %i[red green].freeze
来源：http://exa.daxiang520.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bhq.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://hmv.tian-w.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://thd.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://nir.cucudq.cn

JS:   Object.entries(obj)
来源：http://rgw.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://czy.jqgufenzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nep.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qfu.0kj1m.cn

Ruby: obj.instance_variables
来源：http://flz.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://wze.yonumen.top

================================================================================
来源：http://upi.ywan-chungtsiang.top

H. 异常与错误处理
来源：http://cud.wangdashe.top

================================================================================
来源：http://yto.feifeiyinyue.top

[H01] try / catch 基础
来源：http://mml.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dfo.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hbd.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ltv.zhoulong.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hxs.zhiwuduotai.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nok.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yaq.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hrw.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ijv.52xcode.cn

[H02] finally / ensure 收尾
来源：http://joo.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sbp.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oja.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://aod.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bpw.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mbb.jlsjyb.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wjc.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lym.0kj1m.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dvj.hywenlv.cn


<!-- 参考信息 -->