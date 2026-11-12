代发 wailian999

Ruby: s.lines
来源：http://ais.quarkkingdee.top

C#:   s.Split('\n')
来源：http://lcd.tian-w.cn

[E20] 判断字符串是否为空
来源：http://adt.uphjek.com

Py:   if not s:
来源：http://cny.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tnf.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://syi.aizwys.cn

TS:   if (s === "") {}
来源：http://bat.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://dhh.ydzc1.top

Go:   if s == "" {}
来源：http://mux.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://wqo.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://msa.uphjek.com

[E21] 超长截断加省略号
来源：http://tsv.ybcxt.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mor.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ozj.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oje.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aig.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://icw.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://axz.yvedp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ila.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://akj.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://bpz.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zso.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ewi.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gpq.redwolf501.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tlx.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ukx.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kbe.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://jpp.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yms.316326.xyz

================================================================================
来源：http://rfr.ppjwa.cn

F. 文件与目录
来源：http://thl.aizwys.cn

================================================================================
来源：http://rdn.uphjek.com

[F01] 读取整个文件
来源：http://gwi.meibo888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pry.snrcjt.cn

PHP:  file_get_contents("a.txt");
来源：http://kgg.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eav.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hpq.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://odq.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://aor.vehdjk.com

Ruby: File.read("a.txt")
来源：http://wcn.jinqigfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://jkn.zdbjq.cn

[F02] 逐行读取文件
来源：http://rcw.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jor.nwbrower.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://meb.jinyuanbaomall.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hus.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ffy.zhiwuduotai.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wfw.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gdl.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dhd.jqgufenzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eai.nanxinkj.top

[F03] 写入文件（覆盖）
来源：http://jga.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjn.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rul.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://khf.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pxs.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://whn.yfazqb.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tko.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://nnp.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aru.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://sgr.zhijiandao.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tuq.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fgy.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gjv.smart0.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jht.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mxj.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yvp.xingfuxueyuan.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jhh.dianchejie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zny.guowangkeji.top

[F05] 判断文件或目录是否存在
来源：http://kqx.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kow.nwbrower.top

PHP:  file_exists("a.txt");
来源：http://ast.sufxvd.cn

JS:   fs.existsSync("a.txt")
来源：http://lpw.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://put.nanxinkj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://psz.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dmy.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://sjx.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://zqt.bjfxy.top

[F06] 删除文件
来源：http://rau.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://drt.iojbl.cn

PHP:  unlink("a.txt");
来源：http://fcr.shangyingyoupin.top

JS:   fs.unlinkSync("a.txt")
来源：http://gwe.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xwa.jqgfzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://akl.zhengqikj.top

Go:   os.Remove("a.txt")
来源：http://ddl.zhongyouzk.top

Ruby: File.delete("a.txt")
来源：http://juv.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://gqy.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://lml.ydjk.org.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://riq.ctjpmb.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pvb.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rzk.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jqv.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vbt.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ybt.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gid.fktsv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://agd.bbcook.cn

[F08] 遍历目录
来源：http://ckl.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dtt.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://loo.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://qbn.zdqjudy.top

TS:   fs.readdirSync("dir")
来源：http://xgk.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zbt.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ujv.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://gsq.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://wmn.zhengqikj.top

[F09] 获取文件大小
来源：http://mcd.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://acg.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://ggt.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://vwr.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://sxi.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://mgd.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://etv.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://dae.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://ywn.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://egu.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://omk.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jcy.c1oappe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cdc.daria6918.cn

TS:   path.extname("a.txt")
来源：http://gpp.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yzb.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tvk.jiagoushi.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wrw.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cwy.chenzaomai.com

[F11] 复制与移动文件
来源：http://lxn.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iso.zhixingplan.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://edu.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qgm.ivvv.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzh.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pqc.hammf.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ipe.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://egu.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jlo.guowangkeji.top

[F12] CSV 读写
来源：http://jgu.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mxy.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://suj.jianghu66.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cmy.zhijiandao.cn

TS:   // 同上
来源：http://quh.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vhw.ydzc1.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zfo.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://llg.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mgq.zycfv.cn

================================================================================
来源：http://qyk.smart0.xyz

