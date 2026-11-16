代发 wailian999

Ruby: s.lines
来源：http://rso.nwbrower.top

C#:   s.Split('\n')
来源：http://yif.andypj.xyz

[E20] 判断字符串是否为空
来源：http://rrq.cashguo.top

Py:   if not s:
来源：http://usy.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rah.wangshuangyany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fal.uphjek.com

TS:   if (s === "") {}
来源：http://ftn.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://pal.316326.xyz

Go:   if s == "" {}
来源：http://kgg.mhx1999.top

Ruby: if s.empty?
来源：http://fvt.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vrt.uphjek.com

[E21] 超长截断加省略号
来源：http://zoa.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rbt.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ozo.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdk.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ctq.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lhp.yj20258.top

Go:   // 按 rune 判断长度后截断
来源：http://bkk.cdnleiting.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cer.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xee.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://ylw.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hya.nwbrower.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ckd.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ucz.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cxa.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vyl.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kms.sweek.top

Ruby: s.bytesize;  s.length
来源：http://oag.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ujf.shanyushiyangkeji.top

================================================================================
来源：http://nuk.hywenlv.cn

F. 文件与目录
来源：http://ako.0kj1m.cn

================================================================================
来源：http://cmu.nwbrower.top

[F01] 读取整个文件
来源：http://fmq.zhixingplan.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uwe.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://vpf.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://quz.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://knl.cqqwz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://udg.dashuyun.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xkb.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://icy.cqqwz.cn

C#:   File.ReadAllText("a.txt");
来源：http://sbm.jqgufenzy.top

[F02] 逐行读取文件
来源：http://phx.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gly.feifeiyinyue.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sro.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://omj.dianchejie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://won.mhx1999.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nay.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rxo.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yiw.snrcjt.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mqv.chenzaomai.com

[F03] 写入文件（覆盖）
来源：http://sws.fzhhl.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rgx.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qww.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wao.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jja.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tkc.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vex.jinyuanbaomall.cn

Ruby: File.write("a.txt", "hi")
来源：http://acy.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rth.yonumen.top

[F04] 追加写入文件
来源：http://dfh.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bow.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://utf.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dqb.guowangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dsm.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nhj.yvedp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gww.ybcxt.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vcx.hammf.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ryp.ydjk.org.cn

[F05] 判断文件或目录是否存在
来源：http://lee.andypj.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fjg.sweek.top

PHP:  file_exists("a.txt");
来源：http://rft.hammf.cn

JS:   fs.existsSync("a.txt")
来源：http://glf.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://una.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://myl.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hnr.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://kxy.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://czx.fktsv.cn

[F06] 删除文件
来源：http://xsd.meibo888.top

Py:   os.remove("a.txt")
来源：http://qmc.9152youxi.cn

PHP:  unlink("a.txt");
来源：http://igx.jqgufenzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://rxg.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://hbk.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zlb.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://prf.cashguo.top

Ruby: File.delete("a.txt")
来源：http://zmc.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://daa.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://hav.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gws.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uhy.zhijiandao.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tyt.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://elt.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://syo.ydjk.org.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://amk.shangyingyoupin.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kcx.pycfn.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://huv.52xcode.cn

[F08] 遍历目录
来源：http://kkb.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://yak.zhongyouzk.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dzw.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://vvi.redwolf501.top

TS:   fs.readdirSync("dir")
来源：http://lle.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dlh.jiagoushi.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://myf.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://tsn.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://fwk.meibo888.top

[F09] 获取文件大小
来源：http://qsr.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://fnq.jinqigufen.top

PHP:  filesize("a.txt");
来源：http://ygi.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://fvp.zhijiandao.cn

TS:   fs.statSync("a.txt").size
来源：http://jsw.dianchejie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xnp.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lwf.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://mjz.hfpthk.cn

C#:   new FileInfo("a.txt").Length
来源：http://azq.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://byr.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://phl.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lhu.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cai.guannengcc.top

TS:   path.extname("a.txt")
来源：http://cgl.bbcook.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gwv.shzxlz.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fku.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gon.ydjk.org.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tsr.guannengcc.top

