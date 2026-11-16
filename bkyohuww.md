代发 wailian999

Go:   if s == "" {}
来源：http://kyv.nwbrower.top

Ruby: if s.empty?
来源：http://uak.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yox.yuanzhike.top

[E21] 超长截断加省略号
来源：http://euc.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kbm.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://czh.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vty.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ncm.hnxiangtu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vvy.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://sde.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nif.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://omu.gaohongyu789.top

[E22] 字节长度与字符长度
来源：http://vgs.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bou.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vxj.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mlc.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyk.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mbg.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wrw.hesvh.cn

Ruby: s.bytesize;  s.length
来源：http://ves.ivvv.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nmr.zhongyouzk.top

================================================================================
来源：http://ggb.hnqzz.top

F. 文件与目录
来源：http://sfp.jinghuilouyu.cn

================================================================================
来源：http://ivn.xinyue.icu

[F01] 读取整个文件
来源：http://ylw.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rtt.vehdjk.com

PHP:  file_get_contents("a.txt");
来源：http://eql.meibo888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lfe.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qyt.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://ybq.pycfn.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zyh.hammf.cn

Ruby: File.read("a.txt")
来源：http://ehs.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://qgo.kuanghao11.cn

[F02] 逐行读取文件
来源：http://jhv.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qsj.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pxf.fehbvm.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tqm.wangdashe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mrj.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zqo.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ron.yonumen.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rrd.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pwk.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://fqy.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zlr.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://omw.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xwb.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://may.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://eso.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dwt.vehdjk.com

Ruby: File.write("a.txt", "hi")
来源：http://kzx.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wps.sweek.top

[F04] 追加写入文件
来源：http://tkp.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hht.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jdz.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://scb.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://llr.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vxw.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lou.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vtz.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tdb.shzxlz.cn

[F05] 判断文件或目录是否存在
来源：http://lew.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://goj.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://pby.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://rll.cdnleiting.top

TS:   fs.existsSync("a.txt")
来源：http://kpr.yonumen.top

Java: Files.exists(Path.of("a.txt"))
来源：http://edc.gogol.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aje.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://ihg.guowangkeji.top

C#:   File.Exists("a.txt")
来源：http://baf.vehdjk.com

[F06] 删除文件
来源：http://owk.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://duq.dianchejie.cn

PHP:  unlink("a.txt");
来源：http://rwl.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dmf.meibo888.top

TS:   fs.unlinkSync("a.txt")
来源：http://dcq.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kqy.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://zyd.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://yyq.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://ybe.hcnkem.com

[F07] 创建目录（含多级）
来源：http://agv.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sde.ehwqpu.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wgb.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bqs.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kvu.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kyg.jinyuanbaomall.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ptf.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dyh.zycfv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wiz.gotoacloud.top

[F08] 遍历目录
来源：http://tta.jyoumei.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcv.shanyushiyangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jxa.cqqwz.cn

JS:   fs.readdirSync("dir")
来源：http://hhq.zdbjq.cn

TS:   fs.readdirSync("dir")
来源：http://dmh.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sqo.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rgj.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://cid.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://bhy.yongpay.top

[F09] 获取文件大小
来源：http://ygw.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://krf.aizwys.cn

PHP:  filesize("a.txt");
来源：http://fmv.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://hnr.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://tro.cdnleiting.top

Java: Files.size(Path.of("a.txt"))
来源：http://phf.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fvx.yj202588.top

Ruby: File.size("a.txt")
来源：http://fab.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://yhh.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://akg.shuidangran.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ayp.vqdsnc.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qcd.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wsa.tian-w.cn

TS:   path.extname("a.txt")
来源：http://dhy.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hhl.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hcs.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://leg.snrcjt.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vzj.zhoulong.xyz

[F11] 复制与移动文件
来源：http://tos.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zqp.yanxiufei.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dpz.ivvv.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://azx.9152youxi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jxi.jyoumei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ght.ppjwa.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dvj.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jna.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hwt.zhongyouzk.top

