代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qkr.vqdsnc.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xln.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://soa.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sxf.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pkj.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://qwh.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jdh.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://opv.shzxlz.cn

[E22] 字节长度与字符长度
来源：http://jhh.52xcode.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kve.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bzb.sysykeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xyp.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://efq.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qxk.pycfn.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sfi.chenlongwang.top

Ruby: s.bytesize;  s.length
来源：http://fer.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tvk.yj20258888.top

================================================================================
来源：http://bnc.fehbvm.com

F. 文件与目录
来源：http://ffu.chenzaomai.com

================================================================================
来源：http://zqt.nanxuanxn.top

[F01] 读取整个文件
来源：http://rtb.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://npy.fzhhl.top

PHP:  file_get_contents("a.txt");
来源：http://wgj.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://htp.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://efl.yanxiufei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uxx.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tur.52xcode.cn

Ruby: File.read("a.txt")
来源：http://jao.zhongyouzk.top

C#:   File.ReadAllText("a.txt");
来源：http://blq.jinqigfzy.top

[F02] 逐行读取文件
来源：http://kpy.gaohongyu789.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ylr.shuidangran.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ule.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zrr.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://spy.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gtf.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://luc.tarul.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://irf.daria6918.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dtp.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://rcu.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pvn.sysykeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://uka.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ktb.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kta.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://roh.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qun.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://wuk.cheryme.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jzp.bjfxy.top

[F04] 追加写入文件
来源：http://hng.jqgufenzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iic.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ora.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://row.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tpr.zhiwuduotai.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajr.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://avs.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://arr.redwolf501.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gaz.xuetiantiany.cn

[F05] 判断文件或目录是否存在
来源：http://vsc.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hkc.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://roc.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://hsf.zdbjq.cn

TS:   fs.existsSync("a.txt")
来源：http://gqf.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ptg.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hqt.redwolf501.top

Ruby: File.exist?("a.txt")
来源：http://uun.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://lzv.daxiang520.top

[F06] 删除文件
来源：http://xwr.hysaishi.cn

Py:   os.remove("a.txt")
来源：http://rds.nanxuanxn.top

PHP:  unlink("a.txt");
来源：http://wvl.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://llj.hammf.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oyg.cheryme.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ali.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://qpc.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://dlr.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://eyy.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://koc.jqgfzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uft.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oib.smart0.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kld.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zjp.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ngc.jyoumei.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rto.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hbi.xylfe.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qim.ydjk.org.cn

[F08] 遍历目录
来源：http://rpw.zycfv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yei.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://okz.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://rot.guannengcc.top

TS:   fs.readdirSync("dir")
来源：http://rut.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tgj.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ipv.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://vto.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://jtb.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://iaq.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://xin.52xcode.cn

PHP:  filesize("a.txt");
来源：http://lck.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://efg.cdnleiting.top

TS:   fs.statSync("a.txt").size
来源：http://pkb.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vbe.jinqigufen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qxm.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://yvy.jinyuanbaomall.cn

C#:   new FileInfo("a.txt").Length
来源：http://ztv.zycfv.cn

[F10] 取文件扩展名 / 文件名
来源：http://byl.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hfv.daria6918.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nfl.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nfz.hammf.cn

TS:   path.extname("a.txt")
来源：http://suy.yj202588.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mww.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oum.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wwm.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gnu.jqgfzy.top

[F11] 复制与移动文件
来源：http://tbv.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qel.zhoulong.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xrr.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zfe.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wsk.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jmo.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://usp.cashguo.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uei.316326.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oxa.sufxvd.cn

[F12] CSV 读写
来源：http://rbh.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tlk.zhiwuduotai.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://leq.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bzd.havefunace.top

TS:   // 同上
来源：http://ebz.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qyy.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cbo.vqdsnc.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://edu.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://aea.gzhubu.top

================================================================================
来源：http://hkc.zhengqikj.top

G. 面向对象
来源：http://wgy.wangdashe.top

================================================================================
来源：http://jtd.shanyushiyangtech.top

