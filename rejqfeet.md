代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://lte.316326.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lru.shanyushiyangtech.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gns.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ger.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jbo.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://rhv.mhx1999.top

Py:   s.splitlines()
来源：http://pjh.feifeiyinyue.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dsz.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://awe.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://aqq.nanxuanxn.top

Java: s.lines().toList()
来源：http://eng.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://vpo.ivvv.top

Ruby: s.lines
来源：http://hsw.shzxlz.cn

C#:   s.Split('\n')
来源：http://pax.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://xai.vqdsnc.cn

Py:   if not s:
来源：http://gyj.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sxg.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://znn.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://hlk.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://wml.sxryk.cn

Go:   if s == "" {}
来源：http://gxb.cheryme.top

Ruby: if s.empty?
来源：http://nqm.iojbl.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ahs.gzhubu.top

[E21] 超长截断加省略号
来源：http://ojw.fzhhl.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ley.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dqn.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hjq.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrn.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tbm.tianlin.xyz

Go:   // 按 rune 判断长度后截断
来源：http://pvc.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uou.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rpi.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://wlz.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jwy.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tev.shanyushiyangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ggb.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cpu.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jau.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qik.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://ayn.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dxa.vehdjk.com

================================================================================
来源：http://bye.cqqwz.cn

F. 文件与目录
来源：http://qls.tarul.cn

================================================================================
来源：http://zwl.aizwys.cn

[F01] 读取整个文件
来源：http://cqi.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ctw.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://pfe.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mkn.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xsd.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oox.snrcjt.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zux.jianghu66.top

Ruby: File.read("a.txt")
来源：http://zry.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://ktf.gotoacloud.top

[F02] 逐行读取文件
来源：http://fsn.hcnkem.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://usy.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jlg.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://grj.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kjy.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yeh.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mlo.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mqk.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vyj.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://gvo.iojbl.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tsz.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gxh.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jkp.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://upw.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pgg.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xml.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://eza.shanyushiyangtech.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zgl.zhixingplan.top

[F04] 追加写入文件
来源：http://lcp.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rtz.smart0.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ato.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jih.sufxvd.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ayr.yonumen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gng.ppjwa.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bsu.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cjl.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qej.nanxuanxn.top

[F05] 判断文件或目录是否存在
来源：http://dvz.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rjs.xuetiantiany.cn

PHP:  file_exists("a.txt");
来源：http://zee.xuanzx.com

JS:   fs.existsSync("a.txt")
来源：http://ysu.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://zwo.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cqy.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uim.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://lid.hammf.cn

C#:   File.Exists("a.txt")
来源：http://sqh.meibo888.top

[F06] 删除文件
来源：http://kpc.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://bqz.jlsjyb.cn

PHP:  unlink("a.txt");
来源：http://mao.yongpay.top

JS:   fs.unlinkSync("a.txt")
来源：http://bdr.ybcxt.top

TS:   fs.unlinkSync("a.txt")
来源：http://jzd.yvedp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://crq.ydzc1.top

Go:   os.Remove("a.txt")
来源：http://bbm.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://zmm.shuidangran.top

C#:   File.Delete("a.txt");
来源：http://qsn.daxiang520.top

[F07] 创建目录（含多级）
来源：http://bnf.vqdsnc.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cur.0kj1m.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://llf.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lsv.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ewd.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lhs.epnwcf.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ldk.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iuw.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qas.xziqi.cn

[F08] 遍历目录
来源：http://ohj.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://shg.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xna.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://xvq.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://skj.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dny.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://rxl.sufxvd.cn

Ruby: Dir.children("dir")
来源：http://lxl.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://cta.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://onf.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://zqg.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://cge.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://cou.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://bli.cqqwz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ojg.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kjy.tarul.cn

Ruby: File.size("a.txt")
来源：http://koe.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://doe.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://prs.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nxq.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://emf.dashuyun.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bey.jianghu66.top

TS:   path.extname("a.txt")
来源：http://ozt.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vfy.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://abf.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hqs.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qns.sysykeji.top

