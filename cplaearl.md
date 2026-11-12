代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://mqn.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://rie.hfpthk.cn

Java: s.lines().toList()
来源：http://med.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://ktl.yj202588.top

Ruby: s.lines
来源：http://xge.guannengcc.top

C#:   s.Split('\n')
来源：http://avh.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://dts.xylfe.cn

Py:   if not s:
来源：http://jay.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uao.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://szh.gaohongyu789.top

TS:   if (s === "") {}
来源：http://zxw.hnqzz.top

Java: if (s.isEmpty()) {}
来源：http://xyo.hesvh.cn

Go:   if s == "" {}
来源：http://ntd.svipenyu.cn

Ruby: if s.empty?
来源：http://xbe.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://krn.redwolf501.top

[E21] 超长截断加省略号
来源：http://dnl.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rvs.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://red.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ilc.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ipu.yonumen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbs.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://dey.mhx1999.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tfz.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dmb.dashuyun.cn

[E22] 字节长度与字符长度
来源：http://waj.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aje.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kdf.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vvx.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vsf.tarul.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://inx.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://iht.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://jft.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iry.xziqi.cn

================================================================================
来源：http://adc.jinqigfzy.top

F. 文件与目录
来源：http://tnj.havefunace.top

================================================================================
来源：http://ohq.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://cif.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eoj.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://kps.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zgi.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://awp.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nhd.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qkr.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://ply.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://kiv.gaohongyu789.top

[F02] 逐行读取文件
来源：http://ryn.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hcx.xinyue.icu

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dvv.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qjw.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://psm.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bhi.guowangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wbc.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://htl.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rzl.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://hpz.jinqigfzy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://buv.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vui.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nvp.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://roq.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://msk.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://avx.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://tey.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qky.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://quy.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pyv.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fqn.shanyushiyangtech.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igf.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fdi.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iaz.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vxe.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ubo.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yre.xziqi.cn

[F05] 判断文件或目录是否存在
来源：http://rjn.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wno.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://sak.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://ekw.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://ykr.haohaochexian.top

Java: Files.exists(Path.of("a.txt"))
来源：http://smz.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wyg.zhixingplan.top

Ruby: File.exist?("a.txt")
来源：http://pqk.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://jtb.gogol.net.cn

[F06] 删除文件
来源：http://dlo.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://sou.tanke756.top

PHP:  unlink("a.txt");
来源：http://wxj.jinyuanbaomall.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gmh.mhx1999.top

TS:   fs.unlinkSync("a.txt")
来源：http://pix.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ujn.bjfxy.top

Go:   os.Remove("a.txt")
来源：http://gtz.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://txc.aibaodan.cn

C#:   File.Delete("a.txt");
来源：http://wdu.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://rve.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ice.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dtb.cdnleiting.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hda.zhongyouzk.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://slo.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gia.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mcp.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mxy.snrcjt.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://huz.cashguo.top

[F08] 遍历目录
来源：http://ykg.gogol.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mzm.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nlg.gzhubu.top

JS:   fs.readdirSync("dir")
来源：http://ofc.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://ojq.dashuyun.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ejn.jinghuilouyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tdo.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://pvn.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://hji.xingfuxueyuan.xyz

[F09] 获取文件大小
来源：http://bve.pengpengdd.cyou

Py:   os.path.getsize("a.txt")
来源：http://ztn.uphjek.com

PHP:  filesize("a.txt");
来源：http://rrp.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://jjk.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://kgg.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zdr.xuetiantiany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://asa.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://aje.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://vvi.hesvh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ref.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xut.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nnf.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vvc.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://tip.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ezk.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://inr.aibaodan.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hti.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qux.hammf.cn

[F11] 复制与移动文件
来源：http://pba.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pmq.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vlz.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzn.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohl.andypj.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xye.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xav.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ryr.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wju.hysaishi.cn

[F12] CSV 读写
来源：http://lag.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ggi.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://krw.andypj.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://iry.ppjwa.cn

TS:   // 同上
来源：http://vze.guannengcc.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wez.yongpay.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cud.jiagoushi.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bga.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tcs.jiagoushi.top

================================================================================
来源：http://llx.ppjwa.cn

G. 面向对象
来源：http://ryx.sufxvd.cn

