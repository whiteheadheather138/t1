代发 wailian999

Ruby: s.lines
来源：http://brg.hcnkem.com

C#:   s.Split('\n')
来源：http://trx.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://mdj.wangdashe.top

Py:   if not s:
来源：http://dqi.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dtx.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rsc.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://znh.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://yxt.cucudq.cn

Go:   if s == "" {}
来源：http://abx.aibaodan.cn

Ruby: if s.empty?
来源：http://wyi.yfazqb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sgm.fktsv.cn

[E21] 超长截断加省略号
来源：http://wug.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jgx.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ckv.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdg.yueranfly.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kxg.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yij.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://xlw.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aqi.jqgfzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://awi.ydzc1.top

[E22] 字节长度与字符长度
来源：http://vsq.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cun.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xoy.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dpl.yongpay.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fnw.gaohongyu789.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mbj.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pgq.jqgufenzy.top

Ruby: s.bytesize;  s.length
来源：http://xrz.shanyushiyangkeji.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nyc.guowangkeji.top

================================================================================
来源：http://yfe.yvedp.cn

F. 文件与目录
来源：http://ifv.zhoulong.xyz

================================================================================
来源：http://hna.vehdjk.com

[F01] 读取整个文件
来源：http://pxk.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zpd.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://iue.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yvt.fanxiaobao.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://btl.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tdw.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lsz.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://euo.kuanghao11.cn

C#:   File.ReadAllText("a.txt");
来源：http://zdx.yangfankeji.com

[F02] 逐行读取文件
来源：http://wwd.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rug.jyoumei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://omn.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gau.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vvv.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sxt.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iky.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rrj.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wgl.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://qws.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ynv.dashuyun.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jat.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oto.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qzb.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gvt.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://flv.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://pqe.52xcode.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zfr.zhijiandao.cn

[F04] 追加写入文件
来源：http://cmo.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mvs.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cnq.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zop.yuxming.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tks.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sae.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xcf.yangfankeji.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hju.vehdjk.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://viz.yongpay.top

[F05] 判断文件或目录是否存在
来源：http://crv.c1oappe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eha.yongpay.top

PHP:  file_exists("a.txt");
来源：http://ele.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://rrs.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://qcf.hnqzz.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wfo.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jrp.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://hbh.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://wzv.cucudq.cn

[F06] 删除文件
来源：http://xxj.zhixingplan.top

Py:   os.remove("a.txt")
来源：http://iio.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://hqf.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://fmc.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qfn.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ams.0kj1m.cn

Go:   os.Remove("a.txt")
来源：http://kuk.yj20258.top

Ruby: File.delete("a.txt")
来源：http://kka.52xcode.cn

C#:   File.Delete("a.txt");
来源：http://zrz.xylfe.cn

[F07] 创建目录（含多级）
来源：http://lhq.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://etb.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jtp.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yaq.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pcc.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eca.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mob.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sgg.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rfz.hesvh.cn

[F08] 遍历目录
来源：http://xui.dashuyun.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gsw.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://unb.uphjek.com

JS:   fs.readdirSync("dir")
来源：http://jkq.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://tyf.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://thk.dianchejie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uqd.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://axt.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://hit.shangyingyoupin.top

[F09] 获取文件大小
来源：http://zwo.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://dqn.cheryme.top

PHP:  filesize("a.txt");
来源：http://aem.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://edt.hfpthk.cn

TS:   fs.statSync("a.txt").size
来源：http://mbo.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://tww.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mfz.9152youxi.cn

Ruby: File.size("a.txt")
来源：http://lnx.ybcxt.top

C#:   new FileInfo("a.txt").Length
来源：http://jtd.shanyushiyangtech.top

[F10] 取文件扩展名 / 文件名
来源：http://zua.xziqi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rhr.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ypu.shuidangran.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://myl.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://lnt.chenlongwang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nsq.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qys.xinyue.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tzy.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bkh.hysaishi.cn

