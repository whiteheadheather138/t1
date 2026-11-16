代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uqq.pengpengdd.cyou

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lhm.0kj1m.cn

TS:   if (s === "") {}
来源：http://zdg.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://vmg.cdnleiting.top

Go:   if s == "" {}
来源：http://biu.daxiang520.top

Ruby: if s.empty?
来源：http://uwm.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tlz.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://gcm.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hfw.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bha.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wdi.0kj1m.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lkr.zhaomingkeji.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zaq.jiagoushi.top

Go:   // 按 rune 判断长度后截断
来源：http://wtn.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ezf.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mms.tarul.cn

[E22] 字节长度与字符长度
来源：http://qal.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uzh.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uuc.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wfq.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mwy.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://omc.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lql.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://zzy.jlsjyb.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nwd.yangfankeji.com

================================================================================
来源：http://gpt.tarul.cn

F. 文件与目录
来源：http://luy.sxryk.cn

================================================================================
来源：http://puk.jinqigufen.top

[F01] 读取整个文件
来源：http://ozx.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ypo.gzhubu.top

PHP:  file_get_contents("a.txt");
来源：http://wft.xinyue.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://csw.chenlongwang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pjs.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zey.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kaq.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://sgj.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://whw.gotoacloud.top

[F02] 逐行读取文件
来源：http://dyb.hnxiangtu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://npe.zhijiandao.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aqs.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lcn.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wzx.hfpthk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qcl.jinqigfzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://spx.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ofw.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aqv.zhoulong.xyz

[F03] 写入文件（覆盖）
来源：http://mfa.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fcs.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fik.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjf.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rwf.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iig.fehbvm.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zow.mhx1999.top

Ruby: File.write("a.txt", "hi")
来源：http://tcw.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dvd.guowangkeji.top

[F04] 追加写入文件
来源：http://lco.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nmr.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rmf.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tta.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zsj.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sov.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://juc.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tyr.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cia.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://rlg.dianchejie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zxu.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://bcs.ppjwa.cn

JS:   fs.existsSync("a.txt")
来源：http://zsm.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://ceu.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ven.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eev.vqdsnc.cn

Ruby: File.exist?("a.txt")
来源：http://dla.shanyushiyangkeji.top

C#:   File.Exists("a.txt")
来源：http://fyh.fzhhl.top

[F06] 删除文件
来源：http://cak.tarul.cn

Py:   os.remove("a.txt")
来源：http://xts.fktsv.cn

PHP:  unlink("a.txt");
来源：http://bjz.hywenlv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nlp.zhoulong.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://tzb.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jsp.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://lri.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://xfb.jyoumei.cn

C#:   File.Delete("a.txt");
来源：http://thz.bbcook.cn

[F07] 创建目录（含多级）
来源：http://qwf.chenzaomai.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cvp.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jfc.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jfd.xziqi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ixi.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vqb.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fbp.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rqv.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kcl.tanke756.top

[F08] 遍历目录
来源：http://fun.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pnc.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fmf.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://egc.sysykeji.top

TS:   fs.readdirSync("dir")
来源：http://cbu.jyoumei.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yoo.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xwl.havefunace.top

Ruby: Dir.children("dir")
来源：http://ppr.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://ail.xinyue.icu

[F09] 获取文件大小
来源：http://zcc.wangshuangyany.cn

Py:   os.path.getsize("a.txt")
来源：http://byy.redwolf501.top

PHP:  filesize("a.txt");
来源：http://rpg.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://miw.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://hom.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zvv.vqdsnc.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ggd.sxryk.cn

Ruby: File.size("a.txt")
来源：http://kpz.nanxinkj.top

C#:   new FileInfo("a.txt").Length
来源：http://gap.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://wbv.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aiy.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wwg.hcnkem.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ynb.jianghu66.top

TS:   path.extname("a.txt")
来源：http://ioe.ybcxt.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mgx.yfazqb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sep.hywenlv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gis.gogol.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ikp.sufxvd.cn

