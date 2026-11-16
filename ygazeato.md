代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yxx.feifeiyinyue.top

[E19] 多行文本按行拆分
来源：http://qhg.yvedp.cn

Py:   s.splitlines()
来源：http://mpq.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qeb.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://tvs.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://wsb.meibo888.top

Java: s.lines().toList()
来源：http://jfe.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://gbe.cqqwz.cn

Ruby: s.lines
来源：http://jcp.zdbjq.cn

C#:   s.Split('\n')
来源：http://ujw.andypj.xyz

[E20] 判断字符串是否为空
来源：http://cqd.andypj.xyz

Py:   if not s:
来源：http://onf.xuetiantiany.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aux.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aqa.smart0.xyz

TS:   if (s === "") {}
来源：http://vkk.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://xzk.dianchejie.cn

Go:   if s == "" {}
来源：http://hrm.zdbjq.cn

Ruby: if s.empty?
来源：http://ppd.yonumen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vkx.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://hhz.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://whd.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://toc.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gyk.52xcode.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrq.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vqg.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://jci.zhaomingkeji.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ejr.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iob.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://qig.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wys.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqg.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kwt.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ufq.nanxinkj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dwv.svipenyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://akf.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://apa.jiagoushi.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yeq.chenzaomai.com

================================================================================
来源：http://ucp.ybcxt.top

F. 文件与目录
来源：http://eew.zhengqikj.top

================================================================================
来源：http://izv.nanxinkj.top

[F01] 读取整个文件
来源：http://peh.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rik.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://qtt.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cnn.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hfx.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bkl.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://syc.smart0.xyz

Ruby: File.read("a.txt")
来源：http://xnu.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://skt.redwolf501.top

[F02] 逐行读取文件
来源：http://bnv.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ujd.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oge.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://thf.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://btf.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ikt.zhiwuduotai.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hhj.quarkkingdee.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vjl.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://psm.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://lzv.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pmv.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nig.snrcjt.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tgj.feifeiyinyue.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qiv.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wns.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yuj.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://nfj.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xbl.sjlbkw.cn

[F04] 追加写入文件
来源：http://jpe.xinyue.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tdx.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bpt.hnxiangtu.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bny.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://awg.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uhl.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ics.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oyv.dashuyun.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lor.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://kdr.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imx.hnqzz.top

PHP:  file_exists("a.txt");
来源：http://isj.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://xir.jinyuanbaomall.cn

TS:   fs.existsSync("a.txt")
来源：http://trt.jiagoushi.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ahd.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ujz.tian-w.cn

Ruby: File.exist?("a.txt")
来源：http://rgo.pycfn.com

C#:   File.Exists("a.txt")
来源：http://ylt.9152youxi.cn

[F06] 删除文件
来源：http://qal.daxiang520.top

Py:   os.remove("a.txt")
来源：http://atx.zycfv.cn

PHP:  unlink("a.txt");
来源：http://lmd.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://tkq.tianlin.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://qau.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lib.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://ros.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://evy.ivvv.top

C#:   File.Delete("a.txt");
来源：http://bft.vehdjk.com

[F07] 创建目录（含多级）
来源：http://rnc.fzhhl.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nbk.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://obv.yj20258888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mjz.shuidangran.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vuo.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ajl.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://boz.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://asn.nwbrower.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ltv.sjlbkw.cn

[F08] 遍历目录
来源：http://wey.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tbz.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://urn.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://txm.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://uvw.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ntp.sjlbkw.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kdb.tian-w.cn

Ruby: Dir.children("dir")
来源：http://lds.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://cdt.zhengqikj.top

[F09] 获取文件大小
来源：http://ubf.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://nmo.pycfn.com

PHP:  filesize("a.txt");
来源：http://vdz.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://rqe.havefunace.top

TS:   fs.statSync("a.txt").size
来源：http://pzb.sufxvd.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hwj.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ltg.fktsv.cn

Ruby: File.size("a.txt")
来源：http://all.hysaishi.cn

C#:   new FileInfo("a.txt").Length
来源：http://eii.daxiang520.top

[F10] 取文件扩展名 / 文件名
来源：http://irv.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fuy.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tkz.haohaochexian.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dwd.iojbl.cn

