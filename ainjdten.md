代发 wailian999

Go:   if s == "" {}
来源：http://xis.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://srs.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vje.pycfn.com

[E21] 超长截断加省略号
来源：http://tpq.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hfd.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uez.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rni.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ads.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pjz.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://tcs.mhx1999.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eun.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fut.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://cac.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pbs.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jfx.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ehf.ywan-chungtsiang.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wva.yueranfly.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://crz.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdr.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://xsw.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xzf.fehbvm.com

================================================================================
来源：http://zzp.sjlbkw.cn

F. 文件与目录
来源：http://guy.sysykeji.top

================================================================================
来源：http://ltl.xuetiantiany.cn

[F01] 读取整个文件
来源：http://xls.yvedp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qge.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://ptq.quarkkingdee.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hya.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fxx.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ptf.guannengcc.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jox.sufxvd.cn

Ruby: File.read("a.txt")
来源：http://xoz.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://xaf.0kj1m.cn

[F02] 逐行读取文件
来源：http://mwr.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gbk.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rkq.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zze.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gtc.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qkf.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pap.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ftv.ywan-chungtsiang.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ird.ctjpmb.com

[F03] 写入文件（覆盖）
来源：http://fdy.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://opm.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xhx.zhengqikj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jvk.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bwz.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ykf.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wgl.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://mic.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dlm.fehbvm.com

[F04] 追加写入文件
来源：http://qob.fanxiaobao.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://swl.9152youxi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oto.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofv.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ghq.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hvl.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kzm.yfazqb.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qdh.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eju.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://eve.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mov.cqqwz.cn

PHP:  file_exists("a.txt");
来源：http://tug.jyoumei.cn

JS:   fs.existsSync("a.txt")
来源：http://hdl.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://jcp.zdbjq.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ztw.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://kma.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://zrl.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://aqw.c1oappe.top

[F06] 删除文件
来源：http://bja.andypj.xyz

Py:   os.remove("a.txt")
来源：http://bft.meibo888.top

PHP:  unlink("a.txt");
来源：http://npx.cucudq.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yyj.ydzc1.top

TS:   fs.unlinkSync("a.txt")
来源：http://faa.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hqa.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://yzm.guannengcc.top

Ruby: File.delete("a.txt")
来源：http://apb.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://nhc.uphjek.com

[F07] 创建目录（含多级）
来源：http://gdo.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yne.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ebk.jqgfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjm.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iln.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mni.zhiwuduotai.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dae.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hmn.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ukd.redwolf501.top

[F08] 遍历目录
来源：http://znx.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cmz.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://stt.shangyingyoupin.top

JS:   fs.readdirSync("dir")
来源：http://clm.birdmap.top

TS:   fs.readdirSync("dir")
来源：http://gvz.mhx1999.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://feo.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kzw.ppjwa.cn

Ruby: Dir.children("dir")
来源：http://xar.kuanghao11.cn

C#:   Directory.GetFiles("dir")
来源：http://top.fanxiaobao.xyz

[F09] 获取文件大小
来源：http://arv.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://kzr.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://kyx.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://cmq.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://wbw.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://anq.gzhubu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://efn.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://yyo.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://sgx.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://byb.zhijiandao.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zxt.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dea.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://soh.vehdjk.com

TS:   path.extname("a.txt")
来源：http://lgk.hfpthk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ovm.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lvk.shzxlz.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vpq.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mmz.gzhubu.top

[F11] 复制与移动文件
来源：http://vfb.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mbj.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uht.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hod.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oue.ybcxt.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://znx.zhengqikj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sik.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xig.hcnkem.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nsx.zhijiandao.cn

[F12] CSV 读写
来源：http://aab.sxryk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jfp.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vjq.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sut.daxiang520.top

TS:   // 同上
来源：http://pwv.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pbb.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qga.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jxf.mhx1999.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gtp.chenzaomai.com

================================================================================
来源：http://zfb.andypj.xyz

G. 面向对象
来源：http://nmv.vehdjk.com