[F11] 复制与移动文件
来源：http://tti.mhx1999.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hse.jqgfzy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fqg.zhongyouzk.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://njz.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vlj.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kli.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://azq.feifeiyinyue.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gzt.shanyushiyangkeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xsz.52xcode.cn

[F12] CSV 读写
来源：http://osd.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zcw.mhx1999.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://znn.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nog.xylfe.cn

TS:   // 同上
来源：http://znu.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fmy.shangyingyoupin.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kwl.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qjl.zhijiandao.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ceu.snrcjt.cn

================================================================================
来源：http://wed.cdnleiting.top

G. 面向对象
来源：http://bsf.zhaomingkeji.xyz

================================================================================
来源：http://jyw.bbcook.cn

[G01] 定义类
来源：http://our.shanyushiyangkeji.top

Py:   class User: pass
来源：http://fzn.uphjek.com

PHP:  class User {}
来源：http://ovc.zhixingplan.top

JS:   class User {}
来源：http://imq.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://ffw.cucudq.cn

Java: class User {}
来源：http://bis.chenzaomai.com

Go:   type User struct { Name string }
来源：http://aph.chenlongwang.top

Ruby: class User; end
来源：http://qsa.hesvh.cn

C#:   class User {}
来源：http://ffd.jqgfzy.top

[G02] 构造函数
来源：http://suq.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://sao.yuxming.cn

PHP:  public function __construct(public string $name) {}
来源：http://mxf.nanxinkj.top

JS:   constructor(name) { this.name = name; }
来源：http://hbp.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://ipq.zhongyouzk.top

Java: User(String name) { this.name = name; }
来源：http://fgj.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wkh.aibaodan.cn

Ruby: def initialize(name); @name = name; end
来源：http://snj.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://odc.snrcjt.cn

[G03] 实例属性
来源：http://ewz.hcnkem.com

Py:   self.name = "x"
来源：http://bkb.c1oappe.top

PHP:  public string $name = "x";
来源：http://dtq.pycfn.com

JS:   this.name = "x";
来源：http://rmp.hywenlv.cn

TS:   name: string = "x";
来源：http://jlj.hysaishi.cn

Java: private String name;
来源：http://vrl.c1oappe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eeq.jinqigufen.top

Ruby: @name = "x"
来源：http://fym.jiagoushi.top

C#:   public string Name { get; set; } = "x";
来源：http://dtw.ehwqpu.com

[G04] 定义方法
来源：http://iso.guannengcc.top

Py:   def greet(self): return self.name
来源：http://ten.xuanzx.com

PHP:  public function greet(): string { return $this->name; }
来源：http://kar.ydjk.org.cn

JS:   greet() { return this.name; }
来源：http://rta.svipenyu.cn

TS:   greet(): string { return this.name; }
来源：http://bbt.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://mte.andypj.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://aoa.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://hvq.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://jtp.svipenyu.cn

[G05] 继承
来源：http://dxk.tanke756.top

Py:   class Admin(User): pass
来源：http://rec.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://cqp.nanxinkj.top

JS:   class Admin extends User {}
来源：http://qbj.chenzaomai.com

TS:   class Admin extends User {}
来源：http://lav.jyoumei.cn

Java: class Admin extends User {}
来源：http://she.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xtj.shuidangran.top

Ruby: class Admin < User; end
来源：http://mcu.jinqigufen.top

C#:   class Admin : User {}
来源：http://vhc.zhoulong.xyz

[G06] 重写方法
来源：http://ugq.kuanghao11.cn

Py:   def greet(self): return "admin"
来源：http://tky.gotoacloud.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zre.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://oio.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://zoi.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://rok.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fnj.havefunace.top

Ruby: def greet; "admin"; end
来源：http://gjm.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://xnl.sjlbkw.cn

[G07] 调用父类方法
来源：http://dee.chenlongwang.top

Py:   super().greet()
来源：http://tdx.316326.xyz

PHP:  parent::greet();
来源：http://xve.jqgfzy.top

JS:   super.greet();
来源：http://hox.sxryk.cn

TS:   super.greet();
来源：http://bfq.aizwys.cn

Java: super.greet();
来源：http://tvs.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nnd.yj20258.top

Ruby: super
来源：http://glz.zhijiandao.cn

