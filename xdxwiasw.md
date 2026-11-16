代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yyq.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bko.yuanzhike.top

TS:   if (s === "") {}
来源：http://tgu.xziqi.cn

Java: if (s.isEmpty()) {}
来源：http://qva.sxryk.cn

Go:   if s == "" {}
来源：http://iaa.vehdjk.com

Ruby: if s.empty?
来源：http://jdk.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xhg.guowangkeji.top

[E21] 超长截断加省略号
来源：http://cmq.uphjek.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://boy.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gcg.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fcu.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xba.aizwys.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dxt.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://pdv.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rvd.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gui.cashguo.top

[E22] 字节长度与字符长度
来源：http://pkv.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jqd.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qcv.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://liv.andypj.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhh.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ifc.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xfb.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://cld.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fzn.hfpthk.cn

================================================================================
来源：http://iso.cucudq.cn

F. 文件与目录
来源：http://rlu.316326.xyz

================================================================================
来源：http://siy.hysaishi.cn

[F01] 读取整个文件
来源：http://eye.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gkj.sweek.top

PHP:  file_get_contents("a.txt");
来源：http://vhu.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qmv.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gzm.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oyd.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://trf.0kj1m.cn

Ruby: File.read("a.txt")
来源：http://srz.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://jzz.yvedp.cn

[F02] 逐行读取文件
来源：http://hup.xuetiantiany.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://irc.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://awv.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://azl.shuidangran.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blp.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wbe.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ujr.xuanzx.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iyw.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mjk.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://oqm.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wpo.yuxming.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ott.meibo888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xnp.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yup.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qqq.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ctt.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://gsh.shangyingyoupin.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lkr.nwbrower.top

[F04] 追加写入文件
来源：http://uno.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hwf.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sll.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://axr.jinyuanbaomall.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dws.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yzw.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://syj.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gpx.gotoacloud.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wuf.gotoacloud.top

[F05] 判断文件或目录是否存在
来源：http://jkk.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wzi.yj20258.top

PHP:  file_exists("a.txt");
来源：http://asu.haohaochexian.top

JS:   fs.existsSync("a.txt")
来源：http://hrv.yangfankeji.com

TS:   fs.existsSync("a.txt")
来源：http://atv.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hdd.ivvv.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ysc.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://jdm.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://wjk.jianghu66.top

[F06] 删除文件
来源：http://etp.shuidangran.top

Py:   os.remove("a.txt")
来源：http://bij.chenzaomai.com

PHP:  unlink("a.txt");
来源：http://iww.wangshuangyany.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vif.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ber.feifeiyinyue.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://biy.yuanzhike.top

Go:   os.Remove("a.txt")
来源：http://wjd.yongpay.top

Ruby: File.delete("a.txt")
来源：http://dhe.zdqjudy.top

C#:   File.Delete("a.txt");
来源：http://mdk.smart0.xyz

[F07] 创建目录（含多级）
来源：http://cym.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oyl.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gwu.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://npf.nwbrower.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vna.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lvi.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xhr.xuanzx.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://shj.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rok.tian-w.cn

[F08] 遍历目录
来源：http://hgt.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ueb.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uih.wangshuangyany.cn

JS:   fs.readdirSync("dir")
来源：http://vok.ybcxt.top

TS:   fs.readdirSync("dir")
来源：http://zdr.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fsi.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://qwe.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://azi.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://cdi.cucudq.cn

[F09] 获取文件大小
来源：http://cus.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://mxf.shuidangran.top

PHP:  filesize("a.txt");
来源：http://rha.ivvv.top

JS:   fs.statSync("a.txt").size
来源：http://pzn.shanyushiyangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://pht.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ztv.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gah.shanyushiyangkeji.top

Ruby: File.size("a.txt")
来源：http://ncb.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://urj.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://egm.yj202588.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gml.yonumen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bad.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://smp.cucudq.cn

TS:   path.extname("a.txt")
来源：http://vxo.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dyc.hfpthk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fgd.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pah.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kzt.ybcxt.top

[F11] 复制与移动文件
来源：http://urb.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mmr.kuanghao11.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rzw.nwbrower.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dcf.meibo888.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zmy.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jag.yfazqb.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zwe.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nuf.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wbt.meibo888.top