================================================================================
来源：http://ysx.ivvv.top

[G01] 定义类
来源：http://wce.yuanzhike.top

Py:   class User: pass
来源：http://uhx.ydjk.org.cn

PHP:  class User {}
来源：http://egl.jianghu66.top

JS:   class User {}
来源：http://jff.yj20258888.top

TS:   class User { name: string = ""; }
来源：http://fjm.xziqi.cn

Java: class User {}
来源：http://isr.epnwcf.com

Go:   type User struct { Name string }
来源：http://dac.chenzaomai.com

Ruby: class User; end
来源：http://ils.pengpengdd.cyou

C#:   class User {}
来源：http://lhe.ivvv.top

[G02] 构造函数
来源：http://yej.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://wyz.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://lcf.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ssz.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://yjy.svipenyu.cn

Java: User(String name) { this.name = name; }
来源：http://fgd.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://crz.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://two.shangyingyoupin.top

C#:   public User(string name) { Name = name; }
来源：http://xkj.gzhubu.top

[G03] 实例属性
来源：http://wat.pengpengdd.cyou

Py:   self.name = "x"
来源：http://htw.uphjek.com

PHP:  public string $name = "x";
来源：http://hub.dashuyun.cn

JS:   this.name = "x";
来源：http://cwu.yj20258.top

TS:   name: string = "x";
来源：http://ths.yuxming.cn

Java: private String name;
来源：http://gzw.cucudq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xio.gogol.net.cn

Ruby: @name = "x"
来源：http://rgx.quarkkingdee.top

C#:   public string Name { get; set; } = "x";
来源：http://izn.yueranfly.top

[G04] 定义方法
来源：http://qrk.yj202588.top

Py:   def greet(self): return self.name
来源：http://sce.meibo888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qmc.cashguo.top

JS:   greet() { return this.name; }
来源：http://lrx.hysaishi.cn

TS:   greet(): string { return this.name; }
来源：http://deo.chenjidiqi.icu

Java: String greet() { return name; }
来源：http://kgb.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jyw.jinyuanbaomall.cn

Ruby: def greet; @name; end
来源：http://xcm.ydzc1.top

C#:   public string Greet() => Name;
来源：http://may.haohaochexian.top

[G05] 继承
来源：http://fes.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://oxe.smart0.xyz

PHP:  class Admin extends User {}
来源：http://arq.yfazqb.com

JS:   class Admin extends User {}
来源：http://xud.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://hng.yfazqb.com

Java: class Admin extends User {}
来源：http://hvu.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ggf.ydzc1.top

Ruby: class Admin < User; end
来源：http://zpl.zhengqikj.top

C#:   class Admin : User {}
来源：http://ccd.iojbl.cn

[G06] 重写方法
来源：http://yed.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://ktk.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://skq.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://rye.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://ory.zycfv.cn

Java: @Override String greet() { return "admin"; }
来源：http://vbg.wangdashe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mve.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://zff.nanxuanxn.top

C#:   public override string Greet() => "admin";
来源：http://aoq.yangfankeji.com

[G07] 调用父类方法
来源：http://sig.chenlongwang.top

Py:   super().greet()
来源：http://kat.pengpengdd.cyou

PHP:  parent::greet();
来源：http://ywo.shangyingyoupin.top

JS:   super.greet();
来源：http://ejg.aizwys.cn

TS:   super.greet();
来源：http://kxw.yangfankeji.com

Java: super.greet();
来源：http://vhf.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hbw.zdqjudy.top

Ruby: super
来源：http://tbg.shzxlz.cn

C#:   base.Greet();
来源：http://vhg.snrcjt.cn

[G08] 静态方法与属性
来源：http://xry.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uia.gzhubu.top

PHP:  public static function f() {}
来源：http://wzo.tarul.cn

JS:   static f() {}
来源：http://ekp.nanxinkj.top

TS:   static f(): void {}
来源：http://dxk.vehdjk.com

Java: static void f() {}
来源：http://hqw.ydjk.org.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lau.yonumen.top

