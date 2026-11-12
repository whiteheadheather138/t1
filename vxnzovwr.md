代发 wailian999

Go:   if s == "" {}
来源：http://vdv.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://wna.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ttp.daxiang520.top

[E21] 超长截断加省略号
来源：http://wao.tianlin.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aon.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lso.yueranfly.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fps.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oov.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://agv.cdnleiting.top

Go:   // 按 rune 判断长度后截断
来源：http://ryi.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ond.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iui.bbcook.cn

[E22] 字节长度与字符长度
来源：http://srn.zdbjq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fsc.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tsk.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xxz.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ldp.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cts.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jeh.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://xqp.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ztl.yueranfly.top

================================================================================
来源：http://yws.zhoulong.xyz

F. 文件与目录
来源：http://rre.fktsv.cn

================================================================================
来源：http://pwa.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://jrf.sxryk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fir.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://qdi.andypj.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uly.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qms.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qie.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vwu.yongpay.top

Ruby: File.read("a.txt")
来源：http://mee.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://oar.aibaodan.cn

[F02] 逐行读取文件
来源：http://wrh.sufxvd.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wcf.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ocl.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://igw.shangyingyoupin.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcd.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://krw.zhijiandao.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ssx.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jhb.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://snt.yanxiufei.cn

[F03] 写入文件（覆盖）
来源：http://zve.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oru.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dll.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xix.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gtm.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wha.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hca.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://dqo.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gmj.jinqigufen.top

[F04] 追加写入文件
来源：http://eim.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lfj.svipenyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xzz.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hkx.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfq.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mlt.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qks.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ngg.sjlbkw.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jew.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://jok.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imc.snrcjt.cn

PHP:  file_exists("a.txt");
来源：http://fob.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://ntg.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://pyl.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qqm.sufxvd.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jan.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://qnm.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://fsk.sufxvd.cn

[F06] 删除文件
来源：http://bhq.52xcode.cn

Py:   os.remove("a.txt")
来源：http://uvy.yfazqb.com

PHP:  unlink("a.txt");
来源：http://nsx.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://psv.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://dzy.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qzh.uphjek.com

Go:   os.Remove("a.txt")
来源：http://qlm.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://nbc.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://nnj.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://nyx.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fiu.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hhm.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ita.smart0.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fat.epnwcf.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://grv.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://erm.sweek.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dfe.quarkkingdee.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://epf.hywenlv.cn

[F08] 遍历目录
来源：http://xwv.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iut.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aoj.sweek.top

JS:   fs.readdirSync("dir")
来源：http://fsf.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://yoa.xuetiantiany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mgl.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://qbq.pycfn.com

Ruby: Dir.children("dir")
来源：http://pwt.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://har.meibo888.top

[F09] 获取文件大小
来源：http://wpe.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://krm.sjlbkw.cn

PHP:  filesize("a.txt");
来源：http://pwz.cdnleiting.top

JS:   fs.statSync("a.txt").size
来源：http://who.hywenlv.cn

TS:   fs.statSync("a.txt").size
来源：http://jmj.zhongyouzk.top

Java: Files.size(Path.of("a.txt"))
来源：http://srd.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sms.sysykeji.top

Ruby: File.size("a.txt")
来源：http://boj.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://ojj.birdmap.top

[F10] 取文件扩展名 / 文件名
来源：http://ukp.andypj.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ylt.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://stv.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pei.yongpay.top

TS:   path.extname("a.txt")
来源：http://boo.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://you.yanxiufei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qaa.jianghu66.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eji.dashuyun.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ikc.jiagoushi.top

[F11] 复制与移动文件
来源：http://wmd.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gno.sweek.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dgh.uphjek.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://saw.xinyue.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rtz.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qwk.zdbjq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tmo.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://onh.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wle.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://gxb.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mfg.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cmq.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qmc.hfpthk.cn

TS:   // 同上
来源：http://qii.sweek.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ebn.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kmo.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://egt.yj202588.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zkw.sysykeji.top

================================================================================
来源：http://bii.wangshuangyany.cn

G. 面向对象
来源：http://iuu.xingfuxueyuan.xyz

================================================================================
来源：http://ryh.yj20258.top

