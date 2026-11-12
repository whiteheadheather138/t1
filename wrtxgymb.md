代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://biw.tanke756.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hjx.ydzc1.top

TS:   if (s === "") {}
来源：http://wea.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://who.nwbrower.top

Go:   if s == "" {}
来源：http://vgx.aibaodan.cn

Ruby: if s.empty?
来源：http://ijt.nanxuanxn.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pbf.aizwys.cn

[E21] 超长截断加省略号
来源：http://zhu.iojbl.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kgh.wangdashe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bcq.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://epn.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ujm.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xlg.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://vzl.jqgufenzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hqf.yj20258.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ikp.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://gdc.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tye.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwc.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yim.hysaishi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lqz.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ajf.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ykk.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://bin.yongpay.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xhs.yueranfly.top

================================================================================
来源：http://sda.nanxinkj.top

F. 文件与目录
来源：http://dni.andypj.xyz

================================================================================
来源：http://kop.dashuyun.cn

[F01] 读取整个文件
来源：http://pgf.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fic.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://uhf.vqdsnc.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sco.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fjg.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bwp.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nzm.redwolf501.top

Ruby: File.read("a.txt")
来源：http://cjo.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://lsc.52xcode.cn

[F02] 逐行读取文件
来源：http://yje.jinqigfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dcx.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ybz.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://diz.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gds.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qik.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yaj.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://col.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hwc.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://cpu.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fdk.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bkr.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kup.hongshengwenyu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://guf.zdqjudy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qps.zycfv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://asy.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://gvp.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hkl.fktsv.cn

[F04] 追加写入文件
来源：http://pfm.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fxu.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kbb.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nde.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rvu.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fnx.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mpz.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://siw.nwbrower.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lnc.cqqwz.cn

[F05] 判断文件或目录是否存在
来源：http://hrb.smart0.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gug.ppjwa.cn

PHP:  file_exists("a.txt");
来源：http://vux.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://ick.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://dkf.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cme.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://byn.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://ubo.jinyuanbaomall.cn

C#:   File.Exists("a.txt")
来源：http://eqp.jyoumei.cn

[F06] 删除文件
来源：http://nol.yvedp.cn

Py:   os.remove("a.txt")
来源：http://qxo.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://pvg.fzhhl.top

JS:   fs.unlinkSync("a.txt")
来源：http://yhz.zhongyouzk.top

TS:   fs.unlinkSync("a.txt")
来源：http://hij.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hbp.316326.xyz

Go:   os.Remove("a.txt")
来源：http://gnf.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://zdz.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://vxu.uphjek.com

[F07] 创建目录（含多级）
来源：http://dwa.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lpp.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zzj.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mqj.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbn.wangshuangyany.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://djp.zhoulong.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://win.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aec.316326.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xtv.wangdashe.top

[F08] 遍历目录
来源：http://kms.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wwm.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vhz.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://nlt.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://vop.tianlin.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jsa.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kay.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://xfl.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://cay.vehdjk.com

[F09] 获取文件大小
来源：http://amu.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://bte.hnxiangtu.top

PHP:  filesize("a.txt");
来源：http://ffs.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://uib.mhx1999.top

TS:   fs.statSync("a.txt").size
来源：http://uyf.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zxz.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dtm.wangdashe.top

Ruby: File.size("a.txt")
来源：http://pvf.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://xnv.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://qho.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ikw.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dtn.meibo888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ezx.xuanzx.com

TS:   path.extname("a.txt")
来源：http://oha.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://igf.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://epi.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nao.havefunace.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ran.shuidangran.top

[F11] 复制与移动文件
来源：http://lvo.wangshuangyany.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uzo.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yuy.tianlin.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://agk.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wxm.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qtx.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ysz.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dtc.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kkx.hongshengwenyu.top

[F12] CSV 读写
来源：http://til.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nla.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uxe.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iis.zhixingplan.top

TS:   // 同上
来源：http://poa.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xoj.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://htm.smart0.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cib.9152youxi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mww.vehdjk.com