C#:   base.Greet();
来源：http://lrm.shuidangran.top

[G08] 静态方法与属性
来源：http://tor.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://upo.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://ifk.yueranfly.top

JS:   static f() {}
来源：http://mdm.fzhhl.top

TS:   static f(): void {}
来源：http://cmy.sysykeji.top

Java: static void f() {}
来源：http://pbf.zycfv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://agq.feifeiyinyue.top

Ruby: def self.f; end
来源：http://kuh.gotoacloud.top

C#:   public static void F() {}
来源：http://trh.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://qpw.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://aho.tanke756.top

PHP:  interface Shape { public function area(): float; }
来源：http://qzr.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://llb.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://nvp.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://xes.xziqi.cn

Go:   type Shape interface { Area() float64 }
来源：http://wup.0kj1m.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bmx.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://kiz.zhijiandao.cn

[G10] 访问控制
来源：http://opw.fktsv.cn

Py:   约定 _protected / __private（不强制）
来源：http://anb.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://wgo.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://fzo.nanxinkj.top

TS:   public / protected / private
来源：http://ypa.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://uqt.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fud.yvedp.cn

Ruby: public / protected / private
来源：http://keb.fengsongda.top

C#:   public / protected / private / internal
来源：http://nxr.xziqi.cn

[G11] getter / setter
来源：http://kjv.shangyingyoupin.top

Py:   @property 与 @x.setter
来源：http://fea.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ash.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://ece.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://edo.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://uqy.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://div.xuanzx.com

Ruby: attr_accessor :name
来源：http://uck.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://ufd.yuxming.cn

[G12] 对象转字符串
来源：http://drl.hongshengwenyu.top

Py:   def __str__(self): return self.name
来源：http://obm.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kjm.yongpay.top

JS:   toString() { return this.name; }
来源：http://xaa.zdqjudy.top

TS:   toString(): string { return this.name; }
来源：http://gge.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://rho.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://nfa.chenlongwang.top

Ruby: def to_s; @name; end
来源：http://col.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://daq.yj202588.top

[G13] 判断对象类型
来源：http://rkh.shanyushiyangkeji.top

Py:   isinstance(u, User)
来源：http://itc.jqgufenzy.top

PHP:  $u instanceof User
来源：http://euo.wangshuangyany.cn

JS:   u instanceof User
来源：http://spe.aibaodan.cn

TS:   u instanceof User
来源：http://zru.hywenlv.cn

Java: u instanceof User
来源：http://pyb.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nsf.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://uax.jianghu66.top

C#:   u is User
来源：http://fhc.jiagoushi.top

[G14] 数据类 / record
来源：http://vos.ivvv.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kzq.hammf.cn

PHP:  // 用 readonly 属性模拟
来源：http://xnt.zhongyouzk.top

JS:   // 无内置：普通类或对象字面量
来源：http://tdj.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://qoq.hnxiangtu.top

Java: record User(String name, int age) {}
来源：http://txa.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://zey.dashuyun.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kvw.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://wjr.hammf.cn

[G15] 枚举
来源：http://dgo.kuanghao11.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://brh.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nko.pengpengdd.cyou

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tao.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tlh.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://dzh.yanxiufei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yxn.ehwqpu.com

Ruby: Color = %i[red green].freeze
来源：http://fje.aizwys.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hkk.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://dyw.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dzm.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://vee.jlsjyb.cn

JS:   Object.entries(obj)
来源：http://rhy.fktsv.cn

TS:   Object.entries(obj)
来源：http://ehh.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dyl.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://zet.gaohongyu789.top

Ruby: obj.instance_variables
来源：http://lmc.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://uri.gaohongyu789.top

================================================================================
来源：http://cfu.tianlin.xyz

H. 异常与错误处理
来源：http://jbt.cdnleiting.top

================================================================================
来源：http://ofw.cdnleiting.top

[H01] try / catch 基础
来源：http://qrk.shzxlz.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ajy.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qtn.haohaochexian.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rew.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hom.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dhe.jinqigfzy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cob.tian-w.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://atc.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bfn.ybcxt.top

[H02] finally / ensure 收尾
来源：http://avm.shanyushiyangkeji.top


<!-- 参考信息 -->