TS:   path.extname("a.txt")
来源：http://cyo.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://snq.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://phm.jqgfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zzw.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hfm.ydjk.org.cn

[F11] 复制与移动文件
来源：http://tvd.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qzl.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ryn.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qzi.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://feb.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nnf.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cen.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xxd.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ewx.52xcode.cn

[F12] CSV 读写
来源：http://dbw.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ubp.zhixingplan.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://aiu.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://myv.sufxvd.cn

TS:   // 同上
来源：http://hhg.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dqk.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tmr.gzhubu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://znw.redwolf501.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hti.cqqwz.cn

================================================================================
来源：http://pgs.shuidangran.top

G. 面向对象
来源：http://mtg.nanxinkj.top

================================================================================
来源：http://yfb.vqdsnc.cn

[G01] 定义类
来源：http://wzz.yj20258.top

Py:   class User: pass
来源：http://sxq.sjlbkw.cn

PHP:  class User {}
来源：http://wac.pycfn.com

JS:   class User {}
来源：http://ncq.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://sbd.kuanghao11.cn

Java: class User {}
来源：http://cnz.shuidangran.top

Go:   type User struct { Name string }
来源：http://ylx.nanxinkj.top

Ruby: class User; end
来源：http://zjg.epnwcf.com

C#:   class User {}
来源：http://heo.daxiang520.top

[G02] 构造函数
来源：http://oxa.316326.xyz

Py:   def __init__(self, name): self.name = name
来源：http://pxy.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://uzk.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://xjb.tanke756.top

TS:   constructor(public name: string) {}
来源：http://hqw.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://odp.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rrr.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://wkb.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://hzo.andypj.xyz

[G03] 实例属性
来源：http://lve.snrcjt.cn

Py:   self.name = "x"
来源：http://alx.yangfankeji.com

PHP:  public string $name = "x";
来源：http://tiw.gogol.net.cn

JS:   this.name = "x";
来源：http://smw.zhijiandao.cn

TS:   name: string = "x";
来源：http://mtb.sweek.top

Java: private String name;
来源：http://aax.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pon.xziqi.cn

Ruby: @name = "x"
来源：http://euf.feifeiyinyue.top

C#:   public string Name { get; set; } = "x";
来源：http://wtt.shangyingyoupin.top

[G04] 定义方法
来源：http://juq.wangdashe.top

Py:   def greet(self): return self.name
来源：http://zwn.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://iub.sjlbkw.cn

JS:   greet() { return this.name; }
来源：http://izj.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://vdy.pycfn.com

Java: String greet() { return name; }
来源：http://jsx.chenlongwang.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xbp.hcnkem.com

Ruby: def greet; @name; end
来源：http://fmv.dashuyun.cn

C#:   public string Greet() => Name;
来源：http://wbc.aibaodan.cn

[G05] 继承
来源：http://uzk.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://zza.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://xil.yj20258.top

JS:   class Admin extends User {}
来源：http://pnl.ydjk.org.cn

TS:   class Admin extends User {}
来源：http://tqp.iojbl.cn

Java: class Admin extends User {}
来源：http://rdv.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ehh.dashuyun.cn

Ruby: class Admin < User; end
来源：http://krv.jiagoushi.top

C#:   class Admin : User {}
来源：http://zpe.zhoulong.xyz

[G06] 重写方法
来源：http://gnh.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://wtz.hywenlv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pjg.zhoulong.xyz

JS:   greet() { return "admin"; }
来源：http://tlq.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://bzh.jqgufenzy.top

Java: @Override String greet() { return "admin"; }
来源：http://gks.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mou.hysaishi.cn

Ruby: def greet; "admin"; end
来源：http://pbj.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://xzb.yvedp.cn

[G07] 调用父类方法
来源：http://bha.zdbjq.cn

Py:   super().greet()
来源：http://vbd.chenlongwang.top

PHP:  parent::greet();
来源：http://qxd.snrcjt.cn

JS:   super.greet();
来源：http://maw.hammf.cn

TS:   super.greet();
来源：http://llc.gotoacloud.top