Ruby: def self.f; end
来源：http://abu.0kj1m.cn

C#:   public static void F() {}
来源：http://anp.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://exr.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://kdx.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://jgp.cashguo.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qrj.snrcjt.cn

TS:   interface Shape { area(): number; }
来源：http://kfy.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://uwl.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://krf.svipenyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://apq.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://lpm.hammf.cn

[G10] 访问控制
来源：http://jex.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://goz.mhx1999.top

PHP:  public / protected / private
来源：http://fve.yueranfly.top

JS:   #private 字段；其余公开
来源：http://oav.xingfuxueyuan.xyz

TS:   public / protected / private
来源：http://tjh.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://itb.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qlx.nwbrower.top

Ruby: public / protected / private
来源：http://hqb.fzhhl.top

C#:   public / protected / private / internal
来源：http://ocx.havefunace.top

[G11] getter / setter
来源：http://ixb.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://ndq.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://yta.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://asp.xziqi.cn

TS:   get name(): string { return this._name; }
来源：http://anf.yuanzhike.top

Java: public String getName() { return name; }
来源：http://diy.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://wcd.hywenlv.cn

Ruby: attr_accessor :name
来源：http://rnt.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://ztr.tarul.cn

[G12] 对象转字符串
来源：http://kkn.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://nlf.pengpengdd.cyou

PHP:  public function __toString(): string { return $this->name; }
来源：http://afw.sjlbkw.cn

JS:   toString() { return this.name; }
来源：http://wzz.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://dhu.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://acr.ctjpmb.com

Go:   func (u User) String() string { return u.Name }
来源：http://rbh.vehdjk.com

Ruby: def to_s; @name; end
来源：http://mga.uphjek.com

C#:   public override string ToString() => Name;
来源：http://srb.smart0.xyz

[G13] 判断对象类型
来源：http://fox.fehbvm.com

Py:   isinstance(u, User)
来源：http://sjv.svipenyu.cn

PHP:  $u instanceof User
来源：http://nkk.hfpthk.cn

JS:   u instanceof User
来源：http://yok.ivvv.top

TS:   u instanceof User
来源：http://beu.fktsv.cn

Java: u instanceof User
来源：http://crv.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uru.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://wqm.smart0.xyz

C#:   u is User
来源：http://nfg.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://tvq.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zck.shuidangran.top

PHP:  // 用 readonly 属性模拟
来源：http://lov.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://qpa.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://pyh.316326.xyz

Java: record User(String name, int age) {}
来源：http://ntk.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://por.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cvq.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://ake.guannengcc.top

[G15] 枚举
来源：http://pho.c1oappe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bik.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://daz.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oxo.yongpay.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yvd.gzhubu.top

Java: enum Color { RED, GREEN }
来源：http://gyn.chenzaomai.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nui.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://tuj.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xad.yj202588.top

[G16] 对象转数组 / 字典
来源：http://gfr.uphjek.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qfq.zhengqikj.top

PHP:  get_object_vars($obj);
来源：http://and.wangdashe.top

JS:   Object.entries(obj)
来源：http://qwy.zdbjq.cn

TS:   Object.entries(obj)
来源：http://ucm.snrcjt.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://quj.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ohf.yj20258.top

Ruby: obj.instance_variables
来源：http://wvf.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://ofz.dianchejie.cn

================================================================================
来源：http://jec.xinyue.icu

H. 异常与错误处理
来源：http://lcj.gotoacloud.top

================================================================================
来源：http://pmi.52xcode.cn

[H01] try / catch 基础
来源：http://mcf.birdmap.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://soj.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://amy.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pvu.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgj.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wor.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mha.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kto.hywenlv.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ijv.ydzc1.top

[H02] finally / ensure 收尾
来源：http://ujy.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rwc.ctjpmb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://mnj.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://ihn.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://egj.yj20258888.top

Java: try { f(); } finally { cleanup(); }
来源：http://fck.yvedp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vuj.yuanzhike.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vjd.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pum.yangfankeji.com


<!-- 参考信息 -->