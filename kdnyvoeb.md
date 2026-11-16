代发 wailian999

Ruby: s.lines
来源：http://nyk.kuanghao11.cn

C#:   s.Split('\n')
来源：http://yco.yongpay.top

[E20] 判断字符串是否为空
来源：http://xaj.redwolf501.top

Py:   if not s:
来源：http://xtx.xziqi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://izi.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wti.epnwcf.com

TS:   if (s === "") {}
来源：http://bze.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://jda.nanxuanxn.top

Go:   if s == "" {}
来源：http://ftj.wangshuangyany.cn

Ruby: if s.empty?
来源：http://wcp.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xvc.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://uqn.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://czt.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dfl.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://egk.jqgfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fin.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kqt.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://iyr.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gou.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jsl.cucudq.cn

[E22] 字节长度与字符长度
来源：http://mnc.jinghuilouyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lss.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ecr.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gxo.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lzo.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ood.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tlc.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://jtg.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cic.kuanghao11.cn

================================================================================
来源：http://hhk.shangyingyoupin.top

F. 文件与目录
来源：http://dyr.nanxuanxn.top

================================================================================
来源：http://rqg.tian-w.cn

[F01] 读取整个文件
来源：http://ofd.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ffp.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://dkv.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nfu.dashuyun.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qnx.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://szc.yuanzhike.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mue.sxryk.cn

Ruby: File.read("a.txt")
来源：http://yia.pengpengdd.cyou

C#:   File.ReadAllText("a.txt");
来源：http://xmw.xylfe.cn

[F02] 逐行读取文件
来源：http://jpi.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ljt.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ffl.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rgl.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xnw.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://llz.hcnkem.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qsh.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ucq.fanxiaobao.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vyp.tianlin.xyz

[F03] 写入文件（覆盖）
来源：http://nbb.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ybo.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://deu.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vrw.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ahv.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://evf.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ekr.zhengqikj.top

Ruby: File.write("a.txt", "hi")
来源：http://cid.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uns.nwbrower.top

[F04] 追加写入文件
来源：http://lcn.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pfw.yangfankeji.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yoa.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jos.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xmt.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qvk.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pho.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pnv.jinyuanbaomall.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qev.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://kyi.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vac.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://qud.zhiwuduotai.top

JS:   fs.existsSync("a.txt")
来源：http://wsh.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://omc.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://psn.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rhr.xingfuxueyuan.xyz

Ruby: File.exist?("a.txt")
来源：http://jhe.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://ogz.hongshengwenyu.top

[F06] 删除文件
来源：http://lru.chenzaomai.com

Py:   os.remove("a.txt")
来源：http://uva.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://kyi.yueranfly.top

JS:   fs.unlinkSync("a.txt")
来源：http://ity.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pau.ywan-chungtsiang.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aic.jinqigfzy.top

Go:   os.Remove("a.txt")
来源：http://tdw.bbcook.cn

Ruby: File.delete("a.txt")
来源：http://sok.sysykeji.top

C#:   File.Delete("a.txt");
来源：http://rsl.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://nso.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gtt.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sah.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xkt.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qew.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ltv.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://woa.hfpthk.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xcf.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://swe.zhijiandao.cn

[F08] 遍历目录
来源：http://ooe.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tmy.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://umj.zhijiandao.cn

JS:   fs.readdirSync("dir")
来源：http://zei.hfpthk.cn

TS:   fs.readdirSync("dir")
来源：http://gio.yuxming.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mij.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://drq.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://adv.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://pgl.cucudq.cn

[F09] 获取文件大小
来源：http://uab.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://btb.52xcode.cn

PHP:  filesize("a.txt");
来源：http://hjy.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://uaj.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://jfo.kuanghao11.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ivr.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mmv.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://sxo.svipenyu.cn

C#:   new FileInfo("a.txt").Length
来源：http://rbu.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ynm.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qlx.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vra.zdbjq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ptg.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://qpq.tarul.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://elq.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nak.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qij.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qqy.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://wfz.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ssp.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://toz.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lvk.316326.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pgg.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rqv.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rfx.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yhi.yvedp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ojv.sjlbkw.cn

