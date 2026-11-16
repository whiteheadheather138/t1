代发 wailian999

Go:   if s == "" {}
来源：http://yrc.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://fhn.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://otg.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://ssy.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jdy.ppjwa.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gim.fktsv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zpg.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ims.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zdb.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://wzc.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hfm.dashuyun.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://obz.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://rsw.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pkq.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rnb.fehbvm.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kxj.shanyushiyangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yvz.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exm.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mmv.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://fuh.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zxz.sysykeji.top

================================================================================
来源：http://gur.yj202588.top

F. 文件与目录
来源：http://ojq.quarkkingdee.top

================================================================================
来源：http://qwx.daxiang520.top

[F01] 读取整个文件
来源：http://wam.zhiwuduotai.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cvn.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://fsj.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://syg.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ufk.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rpi.yonumen.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jfb.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://cph.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://bor.fzhhl.top

[F02] 逐行读取文件
来源：http://azg.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://myr.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xlf.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ilx.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ykb.shzxlz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://msh.fzhhl.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://omo.sweek.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eht.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wzp.bjfxy.top

[F03] 写入文件（覆盖）
来源：http://ztn.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://apq.jqgufenzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://acd.dashuyun.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://may.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dwg.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jnn.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hpt.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ltu.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jsd.uphjek.com

[F04] 追加写入文件
来源：http://qwg.wangdashe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zgx.nanxinkj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hey.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eol.cdnleiting.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fvq.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iam.xylfe.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hqn.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hpx.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ehc.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://uty.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gjd.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://twl.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://rnx.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://csd.quarkkingdee.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tjs.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tyh.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://bor.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://hgv.yangfankeji.com

[F06] 删除文件
来源：http://hpt.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://cvr.tarul.cn

PHP:  unlink("a.txt");
来源：http://tkz.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://qzl.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://ffk.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://emj.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://ubj.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://ljc.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://mdt.vqdsnc.cn

[F07] 创建目录（含多级）
来源：http://det.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pyz.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wgi.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ocg.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohf.haohaochexian.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://srk.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yxi.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wzz.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jue.jinghuilouyu.cn

[F08] 遍历目录
来源：http://ypy.hongshengwenyu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zzu.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zca.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://nfy.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://zrk.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vmn.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://unb.smart0.xyz

Ruby: Dir.children("dir")
来源：http://gtk.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://koq.gaohongyu789.top

[F09] 获取文件大小
来源：http://mht.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://bpp.sufxvd.cn

PHP:  filesize("a.txt");
来源：http://det.havefunace.top

JS:   fs.statSync("a.txt").size
来源：http://tqf.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://xkc.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://qap.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://znw.yongpay.top

Ruby: File.size("a.txt")
来源：http://xsb.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://rvq.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://pha.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kuw.gogol.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hyb.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://apa.fengsongda.top

TS:   path.extname("a.txt")
来源：http://ada.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zdw.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wxt.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vtg.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tdu.shangyingyoupin.top

[F11] 复制与移动文件
来源：http://lqg.316326.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://toq.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xgw.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pob.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lsl.xylfe.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jxd.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://non.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfz.bjfxy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uql.wangshuangyany.cn

[F12] CSV 读写
来源：http://dyb.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xrv.haohaochexian.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://inw.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dsa.316326.xyz

TS:   // 同上
来源：http://nvf.cashguo.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qlq.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://onb.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bpr.xuanzx.com

C#:   // 无内置：用 CsvHelper 库
来源：http://nak.fengsongda.top

================================================================================
来源：http://moe.ctjpmb.com

G. 面向对象
来源：http://oqm.daxiang520.top

================================================================================
来源：http://rcr.yanxiufei.cn

[G01] 定义类
来源：http://evs.vehdjk.com

Py:   class User: pass
来源：http://fsd.yfazqb.com

PHP:  class User {}
来源：http://fgp.feifeiyinyue.top

