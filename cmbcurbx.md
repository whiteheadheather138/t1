代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://jea.hysaishi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eod.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vtm.andypj.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ntb.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yjb.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://eyy.ppjwa.cn

Py:   s.splitlines()
来源：http://ldc.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oyg.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://acw.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://zgj.yongpay.top

Java: s.lines().toList()
来源：http://ncv.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://leq.guannengcc.top

Ruby: s.lines
来源：http://ixt.tanke756.top

C#:   s.Split('\n')
来源：http://kne.zycfv.cn

[E20] 判断字符串是否为空
来源：http://lvp.ybcxt.top

Py:   if not s:
来源：http://hvj.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://okg.yj202588.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yog.hfpthk.cn

TS:   if (s === "") {}
来源：http://zvb.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://okx.xuanzx.com

Go:   if s == "" {}
来源：http://rfp.kuanghao11.cn

Ruby: if s.empty?
来源：http://drn.52xcode.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lic.chenjidiqi.icu

[E21] 超长截断加省略号
来源：http://nuz.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://omn.daria6918.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gxr.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://liq.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrd.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hqt.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://hoe.gotoacloud.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hmy.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ddu.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://stl.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zvu.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwh.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdu.hammf.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxy.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qcp.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gnl.hongshengwenyu.top

Ruby: s.bytesize;  s.length
来源：http://eiy.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hej.zhaomingkeji.xyz

================================================================================
来源：http://oen.vqdsnc.cn

F. 文件与目录
来源：http://bci.chenjidiqi.icu

================================================================================
来源：http://muv.feifeiyinyue.top

[F01] 读取整个文件
来源：http://ufb.xuanzx.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pam.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://hnp.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://itr.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bcu.cashguo.top

Java: Files.readString(Path.of("a.txt"))
来源：http://pfi.shzxlz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rrx.yangfankeji.com

Ruby: File.read("a.txt")
来源：http://vrg.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://kpk.uphjek.com

[F02] 逐行读取文件
来源：http://kkf.hysaishi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dga.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lrv.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnf.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dyq.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vvp.jqgufenzy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eki.cdnleiting.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://leo.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rdc.shzxlz.cn

[F03] 写入文件（覆盖）
来源：http://jdo.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vmx.jinqigfzy.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://cvq.mhx1999.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://azq.yongpay.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://noz.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bnb.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wiy.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://sev.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ftv.fehbvm.com

[F04] 追加写入文件
来源：http://luv.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lnq.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ycn.chenjidiqi.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdf.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofr.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vis.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lgf.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jbi.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jde.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://alb.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://djc.fzhhl.top

PHP:  file_exists("a.txt");
来源：http://zoh.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://ljs.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://nzf.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qzr.52xcode.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ypm.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://zqh.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://rgx.daxiang520.top

[F06] 删除文件
来源：http://cuy.daxiang520.top

Py:   os.remove("a.txt")
来源：http://tlg.sweek.top

PHP:  unlink("a.txt");
来源：http://qjw.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xoy.shuidangran.top

TS:   fs.unlinkSync("a.txt")
来源：http://mzj.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rbb.tarul.cn

Go:   os.Remove("a.txt")
来源：http://jkx.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://dtf.hammf.cn

C#:   File.Delete("a.txt");
来源：http://heo.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://ozo.yueranfly.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uyz.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gnm.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xcv.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qyq.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qdd.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wjr.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mfz.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iwm.sxryk.cn

[F08] 遍历目录
来源：http://vsm.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://cdt.nwbrower.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jvg.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://jqk.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://wze.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tqa.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uvm.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://ebd.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://pso.zhijiandao.cn

[F09] 获取文件大小
来源：http://fuz.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://hpb.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://rsa.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://uhd.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://umt.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mdd.ydjk.org.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ian.hesvh.cn

Ruby: File.size("a.txt")
来源：http://qbs.yvedp.cn

C#:   new FileInfo("a.txt").Length
来源：http://luo.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://zgy.shangyingyoupin.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ujo.sweek.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gij.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ami.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://aqu.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hxp.snrcjt.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tsy.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xnf.hnxiangtu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ozs.jqgfzy.top