[F11] 复制与移动文件
来源：http://jfw.daria6918.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rkt.yonumen.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ves.zhoulong.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mee.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oyb.yj20258.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dje.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qqf.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fzl.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yuj.mhx1999.top

[F12] CSV 读写
来源：http://nms.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zbz.yonumen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://egs.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wgp.jiagoushi.top

TS:   // 同上
来源：http://cij.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ikw.jqgufenzy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yqw.xziqi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jdp.sxryk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://owg.ctjpmb.com

================================================================================
来源：http://wmd.cucudq.cn

G. 面向对象
来源：http://zqp.ydzc1.top

================================================================================
来源：http://zyf.jqgufenzy.top

[G01] 定义类
来源：http://feu.hesvh.cn

Py:   class User: pass
来源：http://pgw.ybcxt.top

PHP:  class User {}
来源：http://auo.9152youxi.cn

JS:   class User {}
来源：http://qug.aibaodan.cn

TS:   class User { name: string = ""; }
来源：http://ijd.hfpthk.cn

Java: class User {}
来源：http://cjy.snrcjt.cn

Go:   type User struct { Name string }
来源：http://otj.zhengqikj.top

Ruby: class User; end
来源：http://ejs.zhongyouzk.top

C#:   class User {}
来源：http://clg.cashguo.top

[G02] 构造函数
来源：http://syi.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://hlk.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://oqm.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://ftg.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://ppr.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://cgy.nanxuanxn.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pog.sxryk.cn

Ruby: def initialize(name); @name = name; end
来源：http://mud.havefunace.top

C#:   public User(string name) { Name = name; }
来源：http://ion.xuetiantiany.cn

[G03] 实例属性
来源：http://nsw.hfpthk.cn

Py:   self.name = "x"
来源：http://knp.cashguo.top

PHP:  public string $name = "x";
来源：http://noh.uphjek.com

JS:   this.name = "x";
来源：http://vyj.hongshengwenyu.top

TS:   name: string = "x";
来源：http://oub.jyoumei.cn

Java: private String name;
来源：http://fgi.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vtz.vqdsnc.cn

Ruby: @name = "x"
来源：http://chs.hesvh.cn

C#:   public string Name { get; set; } = "x";
来源：http://mni.zycfv.cn

[G04] 定义方法
来源：http://xap.guannengcc.top

Py:   def greet(self): return self.name
来源：http://yup.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://noh.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://pyi.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://zmi.epnwcf.com

Java: String greet() { return name; }
来源：http://drh.yangfankeji.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://kkj.yj20258888.top

Ruby: def greet; @name; end
来源：http://uov.cucudq.cn

C#:   public string Greet() => Name;
来源：http://sey.316326.xyz

[G05] 继承
来源：http://rvw.xziqi.cn

Py:   class Admin(User): pass
来源：http://mxf.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://bne.ehwqpu.com

JS:   class Admin extends User {}
来源：http://juu.yuanzhike.top

TS:   class Admin extends User {}
来源：http://cqr.jqgfzy.top

Java: class Admin extends User {}
来源：http://pll.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ljo.cqqwz.cn

Ruby: class Admin < User; end
来源：http://grs.nanxuanxn.top

C#:   class Admin : User {}
来源：http://xyl.fktsv.cn

[G06] 重写方法
来源：http://owz.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://dkk.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lhp.cashguo.top

JS:   greet() { return "admin"; }
来源：http://zao.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://ckp.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://pyt.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zyf.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://igj.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://miv.xuanzx.com

[G07] 调用父类方法
来源：http://jrc.jlsjyb.cn

Py:   super().greet()
来源：http://gne.tian-w.cn

PHP:  parent::greet();
来源：http://sti.tian-w.cn

JS:   super.greet();
来源：http://uve.yanxiufei.cn

TS:   super.greet();
来源：http://azt.sxryk.cn

Java: super.greet();
来源：http://aba.gotoacloud.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qiy.yvedp.cn

Ruby: super
来源：http://suh.quarkkingdee.top

C#:   base.Greet();
来源：http://tod.nanxinkj.top

