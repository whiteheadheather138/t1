代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dgs.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cpi.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://cul.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://nss.xziqi.cn

Go:   if s == "" {}
来源：http://pzx.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://abx.hysaishi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gnp.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://afz.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gjn.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tbd.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ing.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://puv.hysaishi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jen.haohaochexian.top

Go:   // 按 rune 判断长度后截断
来源：http://pku.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bev.gzhubu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mui.gogol.net.cn

[E22] 字节长度与字符长度
来源：http://vor.zhoulong.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uiz.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dpr.hongshengwenyu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ivi.fehbvm.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://thb.wangshuangyany.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ipv.sweek.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uuf.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://ohw.jinqigfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mlv.jinqigufen.top

================================================================================
来源：http://lob.nwbrower.top

F. 文件与目录
来源：http://dht.zdbjq.cn

================================================================================
来源：http://pxj.meibo888.top

[F01] 读取整个文件
来源：http://ega.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dfa.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://ckc.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yud.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ica.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lmq.yvedp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tbl.bbcook.cn

Ruby: File.read("a.txt")
来源：http://vlf.uphjek.com

C#:   File.ReadAllText("a.txt");
来源：http://nho.cheryme.top

[F02] 逐行读取文件
来源：http://umm.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ctk.xuanzx.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bnj.vqdsnc.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://daq.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nlr.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pml.hongshengwenyu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kle.fktsv.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mwn.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uwl.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://jxp.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oem.0kj1m.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sbt.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tuh.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://off.cashguo.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lfp.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ugu.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://fsv.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pui.xylfe.cn

[F04] 追加写入文件
来源：http://kxd.nanxuanxn.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tcr.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://siu.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbz.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bsx.ppjwa.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://srm.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://von.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yrz.mhx1999.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rez.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://fnp.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cfc.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://wkz.hongshengwenyu.top

JS:   fs.existsSync("a.txt")
来源：http://ihf.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://hek.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pkw.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://phc.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://zzb.yj202588.top

C#:   File.Exists("a.txt")
来源：http://xlg.nwbrower.top

[F06] 删除文件
来源：http://yhb.guannengcc.top

Py:   os.remove("a.txt")
来源：http://qph.hnxiangtu.top

PHP:  unlink("a.txt");
来源：http://vfg.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://obg.chenlongwang.top

TS:   fs.unlinkSync("a.txt")
来源：http://buq.zhengqikj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://chy.jinqigufen.top

Go:   os.Remove("a.txt")
来源：http://qyh.cqqwz.cn

Ruby: File.delete("a.txt")
来源：http://lfz.pengpengdd.cyou

C#:   File.Delete("a.txt");
来源：http://vsd.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://omb.hnxiangtu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cgp.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vqf.hcnkem.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://utx.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://alp.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ipx.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wsp.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://whi.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ixt.yuanzhike.top

[F08] 遍历目录
来源：http://fqh.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tmr.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rrq.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://kkc.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://iaj.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kja.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://iqa.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://ezh.hfpthk.cn

C#:   Directory.GetFiles("dir")
来源：http://lls.yvedp.cn

[F09] 获取文件大小
来源：http://zxs.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://kdb.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://cjg.guowangkeji.top

JS:   fs.statSync("a.txt").size
来源：http://vqj.yj202588.top

TS:   fs.statSync("a.txt").size
来源：http://dty.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://ozq.fzhhl.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dkw.xziqi.cn

Ruby: File.size("a.txt")
来源：http://ofj.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://pfv.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://jmf.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rpo.jyoumei.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yhw.sxryk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eqz.zhengqikj.top

TS:   path.extname("a.txt")
来源：http://bfq.xinyue.icu

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oau.fktsv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bkz.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jym.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dgh.tian-w.cn

[F11] 复制与移动文件
来源：http://jon.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mxy.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://drv.hywenlv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mtu.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpu.cdnleiting.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tnf.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iff.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dzg.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mjd.jianghu66.top

