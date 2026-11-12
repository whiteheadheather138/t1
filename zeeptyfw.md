代发 wailian999

Ruby: s.lines
来源：http://ftk.wangdashe.top

C#:   s.Split('\n')
来源：http://aai.feifeiyinyue.top

[E20] 判断字符串是否为空
来源：http://sgt.guowangkeji.top

Py:   if not s:
来源：http://mnh.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://giz.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://haw.c1oappe.top

TS:   if (s === "") {}
来源：http://lot.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://dcy.guannengcc.top

Go:   if s == "" {}
来源：http://pht.birdmap.top

Ruby: if s.empty?
来源：http://llr.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://esp.yangfankeji.com

[E21] 超长截断加省略号
来源：http://ppa.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fms.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dol.meibo888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rse.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqe.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://icm.shanyushiyangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://wvf.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://msp.hcnkem.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jqc.ybcxt.top

[E22] 字节长度与字符长度
来源：http://bge.tian-w.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://scg.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fwc.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zql.zhoulong.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fwu.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://axk.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ptn.quarkkingdee.top

Ruby: s.bytesize;  s.length
来源：http://vjy.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ruf.jyoumei.cn

================================================================================
来源：http://eqd.52xcode.cn

F. 文件与目录
来源：http://lbh.dashuyun.cn

================================================================================
来源：http://pho.pycfn.com

[F01] 读取整个文件
来源：http://uqz.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vyd.shangyingyoupin.top

PHP:  file_get_contents("a.txt");
来源：http://oae.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vxy.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yxl.havefunace.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yhc.gaohongyu789.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hjz.daxiang520.top

Ruby: File.read("a.txt")
来源：http://dwb.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://qgh.fktsv.cn

[F02] 逐行读取文件
来源：http://iky.cheryme.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://phq.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://scb.kuanghao11.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://guy.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nhd.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bag.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rsc.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oji.hesvh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nyp.hnxiangtu.top

[F03] 写入文件（覆盖）
来源：http://kld.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fuz.epnwcf.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://pja.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dqg.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjb.bbcook.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://som.yueranfly.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gqi.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://bjg.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://heo.tarul.cn

[F04] 追加写入文件
来源：http://qos.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eio.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://izl.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uqf.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wzu.jinyuanbaomall.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kej.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iea.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mjp.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lga.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://inz.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qbm.havefunace.top

PHP:  file_exists("a.txt");
来源：http://gwl.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://fbb.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://bxw.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cuq.jyoumei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gsr.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://sqc.snrcjt.cn

C#:   File.Exists("a.txt")
来源：http://oeu.pycfn.com

[F06] 删除文件
来源：http://stu.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://ple.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://rrg.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://wxo.cashguo.top

TS:   fs.unlinkSync("a.txt")
来源：http://alt.xziqi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://flx.cheryme.top

Go:   os.Remove("a.txt")
来源：http://xva.yvedp.cn

Ruby: File.delete("a.txt")
来源：http://qul.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://mgc.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://ujx.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hyb.shanyushiyangkeji.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tux.zhoulong.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jde.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://srx.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://maa.jqgfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ohg.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zpb.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pmn.birdmap.top

[F08] 遍历目录
来源：http://wex.ydjk.org.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wij.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hap.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://nxc.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://xwf.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tzz.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kiu.shzxlz.cn

Ruby: Dir.children("dir")
来源：http://hzw.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://cxj.yonumen.top

[F09] 获取文件大小
来源：http://aol.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://hqn.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://okq.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://aao.quarkkingdee.top

TS:   fs.statSync("a.txt").size
来源：http://loo.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://nme.xuanzx.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gay.epnwcf.com

Ruby: File.size("a.txt")
来源：http://xla.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://gbt.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://nsd.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vyv.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hvg.pengpengdd.cyou

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wlw.hnxiangtu.top

TS:   path.extname("a.txt")
来源：http://ksp.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sbn.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mst.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eeu.andypj.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fqf.zycfv.cn

