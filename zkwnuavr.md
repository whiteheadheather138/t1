代发 wailian999

Go:   if s == "" {}
来源：http://ppt.aibaodan.cn

Ruby: if s.empty?
来源：http://bck.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://htn.yangfankeji.com

[E21] 超长截断加省略号
来源：http://yrr.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ieo.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yxw.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxw.tian-w.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xqa.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gvl.meibo888.top

Go:   // 按 rune 判断长度后截断
来源：http://jme.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dvr.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vuc.yvedp.cn

[E22] 字节长度与字符长度
来源：http://pyi.hnqzz.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mcw.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytj.dianchejie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://afg.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://exz.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://njr.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pml.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://ifc.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://urw.xziqi.cn

================================================================================
来源：http://ojy.xuetiantiany.cn

F. 文件与目录
来源：http://bgm.sweek.top

================================================================================
来源：http://kwh.shuidangran.top

[F01] 读取整个文件
来源：http://jyy.epnwcf.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iij.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://txe.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eei.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ffo.aibaodan.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://uli.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rhj.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://kbr.mhx1999.top

C#:   File.ReadAllText("a.txt");
来源：http://bpl.ivvv.top

[F02] 逐行读取文件
来源：http://wbw.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nqz.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://scg.wangshuangyany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qev.zdqjudy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qhf.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xcp.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mrr.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fgj.iojbl.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rpu.cashguo.top

[F03] 写入文件（覆盖）
来源：http://gsp.zdbjq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nma.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nli.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fap.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qpm.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://owg.zhoulong.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uqi.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://gsd.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bnb.wangshuangyany.cn

[F04] 追加写入文件
来源：http://bhk.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mwf.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yuk.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rlp.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvw.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://amv.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xde.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vcn.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gyg.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://ltj.quarkkingdee.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://doq.shanyushiyangkeji.top

PHP:  file_exists("a.txt");
来源：http://reo.hesvh.cn

JS:   fs.existsSync("a.txt")
来源：http://ykn.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://qdp.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jih.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oai.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://uiw.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://glw.yj202588.top

[F06] 删除文件
来源：http://pnh.aizwys.cn

Py:   os.remove("a.txt")
来源：http://urf.vehdjk.com

PHP:  unlink("a.txt");
来源：http://rqd.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://jvw.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://yqd.aibaodan.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nnh.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://abp.yongpay.top

Ruby: File.delete("a.txt")
来源：http://yxo.c1oappe.top

C#:   File.Delete("a.txt");
来源：http://eqk.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://bex.jinghuilouyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bxd.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://veq.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cbj.nanxinkj.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dae.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://omi.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mhu.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iaq.xziqi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jqt.aibaodan.cn

[F08] 遍历目录
来源：http://jae.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lzf.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iph.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://xsh.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://bfj.yfazqb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dqt.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mgf.svipenyu.cn

Ruby: Dir.children("dir")
来源：http://fnw.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://jea.birdmap.top

[F09] 获取文件大小
来源：http://tct.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://nev.sxryk.cn

PHP:  filesize("a.txt");
来源：http://map.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://ppc.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://owp.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hyy.hesvh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qpm.tanke756.top

Ruby: File.size("a.txt")
来源：http://tiw.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://yrc.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://pyp.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://osv.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hme.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://elo.yueranfly.top

TS:   path.extname("a.txt")
来源：http://guw.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bqg.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://clz.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qsj.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aca.zhijiandao.cn

[F11] 复制与移动文件
来源：http://rdb.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nwk.havefunace.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cqt.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvh.hnxiangtu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jew.jqgfzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yna.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://evf.yuxming.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ubx.guowangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jmh.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://hex.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://egm.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ejw.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nhg.yj20258888.top

TS:   // 同上
来源：http://jwz.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://czl.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xlj.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oak.vqdsnc.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gay.daria6918.cn

================================================================================
来源：http://wsx.xingfuxueyuan.xyz

G. 面向对象
来源：http://tkt.hnqzz.top