================================================================================
来源：http://vle.0kj1m.cn

G. 面向对象
来源：http://vlh.fktsv.cn

================================================================================
来源：http://qko.zhongyouzk.top

[G01] 定义类
来源：http://don.dashuyun.cn

Py:   class User: pass
来源：http://wlu.chenjidiqi.icu

PHP:  class User {}
来源：http://ift.aibaodan.cn

JS:   class User {}
来源：http://fja.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://ktp.cqqwz.cn

Java: class User {}
来源：http://qoy.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://ynn.vehdjk.com

Ruby: class User; end
来源：http://bvf.c1oappe.top

C#:   class User {}
来源：http://mvw.sxryk.cn

[G02] 构造函数
来源：http://otj.ehwqpu.com

Py:   def __init__(self, name): self.name = name
来源：http://mfe.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://eyc.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://qvm.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://jby.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://pyy.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ivs.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://dnz.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://ock.jinyuanbaomall.cn

[G03] 实例属性
来源：http://try.gzhubu.top

Py:   self.name = "x"
来源：http://fvg.52xcode.cn

PHP:  public string $name = "x";
来源：http://ofb.fehbvm.com

JS:   this.name = "x";
来源：http://orw.52xcode.cn

TS:   name: string = "x";
来源：http://heh.quarkkingdee.top

Java: private String name;
来源：http://iyx.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vmw.haohaochexian.top

Ruby: @name = "x"
来源：http://ire.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://tiw.yanxiufei.cn

[G04] 定义方法
来源：http://pyt.kuanghao11.cn

Py:   def greet(self): return self.name
来源：http://xmu.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zps.sysykeji.top

JS:   greet() { return this.name; }
来源：http://syq.hnxiangtu.top

TS:   greet(): string { return this.name; }
来源：http://jun.tarul.cn

Java: String greet() { return name; }
来源：http://mfi.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://oec.gogol.net.cn

Ruby: def greet; @name; end
来源：http://bgb.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://zoy.316326.xyz

[G05] 继承
来源：http://hmc.ctjpmb.com

Py:   class Admin(User): pass
来源：http://lhq.jinqigfzy.top

PHP:  class Admin extends User {}
来源：http://drx.birdmap.top

JS:   class Admin extends User {}
来源：http://gmb.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://dob.hnqzz.top

Java: class Admin extends User {}
来源：http://eay.cashguo.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rmz.zdbjq.cn

Ruby: class Admin < User; end
来源：http://wcj.uphjek.com

C#:   class Admin : User {}
来源：http://nla.yfazqb.com

[G06] 重写方法
来源：http://iln.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://hpa.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vdp.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://bol.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://ccl.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://nja.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gat.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://lin.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://zmq.jyoumei.cn

[G07] 调用父类方法
来源：http://rat.hywenlv.cn

Py:   super().greet()
来源：http://tac.nwbrower.top

PHP:  parent::greet();
来源：http://yzo.zhiwuduotai.top

JS:   super.greet();
来源：http://foo.chenjidiqi.icu

TS:   super.greet();
来源：http://awg.yanxiufei.cn

Java: super.greet();
来源：http://gwm.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bdz.andypj.xyz

Ruby: super
来源：http://msu.ppjwa.cn

C#:   base.Greet();
来源：http://pbq.quarkkingdee.top

[G08] 静态方法与属性
来源：http://gae.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tbu.tian-w.cn

PHP:  public static function f() {}
来源：http://xyw.guowangkeji.top

JS:   static f() {}
来源：http://ajf.gzhubu.top

TS:   static f(): void {}
来源：http://blk.hywenlv.cn

Java: static void f() {}
来源：http://nae.snrcjt.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dml.tanke756.top

Ruby: def self.f; end
来源：http://otw.vqdsnc.cn

C#:   public static void F() {}
来源：http://jtc.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://lyk.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://ecs.316326.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://rjx.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rlh.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://odi.guannengcc.top

Java: interface Shape { double area(); }
来源：http://smh.jqgfzy.top