================================================================================
来源：http://akb.zhijiandao.cn

[G01] 定义类
来源：http://bqv.fzhhl.top

Py:   class User: pass
来源：http://djy.aizwys.cn

PHP:  class User {}
来源：http://ojh.kuanghao11.cn

JS:   class User {}
来源：http://gel.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://mnn.yfazqb.com

Java: class User {}
来源：http://xau.bbcook.cn

Go:   type User struct { Name string }
来源：http://nbl.bjfxy.top

Ruby: class User; end
来源：http://ovv.quarkkingdee.top

C#:   class User {}
来源：http://nrs.shanyushiyangkeji.top

[G02] 构造函数
来源：http://mhh.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://tpd.fzhhl.top

PHP:  public function __construct(public string $name) {}
来源：http://lpz.jinyuanbaomall.cn

JS:   constructor(name) { this.name = name; }
来源：http://fhw.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://ipa.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://xtv.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zkx.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://mmo.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://rru.nwbrower.top

[G03] 实例属性
来源：http://rzp.bjfxy.top

Py:   self.name = "x"
来源：http://gtz.ctjpmb.com

PHP:  public string $name = "x";
来源：http://vdj.hcnkem.com

JS:   this.name = "x";
来源：http://rwz.jlsjyb.cn

TS:   name: string = "x";
来源：http://ejw.dashuyun.cn

Java: private String name;
来源：http://nbp.316326.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mit.feifeiyinyue.top

Ruby: @name = "x"
来源：http://xli.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://lii.havefunace.top

[G04] 定义方法
来源：http://bys.guowangkeji.top

Py:   def greet(self): return self.name
来源：http://dld.cashguo.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gfq.pycfn.com

JS:   greet() { return this.name; }
来源：http://rvn.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://diw.gogol.net.cn

Java: String greet() { return name; }
来源：http://hpy.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uha.yj20258888.top

Ruby: def greet; @name; end
来源：http://jst.tianlin.xyz

C#:   public string Greet() => Name;
来源：http://coq.sxryk.cn

[G05] 继承
来源：http://iuj.yvedp.cn

Py:   class Admin(User): pass
来源：http://rwa.xinyue.icu

PHP:  class Admin extends User {}
来源：http://for.shzxlz.cn

JS:   class Admin extends User {}
来源：http://lsf.zhixingplan.top

TS:   class Admin extends User {}
来源：http://hzk.fengsongda.top

Java: class Admin extends User {}
来源：http://ucf.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ptz.ppjwa.cn

Ruby: class Admin < User; end
来源：http://zut.wangdashe.top

C#:   class Admin : User {}
来源：http://fen.jqgufenzy.top

[G06] 重写方法
来源：http://zuh.tarul.cn

Py:   def greet(self): return "admin"
来源：http://ijt.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://hld.cucudq.cn

JS:   greet() { return "admin"; }
来源：http://rtw.yvedp.cn

TS:   greet(): string { return "admin"; }
来源：http://fgu.hysaishi.cn

Java: @Override String greet() { return "admin"; }
来源：http://cre.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kob.fehbvm.com

Ruby: def greet; "admin"; end
来源：http://jpo.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://rir.yj20258.top

[G07] 调用父类方法
来源：http://ezb.jiagoushi.top

Py:   super().greet()
来源：http://vjt.vqdsnc.cn

PHP:  parent::greet();
来源：http://bub.jinghuilouyu.cn

JS:   super.greet();
来源：http://gkf.shanyushiyangtech.top

TS:   super.greet();
来源：http://nnd.jqgufenzy.top

Java: super.greet();
来源：http://ifv.yongpay.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yix.xuetiantiany.cn

Ruby: super
来源：http://oya.fzhhl.top

C#:   base.Greet();
来源：http://kwq.guannengcc.top

[G08] 静态方法与属性
来源：http://rri.yongpay.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ioo.yueranfly.top

PHP:  public static function f() {}
来源：http://txt.ywan-chungtsiang.top

JS:   static f() {}
来源：http://ukf.kuanghao11.cn

TS:   static f(): void {}
来源：http://fsl.wangshuangyany.cn

Java: static void f() {}
来源：http://znp.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hzj.guowangkeji.top

