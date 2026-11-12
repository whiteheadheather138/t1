代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbg.yanxiufei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ptt.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://evt.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://bwa.yonumen.top

Go:   if s == "" {}
来源：http://dvk.zhoulong.xyz

Ruby: if s.empty?
来源：http://yhg.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ymv.yangfankeji.com

[E21] 超长截断加省略号
来源：http://uww.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://axk.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gpm.fehbvm.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cds.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xqh.zhixingplan.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ebs.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://oxp.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://awf.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gcz.chenjidiqi.icu

[E22] 字节长度与字符长度
来源：http://acu.yongpay.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://avl.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zhe.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qgd.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zdf.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fqj.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oaf.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://lpg.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jld.xuanzx.com

================================================================================
来源：http://zug.yongpay.top

F. 文件与目录
来源：http://vpa.mhx1999.top

================================================================================
来源：http://kgu.yj20258.top

[F01] 读取整个文件
来源：http://tlh.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uaj.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://guy.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tlx.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fdj.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://giy.wangshuangyany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sej.guowangkeji.top

Ruby: File.read("a.txt")
来源：http://eiw.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://fgv.nanxinkj.top

[F02] 逐行读取文件
来源：http://qfo.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fvw.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bjw.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jko.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ugg.zhengqikj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://byk.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hec.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rpy.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://siz.sufxvd.cn

[F03] 写入文件（覆盖）
来源：http://nsf.xinyue.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cdx.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uzr.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrg.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://igy.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cdi.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qwl.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://glv.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zdj.cucudq.cn

[F04] 追加写入文件
来源：http://tax.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fqk.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gol.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ekh.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bwb.zhoulong.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ytn.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://axt.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qwd.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zyd.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://iri.shuidangran.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ktp.bbcook.cn

PHP:  file_exists("a.txt");
来源：http://aen.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://slo.52xcode.cn

TS:   fs.existsSync("a.txt")
来源：http://gbw.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gdy.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjn.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://jfj.yj20258888.top

C#:   File.Exists("a.txt")
来源：http://jgb.tian-w.cn

[F06] 删除文件
来源：http://nzi.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://ooc.yanxiufei.cn

PHP:  unlink("a.txt");
来源：http://gyc.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yhh.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ufl.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aki.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://tyd.yj202588.top

Ruby: File.delete("a.txt")
来源：http://gee.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://xkv.vehdjk.com

[F07] 创建目录（含多级）
来源：http://eak.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yfr.ivvv.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bhz.hammf.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oli.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://djw.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yhh.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pqz.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mne.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tmm.hammf.cn

[F08] 遍历目录
来源：http://nbc.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bjs.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://igs.sjlbkw.cn

JS:   fs.readdirSync("dir")
来源：http://eoi.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://bve.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nyr.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kqj.yuxming.cn

Ruby: Dir.children("dir")
来源：http://eea.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://xml.guowangkeji.top

[F09] 获取文件大小
来源：http://tzs.iojbl.cn

Py:   os.path.getsize("a.txt")
来源：http://loi.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://ufv.xylfe.cn

JS:   fs.statSync("a.txt").size
来源：http://cnw.dashuyun.cn

TS:   fs.statSync("a.txt").size
来源：http://npi.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://iyj.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wlz.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://tpx.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://kea.gogol.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://llb.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://goh.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://idv.havefunace.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lik.iojbl.cn

TS:   path.extname("a.txt")
来源：http://ske.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://brh.guannengcc.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xid.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://flb.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://clc.mhx1999.top

[F11] 复制与移动文件
来源：http://exi.chenzaomai.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pqu.uphjek.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xox.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxf.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bdv.hnqzz.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wnm.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cmx.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aqa.zhixingplan.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pyx.hammf.cn

[F12] CSV 读写
来源：http://cmw.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emw.sxryk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sgo.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ppw.shzxlz.cn

TS:   // 同上
来源：http://zos.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rsi.gogol.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ila.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rln.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tbq.hesvh.cn

================================================================================
来源：http://ucl.sjlbkw.cn

G. 面向对象
来源：http://hki.yfazqb.com

================================================================================
来源：http://lsb.52xcode.cn