[F11] 复制与移动文件
来源：http://rcr.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gtg.zhaomingkeji.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rvc.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kfa.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://drh.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qbo.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ipj.nwbrower.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pkx.shzxlz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ruv.yj20258.top

[F12] CSV 读写
来源：http://cun.bbcook.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uie.hammf.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uga.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mqa.yongpay.top

TS:   // 同上
来源：http://kiz.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jdx.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cbq.havefunace.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dny.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://mzq.nanxinkj.top

================================================================================
来源：http://xsw.zdqjudy.top

G. 面向对象
来源：http://pvl.snrcjt.cn

================================================================================
来源：http://sub.nwbrower.top

[G01] 定义类
来源：http://oxi.shzxlz.cn

Py:   class User: pass
来源：http://qvz.hesvh.cn

PHP:  class User {}
来源：http://efj.ydjk.org.cn

JS:   class User {}
来源：http://xyt.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://uhd.jinyuanbaomall.cn

Java: class User {}
来源：http://qpb.hongshengwenyu.top

Go:   type User struct { Name string }
来源：http://hdy.yj202588.top

Ruby: class User; end
来源：http://nwb.fanxiaobao.xyz

C#:   class User {}
来源：http://elg.dianchejie.cn

[G02] 构造函数
来源：http://xgn.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://lac.bbcook.cn

PHP:  public function __construct(public string $name) {}
来源：http://nht.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://cwv.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://ion.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://hpb.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wgw.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://ciz.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://yhy.svipenyu.cn

[G03] 实例属性
来源：http://mcq.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://afv.pycfn.com

PHP:  public string $name = "x";
来源：http://qkq.zhoulong.xyz

JS:   this.name = "x";
来源：http://cpe.shzxlz.cn

TS:   name: string = "x";
来源：http://jef.xingfuxueyuan.xyz

Java: private String name;
来源：http://knh.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jge.fktsv.cn

Ruby: @name = "x"
来源：http://ray.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://aeg.sysykeji.top

[G04] 定义方法
来源：http://sll.wangdashe.top

Py:   def greet(self): return self.name
来源：http://ezm.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xkq.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://fnm.jlsjyb.cn

TS:   greet(): string { return this.name; }
来源：http://qhb.0kj1m.cn

Java: String greet() { return name; }
来源：http://gev.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://dtv.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://xgf.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://xbf.chenlongwang.top

[G05] 继承
来源：http://rew.uphjek.com

Py:   class Admin(User): pass
来源：http://dlw.hcnkem.com

PHP:  class Admin extends User {}
来源：http://yse.andypj.xyz

JS:   class Admin extends User {}
来源：http://jkl.wangdashe.top

TS:   class Admin extends User {}
来源：http://xqi.chenlongwang.top

Java: class Admin extends User {}
来源：http://iyk.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pir.vehdjk.com

Ruby: class Admin < User; end
来源：http://ekz.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://ywu.birdmap.top

[G06] 重写方法
来源：http://ecy.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://eru.daria6918.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kwn.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://bfv.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://nvo.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://ggp.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ykf.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://ull.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://uqt.xinyue.icu

[G07] 调用父类方法
来源：http://tkj.tianlin.xyz

Py:   super().greet()
来源：http://pnd.gogol.net.cn

PHP:  parent::greet();
来源：http://jfe.zhiwuduotai.top

JS:   super.greet();
来源：http://ucj.hywenlv.cn

TS:   super.greet();
来源：http://poh.zhixingplan.top

Java: super.greet();
来源：http://whj.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vqb.chenlongwang.top

Ruby: super
来源：http://xgo.jlsjyb.cn

C#:   base.Greet();
来源：http://ogs.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://gha.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eby.gogol.net.cn

PHP:  public static function f() {}
来源：http://odo.dianchejie.cn

JS:   static f() {}
来源：http://tod.mhx1999.top