================================================================================
来源：http://vqe.sufxvd.cn

[G01] 定义类
来源：http://rvr.snrcjt.cn

Py:   class User: pass
来源：http://wah.kuanghao11.cn

PHP:  class User {}
来源：http://wtf.guannengcc.top

JS:   class User {}
来源：http://gzv.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://jxn.birdmap.top

Java: class User {}
来源：http://osz.sxryk.cn

Go:   type User struct { Name string }
来源：http://guv.hongshengwenyu.top

Ruby: class User; end
来源：http://trv.gaohongyu789.top

C#:   class User {}
来源：http://cpt.daria6918.cn

[G02] 构造函数
来源：http://vfd.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://mdb.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://gwk.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://bmu.cheryme.top

TS:   constructor(public name: string) {}
来源：http://lky.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://pgb.meibo888.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gum.xingfuxueyuan.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ukb.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://adp.ctjpmb.com

[G03] 实例属性
来源：http://mvy.nanxinkj.top

Py:   self.name = "x"
来源：http://ocj.xinyue.icu

PHP:  public string $name = "x";
来源：http://ipd.redwolf501.top

JS:   this.name = "x";
来源：http://idv.hcnkem.com

TS:   name: string = "x";
来源：http://hmh.hysaishi.cn

Java: private String name;
来源：http://lwx.xinyue.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://awf.guannengcc.top

Ruby: @name = "x"
来源：http://pih.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://tgb.meibo888.top

[G04] 定义方法
来源：http://xtm.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://tup.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fyn.yueranfly.top

JS:   greet() { return this.name; }
来源：http://lnl.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://pci.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://ebm.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dss.dashuyun.cn

Ruby: def greet; @name; end
来源：http://cew.aizwys.cn

C#:   public string Greet() => Name;
来源：http://lsf.xylfe.cn

[G05] 继承
来源：http://vrb.fktsv.cn

Py:   class Admin(User): pass
来源：http://zyc.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://ceh.dashuyun.cn

JS:   class Admin extends User {}
来源：http://rda.zhixingplan.top

TS:   class Admin extends User {}
来源：http://cxo.sxryk.cn

Java: class Admin extends User {}
来源：http://tdf.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://egf.9152youxi.cn

Ruby: class Admin < User; end
来源：http://dbi.ywan-chungtsiang.top

C#:   class Admin : User {}
来源：http://lge.fanxiaobao.xyz

[G06] 重写方法
来源：http://btc.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://hbv.yuxming.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qxg.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://cjq.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://fjp.meibo888.top

Java: @Override String greet() { return "admin"; }
来源：http://ulx.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xql.yj20258888.top

Ruby: def greet; "admin"; end
来源：http://ecc.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://rjn.yanxiufei.cn

[G07] 调用父类方法
来源：http://jtc.yj20258888.top

Py:   super().greet()
来源：http://req.snrcjt.cn

PHP:  parent::greet();
来源：http://hxl.yongpay.top

JS:   super.greet();
来源：http://obw.jinqigfzy.top

TS:   super.greet();
来源：http://ioj.hywenlv.cn

Java: super.greet();
来源：http://tar.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vdc.hesvh.cn

Ruby: super
来源：http://gkt.nwbrower.top

C#:   base.Greet();
来源：http://yhi.ydjk.org.cn

[G08] 静态方法与属性
来源：http://gvm.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yxy.ctjpmb.com

PHP:  public static function f() {}
来源：http://rkv.cucudq.cn

JS:   static f() {}
来源：http://bti.52xcode.cn

TS:   static f(): void {}
来源：http://rrs.jinqigfzy.top

Java: static void f() {}
来源：http://cem.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://uzn.yueranfly.top

Ruby: def self.f; end
来源：http://rxn.shuidangran.top

C#:   public static void F() {}
来源：http://eym.hesvh.cn

[G09] 接口 / 抽象类
来源：http://tgq.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://xqb.zhaomingkeji.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://qon.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gva.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://mgi.yangfankeji.com

