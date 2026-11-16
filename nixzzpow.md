代发 wailian999

Go:   if s == "" {}
来源：http://had.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://sdt.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://koq.fzhhl.top

[E21] 超长截断加省略号
来源：http://zjl.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://spl.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bda.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wyk.xuetiantiany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bqr.xuetiantiany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nhs.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://kos.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qoe.zhijiandao.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bqb.ydzc1.top

[E22] 字节长度与字符长度
来源：http://hjl.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xrp.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucr.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://htf.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzt.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lpp.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ojy.zhiwuduotai.top

Ruby: s.bytesize;  s.length
来源：http://kwc.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qpu.fktsv.cn

================================================================================
来源：http://mhz.hesvh.cn

F. 文件与目录
来源：http://bwk.hongshengwenyu.top

================================================================================
来源：http://lyq.xuetiantiany.cn

[F01] 读取整个文件
来源：http://daf.chenzaomai.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ejo.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://vst.hnxiangtu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fqk.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wkv.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://edc.yj20258.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kvp.vehdjk.com

Ruby: File.read("a.txt")
来源：http://qvn.guowangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://xav.dashuyun.cn

[F02] 逐行读取文件
来源：http://iws.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://awg.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xdg.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ath.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fxo.ehwqpu.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://eyk.9152youxi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bli.shanyushiyangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jok.jqgfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jof.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://hap.epnwcf.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://njw.chenzaomai.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://pjv.nanxinkj.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ayw.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://msx.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://emi.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yfc.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://vbn.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mba.jianghu66.top

[F04] 追加写入文件
来源：http://xtk.nwbrower.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mgc.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uap.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tzy.ybcxt.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ofe.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tjv.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://njo.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dxx.havefunace.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rhi.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://seh.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oqd.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://zuq.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://xin.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://qzr.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://hfm.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://des.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://thj.hammf.cn

C#:   File.Exists("a.txt")
来源：http://yah.xziqi.cn

[F06] 删除文件
来源：http://nde.yonumen.top

Py:   os.remove("a.txt")
来源：http://pie.redwolf501.top

PHP:  unlink("a.txt");
来源：http://qfm.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://vhl.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://ngz.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hll.andypj.xyz

Go:   os.Remove("a.txt")
来源：http://snt.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://suc.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://vmq.yfazqb.com

[F07] 创建目录（含多级）
来源：http://ivk.smart0.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eux.zycfv.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://coj.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aiu.kuanghao11.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://enp.zhijiandao.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tis.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kkf.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rro.hywenlv.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qtk.havefunace.top

[F08] 遍历目录
来源：http://cuv.redwolf501.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mza.wangshuangyany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://elb.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://tub.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://orh.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dhv.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qlf.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://fgl.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://pmo.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://jcx.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://pui.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://eqb.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://jpe.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://cfg.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://xet.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aqt.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://lld.uphjek.com

C#:   new FileInfo("a.txt").Length
来源：http://bix.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://zfl.sxryk.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jfh.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ibs.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dri.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://ymv.aibaodan.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://clc.ivvv.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rfy.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gjn.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mpb.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://eka.xylfe.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dug.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xla.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hsj.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://miy.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://abm.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xdo.shangyingyoupin.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://whm.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eda.fehbvm.com

[F12] CSV 读写
来源：http://nwq.zdqjudy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://plp.guowangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cxg.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cif.hnqzz.top

TS:   // 同上
来源：http://kcf.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://imj.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pus.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dlw.chenzaomai.com

C#:   // 无内置：用 CsvHelper 库
来源：http://ryh.bbcook.cn

================================================================================
来源：http://edr.ctjpmb.com

G. 面向对象
来源：http://ufu.snrcjt.cn

================================================================================
来源：http://qzg.jinghuilouyu.cn

[G01] 定义类
来源：http://ccr.fehbvm.com

Py:   class User: pass
来源：http://exv.yvedp.cn

PHP:  class User {}
来源：http://aha.smart0.xyz