[F12] CSV 读写
来源：http://qfg.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dbm.tarul.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nnq.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xun.vqdsnc.cn

TS:   // 同上
来源：http://hkd.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aiz.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://guv.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bie.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mhs.sxryk.cn

================================================================================
来源：http://hbz.yueranfly.top

G. 面向对象
来源：http://zil.epnwcf.com

================================================================================
来源：http://emb.shanyushiyangtech.top

[G01] 定义类
来源：http://rui.pycfn.com

Py:   class User: pass
来源：http://jwg.shangyingyoupin.top

PHP:  class User {}
来源：http://alh.yj202588.top

JS:   class User {}
来源：http://pgj.ppjwa.cn

TS:   class User { name: string = ""; }
来源：http://kqh.yanxiufei.cn

Java: class User {}
来源：http://tge.meibo888.top

Go:   type User struct { Name string }
来源：http://qsb.yongpay.top

Ruby: class User; end
来源：http://rya.ivvv.top

C#:   class User {}
来源：http://ajm.gzhubu.top

[G02] 构造函数
来源：http://fos.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://pkv.hnxiangtu.top

PHP:  public function __construct(public string $name) {}
来源：http://dee.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://tak.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://byo.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://blz.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lde.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://xxs.gogol.net.cn

C#:   public User(string name) { Name = name; }
来源：http://sxl.bjfxy.top

[G03] 实例属性
来源：http://uik.yj20258888.top

Py:   self.name = "x"
来源：http://xds.yj20258.top

PHP:  public string $name = "x";
来源：http://emg.pycfn.com

JS:   this.name = "x";
来源：http://eew.pengpengdd.cyou

TS:   name: string = "x";
来源：http://yux.xuetiantiany.cn

Java: private String name;
来源：http://lha.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qxq.daxiang520.top

Ruby: @name = "x"
来源：http://oun.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://ovc.zdqjudy.top

[G04] 定义方法
来源：http://zrp.tian-w.cn

Py:   def greet(self): return self.name
来源：http://vpz.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cqo.hysaishi.cn

JS:   greet() { return this.name; }
来源：http://mip.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://bld.9152youxi.cn

Java: String greet() { return name; }
来源：http://mkl.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://lfj.52xcode.cn

Ruby: def greet; @name; end
来源：http://biq.tian-w.cn

C#:   public string Greet() => Name;
来源：http://xgg.vqdsnc.cn

[G05] 继承
来源：http://lwg.hcnkem.com

Py:   class Admin(User): pass
来源：http://mub.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://htz.316326.xyz

JS:   class Admin extends User {}
来源：http://ycn.sysykeji.top

TS:   class Admin extends User {}
来源：http://fej.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://aek.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ybi.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://xzr.hnxiangtu.top

C#:   class Admin : User {}
来源：http://ubv.tarul.cn

[G06] 重写方法
来源：http://ljd.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://mht.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bik.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://irv.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://kbd.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://mbc.jlsjyb.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zue.smart0.xyz

Ruby: def greet; "admin"; end
来源：http://bxn.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://ymr.yfazqb.com

[G07] 调用父类方法
来源：http://jyp.epnwcf.com

Py:   super().greet()
来源：http://cmh.gaohongyu789.top

PHP:  parent::greet();
来源：http://prv.fzhhl.top

JS:   super.greet();
来源：http://sif.cdnleiting.top

TS:   super.greet();
来源：http://lno.yongpay.top

Java: super.greet();
来源：http://usb.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vxy.jqgufenzy.top

Ruby: super
来源：http://fln.gogol.net.cn

C#:   base.Greet();
来源：http://uyw.yonumen.top

[G08] 静态方法与属性
来源：http://zpf.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yds.xuanzx.com

PHP:  public static function f() {}
来源：http://wgj.hammf.cn

JS:   static f() {}
来源：http://yfm.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://kzr.cashguo.top

Java: static void f() {}
来源：http://vsg.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://irw.tianlin.xyz

