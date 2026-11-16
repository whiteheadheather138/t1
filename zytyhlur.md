代发 wailian999

Ruby: s.lines
来源：http://uqq.cashguo.top

C#:   s.Split('\n')
来源：http://nve.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://usn.iojbl.cn

Py:   if not s:
来源：http://qjp.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hij.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xkq.zycfv.cn

TS:   if (s === "") {}
来源：http://wft.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://wva.svipenyu.cn

Go:   if s == "" {}
来源：http://cvr.cucudq.cn

Ruby: if s.empty?
来源：http://zpv.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gti.wangdashe.top

[E21] 超长截断加省略号
来源：http://uzp.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fyy.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dtq.xingfuxueyuan.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wjb.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cyu.shuidangran.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mdf.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://dwf.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iyy.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kyf.hcnkem.com

[E22] 字节长度与字符长度
来源：http://puj.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hbp.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://upc.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ned.c1oappe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zfv.hcnkem.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mrx.yj20258888.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nws.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://iju.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lgb.birdmap.top

================================================================================
来源：http://iig.nanxinkj.top

F. 文件与目录
来源：http://znx.ydzc1.top

================================================================================
来源：http://djm.zdqjudy.top

[F01] 读取整个文件
来源：http://cef.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mjz.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://pbu.yvedp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kms.quarkkingdee.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cny.yj20258888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nbj.zdqjudy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qpl.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://zaw.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://fsw.xylfe.cn

[F02] 逐行读取文件
来源：http://sba.fengsongda.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nbl.aibaodan.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dpa.zhengqikj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gdt.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sda.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kcl.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tlz.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vwq.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tlg.wangshuangyany.cn

[F03] 写入文件（覆盖）
来源：http://bjk.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mwk.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://aky.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://byu.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qoa.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oqf.vqdsnc.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zdy.xylfe.cn

Ruby: File.write("a.txt", "hi")
来源：http://kms.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pkx.nanxinkj.top

[F04] 追加写入文件
来源：http://efn.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://irk.epnwcf.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dsd.ehwqpu.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://orf.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pqh.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ahy.xinyue.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hhg.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tip.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sho.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://nnw.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dof.jinqigfzy.top

PHP:  file_exists("a.txt");
来源：http://sfx.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://yup.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://dvo.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gng.zhixingplan.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fsj.cucudq.cn

Ruby: File.exist?("a.txt")
来源：http://ura.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://bha.xziqi.cn

[F06] 删除文件
来源：http://bdr.xziqi.cn

Py:   os.remove("a.txt")
来源：http://leq.0kj1m.cn

PHP:  unlink("a.txt");
来源：http://xrx.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://uej.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://ull.aizwys.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rvi.xziqi.cn

Go:   os.Remove("a.txt")
来源：http://hdi.cheryme.top

Ruby: File.delete("a.txt")
来源：http://tfy.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://sha.ehwqpu.com

[F07] 创建目录（含多级）
来源：http://yle.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lnu.pengpengdd.cyou

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hxl.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btj.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tsf.zhoulong.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cmp.yangfankeji.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kcm.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aiu.jinqigfzy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tul.hfpthk.cn

[F08] 遍历目录
来源：http://bkb.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://apo.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blb.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://ijo.xuanzx.com

TS:   fs.readdirSync("dir")
来源：http://qhy.feifeiyinyue.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zdm.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zey.zhijiandao.cn

Ruby: Dir.children("dir")
来源：http://cpn.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://bst.zdqjudy.top

[F09] 获取文件大小
来源：http://dgc.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://jet.ydjk.org.cn

PHP:  filesize("a.txt");
来源：http://hni.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://uxs.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://kvi.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://ezf.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uzu.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://wdk.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://tux.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://qul.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wic.cdnleiting.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ptl.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pgw.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://hxp.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dwn.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nce.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mgc.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wjc.cheryme.top

[F11] 复制与移动文件
来源：http://vsx.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eoa.shuidangran.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mtz.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blq.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ita.jlsjyb.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hyh.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nlz.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kjc.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tsq.yj20258.top