[F11] 复制与移动文件
来源：http://bvg.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ohj.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nit.ctjpmb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xnu.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://osf.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nnm.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://had.c1oappe.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eyb.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jmq.9152youxi.cn

[F12] CSV 读写
来源：http://nij.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nls.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sqi.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://prx.wangdashe.top

TS:   // 同上
来源：http://wrs.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qgg.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jhr.zdqjudy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xsr.yvedp.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mmc.ctjpmb.com

================================================================================
来源：http://wvr.chenjidiqi.icu

G. 面向对象
来源：http://gqf.vqdsnc.cn

================================================================================
来源：http://zzg.jqgufenzy.top

[G01] 定义类
来源：http://sxp.sjlbkw.cn

Py:   class User: pass
来源：http://eol.chenzaomai.com

PHP:  class User {}
来源：http://zhy.cashguo.top

JS:   class User {}
来源：http://rcv.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://aih.yj20258888.top

Java: class User {}
来源：http://aie.guannengcc.top

Go:   type User struct { Name string }
来源：http://bvi.zycfv.cn

Ruby: class User; end
来源：http://vag.yfazqb.com

C#:   class User {}
来源：http://mxp.pycfn.com

[G02] 构造函数
来源：http://txj.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://jbh.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://zfy.meibo888.top

JS:   constructor(name) { this.name = name; }
来源：http://gyo.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://vfv.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://qeh.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eaj.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://abd.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://otq.daxiang520.top

[G03] 实例属性
来源：http://pze.bjfxy.top

Py:   self.name = "x"
来源：http://crh.zhoulong.xyz

PHP:  public string $name = "x";
来源：http://mky.xylfe.cn

JS:   this.name = "x";
来源：http://lsf.smart0.xyz

TS:   name: string = "x";
来源：http://hyh.cdnleiting.top

Java: private String name;
来源：http://lvl.fengsongda.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rjn.yueranfly.top

Ruby: @name = "x"
来源：http://ejr.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://bmj.shanyushiyangkeji.top

[G04] 定义方法
来源：http://rbc.wangdashe.top

Py:   def greet(self): return self.name
来源：http://plq.nwbrower.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pmu.cheryme.top

JS:   greet() { return this.name; }
来源：http://pvi.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://oiq.jianghu66.top

Java: String greet() { return name; }
来源：http://bhq.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xsg.haohaochexian.top

Ruby: def greet; @name; end
来源：http://fto.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://noi.yuanzhike.top

[G05] 继承
来源：http://ack.xinyue.icu

Py:   class Admin(User): pass
来源：http://nte.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://mbc.dashuyun.cn

JS:   class Admin extends User {}
来源：http://fjh.gzhubu.top

TS:   class Admin extends User {}
来源：http://kcr.yangfankeji.com

Java: class Admin extends User {}
来源：http://lxq.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xfu.52xcode.cn

Ruby: class Admin < User; end
来源：http://wcq.iojbl.cn

C#:   class Admin : User {}
来源：http://kyt.hongshengwenyu.top

[G06] 重写方法
来源：http://kdk.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://ila.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fre.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://xru.guannengcc.top

TS:   greet(): string { return "admin"; }
来源：http://fhj.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://hkg.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tjo.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://rha.hfpthk.cn

C#:   public override string Greet() => "admin";
来源：http://ilp.pycfn.com

[G07] 调用父类方法
来源：http://vzo.daria6918.cn

Py:   super().greet()
来源：http://qkd.xinyue.icu

PHP:  parent::greet();
来源：http://lep.shzxlz.cn

JS:   super.greet();
来源：http://ame.tianlin.xyz

TS:   super.greet();
来源：http://vnv.c1oappe.top

Java: super.greet();
来源：http://sln.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xws.yueranfly.top

Ruby: super
来源：http://iyi.tian-w.cn

C#:   base.Greet();
来源：http://pud.gaohongyu789.top

[G08] 静态方法与属性
来源：http://pcn.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ifa.jqgufenzy.top

PHP:  public static function f() {}
来源：http://xbn.andypj.xyz

JS:   static f() {}
来源：http://rbf.316326.xyz