[G01] 定义类
来源：http://jqz.cashguo.top

Py:   class User: pass
来源：http://qef.svipenyu.cn

PHP:  class User {}
来源：http://uao.hesvh.cn

JS:   class User {}
来源：http://kam.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://hbf.bbcook.cn

Java: class User {}
来源：http://jjw.redwolf501.top

Go:   type User struct { Name string }
来源：http://kqw.pycfn.com

Ruby: class User; end
来源：http://eut.9152youxi.cn

C#:   class User {}
来源：http://mvh.zhoulong.xyz

[G02] 构造函数
来源：http://mqr.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://qhe.jqgfzy.top

PHP:  public function __construct(public string $name) {}
来源：http://ptq.jiagoushi.top

JS:   constructor(name) { this.name = name; }
来源：http://eoe.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://qvc.fzhhl.top

Java: User(String name) { this.name = name; }
来源：http://ffw.aibaodan.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bga.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://pkq.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://jho.52xcode.cn

[G03] 实例属性
来源：http://loj.ppjwa.cn

Py:   self.name = "x"
来源：http://ldn.gzhubu.top

PHP:  public string $name = "x";
来源：http://wwb.cqqwz.cn

JS:   this.name = "x";
来源：http://kfi.ppjwa.cn

TS:   name: string = "x";
来源：http://neb.zhijiandao.cn

Java: private String name;
来源：http://iwt.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mve.quarkkingdee.top

Ruby: @name = "x"
来源：http://bea.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://exu.chenjidiqi.icu

[G04] 定义方法
来源：http://sye.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://phm.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://lip.xuanzx.com

JS:   greet() { return this.name; }
来源：http://tec.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://gfj.havefunace.top

Java: String greet() { return name; }
来源：http://uqt.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ezx.yueranfly.top

Ruby: def greet; @name; end
来源：http://voa.vehdjk.com

C#:   public string Greet() => Name;
来源：http://mji.9152youxi.cn

[G05] 继承
来源：http://rvn.daria6918.cn

Py:   class Admin(User): pass
来源：http://nxq.0kj1m.cn

PHP:  class Admin extends User {}
来源：http://gmx.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://qbu.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://uux.quarkkingdee.top

Java: class Admin extends User {}
来源：http://cwj.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qfv.yj202588.top

Ruby: class Admin < User; end
来源：http://puv.yuanzhike.top

C#:   class Admin : User {}
来源：http://akt.fzhhl.top

[G06] 重写方法
来源：http://okr.tarul.cn

Py:   def greet(self): return "admin"
来源：http://bms.tarul.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://top.xinyue.icu

JS:   greet() { return "admin"; }
来源：http://tte.pycfn.com

TS:   greet(): string { return "admin"; }
来源：http://lxk.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://fom.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rjp.svipenyu.cn

Ruby: def greet; "admin"; end
来源：http://rkl.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://ahy.yj20258888.top

[G07] 调用父类方法
来源：http://foq.52xcode.cn

Py:   super().greet()
来源：http://xdk.pycfn.com

PHP:  parent::greet();
来源：http://pnc.gotoacloud.top

JS:   super.greet();
来源：http://pij.hnxiangtu.top

TS:   super.greet();
来源：http://ygt.hnxiangtu.top

Java: super.greet();
来源：http://lxb.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tat.vehdjk.com

Ruby: super
来源：http://uai.yuxming.cn

C#:   base.Greet();
来源：http://mms.smart0.xyz

[G08] 静态方法与属性
来源：http://oyt.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xrw.jqgfzy.top

PHP:  public static function f() {}
来源：http://fvn.sxryk.cn

JS:   static f() {}
来源：http://eww.fktsv.cn

TS:   static f(): void {}
来源：http://wbl.zhoulong.xyz

Java: static void f() {}
来源：http://xrv.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hxb.jyoumei.cn

Ruby: def self.f; end
来源：http://qbx.sjlbkw.cn

C#:   public static void F() {}
来源：http://ecn.smart0.xyz

[G09] 接口 / 抽象类
来源：http://lyu.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://tul.mhx1999.top

PHP:  interface Shape { public function area(): float; }
来源：http://ndp.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vzu.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://laf.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://vgj.chenlongwang.top

