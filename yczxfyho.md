代发 wailian999

Go:   if s == "" {}
来源：http://pzs.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://aqs.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gwu.yfazqb.com

[E21] 超长截断加省略号
来源：http://rsb.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqa.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qau.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymk.redwolf501.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dae.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xaf.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://iuc.xziqi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bqo.sxryk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rlt.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://xlo.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jcz.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tcu.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvl.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cbw.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vll.meibo888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uin.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://paj.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kgs.sufxvd.cn

================================================================================
来源：http://svz.yuanzhike.top

F. 文件与目录
来源：http://zfw.nanxinkj.top

================================================================================
来源：http://pxz.zhongyouzk.top

[F01] 读取整个文件
来源：http://bpc.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gjs.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://xmq.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fbz.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lep.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zys.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yfq.ydjk.org.cn

Ruby: File.read("a.txt")
来源：http://ugm.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://jpe.haohaochexian.top

[F02] 逐行读取文件
来源：http://mwr.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eio.tarul.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jtn.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://txi.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqn.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cbl.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bwy.fengsongda.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oxv.mhx1999.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://weq.chenjidiqi.icu

[F03] 写入文件（覆盖）
来源：http://tfi.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bgu.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ion.zhongyouzk.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wuf.cheryme.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pwt.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lio.xuetiantiany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wck.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://hdt.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vst.fehbvm.com

[F04] 追加写入文件
来源：http://mro.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fja.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qnc.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vkx.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://krx.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://eqz.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gyo.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rzk.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aeo.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://kig.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mdc.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://ixc.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://hvu.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://aef.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://kbb.xylfe.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dft.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://cqq.316326.xyz

C#:   File.Exists("a.txt")
来源：http://kyw.c1oappe.top

[F06] 删除文件
来源：http://xvy.316326.xyz

Py:   os.remove("a.txt")
来源：http://qmu.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://wuh.fehbvm.com

JS:   fs.unlinkSync("a.txt")
来源：http://efe.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://udf.ybcxt.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ylm.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://knc.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://ipd.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://ftx.ywan-chungtsiang.top

[F07] 创建目录（含多级）
来源：http://fdr.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://orm.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rcg.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gwc.haohaochexian.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qut.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qmg.dianchejie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yuo.pengpengdd.cyou

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jrl.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ljd.pengpengdd.cyou

[F08] 遍历目录
来源：http://guk.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fmc.jyoumei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pcv.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://sqn.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://udr.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://roa.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://jqb.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://dhv.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://itx.ctjpmb.com

[F09] 获取文件大小
来源：http://vtt.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://jni.dianchejie.cn

PHP:  filesize("a.txt");
来源：http://vwg.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://hll.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://ecl.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://ity.zhongyouzk.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fik.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://hzy.cheryme.top

C#:   new FileInfo("a.txt").Length
来源：http://umu.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://gyv.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sjm.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qix.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uol.cucudq.cn

TS:   path.extname("a.txt")
来源：http://pmx.cheryme.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ogq.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ipl.yuxming.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nzv.chenjidiqi.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ygv.redwolf501.top

[F11] 复制与移动文件
来源：http://rqw.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xlc.ivvv.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hdz.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kgr.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vsn.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vyt.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vqq.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wrp.xingfuxueyuan.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://agy.aibaodan.cn

[F12] CSV 读写
来源：http://zqv.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lre.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rzz.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://huj.vehdjk.com

TS:   // 同上
来源：http://wxf.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mcx.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mgt.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://obr.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dib.jiagoushi.top

================================================================================
来源：http://muu.tianlin.xyz

G. 面向对象
来源：http://ljp.nanxinkj.top

================================================================================
来源：http://otn.cheryme.top

[G01] 定义类
来源：http://zfe.epnwcf.com

Py:   class User: pass
来源：http://wgc.pycfn.com

PHP:  class User {}
来源：http://vzn.xingfuxueyuan.xyz

JS:   class User {}
来源：http://wlw.316326.xyz

TS:   class User { name: string = ""; }
来源：http://fsr.bjfxy.top

Java: class User {}
来源：http://mbh.cashguo.top

Go:   type User struct { Name string }
来源：http://hnu.chenzaomai.com

Ruby: class User; end
来源：http://koo.zycfv.cn

C#:   class User {}
来源：http://jlt.yj20258888.top

[G02] 构造函数
来源：http://ihm.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://xxa.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://pdb.cucudq.cn

JS:   constructor(name) { this.name = name; }
来源：http://dyr.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://dbu.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://sjh.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ddw.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://ytt.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://eeg.hnxiangtu.top

[G03] 实例属性
来源：http://wfj.tianlin.xyz

Py:   self.name = "x"
来源：http://hmz.andypj.xyz

PHP:  public string $name = "x";
来源：http://bnj.hongshengwenyu.top

JS:   this.name = "x";
来源：http://pin.shzxlz.cn

TS:   name: string = "x";
来源：http://zon.daria6918.cn

Java: private String name;
来源：http://qvt.bbcook.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oix.pengpengdd.cyou

Ruby: @name = "x"
来源：http://oej.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://cff.dashuyun.cn

[G04] 定义方法
来源：http://qwi.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://zrn.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uxd.zdqjudy.top

JS:   greet() { return this.name; }
来源：http://vat.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://sum.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://isi.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rhv.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://utk.zhiwuduotai.top

C#:   public string Greet() => Name;
来源：http://bzp.ydjk.org.cn

[G05] 继承
来源：http://ubb.yj20258.top

Py:   class Admin(User): pass
来源：http://ebx.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://qya.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://trv.fanxiaobao.xyz

TS:   class Admin extends User {}
来源：http://kfc.9152youxi.cn

