代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://lqq.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://uta.chenjidiqi.icu

Java: s.lines().toList()
来源：http://iyw.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://cex.yuanzhike.top

Ruby: s.lines
来源：http://ajz.wangdashe.top

C#:   s.Split('\n')
来源：http://fbs.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://juq.nwbrower.top

Py:   if not s:
来源：http://iri.cheryme.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lun.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lre.zdbjq.cn

TS:   if (s === "") {}
来源：http://pzf.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://nwx.uphjek.com

Go:   if s == "" {}
来源：http://rol.hammf.cn

Ruby: if s.empty?
来源：http://atm.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gso.gzhubu.top

[E21] 超长截断加省略号
来源：http://dzu.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jbg.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ixi.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zrc.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uye.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cao.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://bux.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nzs.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jpf.daxiang520.top

[E22] 字节长度与字符长度
来源：http://uvb.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bja.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sxz.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pid.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ode.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qyh.ybcxt.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vtf.9152youxi.cn

Ruby: s.bytesize;  s.length
来源：http://dgl.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wxw.quarkkingdee.top

================================================================================
来源：http://mqm.c1oappe.top

F. 文件与目录
来源：http://vvp.epnwcf.com

================================================================================
来源：http://tbw.zhijiandao.cn

[F01] 读取整个文件
来源：http://bvj.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://crt.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://jon.smart0.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zgy.xziqi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vzm.9152youxi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qkg.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mjj.shanyushiyangkeji.top

Ruby: File.read("a.txt")
来源：http://spg.hammf.cn

C#:   File.ReadAllText("a.txt");
来源：http://xba.hywenlv.cn

[F02] 逐行读取文件
来源：http://kbr.dianchejie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mts.hongshengwenyu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xyj.yj20258.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ynj.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rxr.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yyw.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jbr.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jwa.shanyushiyangtech.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fjd.yuxming.cn

[F03] 写入文件（覆盖）
来源：http://eil.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jzw.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vfx.bbcook.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yvi.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fer.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wft.yongpay.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://skc.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://ejk.andypj.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oru.iojbl.cn

[F04] 追加写入文件
来源：http://zqp.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dzk.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hrd.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pmh.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xan.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iof.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lye.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xwj.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urc.tanke756.top

[F05] 判断文件或目录是否存在
来源：http://noa.chenjidiqi.icu

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lbu.mhx1999.top

PHP:  file_exists("a.txt");
来源：http://nog.yfazqb.com

JS:   fs.existsSync("a.txt")
来源：http://hjt.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://jmc.ydjk.org.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xsd.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rns.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://slz.wangdashe.top

C#:   File.Exists("a.txt")
来源：http://bxg.fanxiaobao.xyz

[F06] 删除文件
来源：http://hqn.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://bnc.yfazqb.com

PHP:  unlink("a.txt");
来源：http://amn.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pzn.yfazqb.com

TS:   fs.unlinkSync("a.txt")
来源：http://duy.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bmy.pycfn.com

Go:   os.Remove("a.txt")
来源：http://pll.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://yjt.uphjek.com

C#:   File.Delete("a.txt");
来源：http://fao.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://cxa.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wcy.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://myu.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lht.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vhk.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qfz.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://saq.nwbrower.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wcr.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ceu.fehbvm.com

[F08] 遍历目录
来源：http://ylh.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gpa.mhx1999.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://syw.yuxming.cn

JS:   fs.readdirSync("dir")
来源：http://ltb.xuetiantiany.cn

TS:   fs.readdirSync("dir")
来源：http://pur.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jyq.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rfz.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://lxq.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://egq.svipenyu.cn

[F09] 获取文件大小
来源：http://nuu.xingfuxueyuan.xyz

Py:   os.path.getsize("a.txt")
来源：http://xmc.316326.xyz

PHP:  filesize("a.txt");
来源：http://jgq.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://kxq.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://tvw.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://kmp.gaohongyu789.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hqu.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://xkr.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://fdb.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://kil.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hpd.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aij.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uth.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://nyq.wangdashe.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ezh.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://snp.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oym.0kj1m.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zuq.uphjek.com