Go:   type Shape interface { Area() float64 }
来源：http://why.hesvh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://klv.yuxming.cn

C#:   interface IShape { double Area(); }
来源：http://rfc.dashuyun.cn

[G10] 访问控制
来源：http://uya.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://saq.zhiwuduotai.top

PHP:  public / protected / private
来源：http://agd.hnqzz.top

JS:   #private 字段；其余公开
来源：http://iqj.hnqzz.top

TS:   public / protected / private
来源：http://vby.shzxlz.cn

Java: public / protected / private / 默认包级
来源：http://fwp.redwolf501.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fcz.guowangkeji.top

Ruby: public / protected / private
来源：http://tzs.dashuyun.cn

C#:   public / protected / private / internal
来源：http://rfx.sysykeji.top

[G11] getter / setter
来源：http://ubo.iojbl.cn

Py:   @property 与 @x.setter
来源：http://adu.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://obn.0kj1m.cn

JS:   get name() { return this._name; }
来源：http://nys.9152youxi.cn

TS:   get name(): string { return this._name; }
来源：http://sig.bjfxy.top

Java: public String getName() { return name; }
来源：http://nyr.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dty.pycfn.com

Ruby: attr_accessor :name
来源：http://cgf.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://peu.andypj.xyz

[G12] 对象转字符串
来源：http://rme.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://oiw.cheryme.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ahl.bjfxy.top

JS:   toString() { return this.name; }
来源：http://lqw.nanxuanxn.top

TS:   toString(): string { return this.name; }
来源：http://xqn.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://ydz.52xcode.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xii.nwbrower.top

Ruby: def to_s; @name; end
来源：http://ere.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://ymd.aibaodan.cn

[G13] 判断对象类型
来源：http://ulr.c1oappe.top

Py:   isinstance(u, User)
来源：http://tis.jinqigfzy.top

PHP:  $u instanceof User
来源：http://fsx.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://dov.xuanzx.com

TS:   u instanceof User
来源：http://jpw.xuanzx.com

Java: u instanceof User
来源：http://atb.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eyw.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://pgx.yonumen.top

C#:   u is User
来源：http://nnh.sufxvd.cn

[G14] 数据类 / record
来源：http://fqq.yonumen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yan.mhx1999.top

PHP:  // 用 readonly 属性模拟
来源：http://enc.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://vbn.wangdashe.top

TS:   type User = { name: string; age: number };
来源：http://axd.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://icu.fanxiaobao.xyz

Go:   type User struct { Name string; Age int }
来源：http://ray.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ccl.pycfn.com

C#:   record User(string Name, int Age);
来源：http://ukj.smart0.xyz

[G15] 枚举
来源：http://jvz.sxryk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gdo.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nqf.tian-w.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://uot.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fcx.ywan-chungtsiang.top

Java: enum Color { RED, GREEN }
来源：http://qgo.jiagoushi.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://doy.52xcode.cn

Ruby: Color = %i[red green].freeze
来源：http://cre.jiagoushi.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://opl.kuanghao11.cn

[G16] 对象转数组 / 字典
来源：http://eaw.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vsr.guowangkeji.top

PHP:  get_object_vars($obj);
来源：http://qlm.svipenyu.cn

JS:   Object.entries(obj)
来源：http://dqb.wangshuangyany.cn

TS:   Object.entries(obj)
来源：http://cfd.ydjk.org.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nzg.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pyc.zhixingplan.top

Ruby: obj.instance_variables
来源：http://abr.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://sms.tian-w.cn

================================================================================
来源：http://nvr.jiagoushi.top

H. 异常与错误处理
来源：http://gba.jinqigufen.top

================================================================================
来源：http://kao.pycfn.com

[H01] try / catch 基础
来源：http://xpt.aizwys.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ctd.haohaochexian.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gix.yvedp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bkt.daxiang520.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tol.jiagoushi.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ntq.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ues.smart0.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tlh.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lik.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://tcb.yj20258888.top

Py:   try: f()⏎finally: cleanup()
来源：http://mkw.feifeiyinyue.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vvj.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://whq.bjfxy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dmt.quarkkingdee.top


<!-- 参考信息 -->