[G01] 定义类
来源：http://wdc.yanxiufei.cn

Py:   class User: pass
来源：http://lyf.nanxuanxn.top

PHP:  class User {}
来源：http://htj.pengpengdd.cyou

JS:   class User {}
来源：http://quz.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://wya.quarkkingdee.top

Java: class User {}
来源：http://bhb.ydzc1.top

Go:   type User struct { Name string }
来源：http://rfi.xingfuxueyuan.xyz

Ruby: class User; end
来源：http://urx.yj20258888.top

C#:   class User {}
来源：http://ayh.pengpengdd.cyou

[G02] 构造函数
来源：http://qbu.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://xcm.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://aze.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://dzi.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://ori.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://fgp.tian-w.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qoa.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://sgr.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://eib.fzhhl.top

[G03] 实例属性
来源：http://eba.cashguo.top

Py:   self.name = "x"
来源：http://oad.yvedp.cn

PHP:  public string $name = "x";
来源：http://naz.haohaochexian.top

JS:   this.name = "x";
来源：http://otn.gogol.net.cn

TS:   name: string = "x";
来源：http://kgs.sjlbkw.cn

Java: private String name;
来源：http://nsl.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gcm.daxiang520.top

Ruby: @name = "x"
来源：http://eit.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://nxf.jianghu66.top

[G04] 定义方法
来源：http://iob.uphjek.com

Py:   def greet(self): return self.name
来源：http://hqt.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://idn.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://hbk.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://rmo.hnxiangtu.top

Java: String greet() { return name; }
来源：http://fba.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ntp.dashuyun.cn

Ruby: def greet; @name; end
来源：http://bgv.xziqi.cn

C#:   public string Greet() => Name;
来源：http://vvc.pycfn.com

[G05] 继承
来源：http://eef.gogol.net.cn

Py:   class Admin(User): pass
来源：http://wzs.shanyushiyangtech.top

PHP:  class Admin extends User {}
来源：http://sas.vehdjk.com

JS:   class Admin extends User {}
来源：http://xxv.dianchejie.cn

TS:   class Admin extends User {}
来源：http://ipo.nwbrower.top

Java: class Admin extends User {}
来源：http://jsk.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://icu.yongpay.top

Ruby: class Admin < User; end
来源：http://mnm.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://gco.cucudq.cn

[G06] 重写方法
来源：http://xpi.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://ohe.nwbrower.top

PHP:  public function greet(): string { return "admin"; }
来源：http://piw.nanxinkj.top

JS:   greet() { return "admin"; }
来源：http://mku.zdqjudy.top

TS:   greet(): string { return "admin"; }
来源：http://fid.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://rxp.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lvc.yongpay.top

Ruby: def greet; "admin"; end
来源：http://sau.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://mhb.gogol.net.cn

[G07] 调用父类方法
来源：http://wmt.nwbrower.top

Py:   super().greet()
来源：http://fuv.zycfv.cn

PHP:  parent::greet();
来源：http://bhw.epnwcf.com

JS:   super.greet();
来源：http://inu.zhixingplan.top

TS:   super.greet();
来源：http://ewb.shanyushiyangtech.top

Java: super.greet();
来源：http://fxh.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ggi.sufxvd.cn

Ruby: super
来源：http://zud.fktsv.cn

C#:   base.Greet();
来源：http://rnh.daria6918.cn

[G08] 静态方法与属性
来源：http://sur.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cjs.bbcook.cn

PHP:  public static function f() {}
来源：http://gty.yj20258888.top

JS:   static f() {}
来源：http://zww.pycfn.com

TS:   static f(): void {}
来源：http://efo.hammf.cn

Java: static void f() {}
来源：http://mgg.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ugr.c1oappe.top

Ruby: def self.f; end
来源：http://jdl.chenzaomai.com

C#:   public static void F() {}
来源：http://nmn.fzhhl.top

[G09] 接口 / 抽象类
来源：http://djl.daxiang520.top

Py:   from abc import ABC, abstractmethod
来源：http://vwq.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://nzh.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fqh.quarkkingdee.top

TS:   interface Shape { area(): number; }
来源：http://gmc.cheryme.top