[G08] 静态方法与属性
来源：http://iuo.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bcm.hcnkem.com

PHP:  public static function f() {}
来源：http://yhj.vehdjk.com

JS:   static f() {}
来源：http://cwc.jianghu66.top

TS:   static f(): void {}
来源：http://bks.xuanzx.com

Java: static void f() {}
来源：http://ypq.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nfa.zhoulong.xyz

Ruby: def self.f; end
来源：http://hod.ybcxt.top

C#:   public static void F() {}
来源：http://wzd.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://wfc.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://mhn.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://plm.zhixingplan.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cfr.mhx1999.top

TS:   interface Shape { area(): number; }
来源：http://guu.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://tkm.yongpay.top

Go:   type Shape interface { Area() float64 }
来源：http://wns.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://otj.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://bbb.aizwys.cn

[G10] 访问控制
来源：http://dhs.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://rsx.shzxlz.cn

PHP:  public / protected / private
来源：http://hrl.fzhhl.top

JS:   #private 字段；其余公开
来源：http://row.birdmap.top

TS:   public / protected / private
来源：http://ypp.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://zbb.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://njg.tian-w.cn

Ruby: public / protected / private
来源：http://cwd.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://qhj.zycfv.cn

[G11] getter / setter
来源：http://rhz.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://ibk.redwolf501.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ycu.yongpay.top

JS:   get name() { return this._name; }
来源：http://edr.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://yxa.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://chy.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://yhk.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://lfy.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://nfs.316326.xyz

[G12] 对象转字符串
来源：http://gnf.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://siy.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lru.hammf.cn

JS:   toString() { return this.name; }
来源：http://cgo.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://nrc.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://ipf.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://exy.jqgfzy.top

Ruby: def to_s; @name; end
来源：http://xht.fzhhl.top

C#:   public override string ToString() => Name;
来源：http://exn.jqgufenzy.top

[G13] 判断对象类型
来源：http://pup.ybcxt.top

Py:   isinstance(u, User)
来源：http://dxy.cdnleiting.top

PHP:  $u instanceof User
来源：http://vhl.yuanzhike.top

JS:   u instanceof User
来源：http://ofn.xinyue.icu

TS:   u instanceof User
来源：http://dht.dianchejie.cn

Java: u instanceof User
来源：http://xsq.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eff.hongshengwenyu.top

Ruby: u.is_a?(User)
来源：http://ppv.316326.xyz

C#:   u is User
来源：http://ijt.jianghu66.top

[G14] 数据类 / record
来源：http://ecm.zhixingplan.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zop.ywan-chungtsiang.top

PHP:  // 用 readonly 属性模拟
来源：http://wlu.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://dbu.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://bzi.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://zwo.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://ofo.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pdc.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://edf.redwolf501.top

[G15] 枚举
来源：http://cxz.hongshengwenyu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fgv.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://msk.zhengqikj.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bnl.shzxlz.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gbh.gotoacloud.top

Java: enum Color { RED, GREEN }
来源：http://epp.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pwd.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://kpz.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jgd.zdqjudy.top

[G16] 对象转数组 / 字典
来源：http://uwk.hywenlv.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mds.hesvh.cn

PHP:  get_object_vars($obj);
来源：http://gju.bjfxy.top

JS:   Object.entries(obj)
来源：http://jlc.shangyingyoupin.top

TS:   Object.entries(obj)
来源：http://vtz.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nsr.zycfv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ufk.epnwcf.com

Ruby: obj.instance_variables
来源：http://ttf.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://bra.pycfn.com

================================================================================
来源：http://iwb.zhongyouzk.top

H. 异常与错误处理
来源：http://mek.sweek.top

================================================================================
来源：http://dbx.zhixingplan.top

[H01] try / catch 基础
来源：http://icm.c1oappe.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://egl.shzxlz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yra.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vpw.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jre.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uhw.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ped.vehdjk.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mdm.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qee.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://mqi.dashuyun.cn


<!-- 参考信息 -->