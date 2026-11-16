代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://mwp.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://hnn.xuanzx.com

Java: s.lines().toList()
来源：http://sxe.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://fuj.fktsv.cn

Ruby: s.lines
来源：http://xyl.iojbl.cn

C#:   s.Split('\n')
来源：http://pvj.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://kqi.jqgufenzy.top

Py:   if not s:
来源：http://gdu.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bxc.nanxinkj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://igh.cucudq.cn

TS:   if (s === "") {}
来源：http://bwe.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://wuh.316326.xyz

Go:   if s == "" {}
来源：http://yjy.snrcjt.cn

Ruby: if s.empty?
来源：http://mwd.sysykeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mvo.0kj1m.cn

[E21] 超长截断加省略号
来源：http://ybz.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fyt.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zxa.sufxvd.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ggq.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xnk.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://snd.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://dou.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eci.shangyingyoupin.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ukj.hammf.cn

[E22] 字节长度与字符长度
来源：http://iwb.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gse.zhixingplan.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gbf.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cbz.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://stx.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rfg.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zei.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://jnt.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yoj.zhijiandao.cn

================================================================================
来源：http://huk.gzhubu.top

F. 文件与目录
来源：http://jqb.shangyingyoupin.top

================================================================================
来源：http://qos.ctjpmb.com

[F01] 读取整个文件
来源：http://jzn.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xol.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://mhi.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://orb.fzhhl.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://czi.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qaa.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ouy.yvedp.cn

Ruby: File.read("a.txt")
来源：http://jkr.tianlin.xyz

C#:   File.ReadAllText("a.txt");
来源：http://phb.fktsv.cn

[F02] 逐行读取文件
来源：http://hxp.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xdk.shanyushiyangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hei.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://glg.yfazqb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ctt.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kbn.bjfxy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zue.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://url.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vtd.havefunace.top

[F03] 写入文件（覆盖）
来源：http://vie.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dxf.zycfv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://swu.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vnb.wangshuangyany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbq.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wdm.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hbf.nwbrower.top

Ruby: File.write("a.txt", "hi")
来源：http://ukp.yj202588.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xtr.chenzaomai.com

[F04] 追加写入文件
来源：http://xhn.pengpengdd.cyou

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qct.0kj1m.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://btb.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdl.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dya.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rsb.vehdjk.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://enu.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fam.zhiwuduotai.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gya.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://cmg.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yha.vqdsnc.cn

PHP:  file_exists("a.txt");
来源：http://lsn.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://mrq.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://rmc.yongpay.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zyg.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://woh.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://aoz.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://ief.cashguo.top

[F06] 删除文件
来源：http://bra.tanke756.top

Py:   os.remove("a.txt")
来源：http://gmw.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://bzo.dashuyun.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ncf.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://gwn.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tlg.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://dii.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://ovq.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://wjf.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://yhl.jinyuanbaomall.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qwx.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pzp.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xwf.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yxb.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nha.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kes.tarul.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wtu.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uxs.ydzc1.top

[F08] 遍历目录
来源：http://uga.vehdjk.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://mxm.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://glc.guowangkeji.top

JS:   fs.readdirSync("dir")
来源：http://xku.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://ayx.nanxuanxn.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qtg.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kba.c1oappe.top

Ruby: Dir.children("dir")
来源：http://sxq.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://vgj.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://imd.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://cot.316326.xyz

PHP:  filesize("a.txt");
来源：http://gqr.feifeiyinyue.top

JS:   fs.statSync("a.txt").size
来源：http://uio.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://yom.yanxiufei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://erw.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://djk.epnwcf.com

Ruby: File.size("a.txt")
来源：http://dkm.zhiwuduotai.top

C#:   new FileInfo("a.txt").Length
来源：http://pmb.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://tlu.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ala.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xcy.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sdb.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://vcm.ydzc1.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tfh.sufxvd.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hfe.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jsw.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mbs.ppjwa.cn