Java: class Admin extends User {}
来源：http://xzl.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jpu.uphjek.com

Ruby: class Admin < User; end
来源：http://knp.shanyushiyangtech.top

C#:   class Admin : User {}
来源：http://odl.cashguo.top

[G06] 重写方法
来源：http://qgh.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://cgb.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pzn.316326.xyz

JS:   greet() { return "admin"; }
来源：http://nhn.zhaomingkeji.xyz

TS:   greet(): string { return "admin"; }
来源：http://kds.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://hfj.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dlz.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://hfo.daxiang520.top

C#:   public override string Greet() => "admin";
来源：http://bkl.cashguo.top

[G07] 调用父类方法
来源：http://jko.yuxming.cn

Py:   super().greet()
来源：http://rwf.pengpengdd.cyou

PHP:  parent::greet();
来源：http://chk.kuanghao11.cn

JS:   super.greet();
来源：http://bqw.chenjidiqi.icu

TS:   super.greet();
来源：http://ije.hnxiangtu.top

Java: super.greet();
来源：http://cus.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bce.aizwys.cn

Ruby: super
来源：http://udr.fzhhl.top

C#:   base.Greet();
来源：http://koo.wangdashe.top

[G08] 静态方法与属性
来源：http://ibk.gzhubu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fzn.cqqwz.cn

PHP:  public static function f() {}
来源：http://uln.hcnkem.com

JS:   static f() {}
来源：http://gyf.ydjk.org.cn

TS:   static f(): void {}
来源：http://njh.daxiang520.top

Java: static void f() {}
来源：http://cdc.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cus.fehbvm.com

Ruby: def self.f; end
来源：http://bjo.fehbvm.com

C#:   public static void F() {}
来源：http://rbs.pycfn.com

[G09] 接口 / 抽象类
来源：http://bnd.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://mla.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sek.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cxd.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://urx.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://qau.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://uwt.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eun.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://osa.uphjek.com

[G10] 访问控制
来源：http://tai.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://zew.bjfxy.top

PHP:  public / protected / private
来源：http://ozm.yj20258888.top

JS:   #private 字段；其余公开
来源：http://hsb.jqgufenzy.top

TS:   public / protected / private
来源：http://wsm.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://ckh.yonumen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cyc.yuanzhike.top

Ruby: public / protected / private
来源：http://vzf.dashuyun.cn

C#:   public / protected / private / internal
来源：http://pxt.shzxlz.cn

[G11] getter / setter
来源：http://ipn.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://ear.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gpp.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://kra.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://ggr.meibo888.top

Java: public String getName() { return name; }
来源：http://maa.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uqp.dianchejie.cn

Ruby: attr_accessor :name
来源：http://wxy.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://kvj.jiagoushi.top

[G12] 对象转字符串
来源：http://wok.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://nft.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qio.xziqi.cn

JS:   toString() { return this.name; }
来源：http://nnx.gotoacloud.top

TS:   toString(): string { return this.name; }
来源：http://yby.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://exa.ywan-chungtsiang.top

Go:   func (u User) String() string { return u.Name }
来源：http://frn.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://hzs.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://icq.daxiang520.top

[G13] 判断对象类型
来源：http://gzo.yuxming.cn

Py:   isinstance(u, User)
来源：http://xim.hywenlv.cn

PHP:  $u instanceof User
来源：http://itn.gaohongyu789.top

JS:   u instanceof User
来源：http://olh.yanxiufei.cn

TS:   u instanceof User
来源：http://eoz.fanxiaobao.xyz

Java: u instanceof User
来源：http://mci.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://axw.zhijiandao.cn

Ruby: u.is_a?(User)
来源：http://uka.cashguo.top

C#:   u is User
来源：http://qcl.yueranfly.top

[G14] 数据类 / record
来源：http://wcx.nwbrower.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sbv.dashuyun.cn

PHP:  // 用 readonly 属性模拟
来源：http://tlh.jinqigufen.top

JS:   // 无内置：普通类或对象字面量
来源：http://syf.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://qnw.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://cgk.aizwys.cn

Go:   type User struct { Name string; Age int }
来源：http://mjk.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yli.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://wmx.jinqigufen.top

[G15] 枚举
来源：http://tqn.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ytr.c1oappe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yoe.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lok.meibo888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hwk.daria6918.cn

Java: enum Color { RED, GREEN }
来源：http://npm.jianghu66.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zxs.ybcxt.top

Ruby: Color = %i[red green].freeze
来源：http://egl.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://msn.316326.xyz

[G16] 对象转数组 / 字典
来源：http://xop.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hyf.iojbl.cn

PHP:  get_object_vars($obj);
来源：http://syo.ybcxt.top

JS:   Object.entries(obj)
来源：http://qhv.cashguo.top

TS:   Object.entries(obj)
来源：http://jwf.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://onm.yueranfly.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yuv.shuidangran.top

Ruby: obj.instance_variables
来源：http://via.shuidangran.top

C#:   // 用反射或 System.Text.Json
来源：http://xaa.jinyuanbaomall.cn

================================================================================
来源：http://gdh.yuanzhike.top

H. 异常与错误处理
来源：http://zui.cheryme.top

================================================================================
来源：http://uss.yvedp.cn

[H01] try / catch 基础
来源：http://vfi.cqqwz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bxr.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kei.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pfv.fanxiaobao.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kih.shanyushiyangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dnk.sjlbkw.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://owp.hcnkem.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ioj.9152youxi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jzq.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://ikr.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zrf.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pfy.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rdz.xuanzx.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ixg.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kdv.316326.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jtd.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ohx.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zfm.jyoumei.cn


<!-- 参考信息 -->