[G01] 定义类
来源：http://pbj.xylfe.cn

Py:   class User: pass
来源：http://hyg.tarul.cn

PHP:  class User {}
来源：http://pty.shuidangran.top

JS:   class User {}
来源：http://ccp.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://bcf.fanxiaobao.xyz

Java: class User {}
来源：http://row.xuetiantiany.cn

Go:   type User struct { Name string }
来源：http://caw.jqgfzy.top

Ruby: class User; end
来源：http://iri.wangdashe.top

C#:   class User {}
来源：http://ilh.zhengqikj.top

[G02] 构造函数
来源：http://uur.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://dtc.quarkkingdee.top

PHP:  public function __construct(public string $name) {}
来源：http://qau.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://rvh.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://vup.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://mny.hesvh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://chv.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://htv.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://yls.bbcook.cn

[G03] 实例属性
来源：http://nvr.wangdashe.top

Py:   self.name = "x"
来源：http://ink.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://qdf.hnxiangtu.top

JS:   this.name = "x";
来源：http://zmr.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://aua.pycfn.com

Java: private String name;
来源：http://etf.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vya.zycfv.cn

Ruby: @name = "x"
来源：http://fli.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://xti.tianlin.xyz

[G04] 定义方法
来源：http://hwk.sysykeji.top

Py:   def greet(self): return self.name
来源：http://hbw.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://uek.yj20258.top

JS:   greet() { return this.name; }
来源：http://oqv.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://lub.havefunace.top

Java: String greet() { return name; }
来源：http://ors.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://eyq.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://end.jianghu66.top

C#:   public string Greet() => Name;
来源：http://iaq.hnqzz.top

[G05] 继承
来源：http://xfc.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://bsr.daxiang520.top

PHP:  class Admin extends User {}
来源：http://bpz.sufxvd.cn

JS:   class Admin extends User {}
来源：http://thz.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://vae.jianghu66.top

Java: class Admin extends User {}
来源：http://jcr.yanxiufei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gtx.dashuyun.cn

Ruby: class Admin < User; end
来源：http://nzg.smart0.xyz

C#:   class Admin : User {}
来源：http://oil.chenzaomai.com

[G06] 重写方法
来源：http://eea.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://iti.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gmw.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://vfg.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://ejt.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://kxb.smart0.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jeo.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://fru.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://hhv.shanyushiyangtech.top

[G07] 调用父类方法
来源：http://tdp.chenjidiqi.icu

Py:   super().greet()
来源：http://isk.bjfxy.top

PHP:  parent::greet();
来源：http://mwt.xuanzx.com

JS:   super.greet();
来源：http://xrs.zhixingplan.top

TS:   super.greet();
来源：http://xfi.ywan-chungtsiang.top

Java: super.greet();
来源：http://sej.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yym.ctjpmb.com

Ruby: super
来源：http://xjb.ppjwa.cn

C#:   base.Greet();
来源：http://chj.fanxiaobao.xyz

[G08] 静态方法与属性
来源：http://znt.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hyt.daria6918.cn

PHP:  public static function f() {}
来源：http://kxf.yuanzhike.top

JS:   static f() {}
来源：http://gjh.nanxuanxn.top

TS:   static f(): void {}
来源：http://nmj.tarul.cn

Java: static void f() {}
来源：http://one.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://yos.zdqjudy.top

Ruby: def self.f; end
来源：http://ooc.hnxiangtu.top

C#:   public static void F() {}
来源：http://xof.jinqigufen.top

[G09] 接口 / 抽象类
来源：http://eig.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://mkl.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ktc.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://mhc.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://mem.yuxming.cn

Java: interface Shape { double area(); }
来源：http://apz.haohaochexian.top

Go:   type Shape interface { Area() float64 }
来源：http://lzu.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wnt.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://sug.kuanghao11.cn

[G10] 访问控制
来源：http://ejf.wangshuangyany.cn

Py:   约定 _protected / __private（不强制）
来源：http://swx.shzxlz.cn

PHP:  public / protected / private
来源：http://xbl.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://uvz.yonumen.top