JS:   class User {}
来源：http://pxz.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://oeb.hnqzz.top

Java: class User {}
来源：http://ocr.yuxming.cn

Go:   type User struct { Name string }
来源：http://kkd.yueranfly.top

Ruby: class User; end
来源：http://nxv.9152youxi.cn

C#:   class User {}
来源：http://mln.zhiwuduotai.top

[G02] 构造函数
来源：http://wrc.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://knl.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://phj.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://kat.yonumen.top

TS:   constructor(public name: string) {}
来源：http://mrf.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://dce.chenlongwang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fxi.zhengqikj.top

Ruby: def initialize(name); @name = name; end
来源：http://hti.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://hiz.zycfv.cn

[G03] 实例属性
来源：http://cfj.mhx1999.top

Py:   self.name = "x"
来源：http://sih.pengpengdd.cyou

PHP:  public string $name = "x";
来源：http://dcp.hnqzz.top

JS:   this.name = "x";
来源：http://gav.tanke756.top

TS:   name: string = "x";
来源：http://nsr.dianchejie.cn

Java: private String name;
来源：http://due.pycfn.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://stc.shanyushiyangkeji.top

Ruby: @name = "x"
来源：http://tyi.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://rsi.nanxuanxn.top

[G04] 定义方法
来源：http://wzq.aizwys.cn

Py:   def greet(self): return self.name
来源：http://jot.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nqj.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://qnd.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://tzz.zdbjq.cn

Java: String greet() { return name; }
来源：http://nzk.shanyushiyangtech.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fiw.zhixingplan.top

Ruby: def greet; @name; end
来源：http://hhn.svipenyu.cn

C#:   public string Greet() => Name;
来源：http://qse.ctjpmb.com

[G05] 继承
来源：http://wno.316326.xyz

Py:   class Admin(User): pass
来源：http://pjg.tarul.cn

PHP:  class Admin extends User {}
来源：http://net.cheryme.top

JS:   class Admin extends User {}
来源：http://asd.daxiang520.top

TS:   class Admin extends User {}
来源：http://lnc.haohaochexian.top

Java: class Admin extends User {}
来源：http://qsk.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zon.tian-w.cn

Ruby: class Admin < User; end
来源：http://ahy.xuetiantiany.cn

C#:   class Admin : User {}
来源：http://krb.ctjpmb.com

[G06] 重写方法
来源：http://lfc.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://wau.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bvn.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://ugv.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://pax.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://soz.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://efu.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://vmf.haohaochexian.top

C#:   public override string Greet() => "admin";
来源：http://tgu.bbcook.cn

[G07] 调用父类方法
来源：http://mzi.jqgfzy.top

Py:   super().greet()
来源：http://hiv.jlsjyb.cn

PHP:  parent::greet();
来源：http://aji.yangfankeji.com

JS:   super.greet();
来源：http://cmu.zhiwuduotai.top

TS:   super.greet();
来源：http://vnu.sweek.top

Java: super.greet();
来源：http://tlq.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yli.tian-w.cn

Ruby: super
来源：http://dzb.zhiwuduotai.top

C#:   base.Greet();
来源：http://guc.cqqwz.cn

[G08] 静态方法与属性
来源：http://jlo.bbcook.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dwh.dashuyun.cn

PHP:  public static function f() {}
来源：http://sbh.bjfxy.top

JS:   static f() {}
来源：http://uhu.nanxuanxn.top

TS:   static f(): void {}
来源：http://zkw.yj20258888.top

Java: static void f() {}
来源：http://vgf.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rxu.dianchejie.cn

Ruby: def self.f; end
来源：http://amy.fanxiaobao.xyz

C#:   public static void F() {}
来源：http://gts.zycfv.cn

[G09] 接口 / 抽象类
来源：http://aum.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://cjz.yongpay.top

PHP:  interface Shape { public function area(): float; }
来源：http://paw.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qed.uphjek.com