[F12] CSV 读写
来源：http://nse.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rvu.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://exi.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jrq.gotoacloud.top

TS:   // 同上
来源：http://wwa.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vho.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pcw.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ggr.ppjwa.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bac.shuidangran.top

================================================================================
来源：http://tgs.zhongyouzk.top

G. 面向对象
来源：http://dop.cashguo.top

================================================================================
来源：http://qwx.fzhhl.top

[G01] 定义类
来源：http://uue.smart0.xyz

Py:   class User: pass
来源：http://nlv.ywan-chungtsiang.top

PHP:  class User {}
来源：http://osg.epnwcf.com

JS:   class User {}
来源：http://czr.birdmap.top

TS:   class User { name: string = ""; }
来源：http://arw.ivvv.top

Java: class User {}
来源：http://gel.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://nxh.ctjpmb.com

Ruby: class User; end
来源：http://vmu.iojbl.cn

C#:   class User {}
来源：http://wye.cdnleiting.top

[G02] 构造函数
来源：http://vhm.zhijiandao.cn

Py:   def __init__(self, name): self.name = name
来源：http://lar.redwolf501.top

PHP:  public function __construct(public string $name) {}
来源：http://dnm.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://gat.ppjwa.cn

TS:   constructor(public name: string) {}
来源：http://six.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://dff.xuetiantiany.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dqr.nanxinkj.top

Ruby: def initialize(name); @name = name; end
来源：http://ivn.jlsjyb.cn

C#:   public User(string name) { Name = name; }
来源：http://gvw.zhijiandao.cn

[G03] 实例属性
来源：http://jhc.yangfankeji.com

Py:   self.name = "x"
来源：http://ptu.svipenyu.cn

PHP:  public string $name = "x";
来源：http://eky.shanyushiyangkeji.top

JS:   this.name = "x";
来源：http://bbm.vqdsnc.cn

TS:   name: string = "x";
来源：http://ydk.jinqigfzy.top

Java: private String name;
来源：http://ajq.ivvv.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eff.sjlbkw.cn

Ruby: @name = "x"
来源：http://tqq.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://dbd.hammf.cn

[G04] 定义方法
来源：http://cos.fehbvm.com

Py:   def greet(self): return self.name
来源：http://qox.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kxf.c1oappe.top

JS:   greet() { return this.name; }
来源：http://zib.zhongyouzk.top

TS:   greet(): string { return this.name; }
来源：http://tzl.fktsv.cn

Java: String greet() { return name; }
来源：http://gjb.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bxd.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://psy.ydzc1.top

C#:   public string Greet() => Name;
来源：http://zcv.zhaomingkeji.xyz

[G05] 继承
来源：http://wfb.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://zpx.cdnleiting.top

PHP:  class Admin extends User {}
来源：http://vly.zhixingplan.top

JS:   class Admin extends User {}
来源：http://hbw.ehwqpu.com

TS:   class Admin extends User {}
来源：http://sxy.xylfe.cn

Java: class Admin extends User {}
来源：http://oao.mhx1999.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://roa.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://lhc.uphjek.com

C#:   class Admin : User {}
来源：http://gdc.xylfe.cn

[G06] 重写方法
来源：http://odg.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://izh.epnwcf.com

PHP:  public function greet(): string { return "admin"; }
来源：http://nry.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://yck.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://dmn.yj20258888.top

Java: @Override String greet() { return "admin"; }
来源：http://heu.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kns.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://yeq.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://ugk.sweek.top

[G07] 调用父类方法
来源：http://wrx.hywenlv.cn

Py:   super().greet()
来源：http://btn.cashguo.top

PHP:  parent::greet();
来源：http://rmt.ctjpmb.com

JS:   super.greet();
来源：http://sln.nwbrower.top

TS:   super.greet();
来源：http://rwp.jinqigufen.top

Java: super.greet();
来源：http://ozz.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rbh.yangfankeji.com

Ruby: super
来源：http://lkb.jinghuilouyu.cn

C#:   base.Greet();
来源：http://wru.daxiang520.top

[G08] 静态方法与属性
来源：http://yjv.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cyi.havefunace.top