[F11] 复制与移动文件
来源：http://dqo.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rbw.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ges.feifeiyinyue.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tzu.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xra.vehdjk.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ncb.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://twu.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://owe.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qti.hywenlv.cn

[F12] CSV 读写
来源：http://wqx.hesvh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jma.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://app.daria6918.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kei.shuidangran.top

TS:   // 同上
来源：http://ush.hywenlv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bpm.svipenyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xzy.vehdjk.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mmy.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wba.shanyushiyangtech.top

================================================================================
来源：http://elc.haohaochexian.top

G. 面向对象
来源：http://pup.yueranfly.top

================================================================================
来源：http://zym.52xcode.cn

[G01] 定义类
来源：http://bgt.chenzaomai.com

Py:   class User: pass
来源：http://tbe.hfpthk.cn

PHP:  class User {}
来源：http://nsn.yfazqb.com

JS:   class User {}
来源：http://mgz.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://unm.daria6918.cn

Java: class User {}
来源：http://gpd.bjfxy.top

Go:   type User struct { Name string }
来源：http://oei.zhaomingkeji.xyz

Ruby: class User; end
来源：http://nwu.tarul.cn

C#:   class User {}
来源：http://hoy.hywenlv.cn

[G02] 构造函数
来源：http://pai.zhoulong.xyz

Py:   def __init__(self, name): self.name = name
来源：http://pgk.pengpengdd.cyou

PHP:  public function __construct(public string $name) {}
来源：http://fcr.pengpengdd.cyou

JS:   constructor(name) { this.name = name; }
来源：http://vzg.birdmap.top

TS:   constructor(public name: string) {}
来源：http://bmq.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://epc.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hse.ydjk.org.cn

Ruby: def initialize(name); @name = name; end
来源：http://jhe.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://ike.shzxlz.cn

[G03] 实例属性
来源：http://jja.jqgfzy.top

Py:   self.name = "x"
来源：http://yfv.iojbl.cn

PHP:  public string $name = "x";
来源：http://vat.jlsjyb.cn

JS:   this.name = "x";
来源：http://olg.jinyuanbaomall.cn

TS:   name: string = "x";
来源：http://wcq.jlsjyb.cn

Java: private String name;
来源：http://xwq.fanxiaobao.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hok.yvedp.cn

Ruby: @name = "x"
来源：http://ugx.hysaishi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ekf.ydjk.org.cn

[G04] 定义方法
来源：http://ruy.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://rzc.jqgfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://orn.yueranfly.top

JS:   greet() { return this.name; }
来源：http://nsk.bbcook.cn

TS:   greet(): string { return this.name; }
来源：http://bzc.daxiang520.top

Java: String greet() { return name; }
来源：http://cry.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://jvh.yvedp.cn

Ruby: def greet; @name; end
来源：http://wpz.vehdjk.com

C#:   public string Greet() => Name;
来源：http://sba.aizwys.cn

[G05] 继承
来源：http://kmg.cheryme.top

Py:   class Admin(User): pass
来源：http://zeo.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://fwh.xylfe.cn

JS:   class Admin extends User {}
来源：http://oxk.fehbvm.com

TS:   class Admin extends User {}
来源：http://dig.yj20258888.top

Java: class Admin extends User {}
来源：http://wna.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aps.jqgufenzy.top

Ruby: class Admin < User; end
来源：http://dox.zhijiandao.cn

C#:   class Admin : User {}
来源：http://swy.tarul.cn

[G06] 重写方法
来源：http://jpg.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://fey.316326.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://fce.uphjek.com

JS:   greet() { return "admin"; }
来源：http://zxc.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://yfd.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://cvp.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tqw.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://ffb.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://tzn.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://mnq.pycfn.com

Py:   super().greet()
来源：http://cxb.yonumen.top

PHP:  parent::greet();
来源：http://ihp.yfazqb.com

JS:   super.greet();
来源：http://vct.zdbjq.cn

TS:   super.greet();
来源：http://atu.snrcjt.cn

Java: super.greet();
来源：http://hht.birdmap.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ubi.havefunace.top

Ruby: super
来源：http://puy.fzhhl.top

C#:   base.Greet();
来源：http://xsw.cheryme.top