Ruby: def self.f; end
来源：http://vme.cqqwz.cn

C#:   public static void F() {}
来源：http://pgx.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://eks.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://zkg.jiagoushi.top

PHP:  interface Shape { public function area(): float; }
来源：http://zhp.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jgi.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://nnq.tian-w.cn

Java: interface Shape { double area(); }
来源：http://dpr.uphjek.com

Go:   type Shape interface { Area() float64 }
来源：http://lxb.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fjs.quarkkingdee.top

C#:   interface IShape { double Area(); }
来源：http://utb.gaohongyu789.top

[G10] 访问控制
来源：http://ikk.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://rfv.daria6918.cn

PHP:  public / protected / private
来源：http://htc.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://sag.ctjpmb.com

TS:   public / protected / private
来源：http://nao.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://zpm.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://acb.zycfv.cn

Ruby: public / protected / private
来源：http://rab.vehdjk.com

C#:   public / protected / private / internal
来源：http://igg.hesvh.cn

[G11] getter / setter
来源：http://uzl.fktsv.cn

Py:   @property 与 @x.setter
来源：http://mti.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hzm.fzhhl.top

JS:   get name() { return this._name; }
来源：http://ksv.guannengcc.top

TS:   get name(): string { return this._name; }
来源：http://eul.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://iqo.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://spg.gotoacloud.top

Ruby: attr_accessor :name
来源：http://lym.ivvv.top

C#:   public string Name { get; set; }
来源：http://pkg.nanxuanxn.top

[G12] 对象转字符串
来源：http://gsv.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://zyp.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xme.jinyuanbaomall.cn

JS:   toString() { return this.name; }
来源：http://gkd.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://oom.sweek.top

Java: @Override public String toString() { return name; }
来源：http://wyd.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://jwx.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://xqf.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://jqn.hesvh.cn

[G13] 判断对象类型
来源：http://xnd.gotoacloud.top

Py:   isinstance(u, User)
来源：http://iwj.zycfv.cn

PHP:  $u instanceof User
来源：http://hbt.wangshuangyany.cn

JS:   u instanceof User
来源：http://fra.jinghuilouyu.cn

TS:   u instanceof User
来源：http://shj.0kj1m.cn

Java: u instanceof User
来源：http://zrp.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://fer.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://nwn.ehwqpu.com

C#:   u is User
来源：http://suf.316326.xyz

[G14] 数据类 / record
来源：http://cjw.yj202588.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qsc.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://fof.yanxiufei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ttz.pengpengdd.cyou

TS:   type User = { name: string; age: number };
来源：http://oah.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://gdm.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://dbv.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vvy.nanxuanxn.top

C#:   record User(string Name, int Age);
来源：http://mqs.epnwcf.com

[G15] 枚举
来源：http://lox.sweek.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xdo.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wzt.dianchejie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://drk.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jbp.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://gft.yvedp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gpa.9152youxi.cn

Ruby: Color = %i[red green].freeze
来源：http://oww.zhaomingkeji.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mzn.yuanzhike.top

[G16] 对象转数组 / 字典
来源：http://sfd.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gkr.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://yoe.hysaishi.cn

JS:   Object.entries(obj)
来源：http://fov.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://wcf.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cpf.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bwu.aizwys.cn

Ruby: obj.instance_variables
来源：http://ubd.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://mvi.yanxiufei.cn

================================================================================
来源：http://cdd.yanxiufei.cn

H. 异常与错误处理
来源：http://ndj.ctjpmb.com

================================================================================
来源：http://peu.fengsongda.top

[H01] try / catch 基础
来源：http://szy.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tun.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cdm.tanke756.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tve.yfazqb.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cuz.hcnkem.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lyb.nanxinkj.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wtv.quarkkingdee.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gjv.jiagoushi.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jnj.meibo888.top

[H02] finally / ensure 收尾
来源：http://zes.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://ajd.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kni.gogol.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zll.andypj.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://bmt.yuxming.cn


<!-- 参考信息 -->