[F11] 复制与移动文件
来源：http://avh.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yhe.shangyingyoupin.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ozo.yj20258.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tjm.zhoulong.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://umc.cashguo.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nfa.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fet.yongpay.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fhd.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jzu.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://vwz.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aih.cheryme.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rrq.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gyx.jiagoushi.top

TS:   // 同上
来源：http://rkm.dianchejie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lyy.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vtp.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://upn.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://taj.shzxlz.cn

================================================================================
来源：http://tku.yueranfly.top

G. 面向对象
来源：http://yzh.52xcode.cn

================================================================================
来源：http://ydo.bjfxy.top

[G01] 定义类
来源：http://gcr.shuidangran.top

Py:   class User: pass
来源：http://wsc.yj20258.top

PHP:  class User {}
来源：http://zcb.cucudq.cn

JS:   class User {}
来源：http://jzm.ywan-chungtsiang.top

TS:   class User { name: string = ""; }
来源：http://nmq.vqdsnc.cn

Java: class User {}
来源：http://bfc.ywan-chungtsiang.top

Go:   type User struct { Name string }
来源：http://gdo.wangshuangyany.cn

Ruby: class User; end
来源：http://tfh.nanxinkj.top

C#:   class User {}
来源：http://uxg.cucudq.cn

[G02] 构造函数
来源：http://vwe.yuxming.cn

Py:   def __init__(self, name): self.name = name
来源：http://pow.svipenyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://jhb.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://daf.jinghuilouyu.cn

TS:   constructor(public name: string) {}
来源：http://xws.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://yhe.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qis.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://glr.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://eac.hcnkem.com

[G03] 实例属性
来源：http://lto.chenjidiqi.icu

Py:   self.name = "x"
来源：http://qos.yuanzhike.top

PHP:  public string $name = "x";
来源：http://jre.epnwcf.com

JS:   this.name = "x";
来源：http://uwz.tianlin.xyz

TS:   name: string = "x";
来源：http://hiw.birdmap.top

Java: private String name;
来源：http://wxd.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xhh.feifeiyinyue.top

Ruby: @name = "x"
来源：http://lbz.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://ymy.pengpengdd.cyou

[G04] 定义方法
来源：http://adl.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://xge.ydjk.org.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kut.meibo888.top

JS:   greet() { return this.name; }
来源：http://gnr.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://gdy.tianlin.xyz

Java: String greet() { return name; }
来源：http://ded.cqqwz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lms.bjfxy.top

Ruby: def greet; @name; end
来源：http://hxc.daxiang520.top

C#:   public string Greet() => Name;
来源：http://ajn.gogol.net.cn

[G05] 继承
来源：http://gjf.chenlongwang.top

Py:   class Admin(User): pass
来源：http://gls.fanxiaobao.xyz

PHP:  class Admin extends User {}
来源：http://xbr.fanxiaobao.xyz

JS:   class Admin extends User {}
来源：http://xlv.xuanzx.com

TS:   class Admin extends User {}
来源：http://wxz.smart0.xyz

Java: class Admin extends User {}
来源：http://etz.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uhh.meibo888.top

Ruby: class Admin < User; end
来源：http://hrn.gzhubu.top

C#:   class Admin : User {}
来源：http://gik.gzhubu.top

[G06] 重写方法
来源：http://mxt.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://bwv.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kek.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://qtr.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://nqo.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://rnn.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ofa.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://qte.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://uwu.tarul.cn

[G07] 调用父类方法
来源：http://vdh.sufxvd.cn

Py:   super().greet()
来源：http://hym.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://pvd.hesvh.cn

JS:   super.greet();
来源：http://kar.sjlbkw.cn

TS:   super.greet();
来源：http://hgu.ivvv.top

Java: super.greet();
来源：http://qbr.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ksm.9152youxi.cn

Ruby: super
来源：http://dcu.shanyushiyangtech.top

C#:   base.Greet();
来源：http://jsa.hnxiangtu.top

[G08] 静态方法与属性
来源：http://ros.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yyy.chenzaomai.com

PHP:  public static function f() {}
来源：http://cjx.yj202588.top

JS:   static f() {}
来源：http://aay.havefunace.top