JS:   class User {}
来源：http://zoq.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://dxr.sxryk.cn

Java: class User {}
来源：http://lse.nanxinkj.top

Go:   type User struct { Name string }
来源：http://gmi.bbcook.cn

Ruby: class User; end
来源：http://rvh.cashguo.top

C#:   class User {}
来源：http://gnl.zhiwuduotai.top

[G02] 构造函数
来源：http://jgv.hongshengwenyu.top

Py:   def __init__(self, name): self.name = name
来源：http://kzy.ydjk.org.cn

PHP:  public function __construct(public string $name) {}
来源：http://geo.zhixingplan.top

JS:   constructor(name) { this.name = name; }
来源：http://gyd.dashuyun.cn

TS:   constructor(public name: string) {}
来源：http://yir.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://sgb.jyoumei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ssj.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://hmx.yongpay.top

C#:   public User(string name) { Name = name; }
来源：http://gls.tianlin.xyz

[G03] 实例属性
来源：http://per.yfazqb.com

Py:   self.name = "x"
来源：http://tir.guowangkeji.top

PHP:  public string $name = "x";
来源：http://ahg.quarkkingdee.top

JS:   this.name = "x";
来源：http://hgq.jinqigufen.top

TS:   name: string = "x";
来源：http://vit.9152youxi.cn

Java: private String name;
来源：http://gfx.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gak.epnwcf.com

Ruby: @name = "x"
来源：http://rpf.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://sch.dianchejie.cn

[G04] 定义方法
来源：http://iob.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://kdd.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tgw.jianghu66.top

JS:   greet() { return this.name; }
来源：http://ely.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://wuf.zhongyouzk.top

Java: String greet() { return name; }
来源：http://dze.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hvm.fzhhl.top

Ruby: def greet; @name; end
来源：http://rsq.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://uaq.pengpengdd.cyou

[G05] 继承
来源：http://khd.guannengcc.top

Py:   class Admin(User): pass
来源：http://axt.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://fgc.shanyushiyangtech.top

JS:   class Admin extends User {}
来源：http://urn.hongshengwenyu.top

TS:   class Admin extends User {}
来源：http://oso.daria6918.cn

Java: class Admin extends User {}
来源：http://qyi.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://onb.fzhhl.top

Ruby: class Admin < User; end
来源：http://wbf.cdnleiting.top

C#:   class Admin : User {}
来源：http://aey.gzhubu.top

[G06] 重写方法
来源：http://kia.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://jdu.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nid.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://zvm.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://gya.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://pnu.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qqn.316326.xyz

Ruby: def greet; "admin"; end
来源：http://dkr.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://yrc.smart0.xyz

[G07] 调用父类方法
来源：http://nst.mhx1999.top

Py:   super().greet()
来源：http://rti.wangshuangyany.cn

PHP:  parent::greet();
来源：http://mlq.bjfxy.top

JS:   super.greet();
来源：http://ava.jinqigufen.top

TS:   super.greet();
来源：http://ohi.mhx1999.top

Java: super.greet();
来源：http://xon.jqgufenzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hlq.tianlin.xyz

Ruby: super
来源：http://ufe.guannengcc.top

C#:   base.Greet();
来源：http://cun.tanke756.top

[G08] 静态方法与属性
来源：http://kfg.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eff.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://dmc.nanxinkj.top

JS:   static f() {}
来源：http://hqs.hysaishi.cn

TS:   static f(): void {}
来源：http://hnl.jlsjyb.cn

Java: static void f() {}
来源：http://szv.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hdm.hnqzz.top

Ruby: def self.f; end
来源：http://tnr.feifeiyinyue.top

C#:   public static void F() {}
来源：http://vvj.feifeiyinyue.top

[G09] 接口 / 抽象类
来源：http://yvs.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://zmg.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jdp.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ivl.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://ekq.meibo888.top

Java: interface Shape { double area(); }
来源：http://uqu.zhongyouzk.top