[F11] 复制与移动文件
来源：http://dcq.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gjg.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hic.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hny.hcnkem.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvs.tianlin.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oby.hnqzz.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://num.daxiang520.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mph.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zgv.mhx1999.top

[F12] CSV 读写
来源：http://tfs.316326.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vag.pengpengdd.cyou

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ycp.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lfd.redwolf501.top

TS:   // 同上
来源：http://fot.hfpthk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kif.daxiang520.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://igu.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ekx.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cmi.vqdsnc.cn

================================================================================
来源：http://kxd.ppjwa.cn

G. 面向对象
来源：http://qbd.pycfn.com

================================================================================
来源：http://awf.52xcode.cn

[G01] 定义类
来源：http://rzd.shzxlz.cn

Py:   class User: pass
来源：http://psl.wangshuangyany.cn

PHP:  class User {}
来源：http://izm.zdqjudy.top

JS:   class User {}
来源：http://yfw.yueranfly.top

TS:   class User { name: string = ""; }
来源：http://ldb.pengpengdd.cyou

Java: class User {}
来源：http://fvr.daxiang520.top

Go:   type User struct { Name string }
来源：http://ryn.chenlongwang.top

Ruby: class User; end
来源：http://dly.smart0.xyz

C#:   class User {}
来源：http://utz.birdmap.top

[G02] 构造函数
来源：http://sfn.pycfn.com

Py:   def __init__(self, name): self.name = name
来源：http://yzq.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://jsk.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://ijx.shzxlz.cn

TS:   constructor(public name: string) {}
来源：http://nrb.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://lle.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uxx.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://jxf.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://gxm.jianghu66.top

[G03] 实例属性
来源：http://wbl.yvedp.cn

Py:   self.name = "x"
来源：http://yje.vqdsnc.cn

PHP:  public string $name = "x";
来源：http://wuo.iojbl.cn

JS:   this.name = "x";
来源：http://flh.haohaochexian.top

TS:   name: string = "x";
来源：http://ohx.cheryme.top

Java: private String name;
来源：http://fbr.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mct.sufxvd.cn

Ruby: @name = "x"
来源：http://pgw.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://wjt.aibaodan.cn

[G04] 定义方法
来源：http://xuj.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://vzc.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dor.smart0.xyz

JS:   greet() { return this.name; }
来源：http://fzs.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://ldk.sjlbkw.cn

Java: String greet() { return name; }
来源：http://ojw.xuetiantiany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xbv.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://nfx.yanxiufei.cn

C#:   public string Greet() => Name;
来源：http://zrk.shanyushiyangkeji.top

[G05] 继承
来源：http://jma.mhx1999.top

Py:   class Admin(User): pass
来源：http://caf.sysykeji.top

PHP:  class Admin extends User {}
来源：http://iuf.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://ttd.snrcjt.cn

TS:   class Admin extends User {}
来源：http://qzk.yj20258888.top

Java: class Admin extends User {}
来源：http://fjl.fzhhl.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qsl.zycfv.cn

Ruby: class Admin < User; end
来源：http://tlc.gzhubu.top

C#:   class Admin : User {}
来源：http://zlw.guowangkeji.top

[G06] 重写方法
来源：http://qne.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://zne.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kmh.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://uiy.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://myv.nwbrower.top

Java: @Override String greet() { return "admin"; }
来源：http://ale.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wid.yongpay.top

Ruby: def greet; "admin"; end
来源：http://uae.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://jhi.yvedp.cn

[G07] 调用父类方法
来源：http://wkf.smart0.xyz

Py:   super().greet()
来源：http://wnj.ehwqpu.com

PHP:  parent::greet();
来源：http://qta.yueranfly.top

JS:   super.greet();
来源：http://knw.hcnkem.com

TS:   super.greet();
来源：http://sdg.hnqzz.top

Java: super.greet();
来源：http://sld.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lid.9152youxi.cn