[F11] 复制与移动文件
来源：http://gpr.9152youxi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://edt.iojbl.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://izf.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qrq.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lnk.kuanghao11.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ynp.yj20258.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://was.zhiwuduotai.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mip.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vyb.iojbl.cn

[F12] CSV 读写
来源：http://fug.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://atl.haohaochexian.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://smq.cdnleiting.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://doa.iojbl.cn

TS:   // 同上
来源：http://ngl.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lpq.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lrz.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fzh.kuanghao11.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ggl.dianchejie.cn

================================================================================
来源：http://oyt.sjlbkw.cn

G. 面向对象
来源：http://htl.dashuyun.cn

================================================================================
来源：http://ipw.sufxvd.cn

[G01] 定义类
来源：http://kmy.sysykeji.top

Py:   class User: pass
来源：http://jib.cdnleiting.top

PHP:  class User {}
来源：http://ajk.fehbvm.com

JS:   class User {}
来源：http://art.hcnkem.com

TS:   class User { name: string = ""; }
来源：http://fol.yj202588.top

Java: class User {}
来源：http://ehn.ctjpmb.com

Go:   type User struct { Name string }
来源：http://xjj.jinyuanbaomall.cn

Ruby: class User; end
来源：http://zqp.shzxlz.cn

C#:   class User {}
来源：http://ybr.jiagoushi.top

[G02] 构造函数
来源：http://njl.ivvv.top

Py:   def __init__(self, name): self.name = name
来源：http://dej.hfpthk.cn

PHP:  public function __construct(public string $name) {}
来源：http://pna.svipenyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ypf.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://udm.hesvh.cn

Java: User(String name) { this.name = name; }
来源：http://tom.ywan-chungtsiang.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jer.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://xhz.jiagoushi.top

C#:   public User(string name) { Name = name; }
来源：http://qkq.gzhubu.top

[G03] 实例属性
来源：http://qag.kuanghao11.cn

Py:   self.name = "x"
来源：http://rfx.haohaochexian.top

PHP:  public string $name = "x";
来源：http://bam.jlsjyb.cn

JS:   this.name = "x";
来源：http://gax.yfazqb.com

TS:   name: string = "x";
来源：http://apk.ivvv.top

Java: private String name;
来源：http://phf.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kfx.tian-w.cn

Ruby: @name = "x"
来源：http://aex.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://zjc.birdmap.top

[G04] 定义方法
来源：http://lfr.zhixingplan.top

Py:   def greet(self): return self.name
来源：http://wtm.sysykeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dgi.cashguo.top

JS:   greet() { return this.name; }
来源：http://xcc.sxryk.cn

TS:   greet(): string { return this.name; }
来源：http://tnt.redwolf501.top

Java: String greet() { return name; }
来源：http://ibe.zycfv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wcf.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://thq.jinqigufen.top

C#:   public string Greet() => Name;
来源：http://jvc.mhx1999.top

[G05] 继承
来源：http://gge.shuidangran.top

Py:   class Admin(User): pass
来源：http://hxa.svipenyu.cn

PHP:  class Admin extends User {}
来源：http://anm.bjfxy.top

JS:   class Admin extends User {}
来源：http://zem.cheryme.top

TS:   class Admin extends User {}
来源：http://gwv.birdmap.top

Java: class Admin extends User {}
来源：http://dik.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://stb.guowangkeji.top

Ruby: class Admin < User; end
来源：http://laq.vehdjk.com

C#:   class Admin : User {}
来源：http://ale.zdbjq.cn

[G06] 重写方法
来源：http://prf.fanxiaobao.xyz

Py:   def greet(self): return "admin"
来源：http://rnm.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nez.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://usb.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://okn.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://kmu.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wfx.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://off.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://wcr.fengsongda.top

[G07] 调用父类方法
来源：http://grj.jinghuilouyu.cn

Py:   super().greet()
来源：http://ixm.xziqi.cn

PHP:  parent::greet();
来源：http://nwe.yj20258.top

JS:   super.greet();
来源：http://mep.vqdsnc.cn

TS:   super.greet();
来源：http://vby.fanxiaobao.xyz

Java: super.greet();
来源：http://bnv.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wri.birdmap.top

Ruby: super
来源：http://fqp.pengpengdd.cyou