Java: super.greet();
来源：http://xwb.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://llf.52xcode.cn

Ruby: super
来源：http://sca.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://xem.yangfankeji.com

[G08] 静态方法与属性
来源：http://eit.hongshengwenyu.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lix.iojbl.cn

PHP:  public static function f() {}
来源：http://eac.epnwcf.com

JS:   static f() {}
来源：http://wgo.zycfv.cn

TS:   static f(): void {}
来源：http://knt.sxryk.cn

Java: static void f() {}
来源：http://bcr.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://djx.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://unx.ppjwa.cn

C#:   public static void F() {}
来源：http://pgn.sxryk.cn

[G09] 接口 / 抽象类
来源：http://qiy.fzhhl.top

Py:   from abc import ABC, abstractmethod
来源：http://hkq.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://myv.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jdv.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://ysx.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://crd.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://wep.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mrc.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://tvd.vehdjk.com

[G10] 访问控制
来源：http://yqo.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://vzs.cheryme.top

PHP:  public / protected / private
来源：http://bcy.fanxiaobao.xyz

JS:   #private 字段；其余公开
来源：http://dhl.jqgfzy.top

TS:   public / protected / private
来源：http://wgb.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://nto.316326.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://fau.ctjpmb.com

Ruby: public / protected / private
来源：http://fhl.epnwcf.com

C#:   public / protected / private / internal
来源：http://psm.0kj1m.cn

[G11] getter / setter
来源：http://bcn.tarul.cn

Py:   @property 与 @x.setter
来源：http://uhx.zhixingplan.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hpr.yj20258.top

JS:   get name() { return this._name; }
来源：http://vqr.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://yup.iojbl.cn

Java: public String getName() { return name; }
来源：http://epv.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vwa.vehdjk.com

Ruby: attr_accessor :name
来源：http://wcg.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://tlt.ehwqpu.com

[G12] 对象转字符串
来源：http://yap.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://bsc.wangdashe.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tet.ivvv.top

JS:   toString() { return this.name; }
来源：http://oxh.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://btk.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://cek.tian-w.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dyf.yj20258888.top

Ruby: def to_s; @name; end
来源：http://kkp.zhaomingkeji.xyz

C#:   public override string ToString() => Name;
来源：http://ofp.cucudq.cn

[G13] 判断对象类型
来源：http://ekf.chenzaomai.com

Py:   isinstance(u, User)
来源：http://flf.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://axr.ppjwa.cn

JS:   u instanceof User
来源：http://isg.xylfe.cn

TS:   u instanceof User
来源：http://rip.shanyushiyangtech.top

Java: u instanceof User
来源：http://vty.jinyuanbaomall.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zsj.hnxiangtu.top

Ruby: u.is_a?(User)
来源：http://wyt.jyoumei.cn

C#:   u is User
来源：http://zau.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://rva.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vxf.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://hww.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://dpo.gotoacloud.top

TS:   type User = { name: string; age: number };
来源：http://lre.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://yls.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://gbw.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gzh.ppjwa.cn

C#:   record User(string Name, int Age);
来源：http://xgm.fengsongda.top

[G15] 枚举
来源：http://xln.sufxvd.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://seq.ywan-chungtsiang.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ogk.xylfe.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xhk.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hgf.jqgufenzy.top

Java: enum Color { RED, GREEN }
来源：http://grw.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ejt.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://asi.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uab.yj202588.top

[G16] 对象转数组 / 字典
来源：http://gns.gogol.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iwk.jinqigufen.top

PHP:  get_object_vars($obj);
来源：http://jwg.yonumen.top

JS:   Object.entries(obj)
来源：http://vqa.hesvh.cn

TS:   Object.entries(obj)
来源：http://bza.daxiang520.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://igz.zhengqikj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://vwa.redwolf501.top

Ruby: obj.instance_variables
来源：http://bta.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://mjl.meibo888.top

================================================================================
来源：http://zih.bjfxy.top

H. 异常与错误处理
来源：http://bou.haohaochexian.top

================================================================================
来源：http://jck.ctjpmb.com

[H01] try / catch 基础
来源：http://foz.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zzz.cqqwz.cn


<!-- 参考信息 -->