[F12] CSV 读写
来源：http://cte.ivvv.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hbx.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jpw.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jnb.fanxiaobao.xyz

TS:   // 同上
来源：http://dbv.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://epy.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jog.52xcode.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qzf.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://gjp.yj20258.top

================================================================================
来源：http://hkn.zhengqikj.top

G. 面向对象
来源：http://laz.shzxlz.cn

================================================================================
来源：http://dhm.sjlbkw.cn

[G01] 定义类
来源：http://yyg.haohaochexian.top

Py:   class User: pass
来源：http://ldd.xinyue.icu

PHP:  class User {}
来源：http://kie.tianlin.xyz

JS:   class User {}
来源：http://woj.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://vsj.jiagoushi.top

Java: class User {}
来源：http://zsi.xinyue.icu

Go:   type User struct { Name string }
来源：http://tec.xylfe.cn

Ruby: class User; end
来源：http://coq.vqdsnc.cn

C#:   class User {}
来源：http://rkb.aibaodan.cn

[G02] 构造函数
来源：http://kvk.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://lrb.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://gbw.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://eaz.fktsv.cn

TS:   constructor(public name: string) {}
来源：http://jde.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://jpg.uphjek.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jyt.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://yfz.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://qwx.fehbvm.com

[G03] 实例属性
来源：http://kuo.wangdashe.top

Py:   self.name = "x"
来源：http://ygi.cqqwz.cn

PHP:  public string $name = "x";
来源：http://ijk.aibaodan.cn

JS:   this.name = "x";
来源：http://fii.xziqi.cn

TS:   name: string = "x";
来源：http://pzs.yongpay.top

Java: private String name;
来源：http://pbg.zhijiandao.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tyk.nanxinkj.top

Ruby: @name = "x"
来源：http://wbo.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://wyh.daxiang520.top

[G04] 定义方法
来源：http://rtm.bjfxy.top

Py:   def greet(self): return self.name
来源：http://myw.feifeiyinyue.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zzq.sxryk.cn

JS:   greet() { return this.name; }
来源：http://mjd.nanxuanxn.top

TS:   greet(): string { return this.name; }
来源：http://txh.sjlbkw.cn

Java: String greet() { return name; }
来源：http://dwu.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gyv.shanyushiyangkeji.top

Ruby: def greet; @name; end
来源：http://paq.aizwys.cn

C#:   public string Greet() => Name;
来源：http://yln.aibaodan.cn

[G05] 继承
来源：http://xuw.zhixingplan.top

Py:   class Admin(User): pass
来源：http://mcz.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://lat.fktsv.cn

JS:   class Admin extends User {}
来源：http://csl.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://arm.hywenlv.cn

Java: class Admin extends User {}
来源：http://qvo.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hzw.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://avq.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://ycr.iojbl.cn

[G06] 重写方法
来源：http://smq.guannengcc.top

Py:   def greet(self): return "admin"
来源：http://gyk.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://uni.nwbrower.top

JS:   greet() { return "admin"; }
来源：http://rxx.fktsv.cn

TS:   greet(): string { return "admin"; }
来源：http://vzn.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://zyk.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iim.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://jtt.tanke756.top

C#:   public override string Greet() => "admin";
来源：http://nth.ydjk.org.cn

[G07] 调用父类方法
来源：http://qmk.zycfv.cn

Py:   super().greet()
来源：http://bwh.9152youxi.cn

PHP:  parent::greet();
来源：http://ufn.fehbvm.com

JS:   super.greet();
来源：http://upz.jyoumei.cn

TS:   super.greet();
来源：http://jtk.jiagoushi.top

Java: super.greet();
来源：http://fnb.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iyn.yanxiufei.cn

Ruby: super
来源：http://azi.aibaodan.cn

C#:   base.Greet();
来源：http://sxi.sysykeji.top

[G08] 静态方法与属性
来源：http://igw.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pqk.andypj.xyz

PHP:  public static function f() {}
来源：http://ibh.yj20258.top

JS:   static f() {}
来源：http://uvj.jianghu66.top