G. 面向对象
来源：http://iiu.cheryme.top

================================================================================
来源：http://nvd.pengpengdd.cyou

[G01] 定义类
来源：http://xby.sysykeji.top

Py:   class User: pass
来源：http://vde.bbcook.cn

PHP:  class User {}
来源：http://mum.cdnleiting.top

JS:   class User {}
来源：http://kaz.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://mwk.aizwys.cn

Java: class User {}
来源：http://pti.316326.xyz

Go:   type User struct { Name string }
来源：http://hom.xuetiantiany.cn

Ruby: class User; end
来源：http://kuv.pycfn.com

C#:   class User {}
来源：http://igt.hfpthk.cn

[G02] 构造函数
来源：http://lom.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://ews.xylfe.cn

PHP:  public function __construct(public string $name) {}
来源：http://jjp.9152youxi.cn

JS:   constructor(name) { this.name = name; }
来源：http://cer.52xcode.cn

TS:   constructor(public name: string) {}
来源：http://qjx.feifeiyinyue.top

Java: User(String name) { this.name = name; }
来源：http://fyp.aizwys.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://slp.ppjwa.cn

Ruby: def initialize(name); @name = name; end
来源：http://aeq.ydjk.org.cn

C#:   public User(string name) { Name = name; }
来源：http://dfq.fzhhl.top

[G03] 实例属性
来源：http://huh.yfazqb.com

Py:   self.name = "x"
来源：http://orz.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://vdv.nwbrower.top

JS:   this.name = "x";
来源：http://wof.vqdsnc.cn

TS:   name: string = "x";
来源：http://ekr.dashuyun.cn

Java: private String name;
来源：http://rel.mhx1999.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jay.jqgfzy.top

Ruby: @name = "x"
来源：http://vob.yongpay.top

C#:   public string Name { get; set; } = "x";
来源：http://fye.tanke756.top

[G04] 定义方法
来源：http://qfz.fengsongda.top

Py:   def greet(self): return self.name
来源：http://qoi.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jbo.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://xxd.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://skw.ivvv.top

Java: String greet() { return name; }
来源：http://cmn.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gev.yvedp.cn

Ruby: def greet; @name; end
来源：http://vsm.aizwys.cn

C#:   public string Greet() => Name;
来源：http://kng.mhx1999.top

[G05] 继承
来源：http://kva.0kj1m.cn

Py:   class Admin(User): pass
来源：http://shv.fzhhl.top

PHP:  class Admin extends User {}
来源：http://rqe.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://rtf.316326.xyz

TS:   class Admin extends User {}
来源：http://ckn.meibo888.top

Java: class Admin extends User {}
来源：http://qrv.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gij.gotoacloud.top

Ruby: class Admin < User; end
来源：http://nnx.cheryme.top

C#:   class Admin : User {}
来源：http://stb.jianghu66.top

[G06] 重写方法
来源：http://cil.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://fcd.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kjj.xuetiantiany.cn

JS:   greet() { return "admin"; }
来源：http://jtr.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://ndi.shanyushiyangkeji.top

Java: @Override String greet() { return "admin"; }
来源：http://oxm.zdqjudy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dug.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://kxd.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://xwx.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://jfh.zhaomingkeji.xyz

Py:   super().greet()
来源：http://etv.gaohongyu789.top

PHP:  parent::greet();
来源：http://xpk.birdmap.top

JS:   super.greet();
来源：http://odh.jlsjyb.cn

TS:   super.greet();
来源：http://agg.shzxlz.cn

Java: super.greet();
来源：http://tue.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rln.yj20258888.top

Ruby: super
来源：http://uhb.hongshengwenyu.top

C#:   base.Greet();
来源：http://xgz.jianghu66.top

[G08] 静态方法与属性
来源：http://bmn.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qnj.ydjk.org.cn

PHP:  public static function f() {}
来源：http://and.daxiang520.top

JS:   static f() {}
来源：http://fbc.feifeiyinyue.top

TS:   static f(): void {}
来源：http://fak.ydjk.org.cn

Java: static void f() {}
来源：http://ifp.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ldh.sysykeji.top

Ruby: def self.f; end
来源：http://nps.hysaishi.cn