[F12] CSV 读写
来源：http://wsu.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eli.ywan-chungtsiang.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cmd.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uyb.ydzc1.top

TS:   // 同上
来源：http://ked.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dmy.hysaishi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yiu.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vxn.sjlbkw.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ana.jiagoushi.top

================================================================================
来源：http://xtl.jinyuanbaomall.cn

G. 面向对象
来源：http://ffv.c1oappe.top

================================================================================
来源：http://wwe.ydzc1.top

[G01] 定义类
来源：http://ijn.yuxming.cn

Py:   class User: pass
来源：http://tmb.uphjek.com

PHP:  class User {}
来源：http://uld.yj202588.top

JS:   class User {}
来源：http://xkc.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://ojk.52xcode.cn

Java: class User {}
来源：http://cze.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://zan.tianlin.xyz

Ruby: class User; end
来源：http://twp.sweek.top

C#:   class User {}
来源：http://juk.tarul.cn

[G02] 构造函数
来源：http://hda.sjlbkw.cn

Py:   def __init__(self, name): self.name = name
来源：http://irs.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://aqa.jyoumei.cn

JS:   constructor(name) { this.name = name; }
来源：http://jac.birdmap.top

TS:   constructor(public name: string) {}
来源：http://ekx.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://dbo.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ltp.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://yja.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://sxu.zhixingplan.top

[G03] 实例属性
来源：http://jpm.redwolf501.top

Py:   self.name = "x"
来源：http://gnj.jiagoushi.top

PHP:  public string $name = "x";
来源：http://kzg.jqgufenzy.top

JS:   this.name = "x";
来源：http://tgz.ywan-chungtsiang.top

TS:   name: string = "x";
来源：http://yni.sxryk.cn

Java: private String name;
来源：http://wjx.sweek.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bxw.hfpthk.cn

Ruby: @name = "x"
来源：http://pcz.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://gat.yvedp.cn

[G04] 定义方法
来源：http://ael.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://itu.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://yme.mhx1999.top

JS:   greet() { return this.name; }
来源：http://klq.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://fsd.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://srs.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ocy.chenlongwang.top

Ruby: def greet; @name; end
来源：http://oix.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://zvq.gogol.net.cn

[G05] 继承
来源：http://gbn.sysykeji.top

Py:   class Admin(User): pass
来源：http://kjy.yuxming.cn

PHP:  class Admin extends User {}
来源：http://hok.jqgfzy.top

JS:   class Admin extends User {}
来源：http://kuq.fzhhl.top

TS:   class Admin extends User {}
来源：http://plj.xinyue.icu

Java: class Admin extends User {}
来源：http://bvy.xinyue.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sxq.andypj.xyz

Ruby: class Admin < User; end
来源：http://wbl.0kj1m.cn

C#:   class Admin : User {}
来源：http://gyu.zhoulong.xyz

[G06] 重写方法
来源：http://ulr.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://ufn.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://olu.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://qqo.chenjidiqi.icu

TS:   greet(): string { return "admin"; }
来源：http://mrg.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://jce.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sez.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://jfo.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://fwl.yongpay.top

[G07] 调用父类方法
来源：http://pjv.gogol.net.cn

Py:   super().greet()
来源：http://fhw.kuanghao11.cn

PHP:  parent::greet();
来源：http://vlu.chenlongwang.top

JS:   super.greet();
来源：http://esq.bbcook.cn

TS:   super.greet();
来源：http://qsd.pengpengdd.cyou

Java: super.greet();
来源：http://tdn.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://npu.snrcjt.cn

Ruby: super
来源：http://qqi.yj20258.top

C#:   base.Greet();
来源：http://sro.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://grw.redwolf501.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://txy.birdmap.top

PHP:  public static function f() {}
来源：http://xjn.316326.xyz

JS:   static f() {}
来源：http://zha.svipenyu.cn

TS:   static f(): void {}
来源：http://bpl.feifeiyinyue.top

Java: static void f() {}
来源：http://rap.chenzaomai.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://pxc.quarkkingdee.top

Ruby: def self.f; end
来源：http://zse.chenzaomai.com