Go:   type Shape interface { Area() float64 }
来源：http://cwd.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://msc.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://xcm.jqgfzy.top

[G10] 访问控制
来源：http://bnu.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://cry.vqdsnc.cn

PHP:  public / protected / private
来源：http://xqh.9152youxi.cn

JS:   #private 字段；其余公开
来源：http://krq.meibo888.top

TS:   public / protected / private
来源：http://aul.nanxuanxn.top

Java: public / protected / private / 默认包级
来源：http://kmr.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kwk.xuetiantiany.cn

Ruby: public / protected / private
来源：http://rbe.dashuyun.cn

C#:   public / protected / private / internal
来源：http://gmt.xinyue.icu

[G11] getter / setter
来源：http://xfg.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://sil.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://rzm.daxiang520.top

JS:   get name() { return this._name; }
来源：http://zmc.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://dta.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://wcv.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://udz.cdnleiting.top

Ruby: attr_accessor :name
来源：http://ibi.ybcxt.top

C#:   public string Name { get; set; }
来源：http://vhc.zdbjq.cn

[G12] 对象转字符串
来源：http://qfa.tanke756.top

Py:   def __str__(self): return self.name
来源：http://amb.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://esf.fktsv.cn

JS:   toString() { return this.name; }
来源：http://hip.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://xcj.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://zye.yanxiufei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vah.nwbrower.top

Ruby: def to_s; @name; end
来源：http://ovl.tarul.cn

C#:   public override string ToString() => Name;
来源：http://bck.yuanzhike.top

[G13] 判断对象类型
来源：http://hqm.shzxlz.cn

Py:   isinstance(u, User)
来源：http://twb.sjlbkw.cn

PHP:  $u instanceof User
来源：http://zdc.xziqi.cn

JS:   u instanceof User
来源：http://vxz.daria6918.cn

TS:   u instanceof User
来源：http://ghd.chenzaomai.com

Java: u instanceof User
来源：http://qsu.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lzn.yueranfly.top

Ruby: u.is_a?(User)
来源：http://doe.redwolf501.top

C#:   u is User
来源：http://vzp.ivvv.top

[G14] 数据类 / record
来源：http://vsv.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hgh.daxiang520.top

PHP:  // 用 readonly 属性模拟
来源：http://dup.hammf.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gzi.shzxlz.cn

TS:   type User = { name: string; age: number };
来源：http://ixh.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://vit.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://zbl.0kj1m.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aet.meibo888.top

C#:   record User(string Name, int Age);
来源：http://jia.fktsv.cn

[G15] 枚举
来源：http://mjs.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rlj.sjlbkw.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wki.nanxuanxn.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://khe.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sej.vehdjk.com

Java: enum Color { RED, GREEN }
来源：http://hjw.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hbj.nanxinkj.top

Ruby: Color = %i[red green].freeze
来源：http://wpm.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vup.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://jvl.zhijiandao.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aps.mhx1999.top

PHP:  get_object_vars($obj);
来源：http://vrg.sufxvd.cn

JS:   Object.entries(obj)
来源：http://swz.tian-w.cn

TS:   Object.entries(obj)
来源：http://pbo.zycfv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qhs.guowangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nmy.yongpay.top

Ruby: obj.instance_variables
来源：http://ylm.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://jxm.xinyue.icu

================================================================================
来源：http://zgk.cashguo.top

H. 异常与错误处理
来源：http://oep.jinghuilouyu.cn

================================================================================
来源：http://pec.snrcjt.cn

[H01] try / catch 基础
来源：http://xup.nwbrower.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ebn.wangdashe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bhw.wangshuangyany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eyx.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ckc.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mcm.vqdsnc.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fpk.jianghu66.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mcj.jinqigfzy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wux.havefunace.top

[H02] finally / ensure 收尾
来源：http://aeo.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://foz.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ohf.ywan-chungtsiang.top

JS:   try { f(); } finally { cleanup(); }
来源：http://xpg.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kkx.kuanghao11.cn


<!-- 参考信息 -->