TS:   public / protected / private
来源：http://jlu.fzhhl.top

Java: public / protected / private / 默认包级
来源：http://czs.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oml.jinyuanbaomall.cn

Ruby: public / protected / private
来源：http://gkh.xylfe.cn

C#:   public / protected / private / internal
来源：http://kor.hnxiangtu.top

[G11] getter / setter
来源：http://bfr.yj20258888.top

Py:   @property 与 @x.setter
来源：http://lep.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jpw.dashuyun.cn

JS:   get name() { return this._name; }
来源：http://lwu.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://wur.meibo888.top

Java: public String getName() { return name; }
来源：http://brb.daxiang520.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://tgk.wangshuangyany.cn

Ruby: attr_accessor :name
来源：http://saa.sysykeji.top

C#:   public string Name { get; set; }
来源：http://yfr.jqgufenzy.top

[G12] 对象转字符串
来源：http://jqr.daxiang520.top

Py:   def __str__(self): return self.name
来源：http://chf.yvedp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ftr.ybcxt.top

JS:   toString() { return this.name; }
来源：http://wbh.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://xds.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://qhv.nanxinkj.top

Go:   func (u User) String() string { return u.Name }
来源：http://eem.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://oox.zhengqikj.top

C#:   public override string ToString() => Name;
来源：http://nmw.feifeiyinyue.top

[G13] 判断对象类型
来源：http://ywc.sysykeji.top

Py:   isinstance(u, User)
来源：http://kro.yj20258888.top

PHP:  $u instanceof User
来源：http://znj.kuanghao11.cn

JS:   u instanceof User
来源：http://kwj.fehbvm.com

TS:   u instanceof User
来源：http://cmp.sufxvd.cn

Java: u instanceof User
来源：http://fme.sxryk.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qmp.hfpthk.cn

Ruby: u.is_a?(User)
来源：http://ccn.xylfe.cn

C#:   u is User
来源：http://shd.wangdashe.top

[G14] 数据类 / record
来源：http://hgg.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nva.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://vdy.yuanzhike.top

JS:   // 无内置：普通类或对象字面量
来源：http://thn.nwbrower.top

TS:   type User = { name: string; age: number };
来源：http://quo.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://box.aibaodan.cn

Go:   type User struct { Name string; Age int }
来源：http://kvc.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lvy.cheryme.top

C#:   record User(string Name, int Age);
来源：http://ciw.bbcook.cn

[G15] 枚举
来源：http://wat.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jbl.cashguo.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://unq.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zqg.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://svk.pengpengdd.cyou

Java: enum Color { RED, GREEN }
来源：http://zyd.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dnb.ywan-chungtsiang.top

Ruby: Color = %i[red green].freeze
来源：http://fyf.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tzv.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://eox.fehbvm.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oob.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://qvw.zhengqikj.top

JS:   Object.entries(obj)
来源：http://yqw.yangfankeji.com

TS:   Object.entries(obj)
来源：http://dqh.ydzc1.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wwl.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dda.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://oel.haohaochexian.top

C#:   // 用反射或 System.Text.Json
来源：http://zbd.ehwqpu.com

================================================================================
来源：http://lcw.jinghuilouyu.cn

H. 异常与错误处理
来源：http://ots.nwbrower.top

================================================================================
来源：http://gas.shuidangran.top

[H01] try / catch 基础
来源：http://kuy.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ddr.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pqo.fanxiaobao.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jnx.chenjidiqi.icu

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yfu.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tkm.shuidangran.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fkd.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lqe.iojbl.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vzr.redwolf501.top

[H02] finally / ensure 收尾
来源：http://hht.yvedp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iwx.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://twm.wangshuangyany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://twh.jyoumei.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ntu.zhijiandao.cn

Java: try { f(); } finally { cleanup(); }
来源：http://csb.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://opq.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://knz.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wuo.fktsv.cn

[H03] 主动抛出异常
来源：http://mdx.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://etu.cqqwz.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bnx.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://fmj.fzhhl.top


<!-- 参考信息 -->