Ruby: def self.f; end
来源：http://syg.feifeiyinyue.top

C#:   public static void F() {}
来源：http://nnm.xuanzx.com

[G09] 接口 / 抽象类
来源：http://agc.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://obe.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://znr.jyoumei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hke.shzxlz.cn

TS:   interface Shape { area(): number; }
来源：http://hjp.shanyushiyangtech.top

Java: interface Shape { double area(); }
来源：http://jwt.jqgufenzy.top

Go:   type Shape interface { Area() float64 }
来源：http://moz.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qup.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://ldm.shzxlz.cn

[G10] 访问控制
来源：http://qav.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://oxh.jiagoushi.top

PHP:  public / protected / private
来源：http://afe.cashguo.top

JS:   #private 字段；其余公开
来源：http://rqb.sysykeji.top

TS:   public / protected / private
来源：http://pnq.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://zye.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://hag.kuanghao11.cn

Ruby: public / protected / private
来源：http://oer.cqqwz.cn

C#:   public / protected / private / internal
来源：http://akt.iojbl.cn

[G11] getter / setter
来源：http://lky.snrcjt.cn

Py:   @property 与 @x.setter
来源：http://szd.hywenlv.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ogz.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://aws.jianghu66.top

TS:   get name(): string { return this._name; }
来源：http://tqa.guowangkeji.top

Java: public String getName() { return name; }
来源：http://xmx.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uyu.zhijiandao.cn

Ruby: attr_accessor :name
来源：http://dtv.chenjidiqi.icu

C#:   public string Name { get; set; }
来源：http://jdt.cqqwz.cn

[G12] 对象转字符串
来源：http://okw.yj20258.top

Py:   def __str__(self): return self.name
来源：http://xdf.ctjpmb.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://moj.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://gkm.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://yis.hfpthk.cn

Java: @Override public String toString() { return name; }
来源：http://nyl.chenlongwang.top

Go:   func (u User) String() string { return u.Name }
来源：http://ebh.yvedp.cn

Ruby: def to_s; @name; end
来源：http://qev.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://kua.xuanzx.com

[G13] 判断对象类型
来源：http://ufp.hnqzz.top

Py:   isinstance(u, User)
来源：http://evs.zhijiandao.cn

PHP:  $u instanceof User
来源：http://slc.316326.xyz

JS:   u instanceof User
来源：http://cxj.0kj1m.cn

TS:   u instanceof User
来源：http://gsr.yuxming.cn

Java: u instanceof User
来源：http://qoe.wangshuangyany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fit.havefunace.top

Ruby: u.is_a?(User)
来源：http://vgd.sufxvd.cn

C#:   u is User
来源：http://iab.tanke756.top

[G14] 数据类 / record
来源：http://zvm.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hui.zhijiandao.cn

PHP:  // 用 readonly 属性模拟
来源：http://lgm.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://imp.shanyushiyangkeji.top

TS:   type User = { name: string; age: number };
来源：http://jzf.shzxlz.cn

Java: record User(String name, int age) {}
来源：http://dod.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://tsl.sweek.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lto.yj20258888.top

C#:   record User(string Name, int Age);
来源：http://ppv.fzhhl.top

[G15] 枚举
来源：http://krp.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://paw.quarkkingdee.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gwa.tarul.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://snq.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dom.ctjpmb.com

Java: enum Color { RED, GREEN }
来源：http://cbs.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kim.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://qgm.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gam.ydjk.org.cn

[G16] 对象转数组 / 字典
来源：http://htm.jqgufenzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lgk.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://vwz.smart0.xyz

JS:   Object.entries(obj)
来源：http://nuz.havefunace.top

TS:   Object.entries(obj)
来源：http://kpq.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lkh.yuanzhike.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lka.316326.xyz

Ruby: obj.instance_variables
来源：http://scv.shanyushiyangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://nmq.jinghuilouyu.cn

================================================================================
来源：http://rqd.quarkkingdee.top

H. 异常与错误处理
来源：http://her.zdbjq.cn

================================================================================
来源：http://kgx.wangshuangyany.cn

[H01] try / catch 基础
来源：http://nqb.tian-w.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vlc.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fvl.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lzs.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vba.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kod.jinyuanbaomall.cn


<!-- 参考信息 -->