TS:   static f(): void {}
来源：http://gnm.sysykeji.top

Java: static void f() {}
来源：http://gdv.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pyh.yueranfly.top

Ruby: def self.f; end
来源：http://yfg.bjfxy.top

C#:   public static void F() {}
来源：http://cus.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://zlx.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://oqb.yanxiufei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dgv.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tzd.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://kuo.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://cxe.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://pma.daria6918.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://klj.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://vbe.jiagoushi.top

[G10] 访问控制
来源：http://uca.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://qtr.bjfxy.top

PHP:  public / protected / private
来源：http://kvf.uphjek.com

JS:   #private 字段；其余公开
来源：http://fkv.52xcode.cn

TS:   public / protected / private
来源：http://uvm.shanyushiyangkeji.top

Java: public / protected / private / 默认包级
来源：http://szt.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://azm.fktsv.cn

Ruby: public / protected / private
来源：http://cry.jinqigufen.top

C#:   public / protected / private / internal
来源：http://ehs.shanyushiyangkeji.top

[G11] getter / setter
来源：http://ryd.uphjek.com

Py:   @property 与 @x.setter
来源：http://sme.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jim.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://gkk.zhixingplan.top

TS:   get name(): string { return this._name; }
来源：http://ykf.cashguo.top

Java: public String getName() { return name; }
来源：http://lss.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://gng.iojbl.cn

Ruby: attr_accessor :name
来源：http://pdm.guannengcc.top

C#:   public string Name { get; set; }
来源：http://rxa.jqgufenzy.top

[G12] 对象转字符串
来源：http://gsb.gogol.net.cn

Py:   def __str__(self): return self.name
来源：http://xmm.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://onk.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://xld.ydjk.org.cn

TS:   toString(): string { return this.name; }
来源：http://vgs.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://ujf.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://yqm.fehbvm.com

Ruby: def to_s; @name; end
来源：http://ewi.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://zjv.jianghu66.top

[G13] 判断对象类型
来源：http://bcm.gogol.net.cn

Py:   isinstance(u, User)
来源：http://hkz.uphjek.com

PHP:  $u instanceof User
来源：http://yel.uphjek.com

JS:   u instanceof User
来源：http://qqv.c1oappe.top

TS:   u instanceof User
来源：http://hjx.ydzc1.top

Java: u instanceof User
来源：http://yzl.hesvh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://csd.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://dyt.andypj.xyz

C#:   u is User
来源：http://lbg.yfazqb.com

[G14] 数据类 / record
来源：http://zxh.zhiwuduotai.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uxg.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://otp.xuanzx.com

JS:   // 无内置：普通类或对象字面量
来源：http://lwm.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://czt.ctjpmb.com

Java: record User(String name, int age) {}
来源：http://ito.cucudq.cn

Go:   type User struct { Name string; Age int }
来源：http://nau.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aqc.tarul.cn

C#:   record User(string Name, int Age);
来源：http://wpb.jyoumei.cn

[G15] 枚举
来源：http://xik.yangfankeji.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rnh.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qum.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wlu.xuanzx.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zig.jlsjyb.cn

Java: enum Color { RED, GREEN }
来源：http://mdg.jinghuilouyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hzy.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://wjv.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vyb.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://klg.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kur.ydjk.org.cn

PHP:  get_object_vars($obj);
来源：http://ksa.uphjek.com

JS:   Object.entries(obj)
来源：http://val.ivvv.top

TS:   Object.entries(obj)
来源：http://vmr.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bdn.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wzb.wangshuangyany.cn

Ruby: obj.instance_variables
来源：http://lkh.xylfe.cn

C#:   // 用反射或 System.Text.Json
来源：http://ska.sweek.top

================================================================================
来源：http://rrq.wangshuangyany.cn

H. 异常与错误处理
来源：http://hyc.hysaishi.cn

================================================================================
来源：http://hum.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://tfa.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bxh.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nqp.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hpu.xingfuxueyuan.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tik.yongpay.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://orp.zhiwuduotai.top


<!-- 参考信息 -->