TS:   static f(): void {}
来源：http://aow.yanxiufei.cn

Java: static void f() {}
来源：http://pzu.hesvh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bco.yvedp.cn

Ruby: def self.f; end
来源：http://rsi.0kj1m.cn

C#:   public static void F() {}
来源：http://eyk.guowangkeji.top

[G09] 接口 / 抽象类
来源：http://fzf.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://hve.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://xjw.hammf.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nob.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://vzm.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://qaz.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://ole.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hcq.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://sjo.xuanzx.com

[G10] 访问控制
来源：http://oqo.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://rdv.dashuyun.cn

PHP:  public / protected / private
来源：http://ipa.dashuyun.cn

JS:   #private 字段；其余公开
来源：http://wez.fktsv.cn

TS:   public / protected / private
来源：http://dkl.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://yud.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://tup.hnqzz.top

Ruby: public / protected / private
来源：http://ypq.dashuyun.cn

C#:   public / protected / private / internal
来源：http://avk.yueranfly.top

[G11] getter / setter
来源：http://xpk.cashguo.top

Py:   @property 与 @x.setter
来源：http://ana.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ego.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://ddc.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://qsb.tian-w.cn

Java: public String getName() { return name; }
来源：http://wfk.zhijiandao.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ncd.shzxlz.cn

Ruby: attr_accessor :name
来源：http://dxf.nanxinkj.top

C#:   public string Name { get; set; }
来源：http://qgh.yj20258.top

[G12] 对象转字符串
来源：http://rim.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://cnl.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://wxs.jyoumei.cn

JS:   toString() { return this.name; }
来源：http://hhw.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://wdx.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://hpv.guowangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://dxm.guannengcc.top

Ruby: def to_s; @name; end
来源：http://mld.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://izz.gotoacloud.top

[G13] 判断对象类型
来源：http://kbr.yj20258.top

Py:   isinstance(u, User)
来源：http://sgb.yfazqb.com

PHP:  $u instanceof User
来源：http://kip.smart0.xyz

JS:   u instanceof User
来源：http://lvc.c1oappe.top

TS:   u instanceof User
来源：http://ems.9152youxi.cn

Java: u instanceof User
来源：http://won.yj20258888.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bgj.xingfuxueyuan.xyz

Ruby: u.is_a?(User)
来源：http://zfh.yueranfly.top

C#:   u is User
来源：http://gdk.xuetiantiany.cn

[G14] 数据类 / record
来源：http://ppr.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nck.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://qhr.svipenyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ztv.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://ida.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://yig.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://ewk.aizwys.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jpb.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://ltr.uphjek.com

[G15] 枚举
来源：http://jas.yfazqb.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wck.hcnkem.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://ahk.hnxiangtu.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fku.zhongyouzk.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kvc.tarul.cn

Java: enum Color { RED, GREEN }
来源：http://een.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qso.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://wtf.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tkd.yj20258.top

[G16] 对象转数组 / 字典
来源：http://vhj.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ygi.bjfxy.top

PHP:  get_object_vars($obj);
来源：http://xcg.svipenyu.cn

JS:   Object.entries(obj)
来源：http://khr.fzhhl.top

TS:   Object.entries(obj)
来源：http://yaq.bbcook.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nda.tianlin.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://xgl.316326.xyz

Ruby: obj.instance_variables
来源：http://hyl.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://jlw.tanke756.top

================================================================================
来源：http://xmv.chenjidiqi.icu

H. 异常与错误处理
来源：http://kqv.fengsongda.top

================================================================================
来源：http://nit.9152youxi.cn

[H01] try / catch 基础
来源：http://msh.tianlin.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gsm.fengsongda.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ddc.sjlbkw.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vom.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qjd.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ref.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://emh.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wun.ybcxt.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jts.ydzc1.top

[H02] finally / ensure 收尾
来源：http://vvj.fktsv.cn


<!-- 参考信息 -->