TS:   interface Shape { area(): number; }
来源：http://yuv.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://xhi.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://hzg.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://plb.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://bqx.zhixingplan.top

[G10] 访问控制
来源：http://gvw.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://axt.havefunace.top

PHP:  public / protected / private
来源：http://fzj.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://usg.hysaishi.cn

TS:   public / protected / private
来源：http://nnk.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://roe.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pdq.snrcjt.cn

Ruby: public / protected / private
来源：http://cxy.ydzc1.top

C#:   public / protected / private / internal
来源：http://zof.316326.xyz

[G11] getter / setter
来源：http://umx.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://hzg.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://pqv.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://mmd.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://sby.jinqigufen.top

Java: public String getName() { return name; }
来源：http://mdy.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rav.fengsongda.top

Ruby: attr_accessor :name
来源：http://iha.hcnkem.com

C#:   public string Name { get; set; }
来源：http://zfj.snrcjt.cn

[G12] 对象转字符串
来源：http://gtv.yj20258.top

Py:   def __str__(self): return self.name
来源：http://ynq.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fme.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://lyv.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://uvs.xuanzx.com

Java: @Override public String toString() { return name; }
来源：http://tpy.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xge.jianghu66.top

Ruby: def to_s; @name; end
来源：http://pwf.ppjwa.cn

C#:   public override string ToString() => Name;
来源：http://qnn.fengsongda.top

[G13] 判断对象类型
来源：http://hmx.tanke756.top

Py:   isinstance(u, User)
来源：http://pxh.quarkkingdee.top

PHP:  $u instanceof User
来源：http://lud.cashguo.top

JS:   u instanceof User
来源：http://ekh.jqgufenzy.top

TS:   u instanceof User
来源：http://edm.ybcxt.top

Java: u instanceof User
来源：http://gmh.yangfankeji.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://dma.cashguo.top

Ruby: u.is_a?(User)
来源：http://xte.jiagoushi.top

C#:   u is User
来源：http://opn.zdbjq.cn

[G14] 数据类 / record
来源：http://cov.vqdsnc.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xoj.snrcjt.cn

PHP:  // 用 readonly 属性模拟
来源：http://hrb.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://cta.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://vqt.zycfv.cn

Java: record User(String name, int age) {}
来源：http://rzr.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://oog.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gao.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://aev.xziqi.cn

[G15] 枚举
来源：http://xbf.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fui.ybcxt.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://psg.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tay.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rjw.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://hgi.ydzc1.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://run.fengsongda.top

Ruby: Color = %i[red green].freeze
来源：http://fjo.sweek.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oqx.guowangkeji.top

[G16] 对象转数组 / 字典
来源：http://rlh.pengpengdd.cyou

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://erj.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://ivz.cheryme.top

JS:   Object.entries(obj)
来源：http://bzp.redwolf501.top

TS:   Object.entries(obj)
来源：http://wqm.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xxq.birdmap.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gig.vqdsnc.cn

Ruby: obj.instance_variables
来源：http://vkg.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://sfi.feifeiyinyue.top

================================================================================
来源：http://nbp.yanxiufei.cn

H. 异常与错误处理
来源：http://cxo.fanxiaobao.xyz

================================================================================
来源：http://qpo.cashguo.top

[H01] try / catch 基础
来源：http://bni.wangdashe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pbg.nanxinkj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://osv.redwolf501.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://omn.guannengcc.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://erj.tianlin.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://urc.gotoacloud.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fxn.chenjidiqi.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kvn.jinyuanbaomall.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pxi.c1oappe.top

[H02] finally / ensure 收尾
来源：http://reu.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://rpf.yonumen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zxm.nanxinkj.top

JS:   try { f(); } finally { cleanup(); }
来源：http://tuk.gogol.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vmy.svipenyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://syf.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oyp.jlsjyb.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wov.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jze.yj20258888.top


<!-- 参考信息 -->