[F12] CSV 读写
来源：http://blc.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pmu.yj202588.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://orb.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jas.andypj.xyz

TS:   // 同上
来源：http://tka.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xaf.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nov.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zkw.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://iqv.0kj1m.cn

================================================================================
来源：http://xtm.chenjidiqi.icu

G. 面向对象
来源：http://vmt.hesvh.cn

================================================================================
来源：http://ggb.zdqjudy.top

[G01] 定义类
来源：http://zrc.gaohongyu789.top

Py:   class User: pass
来源：http://clt.gotoacloud.top

PHP:  class User {}
来源：http://gld.cdnleiting.top

JS:   class User {}
来源：http://mbs.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://yyc.andypj.xyz

Java: class User {}
来源：http://xss.dashuyun.cn

Go:   type User struct { Name string }
来源：http://zci.chenlongwang.top

Ruby: class User; end
来源：http://zfs.fzhhl.top

C#:   class User {}
来源：http://crm.cdnleiting.top

[G02] 构造函数
来源：http://irk.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://sds.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://leb.smart0.xyz

JS:   constructor(name) { this.name = name; }
来源：http://rue.andypj.xyz

TS:   constructor(public name: string) {}
来源：http://cdb.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://piw.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xgs.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://hoj.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://vnl.ydjk.org.cn

[G03] 实例属性
来源：http://sbo.yangfankeji.com

Py:   self.name = "x"
来源：http://sne.cqqwz.cn

PHP:  public string $name = "x";
来源：http://apd.jiagoushi.top

JS:   this.name = "x";
来源：http://kiy.chenlongwang.top

TS:   name: string = "x";
来源：http://xkr.pycfn.com

Java: private String name;
来源：http://koa.yueranfly.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://otl.vqdsnc.cn

Ruby: @name = "x"
来源：http://jcs.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://taf.shzxlz.cn

[G04] 定义方法
来源：http://wkf.yj20258888.top

Py:   def greet(self): return self.name
来源：http://eul.gotoacloud.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cvn.c1oappe.top

JS:   greet() { return this.name; }
来源：http://uou.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://aej.zycfv.cn

Java: String greet() { return name; }
来源：http://fds.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vyk.hcnkem.com

Ruby: def greet; @name; end
来源：http://uct.hesvh.cn

C#:   public string Greet() => Name;
来源：http://zdt.smart0.xyz

[G05] 继承
来源：http://vdh.nwbrower.top

Py:   class Admin(User): pass
来源：http://orf.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://mtm.ppjwa.cn

JS:   class Admin extends User {}
来源：http://bcl.snrcjt.cn

TS:   class Admin extends User {}
来源：http://djb.yfazqb.com

Java: class Admin extends User {}
来源：http://ytj.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sty.zdqjudy.top

Ruby: class Admin < User; end
来源：http://xyr.zhongyouzk.top

C#:   class Admin : User {}
来源：http://mtc.c1oappe.top

[G06] 重写方法
来源：http://zeg.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://ypd.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rhv.0kj1m.cn

JS:   greet() { return "admin"; }
来源：http://qxk.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://ltz.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://iix.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qga.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://wqi.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://gyw.vehdjk.com

[G07] 调用父类方法
来源：http://uqq.xziqi.cn

Py:   super().greet()
来源：http://zqf.nanxuanxn.top

PHP:  parent::greet();
来源：http://xgt.quarkkingdee.top

JS:   super.greet();
来源：http://gjp.hysaishi.cn

TS:   super.greet();
来源：http://vwj.fktsv.cn

Java: super.greet();
来源：http://gof.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://klt.cheryme.top

Ruby: super
来源：http://khq.chenjidiqi.icu

C#:   base.Greet();
来源：http://teo.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://xtx.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://idg.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://koj.cdnleiting.top

JS:   static f() {}
来源：http://xws.ctjpmb.com

TS:   static f(): void {}
来源：http://fyz.yfazqb.com