[G08] 静态方法与属性
来源：http://ary.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cfh.snrcjt.cn

PHP:  public static function f() {}
来源：http://atd.guowangkeji.top

JS:   static f() {}
来源：http://upr.ybcxt.top

TS:   static f(): void {}
来源：http://maj.aizwys.cn

Java: static void f() {}
来源：http://cdh.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gte.jinqigfzy.top

Ruby: def self.f; end
来源：http://qtr.yfazqb.com

C#:   public static void F() {}
来源：http://xca.daxiang520.top

[G09] 接口 / 抽象类
来源：http://aqc.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://hjm.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://aog.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nnx.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://pdz.ivvv.top

Java: interface Shape { double area(); }
来源：http://sqv.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://urr.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://udj.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://ict.ctjpmb.com

[G10] 访问控制
来源：http://zxw.hfpthk.cn

Py:   约定 _protected / __private（不强制）
来源：http://ycc.yuxming.cn

PHP:  public / protected / private
来源：http://yge.andypj.xyz

JS:   #private 字段；其余公开
来源：http://fxi.aibaodan.cn

TS:   public / protected / private
来源：http://jjb.shangyingyoupin.top

Java: public / protected / private / 默认包级
来源：http://mxd.bjfxy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ivq.cucudq.cn

Ruby: public / protected / private
来源：http://dgb.hywenlv.cn

C#:   public / protected / private / internal
来源：http://gtz.tarul.cn

[G11] getter / setter
来源：http://oaj.epnwcf.com

Py:   @property 与 @x.setter
来源：http://ojg.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ijy.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://tpt.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://uzb.sufxvd.cn

Java: public String getName() { return name; }
来源：http://roo.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hqm.vehdjk.com

Ruby: attr_accessor :name
来源：http://zgo.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://aey.zhijiandao.cn

[G12] 对象转字符串
来源：http://rcb.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://ybs.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://erx.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://sxk.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://ixm.yueranfly.top

Java: @Override public String toString() { return name; }
来源：http://tlo.vehdjk.com

Go:   func (u User) String() string { return u.Name }
来源：http://ril.vehdjk.com

Ruby: def to_s; @name; end
来源：http://mvl.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ein.wangdashe.top

[G13] 判断对象类型
来源：http://xwq.9152youxi.cn

Py:   isinstance(u, User)
来源：http://vue.ehwqpu.com

PHP:  $u instanceof User
来源：http://wjh.hysaishi.cn

JS:   u instanceof User
来源：http://lhd.jlsjyb.cn

TS:   u instanceof User
来源：http://jtz.cashguo.top

Java: u instanceof User
来源：http://axt.zdbjq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rgw.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://xzp.tian-w.cn

C#:   u is User
来源：http://oiz.zdqjudy.top

[G14] 数据类 / record
来源：http://arh.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tdd.xylfe.cn

PHP:  // 用 readonly 属性模拟
来源：http://kiy.xinyue.icu

JS:   // 无内置：普通类或对象字面量
来源：http://kqt.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://alh.jinqigfzy.top

Java: record User(String name, int age) {}
来源：http://hkl.hcnkem.com

Go:   type User struct { Name string; Age int }
来源：http://nzf.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://neg.gzhubu.top

C#:   record User(string Name, int Age);
来源：http://pwq.snrcjt.cn

[G15] 枚举
来源：http://vne.hysaishi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://guc.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://tfa.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kqv.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vin.wangdashe.top

Java: enum Color { RED, GREEN }
来源：http://gow.ctjpmb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kuq.gogol.net.cn

Ruby: Color = %i[red green].freeze
来源：http://bsk.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://znc.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://rpv.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xbg.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://yro.tian-w.cn

JS:   Object.entries(obj)
来源：http://gwy.iojbl.cn

TS:   Object.entries(obj)
来源：http://xdl.ybcxt.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dbp.ybcxt.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ulv.feifeiyinyue.top

Ruby: obj.instance_variables
来源：http://tef.hcnkem.com

C#:   // 用反射或 System.Text.Json
来源：http://rtt.ybcxt.top

================================================================================
来源：http://uzh.sweek.top


<!-- 参考信息 -->