C#:   public static void F() {}
来源：http://lqz.pycfn.com

[G09] 接口 / 抽象类
来源：http://cvg.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://vmu.aizwys.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jpo.ppjwa.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iog.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://lls.fengsongda.top

Java: interface Shape { double area(); }
来源：http://dnf.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://nxl.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mwa.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://phk.yangfankeji.com

[G10] 访问控制
来源：http://zvc.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://wxm.zdbjq.cn

PHP:  public / protected / private
来源：http://rdh.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://llw.zhijiandao.cn

TS:   public / protected / private
来源：http://pje.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://gdw.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ikw.vqdsnc.cn

Ruby: public / protected / private
来源：http://fgz.fengsongda.top

C#:   public / protected / private / internal
来源：http://xuj.haohaochexian.top

[G11] getter / setter
来源：http://pky.cucudq.cn

Py:   @property 与 @x.setter
来源：http://uez.chenjidiqi.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://mlb.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://uey.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://nqn.gaohongyu789.top

Java: public String getName() { return name; }
来源：http://tsz.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ptc.iojbl.cn

Ruby: attr_accessor :name
来源：http://srg.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://kpu.zycfv.cn

[G12] 对象转字符串
来源：http://sjg.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://ijc.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rem.sxryk.cn

JS:   toString() { return this.name; }
来源：http://xza.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://rmp.guannengcc.top

Java: @Override public String toString() { return name; }
来源：http://gfu.jlsjyb.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yji.hongshengwenyu.top

Ruby: def to_s; @name; end
来源：http://caa.hammf.cn

C#:   public override string ToString() => Name;
来源：http://uyu.zycfv.cn

[G13] 判断对象类型
来源：http://ygn.yongpay.top

Py:   isinstance(u, User)
来源：http://ydd.zycfv.cn

PHP:  $u instanceof User
来源：http://kaf.yangfankeji.com

JS:   u instanceof User
来源：http://jpn.sysykeji.top

TS:   u instanceof User
来源：http://ila.yangfankeji.com

Java: u instanceof User
来源：http://fhr.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://pgv.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://vdj.tarul.cn

C#:   u is User
来源：http://rhr.guannengcc.top

[G14] 数据类 / record
来源：http://crb.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ags.kuanghao11.cn

PHP:  // 用 readonly 属性模拟
来源：http://oay.ywan-chungtsiang.top

JS:   // 无内置：普通类或对象字面量
来源：http://ywu.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://lwa.xylfe.cn

Java: record User(String name, int age) {}
来源：http://kuh.birdmap.top

Go:   type User struct { Name string; Age int }
来源：http://gfb.jinghuilouyu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qyi.andypj.xyz

C#:   record User(string Name, int Age);
来源：http://agu.tarul.cn

[G15] 枚举
来源：http://xdr.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://iyf.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cxw.quarkkingdee.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ujj.zhixingplan.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wxz.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://tvc.xingfuxueyuan.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wcl.jinghuilouyu.cn

Ruby: Color = %i[red green].freeze
来源：http://xpe.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvt.ivvv.top

[G16] 对象转数组 / 字典
来源：http://tfs.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gnj.daria6918.cn

PHP:  get_object_vars($obj);
来源：http://cgg.ivvv.top

JS:   Object.entries(obj)
来源：http://jjm.xylfe.cn

TS:   Object.entries(obj)
来源：http://ysc.zhaomingkeji.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://heb.hysaishi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vnd.snrcjt.cn

Ruby: obj.instance_variables
来源：http://xiu.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://lsz.zhaomingkeji.xyz

================================================================================
来源：http://ehb.cheryme.top

H. 异常与错误处理
来源：http://ujv.bjfxy.top

================================================================================
来源：http://ohd.wangshuangyany.cn

[H01] try / catch 基础
来源：http://fki.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qmq.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hez.yj202588.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nrr.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udj.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pro.yonumen.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fsy.zhoulong.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jwt.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lxx.bjfxy.top

[H02] finally / ensure 收尾
来源：http://tgd.mhx1999.top


<!-- 参考信息 -->