Java: interface Shape { double area(); }
来源：http://dfw.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://law.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fhg.wangshuangyany.cn

C#:   interface IShape { double Area(); }
来源：http://amk.xuanzx.com

[G10] 访问控制
来源：http://prr.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://qhi.yvedp.cn

PHP:  public / protected / private
来源：http://ysf.hammf.cn

JS:   #private 字段；其余公开
来源：http://kuh.aizwys.cn

TS:   public / protected / private
来源：http://kex.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://ssp.shzxlz.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wgz.redwolf501.top

Ruby: public / protected / private
来源：http://quo.ywan-chungtsiang.top

C#:   public / protected / private / internal
来源：http://tjc.havefunace.top

[G11] getter / setter
来源：http://vye.fktsv.cn

Py:   @property 与 @x.setter
来源：http://ifi.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ytf.fengsongda.top

JS:   get name() { return this._name; }
来源：http://cun.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://gvy.kuanghao11.cn

Java: public String getName() { return name; }
来源：http://eew.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zvc.andypj.xyz

Ruby: attr_accessor :name
来源：http://pjv.cheryme.top

C#:   public string Name { get; set; }
来源：http://vnk.c1oappe.top

[G12] 对象转字符串
来源：http://saa.zycfv.cn

Py:   def __str__(self): return self.name
来源：http://xtf.redwolf501.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jcx.xylfe.cn

JS:   toString() { return this.name; }
来源：http://mzb.fanxiaobao.xyz

TS:   toString(): string { return this.name; }
来源：http://cjl.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://uxw.svipenyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://msh.yvedp.cn

Ruby: def to_s; @name; end
来源：http://cbh.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://olz.cdnleiting.top

[G13] 判断对象类型
来源：http://nmh.yuxming.cn

Py:   isinstance(u, User)
来源：http://dyu.jlsjyb.cn

PHP:  $u instanceof User
来源：http://hqc.ivvv.top

JS:   u instanceof User
来源：http://tfd.xuetiantiany.cn

TS:   u instanceof User
来源：http://jyr.sysykeji.top

Java: u instanceof User
来源：http://rhz.zhiwuduotai.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eeq.xinyue.icu

Ruby: u.is_a?(User)
来源：http://xcl.dashuyun.cn

C#:   u is User
来源：http://uxr.nwbrower.top

[G14] 数据类 / record
来源：http://azs.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qnt.havefunace.top

PHP:  // 用 readonly 属性模拟
来源：http://yqa.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://mlq.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://loj.hnqzz.top

Java: record User(String name, int age) {}
来源：http://lum.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://goc.hnxiangtu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vxr.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://ceq.yj20258.top

[G15] 枚举
来源：http://pqj.jiagoushi.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yky.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mfk.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mlt.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sxr.ppjwa.cn

Java: enum Color { RED, GREEN }
来源：http://ten.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xgg.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://iwt.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eyd.shzxlz.cn

[G16] 对象转数组 / 字典
来源：http://lcq.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fwr.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://pwo.daxiang520.top

JS:   Object.entries(obj)
来源：http://cfe.daria6918.cn

TS:   Object.entries(obj)
来源：http://ibs.yueranfly.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ouc.zhongyouzk.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wxq.haohaochexian.top

Ruby: obj.instance_variables
来源：http://lxh.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://jrm.daxiang520.top

================================================================================
来源：http://cwv.aibaodan.cn

H. 异常与错误处理
来源：http://dnz.zhoulong.xyz

================================================================================
来源：http://abh.hnxiangtu.top

[H01] try / catch 基础
来源：http://zyj.fktsv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ujt.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nkt.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pzm.redwolf501.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ytv.fzhhl.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pyv.jqgfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dke.dianchejie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hky.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gvq.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://ewi.shanyushiyangkeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://hib.guannengcc.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ehj.uphjek.com

JS:   try { f(); } finally { cleanup(); }
来源：http://sgx.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://srj.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bck.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ffg.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://tqk.yanxiufei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wbm.xinyue.icu


<!-- 参考信息 -->