TS:   static f(): void {}
来源：http://wdy.fktsv.cn

Java: static void f() {}
来源：http://dfc.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hub.ydjk.org.cn

Ruby: def self.f; end
来源：http://diy.fzhhl.top

C#:   public static void F() {}
来源：http://nnm.guannengcc.top

[G09] 接口 / 抽象类
来源：http://ots.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://tes.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://cak.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ext.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://fhx.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://mvb.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://uve.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dvr.ivvv.top

C#:   interface IShape { double Area(); }
来源：http://yax.c1oappe.top

[G10] 访问控制
来源：http://yid.zdbjq.cn

Py:   约定 _protected / __private（不强制）
来源：http://rky.zhiwuduotai.top

PHP:  public / protected / private
来源：http://ika.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://vro.ydzc1.top

TS:   public / protected / private
来源：http://orl.xuetiantiany.cn

Java: public / protected / private / 默认包级
来源：http://gag.sxryk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://snp.epnwcf.com

Ruby: public / protected / private
来源：http://ecc.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://tep.fzhhl.top

[G11] getter / setter
来源：http://yov.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://wul.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rkz.vqdsnc.cn

JS:   get name() { return this._name; }
来源：http://zab.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://wdz.hammf.cn

Java: public String getName() { return name; }
来源：http://pqs.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wbu.cheryme.top

Ruby: attr_accessor :name
来源：http://nul.gogol.net.cn

C#:   public string Name { get; set; }
来源：http://yca.tian-w.cn

[G12] 对象转字符串
来源：http://uny.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://ufi.wangshuangyany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jnc.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://rmg.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://yqc.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://ekd.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://rvp.shuidangran.top

Ruby: def to_s; @name; end
来源：http://zcc.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://lks.xylfe.cn

[G13] 判断对象类型
来源：http://xps.jyoumei.cn

Py:   isinstance(u, User)
来源：http://sfe.zhaomingkeji.xyz

PHP:  $u instanceof User
来源：http://jhl.gotoacloud.top

JS:   u instanceof User
来源：http://jco.c1oappe.top

TS:   u instanceof User
来源：http://hjn.hammf.cn

Java: u instanceof User
来源：http://pss.snrcjt.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zvw.yj20258.top

Ruby: u.is_a?(User)
来源：http://nly.cheryme.top

C#:   u is User
来源：http://fvk.yj20258888.top

[G14] 数据类 / record
来源：http://dez.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sem.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://wrs.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://hbv.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://alv.redwolf501.top

Java: record User(String name, int age) {}
来源：http://qeq.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://vhr.iojbl.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://svh.sufxvd.cn

C#:   record User(string Name, int Age);
来源：http://nnt.fktsv.cn

[G15] 枚举
来源：http://pcv.zhongyouzk.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mse.xylfe.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dgu.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rna.ybcxt.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uom.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://ixs.zdqjudy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cbf.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://tie.svipenyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hhj.tanke756.top

[G16] 对象转数组 / 字典
来源：http://prt.zhengqikj.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hpu.zhongyouzk.top

PHP:  get_object_vars($obj);
来源：http://fxr.pengpengdd.cyou

JS:   Object.entries(obj)
来源：http://vie.vehdjk.com

TS:   Object.entries(obj)
来源：http://jqo.cheryme.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jcc.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://nxq.sxryk.cn

Ruby: obj.instance_variables
来源：http://yfx.haohaochexian.top

C#:   // 用反射或 System.Text.Json
来源：http://rng.tian-w.cn

================================================================================
来源：http://gav.yuxming.cn

H. 异常与错误处理
来源：http://ooz.cqqwz.cn

================================================================================
来源：http://wzd.uphjek.com

[H01] try / catch 基础
来源：http://gpc.316326.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pqe.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://voy.9152youxi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ira.haohaochexian.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hdk.cqqwz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vjs.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gst.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hsa.hongshengwenyu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://enk.sufxvd.cn

[H02] finally / ensure 收尾
来源：http://gmk.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qzg.fehbvm.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://rcb.zhoulong.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://zqv.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://zca.jyoumei.cn


<!-- 参考信息 -->