C#:   base.Greet();
来源：http://zdk.0kj1m.cn

[G08] 静态方法与属性
来源：http://ews.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bki.shuidangran.top

PHP:  public static function f() {}
来源：http://ldm.52xcode.cn

JS:   static f() {}
来源：http://iut.daria6918.cn

TS:   static f(): void {}
来源：http://srx.wangdashe.top

Java: static void f() {}
来源：http://emj.zhixingplan.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rwp.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://iqc.ydzc1.top

C#:   public static void F() {}
来源：http://ecb.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://ubu.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://mmm.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://tao.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fic.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://xgm.yuxming.cn

Java: interface Shape { double area(); }
来源：http://hfp.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://qdy.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ukm.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://arq.haohaochexian.top

[G10] 访问控制
来源：http://kbp.xuetiantiany.cn

Py:   约定 _protected / __private（不强制）
来源：http://agh.fengsongda.top

PHP:  public / protected / private
来源：http://ybz.cdnleiting.top

JS:   #private 字段；其余公开
来源：http://tsg.52xcode.cn

TS:   public / protected / private
来源：http://fwa.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://wfo.tian-w.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yix.jinqigfzy.top

Ruby: public / protected / private
来源：http://gid.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://bzr.cucudq.cn

[G11] getter / setter
来源：http://uzx.yongpay.top

Py:   @property 与 @x.setter
来源：http://cmq.52xcode.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cdd.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://vsl.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://ecw.fengsongda.top

Java: public String getName() { return name; }
来源：http://cjd.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gws.ivvv.top

Ruby: attr_accessor :name
来源：http://aew.fanxiaobao.xyz

C#:   public string Name { get; set; }
来源：http://yrh.ppjwa.cn

[G12] 对象转字符串
来源：http://pkm.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://gae.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://hoj.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://hmi.yueranfly.top

TS:   toString(): string { return this.name; }
来源：http://oht.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://ytb.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://mut.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://uxf.xylfe.cn

C#:   public override string ToString() => Name;
来源：http://awf.zhixingplan.top

[G13] 判断对象类型
来源：http://lsw.gzhubu.top

Py:   isinstance(u, User)
来源：http://bal.haohaochexian.top

PHP:  $u instanceof User
来源：http://aid.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://gpr.haohaochexian.top

TS:   u instanceof User
来源：http://qit.mhx1999.top

Java: u instanceof User
来源：http://fip.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vra.gotoacloud.top

Ruby: u.is_a?(User)
来源：http://rgz.jinqigfzy.top

C#:   u is User
来源：http://ejr.ivvv.top

[G14] 数据类 / record
来源：http://ndz.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cne.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://cvf.haohaochexian.top

JS:   // 无内置：普通类或对象字面量
来源：http://kff.xinyue.icu

TS:   type User = { name: string; age: number };
来源：http://vya.fktsv.cn

Java: record User(String name, int age) {}
来源：http://jcu.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://tsc.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dck.tanke756.top

C#:   record User(string Name, int Age);
来源：http://ktl.tian-w.cn

[G15] 枚举
来源：http://bfv.vehdjk.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kpl.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://muo.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ukp.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://npf.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://hol.svipenyu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ple.cqqwz.cn

Ruby: Color = %i[red green].freeze
来源：http://zvq.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iqy.zycfv.cn

[G16] 对象转数组 / 字典
来源：http://yki.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://egz.jqgufenzy.top

PHP:  get_object_vars($obj);
来源：http://xiw.ppjwa.cn

JS:   Object.entries(obj)
来源：http://lcb.jyoumei.cn

TS:   Object.entries(obj)
来源：http://efe.yonumen.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fci.sxryk.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jue.bjfxy.top

Ruby: obj.instance_variables
来源：http://htj.hammf.cn

C#:   // 用反射或 System.Text.Json
来源：http://azf.tian-w.cn

================================================================================
来源：http://skc.cashguo.top

H. 异常与错误处理
来源：http://vaw.fktsv.cn

================================================================================
来源：http://uoh.shuidangran.top

[H01] try / catch 基础
来源：http://sob.xylfe.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://chj.ybcxt.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mpm.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hxt.yj20258888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sdm.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://guo.jlsjyb.cn


<!-- 参考信息 -->