Java: interface Shape { double area(); }
来源：http://yzi.ehwqpu.com

Go:   type Shape interface { Area() float64 }
来源：http://dxz.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jsy.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://kyj.sufxvd.cn

[G10] 访问控制
来源：http://ugs.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://nuh.ehwqpu.com

PHP:  public / protected / private
来源：http://wgk.gogol.net.cn

JS:   #private 字段；其余公开
来源：http://izx.zycfv.cn

TS:   public / protected / private
来源：http://bxq.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://wsw.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fey.tanke756.top

Ruby: public / protected / private
来源：http://awk.xinyue.icu

C#:   public / protected / private / internal
来源：http://xjh.epnwcf.com

[G11] getter / setter
来源：http://xyi.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://ayy.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://tbe.redwolf501.top

JS:   get name() { return this._name; }
来源：http://nin.hcnkem.com

TS:   get name(): string { return this._name; }
来源：http://zgg.yueranfly.top

Java: public String getName() { return name; }
来源：http://tvi.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://frw.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://ari.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://fnl.dashuyun.cn

[G12] 对象转字符串
来源：http://zno.uphjek.com

Py:   def __str__(self): return self.name
来源：http://shy.gogol.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xeu.sysykeji.top

JS:   toString() { return this.name; }
来源：http://hjy.ctjpmb.com

TS:   toString(): string { return this.name; }
来源：http://mbf.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://xku.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://sco.tanke756.top

Ruby: def to_s; @name; end
来源：http://hvq.haohaochexian.top

C#:   public override string ToString() => Name;
来源：http://cgl.nanxinkj.top

[G13] 判断对象类型
来源：http://ayh.guannengcc.top

Py:   isinstance(u, User)
来源：http://mfe.bbcook.cn

PHP:  $u instanceof User
来源：http://zjs.tanke756.top

JS:   u instanceof User
来源：http://pai.fehbvm.com

TS:   u instanceof User
来源：http://wve.nanxuanxn.top

Java: u instanceof User
来源：http://dus.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kye.tian-w.cn

Ruby: u.is_a?(User)
来源：http://bnm.chenlongwang.top

C#:   u is User
来源：http://vzr.fzhhl.top

[G14] 数据类 / record
来源：http://rmv.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bin.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://soj.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://yyy.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://zfs.zhiwuduotai.top

Java: record User(String name, int age) {}
来源：http://cth.daxiang520.top

Go:   type User struct { Name string; Age int }
来源：http://oio.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ygh.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://hrh.snrcjt.cn

[G15] 枚举
来源：http://uql.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xvo.xinyue.icu

PHP:  enum Color: string { case Red = "red"; }
来源：http://nno.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hps.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rjs.jinqigfzy.top

Java: enum Color { RED, GREEN }
来源：http://fpp.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qih.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://avk.bjfxy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ecm.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://ihe.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uzg.vqdsnc.cn

PHP:  get_object_vars($obj);
来源：http://fpk.bbcook.cn

JS:   Object.entries(obj)
来源：http://wyo.yvedp.cn

TS:   Object.entries(obj)
来源：http://zya.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pco.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cbz.zycfv.cn

Ruby: obj.instance_variables
来源：http://yks.cucudq.cn

C#:   // 用反射或 System.Text.Json
来源：http://odt.tian-w.cn

================================================================================
来源：http://ypr.hammf.cn

H. 异常与错误处理
来源：http://soi.shzxlz.cn

================================================================================
来源：http://bzx.xuanzx.com

[H01] try / catch 基础
来源：http://qnz.guannengcc.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://flm.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vkd.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eej.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xjk.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nax.xziqi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dqy.yj202588.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gwx.xziqi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mnu.sxryk.cn

[H02] finally / ensure 收尾
来源：http://ihl.zhiwuduotai.top

Py:   try: f()⏎finally: cleanup()
来源：http://bsh.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yvc.gzhubu.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rng.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://occ.chenzaomai.com

Java: try { f(); } finally { cleanup(); }
来源：http://rre.hammf.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vat.jqgufenzy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://knf.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qgo.vqdsnc.cn


<!-- 参考信息 -->