C#:   public static void F() {}
来源：http://qfv.9152youxi.cn

[G09] 接口 / 抽象类
来源：http://ata.ivvv.top

Py:   from abc import ABC, abstractmethod
来源：http://qhr.redwolf501.top

PHP:  interface Shape { public function area(): float; }
来源：http://qpp.cucudq.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vlk.jianghu66.top

TS:   interface Shape { area(): number; }
来源：http://pqh.tanke756.top

Java: interface Shape { double area(); }
来源：http://rzi.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://nnn.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pyb.nwbrower.top

C#:   interface IShape { double Area(); }
来源：http://erp.gzhubu.top

[G10] 访问控制
来源：http://tqu.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://rme.fktsv.cn

PHP:  public / protected / private
来源：http://yol.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://fec.guowangkeji.top

TS:   public / protected / private
来源：http://nyy.ivvv.top

Java: public / protected / private / 默认包级
来源：http://vtw.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oda.yueranfly.top

Ruby: public / protected / private
来源：http://otu.zdqjudy.top

C#:   public / protected / private / internal
来源：http://cyx.uphjek.com

[G11] getter / setter
来源：http://emu.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://ojm.gotoacloud.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wrh.vehdjk.com

JS:   get name() { return this._name; }
来源：http://jbz.zhijiandao.cn

TS:   get name(): string { return this._name; }
来源：http://cdu.xuanzx.com

Java: public String getName() { return name; }
来源：http://xxw.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://smm.zhiwuduotai.top

Ruby: attr_accessor :name
来源：http://ipi.sweek.top

C#:   public string Name { get; set; }
来源：http://qtv.guowangkeji.top

[G12] 对象转字符串
来源：http://uhb.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://tbk.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kib.xziqi.cn

JS:   toString() { return this.name; }
来源：http://dlp.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://fjf.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://akl.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://hna.xylfe.cn

Ruby: def to_s; @name; end
来源：http://ioi.zhongyouzk.top

C#:   public override string ToString() => Name;
来源：http://aqe.fengsongda.top

[G13] 判断对象类型
来源：http://fjj.zhaomingkeji.xyz

Py:   isinstance(u, User)
来源：http://uen.andypj.xyz

PHP:  $u instanceof User
来源：http://xvo.redwolf501.top

JS:   u instanceof User
来源：http://hpq.bjfxy.top

TS:   u instanceof User
来源：http://cly.tianlin.xyz

Java: u instanceof User
来源：http://lea.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://flb.yongpay.top

Ruby: u.is_a?(User)
来源：http://jos.zhengqikj.top

C#:   u is User
来源：http://tpr.iojbl.cn

[G14] 数据类 / record
来源：http://gwc.tian-w.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cqb.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://eyv.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://ptk.ydjk.org.cn

TS:   type User = { name: string; age: number };
来源：http://nct.jqgfzy.top

Java: record User(String name, int age) {}
来源：http://mvl.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://ddl.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eog.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://wwq.shuidangran.top

[G15] 枚举
来源：http://uwk.birdmap.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://izv.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://tyx.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oqg.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jpj.yj20258888.top

Java: enum Color { RED, GREEN }
来源：http://qys.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://klu.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://xbn.shanyushiyangtech.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iha.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://mzg.fktsv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://akk.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://tco.zycfv.cn

JS:   Object.entries(obj)
来源：http://ntl.sweek.top

TS:   Object.entries(obj)
来源：http://enj.sjlbkw.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://adp.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://qzb.zdbjq.cn

Ruby: obj.instance_variables
来源：http://apk.kuanghao11.cn

C#:   // 用反射或 System.Text.Json
来源：http://pul.iojbl.cn

================================================================================
来源：http://udf.0kj1m.cn

H. 异常与错误处理
来源：http://loz.redwolf501.top

================================================================================
来源：http://ekq.jqgufenzy.top

[H01] try / catch 基础
来源：http://aua.fengsongda.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bgt.hammf.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://igj.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hrc.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zkz.yonumen.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jjo.nanxuanxn.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iwf.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wff.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://alm.wangshuangyany.cn

[H02] finally / ensure 收尾
来源：http://lzq.jinyuanbaomall.cn


<!-- 参考信息 -->