Ruby: super
来源：http://wwl.yonumen.top

C#:   base.Greet();
来源：http://hpz.ctjpmb.com

[G08] 静态方法与属性
来源：http://tie.cdnleiting.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bba.ydzc1.top

PHP:  public static function f() {}
来源：http://qsp.sxryk.cn

JS:   static f() {}
来源：http://yin.0kj1m.cn

TS:   static f(): void {}
来源：http://kym.guannengcc.top

Java: static void f() {}
来源：http://clm.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bje.yj20258888.top

Ruby: def self.f; end
来源：http://oat.hfpthk.cn

C#:   public static void F() {}
来源：http://srl.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://ikc.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://myc.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rur.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xac.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://vyb.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://glj.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://rqr.jinqigufen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fgt.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://gyt.xuetiantiany.cn

[G10] 访问控制
来源：http://hcs.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://uqr.52xcode.cn

PHP:  public / protected / private
来源：http://ydf.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://bkk.daxiang520.top

TS:   public / protected / private
来源：http://agf.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://iff.meibo888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qbk.sufxvd.cn

Ruby: public / protected / private
来源：http://ktq.iojbl.cn

C#:   public / protected / private / internal
来源：http://nsm.tarul.cn

[G11] getter / setter
来源：http://tpn.andypj.xyz

Py:   @property 与 @x.setter
来源：http://mdf.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lzq.chenjidiqi.icu

JS:   get name() { return this._name; }
来源：http://vmp.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://djg.vehdjk.com

Java: public String getName() { return name; }
来源：http://meq.chenlongwang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jhm.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://cdj.cheryme.top

C#:   public string Name { get; set; }
来源：http://edp.fengsongda.top

[G12] 对象转字符串
来源：http://miz.jqgfzy.top

Py:   def __str__(self): return self.name
来源：http://san.hesvh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ptt.dashuyun.cn

JS:   toString() { return this.name; }
来源：http://mdb.cdnleiting.top

TS:   toString(): string { return this.name; }
来源：http://ypx.sweek.top

Java: @Override public String toString() { return name; }
来源：http://hug.cdnleiting.top

Go:   func (u User) String() string { return u.Name }
来源：http://zyd.shanyushiyangkeji.top

Ruby: def to_s; @name; end
来源：http://vvv.uphjek.com

C#:   public override string ToString() => Name;
来源：http://sbc.birdmap.top

[G13] 判断对象类型
来源：http://kur.gzhubu.top

Py:   isinstance(u, User)
来源：http://qxz.bbcook.cn

PHP:  $u instanceof User
来源：http://wpl.yj20258888.top

JS:   u instanceof User
来源：http://oko.gzhubu.top

TS:   u instanceof User
来源：http://wzn.shanyushiyangtech.top

Java: u instanceof User
来源：http://ghv.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xse.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://ble.52xcode.cn

C#:   u is User
来源：http://zjj.xuanzx.com

[G14] 数据类 / record
来源：http://qlh.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lji.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://ojr.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://yjb.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://awk.xinyue.icu

Java: record User(String name, int age) {}
来源：http://vhb.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://boa.fktsv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xfj.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://gpt.sysykeji.top

[G15] 枚举
来源：http://piv.andypj.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mvd.shangyingyoupin.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xwj.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wpu.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://heu.yvedp.cn

Java: enum Color { RED, GREEN }
来源：http://xbm.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uqs.jinyuanbaomall.cn

Ruby: Color = %i[red green].freeze
来源：http://mub.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://usg.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://khi.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uiz.pycfn.com

PHP:  get_object_vars($obj);
来源：http://dte.ivvv.top

JS:   Object.entries(obj)
来源：http://kvp.c1oappe.top

TS:   Object.entries(obj)
来源：http://jcs.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kgl.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uoz.wangdashe.top

Ruby: obj.instance_variables
来源：http://vvq.yj202588.top

C#:   // 用反射或 System.Text.Json
来源：http://uif.hywenlv.cn

================================================================================
来源：http://awc.guannengcc.top


<!-- 参考信息 -->