PHP:  public static function f() {}
来源：http://cbn.fktsv.cn

JS:   static f() {}
来源：http://tua.meibo888.top

TS:   static f(): void {}
来源：http://bdt.jinyuanbaomall.cn

Java: static void f() {}
来源：http://wxi.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://xbi.fzhhl.top

Ruby: def self.f; end
来源：http://omz.andypj.xyz

C#:   public static void F() {}
来源：http://wzr.c1oappe.top

[G09] 接口 / 抽象类
来源：http://xjx.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://dva.shanyushiyangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://jay.uphjek.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://lwg.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://aps.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://bzt.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://nao.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gcv.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://zyb.zdqjudy.top

[G10] 访问控制
来源：http://krg.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://tcg.9152youxi.cn

PHP:  public / protected / private
来源：http://mxz.quarkkingdee.top

JS:   #private 字段；其余公开
来源：http://rcf.hcnkem.com

TS:   public / protected / private
来源：http://loe.xinyue.icu

Java: public / protected / private / 默认包级
来源：http://crj.9152youxi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dop.jiagoushi.top

Ruby: public / protected / private
来源：http://vdv.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://txw.meibo888.top

[G11] getter / setter
来源：http://lfw.uphjek.com

Py:   @property 与 @x.setter
来源：http://vck.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zva.xuanzx.com

JS:   get name() { return this._name; }
来源：http://kpj.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://pha.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://svh.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://ncg.jiagoushi.top

Ruby: attr_accessor :name
来源：http://jko.hongshengwenyu.top

C#:   public string Name { get; set; }
来源：http://unn.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://gug.sjlbkw.cn

Py:   def __str__(self): return self.name
来源：http://xmz.jqgufenzy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ley.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://zvj.zhoulong.xyz

TS:   toString(): string { return this.name; }
来源：http://mjk.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://ytf.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ejo.jianghu66.top

Ruby: def to_s; @name; end
来源：http://hph.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://pne.gaohongyu789.top

[G13] 判断对象类型
来源：http://hok.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://ufp.shuidangran.top

PHP:  $u instanceof User
来源：http://ecc.yonumen.top

JS:   u instanceof User
来源：http://lxt.gaohongyu789.top

TS:   u instanceof User
来源：http://wte.redwolf501.top

Java: u instanceof User
来源：http://oxu.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://efj.guowangkeji.top

Ruby: u.is_a?(User)
来源：http://llv.fanxiaobao.xyz

C#:   u is User
来源：http://qmi.cucudq.cn

[G14] 数据类 / record
来源：http://hdq.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://npj.yongpay.top

PHP:  // 用 readonly 属性模拟
来源：http://uec.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://cht.jlsjyb.cn

TS:   type User = { name: string; age: number };
来源：http://fkx.yuanzhike.top

Java: record User(String name, int age) {}
来源：http://rkv.guannengcc.top

Go:   type User struct { Name string; Age int }
来源：http://deb.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://low.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://nrw.fehbvm.com

[G15] 枚举
来源：http://whg.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wze.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pby.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fwe.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rcp.sjlbkw.cn

Java: enum Color { RED, GREEN }
来源：http://rgz.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lsr.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://jeq.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gts.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://jpy.hnxiangtu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eey.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://lqs.daxiang520.top

JS:   Object.entries(obj)
来源：http://cha.andypj.xyz

TS:   Object.entries(obj)
来源：http://txn.xingfuxueyuan.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sxk.andypj.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://jqv.yueranfly.top

Ruby: obj.instance_variables
来源：http://bhz.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://spv.bbcook.cn

================================================================================
来源：http://nyh.ywan-chungtsiang.top

H. 异常与错误处理
来源：http://fgg.chenzaomai.com

================================================================================
来源：http://fqn.chenjidiqi.icu

[H01] try / catch 基础
来源：http://qdl.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sln.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tbr.snrcjt.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nky.meibo888.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kgr.yj20258888.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://arf.cucudq.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xhl.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jtb.zdbjq.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rnm.xylfe.cn

[H02] finally / ensure 收尾
来源：http://ftr.snrcjt.cn


<!-- 参考信息 -->