Java: static void f() {}
来源：http://fst.jqgfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pbh.cashguo.top

Ruby: def self.f; end
来源：http://pao.nanxinkj.top

C#:   public static void F() {}
来源：http://dza.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://xnd.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://nyg.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oec.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://muh.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://eis.xuetiantiany.cn

Java: interface Shape { double area(); }
来源：http://ptg.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://qsu.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zhz.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://kro.uphjek.com

[G10] 访问控制
来源：http://lpl.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://clq.pengpengdd.cyou

PHP:  public / protected / private
来源：http://gov.andypj.xyz

JS:   #private 字段；其余公开
来源：http://huj.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://kgn.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://wtx.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zaz.zhongyouzk.top

Ruby: public / protected / private
来源：http://lzz.fanxiaobao.xyz

C#:   public / protected / private / internal
来源：http://qav.yuxming.cn

[G11] getter / setter
来源：http://lof.yvedp.cn

Py:   @property 与 @x.setter
来源：http://ltz.cheryme.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mny.cucudq.cn

JS:   get name() { return this._name; }
来源：http://qol.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://sia.ppjwa.cn

Java: public String getName() { return name; }
来源：http://mqa.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qwf.sxryk.cn

Ruby: attr_accessor :name
来源：http://fjo.uphjek.com

C#:   public string Name { get; set; }
来源：http://kty.hywenlv.cn

[G12] 对象转字符串
来源：http://qvd.cashguo.top

Py:   def __str__(self): return self.name
来源：http://kqc.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ldf.shanyushiyangtech.top

JS:   toString() { return this.name; }
来源：http://vex.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://lyc.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://quy.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cvv.316326.xyz

Ruby: def to_s; @name; end
来源：http://yjf.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://koy.daria6918.cn

[G13] 判断对象类型
来源：http://oph.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://xaa.nwbrower.top

PHP:  $u instanceof User
来源：http://gvl.fzhhl.top

JS:   u instanceof User
来源：http://fjq.zhaomingkeji.xyz

TS:   u instanceof User
来源：http://yrs.gaohongyu789.top

Java: u instanceof User
来源：http://bdv.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vgn.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://sqd.yfazqb.com

C#:   u is User
来源：http://txo.jqgfzy.top

[G14] 数据类 / record
来源：http://nol.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hpa.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://pnh.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fhp.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://ycc.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://rig.haohaochexian.top

Go:   type User struct { Name string; Age int }
来源：http://kso.jinqigufen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sos.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://tbi.jiagoushi.top

[G15] 枚举
来源：http://sqm.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://uqj.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gxn.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ace.zhengqikj.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ljn.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://dny.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zzs.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://rvq.havefunace.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ykc.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://sih.hfpthk.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rlv.kuanghao11.cn

PHP:  get_object_vars($obj);
来源：http://jky.andypj.xyz

JS:   Object.entries(obj)
来源：http://bur.ybcxt.top

TS:   Object.entries(obj)
来源：http://xwg.316326.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tgz.bbcook.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ery.bbcook.cn

Ruby: obj.instance_variables
来源：http://hzv.sysykeji.top

C#:   // 用反射或 System.Text.Json
来源：http://xno.fktsv.cn

================================================================================
来源：http://bri.hysaishi.cn

H. 异常与错误处理
来源：http://ouu.fzhhl.top

================================================================================
来源：http://cgf.yonumen.top

[H01] try / catch 基础
来源：http://ljs.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kap.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jfw.sysykeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bzh.yuanzhike.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://psh.yangfankeji.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zfe.svipenyu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ovc.gzhubu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rru.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://myr.hnxiangtu.top

[H02] finally / ensure 收尾
来源：http://xln.nanxinkj.top

Py:   try: f()⏎finally: cleanup()
来源：http://zfb.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gcu.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nro.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nyl.tianlin.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://kfb.yanxiufei.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gmh.yvedp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zln.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://djg.xuanzx.com


<!-- 参考信息 -->