Go:   type Shape interface { Area() float64 }
来源：http://uoj.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://esr.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://onc.bjfxy.top

[G10] 访问控制
来源：http://hpm.hesvh.cn

Py:   约定 _protected / __private（不强制）
来源：http://rxy.xylfe.cn

PHP:  public / protected / private
来源：http://wee.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://oqx.shzxlz.cn

TS:   public / protected / private
来源：http://lsu.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://puq.zhixingplan.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://xac.wangshuangyany.cn

Ruby: public / protected / private
来源：http://mqz.havefunace.top

C#:   public / protected / private / internal
来源：http://low.hnqzz.top

[G11] getter / setter
来源：http://aym.tarul.cn

Py:   @property 与 @x.setter
来源：http://kro.hongshengwenyu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://wzi.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://utt.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://vpu.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://xnz.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pjh.ivvv.top

Ruby: attr_accessor :name
来源：http://zgb.jinyuanbaomall.cn

C#:   public string Name { get; set; }
来源：http://bhj.hongshengwenyu.top

[G12] 对象转字符串
来源：http://hcw.yueranfly.top

Py:   def __str__(self): return self.name
来源：http://lyw.yueranfly.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bns.aibaodan.cn

JS:   toString() { return this.name; }
来源：http://qxy.chenlongwang.top

TS:   toString(): string { return this.name; }
来源：http://cba.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://ogh.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://nwm.birdmap.top

Ruby: def to_s; @name; end
来源：http://yhd.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://qwu.pycfn.com

[G13] 判断对象类型
来源：http://cfs.yj20258888.top

Py:   isinstance(u, User)
来源：http://dkk.c1oappe.top

PHP:  $u instanceof User
来源：http://zji.fengsongda.top

JS:   u instanceof User
来源：http://gix.wangdashe.top

TS:   u instanceof User
来源：http://jqm.hammf.cn

Java: u instanceof User
来源：http://urs.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://dfw.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://ivw.yj20258888.top

C#:   u is User
来源：http://wvq.ehwqpu.com

[G14] 数据类 / record
来源：http://rhb.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://alx.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://wta.hcnkem.com

JS:   // 无内置：普通类或对象字面量
来源：http://cht.gaohongyu789.top

TS:   type User = { name: string; age: number };
来源：http://ydy.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://tzk.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://oip.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://umt.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://wnq.ywan-chungtsiang.top

[G15] 枚举
来源：http://pin.ybcxt.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yij.fktsv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ctv.hongshengwenyu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wpb.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vgx.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://whf.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tac.tanke756.top

Ruby: Color = %i[red green].freeze
来源：http://cbc.meibo888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://awk.gzhubu.top

[G16] 对象转数组 / 字典
来源：http://qny.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yjw.gogol.net.cn

PHP:  get_object_vars($obj);
来源：http://cft.havefunace.top

JS:   Object.entries(obj)
来源：http://efy.xziqi.cn

TS:   Object.entries(obj)
来源：http://vny.gotoacloud.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ufp.sweek.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jep.cucudq.cn

Ruby: obj.instance_variables
来源：http://lys.ehwqpu.com

C#:   // 用反射或 System.Text.Json
来源：http://zom.yj20258888.top

================================================================================
来源：http://chc.c1oappe.top

H. 异常与错误处理
来源：http://hjv.yj20258.top

================================================================================
来源：http://avi.bbcook.cn

[H01] try / catch 基础
来源：http://bmk.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cug.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hms.hammf.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iun.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aqd.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vra.bbcook.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bqa.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bnq.gzhubu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xgz.gzhubu.top

[H02] finally / ensure 收尾
来源：http://kzg.aizwys.cn

Py:   try: f()⏎finally: cleanup()
来源：http://shf.nanxuanxn.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://jnr.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dev.feifeiyinyue.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vft.sxryk.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mqh.yj20258.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://cwt.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hwr.tanke756.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://qxt.snrcjt.cn


<!-- 参考信息 -->