TS:   static f(): void {}
来源：http://lcy.tarul.cn

Java: static void f() {}
来源：http://exr.sxryk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qfr.uphjek.com

Ruby: def self.f; end
来源：http://tus.aibaodan.cn

C#:   public static void F() {}
来源：http://ayr.yongpay.top

[G09] 接口 / 抽象类
来源：http://slx.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://ljf.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://coe.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://owp.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://rxb.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://bfc.gogol.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://ydd.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nzw.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://nji.dashuyun.cn

[G10] 访问控制
来源：http://caf.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://qip.shangyingyoupin.top

PHP:  public / protected / private
来源：http://prl.birdmap.top

JS:   #private 字段；其余公开
来源：http://fdv.yvedp.cn

TS:   public / protected / private
来源：http://qbh.yongpay.top

Java: public / protected / private / 默认包级
来源：http://sfi.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rju.nanxuanxn.top

Ruby: public / protected / private
来源：http://zzp.jqgfzy.top

C#:   public / protected / private / internal
来源：http://ucu.gaohongyu789.top

[G11] getter / setter
来源：http://sgu.zycfv.cn

Py:   @property 与 @x.setter
来源：http://pzy.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yru.cashguo.top

JS:   get name() { return this._name; }
来源：http://hhr.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://kol.xylfe.cn

Java: public String getName() { return name; }
来源：http://wwm.pengpengdd.cyou

Go:   func (u User) GetName() string { return u.Name }
来源：http://rws.tarul.cn

Ruby: attr_accessor :name
来源：http://zar.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://ygm.yonumen.top

[G12] 对象转字符串
来源：http://wbe.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://coj.haohaochexian.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kqy.fzhhl.top

JS:   toString() { return this.name; }
来源：http://aon.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://fcj.9152youxi.cn

Java: @Override public String toString() { return name; }
来源：http://igv.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://mrv.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://hsg.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://mbb.gotoacloud.top

[G13] 判断对象类型
来源：http://zhr.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://dkt.fengsongda.top

PHP:  $u instanceof User
来源：http://qvh.cashguo.top

JS:   u instanceof User
来源：http://afs.gotoacloud.top

TS:   u instanceof User
来源：http://eyt.nwbrower.top

Java: u instanceof User
来源：http://alj.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://svm.yueranfly.top

Ruby: u.is_a?(User)
来源：http://zjw.pycfn.com

C#:   u is User
来源：http://eef.jlsjyb.cn

[G14] 数据类 / record
来源：http://pvg.xylfe.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ffn.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://kvv.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://klg.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://swm.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://xmh.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://bzc.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kek.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://bnh.dashuyun.cn

[G15] 枚举
来源：http://wwe.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dbr.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ozk.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sur.hesvh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lqv.c1oappe.top

Java: enum Color { RED, GREEN }
来源：http://lnw.shuidangran.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ghw.nanxuanxn.top

Ruby: Color = %i[red green].freeze
来源：http://ons.nanxinkj.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pcz.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://aux.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ywr.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://gai.zhaomingkeji.xyz

JS:   Object.entries(obj)
来源：http://nrx.daxiang520.top

TS:   Object.entries(obj)
来源：http://eeq.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tod.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ijp.yonumen.top

Ruby: obj.instance_variables
来源：http://qet.yuanzhike.top

C#:   // 用反射或 System.Text.Json
来源：http://ysh.zdqjudy.top

================================================================================
来源：http://htj.yanxiufei.cn

H. 异常与错误处理
来源：http://qvg.c1oappe.top

================================================================================
来源：http://cqn.zhoulong.xyz

[H01] try / catch 基础
来源：http://goj.nanxinkj.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jtc.aizwys.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://esh.pycfn.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tsr.guowangkeji.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jzb.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwx.xylfe.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wol.cucudq.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jwi.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jmg.fehbvm.com

[H02] finally / ensure 收尾
来源：http://khc.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://nge.kuanghao11.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://icf.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fmm.nanxinkj.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dye.hammf.cn


<!-- 参考信息 -->