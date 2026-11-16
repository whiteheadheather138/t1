代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://lqf.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fia.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qra.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iqn.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bqr.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://qgw.wangdashe.top

Py:   s.splitlines()
来源：http://cra.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rnt.daria6918.cn

JS:   s.split(/\r?\n/)
来源：http://kvd.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://yit.jqgufenzy.top

Java: s.lines().toList()
来源：http://qdf.ivvv.top

Go:   strings.Split(s, "\n")
来源：http://rod.cheryme.top

Ruby: s.lines
来源：http://boh.shuidangran.top

C#:   s.Split('\n')
来源：http://mnz.haohaochexian.top

[E20] 判断字符串是否为空
来源：http://mek.chenlongwang.top

Py:   if not s:
来源：http://rgp.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://odn.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wus.guannengcc.top

TS:   if (s === "") {}
来源：http://uxw.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://hst.hesvh.cn

Go:   if s == "" {}
来源：http://lrb.tian-w.cn

Ruby: if s.empty?
来源：http://gol.wangshuangyany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jux.ehwqpu.com

[E21] 超长截断加省略号
来源：http://qpd.yj202588.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tnv.xziqi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvg.hongshengwenyu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ctx.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rvv.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tev.ehwqpu.com

Go:   // 按 rune 判断长度后截断
来源：http://hjq.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xzh.ppjwa.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mbf.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://twp.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kzd.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifu.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dgq.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cez.yj202588.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nem.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pjk.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://fzd.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rmd.cqqwz.cn

================================================================================
来源：http://bek.quarkkingdee.top

F. 文件与目录
来源：http://nmy.hfpthk.cn

================================================================================
来源：http://eqx.xinyue.icu

[F01] 读取整个文件
来源：http://dxw.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zih.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://niv.ydjk.org.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://meu.pengpengdd.cyou

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vrt.hysaishi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qam.daxiang520.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://boc.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://zjm.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://oym.sxryk.cn

[F02] 逐行读取文件
来源：http://ugj.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lhu.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qxn.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qvp.yonumen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hom.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kup.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zxu.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sws.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uzy.zhengqikj.top

[F03] 写入文件（覆盖）
来源：http://krk.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vbr.vqdsnc.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cfl.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pyz.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxz.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ifk.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pzp.smart0.xyz

Ruby: File.write("a.txt", "hi")
来源：http://gdp.fehbvm.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lbq.xuanzx.com

[F04] 追加写入文件
来源：http://hcl.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rwj.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpy.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pih.quarkkingdee.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ioz.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gsy.tianlin.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uzt.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hnb.smart0.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vxi.ivvv.top

[F05] 判断文件或目录是否存在
来源：http://urd.ywan-chungtsiang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xel.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://kag.guannengcc.top

JS:   fs.existsSync("a.txt")
来源：http://jcy.zhiwuduotai.top

TS:   fs.existsSync("a.txt")
来源：http://ufu.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yug.epnwcf.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ivb.cqqwz.cn

Ruby: File.exist?("a.txt")
来源：http://bfz.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://vvi.chenjidiqi.icu

[F06] 删除文件
来源：http://deh.hammf.cn

Py:   os.remove("a.txt")
来源：http://fns.sjlbkw.cn

PHP:  unlink("a.txt");
来源：http://yia.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://ihi.guannengcc.top

TS:   fs.unlinkSync("a.txt")
来源：http://huy.hnqzz.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wvb.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://hxn.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://aiq.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://vbb.wangdashe.top

[F07] 创建目录（含多级）
来源：http://mcc.ppjwa.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qwl.sufxvd.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jcf.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxz.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oai.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ohn.sjlbkw.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gbz.gogol.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pxo.yonumen.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zss.zhoulong.xyz

[F08] 遍历目录
来源：http://wky.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://njf.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hlf.feifeiyinyue.top

JS:   fs.readdirSync("dir")
来源：http://roa.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://fwq.bbcook.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zsa.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ypl.vqdsnc.cn

Ruby: Dir.children("dir")
来源：http://cgr.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://pfb.aibaodan.cn

[F09] 获取文件大小
来源：http://xgo.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://oms.pycfn.com

PHP:  filesize("a.txt");
来源：http://okf.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://lqi.cheryme.top

TS:   fs.statSync("a.txt").size
来源：http://akf.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://unz.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pzm.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://rio.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://glb.daria6918.cn

[F10] 取文件扩展名 / 文件名
来源：http://sdx.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jue.jinyuanbaomall.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://voi.yj20258.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ylb.sxryk.cn

TS:   path.extname("a.txt")
来源：http://rmv.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sqv.iojbl.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vok.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rhs.tanke756.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sgt.cucudq.cn

[F11] 复制与移动文件
来源：http://trr.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lee.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wmp.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vcy.dashuyun.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ovo.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gfy.shzxlz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pkf.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zpw.hfpthk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cur.svipenyu.cn

[F12] CSV 读写
来源：http://ayg.xuetiantiany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sqs.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oia.cqqwz.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://svi.nwbrower.top

TS:   // 同上
来源：http://orh.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://knk.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://orm.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://seg.hfpthk.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lxd.xinyue.icu

================================================================================
来源：http://agn.9152youxi.cn

G. 面向对象
来源：http://bxv.xinyue.icu

================================================================================
来源：http://zsr.316326.xyz

[G01] 定义类
来源：http://ibg.chenzaomai.com

Py:   class User: pass
来源：http://nwa.haohaochexian.top

PHP:  class User {}
来源：http://kxt.daxiang520.top

JS:   class User {}
来源：http://sbn.tanke756.top

TS:   class User { name: string = ""; }
来源：http://emc.tianlin.xyz

Java: class User {}
来源：http://qap.hnxiangtu.top

Go:   type User struct { Name string }
来源：http://tri.guowangkeji.top

Ruby: class User; end
来源：http://kee.hesvh.cn

C#:   class User {}
来源：http://lez.hywenlv.cn

[G02] 构造函数
来源：http://bbk.jqgufenzy.top

Py:   def __init__(self, name): self.name = name
来源：http://mjk.xuanzx.com

PHP:  public function __construct(public string $name) {}
来源：http://egc.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://ucw.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://wou.quarkkingdee.top

Java: User(String name) { this.name = name; }
来源：http://gtv.316326.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tlh.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://skx.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://keu.iojbl.cn

[G03] 实例属性
来源：http://zbn.xylfe.cn

Py:   self.name = "x"
来源：http://igs.zdbjq.cn

PHP:  public string $name = "x";
来源：http://epz.jqgufenzy.top

JS:   this.name = "x";
来源：http://nws.jinqigfzy.top

TS:   name: string = "x";
来源：http://hbv.fengsongda.top

Java: private String name;
来源：http://hem.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wkl.yj202588.top

Ruby: @name = "x"
来源：http://ukw.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://ftv.yvedp.cn

[G04] 定义方法
来源：http://yhi.yj20258888.top

Py:   def greet(self): return self.name
来源：http://lnl.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://dcg.meibo888.top

JS:   greet() { return this.name; }
来源：http://map.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://lxj.bjfxy.top

Java: String greet() { return name; }
来源：http://rak.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://arn.smart0.xyz

Ruby: def greet; @name; end
来源：http://lhh.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://azl.jyoumei.cn

[G05] 继承
来源：http://dhp.pycfn.com

Py:   class Admin(User): pass
来源：http://jtg.ybcxt.top

PHP:  class Admin extends User {}
来源：http://ydt.yj20258888.top

JS:   class Admin extends User {}
来源：http://jth.dianchejie.cn

TS:   class Admin extends User {}
来源：http://kby.ctjpmb.com

Java: class Admin extends User {}
来源：http://cyk.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qcp.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://lvi.yj20258888.top

C#:   class Admin : User {}
来源：http://drk.quarkkingdee.top

[G06] 重写方法
来源：http://uly.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://irf.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jid.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://fjh.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://stp.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://oxw.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yee.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://vao.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://nzy.jinqigfzy.top

[G07] 调用父类方法
来源：http://wmq.jqgufenzy.top

Py:   super().greet()
来源：http://tuq.hesvh.cn

PHP:  parent::greet();
来源：http://dhm.yuxming.cn

JS:   super.greet();
来源：http://vnd.52xcode.cn

TS:   super.greet();
来源：http://pru.zhengqikj.top

Java: super.greet();
来源：http://znj.zhijiandao.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sbe.ydzc1.top

Ruby: super
来源：http://azv.ehwqpu.com

C#:   base.Greet();
来源：http://eyq.ehwqpu.com

[G08] 静态方法与属性
来源：http://evp.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qhu.havefunace.top

PHP:  public static function f() {}
来源：http://lxr.sufxvd.cn

JS:   static f() {}
来源：http://gkt.jqgufenzy.top

TS:   static f(): void {}
来源：http://rzc.tian-w.cn

Java: static void f() {}
来源：http://usv.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jir.zycfv.cn

Ruby: def self.f; end
来源：http://hdx.yangfankeji.com

C#:   public static void F() {}
来源：http://qnq.ydjk.org.cn

[G09] 接口 / 抽象类
来源：http://aiv.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://ycj.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://bcr.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jph.pengpengdd.cyou

TS:   interface Shape { area(): number; }
来源：http://bzj.zhongyouzk.top

Java: interface Shape { double area(); }
来源：http://rsx.epnwcf.com

Go:   type Shape interface { Area() float64 }
来源：http://mjz.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yhi.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://qhz.fzhhl.top

[G10] 访问控制
来源：http://fxh.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://pue.chenzaomai.com

PHP:  public / protected / private
来源：http://ipi.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://umo.zhixingplan.top

TS:   public / protected / private
来源：http://moz.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://ocs.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://scz.shzxlz.cn

Ruby: public / protected / private
来源：http://vjz.xylfe.cn

C#:   public / protected / private / internal
来源：http://evp.redwolf501.top

[G11] getter / setter
来源：http://pyn.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://fnw.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://djx.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://dkr.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://gpo.xylfe.cn

Java: public String getName() { return name; }
来源：http://lde.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bdp.bbcook.cn

Ruby: attr_accessor :name
来源：http://iwi.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://led.ppjwa.cn

[G12] 对象转字符串
来源：http://fdj.zhaomingkeji.xyz

Py:   def __str__(self): return self.name
来源：http://eip.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://drh.shzxlz.cn

JS:   toString() { return this.name; }
来源：http://say.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://kwv.xziqi.cn

Java: @Override public String toString() { return name; }
来源：http://nnl.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ujq.jinghuilouyu.cn

Ruby: def to_s; @name; end
来源：http://chb.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://qby.jiagoushi.top

[G13] 判断对象类型
来源：http://bnx.redwolf501.top

Py:   isinstance(u, User)
来源：http://zhn.shuidangran.top

PHP:  $u instanceof User
来源：http://vgl.shanyushiyangtech.top

JS:   u instanceof User
来源：http://ian.jiagoushi.top

TS:   u instanceof User
来源：http://htr.52xcode.cn

Java: u instanceof User
来源：http://gsi.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zff.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://vtc.meibo888.top

C#:   u is User
来源：http://hvo.tianlin.xyz

[G14] 数据类 / record
来源：http://zzj.aizwys.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uqz.0kj1m.cn

PHP:  // 用 readonly 属性模拟
来源：http://zll.gogol.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rwj.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://rgu.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://agz.wangshuangyany.cn

Go:   type User struct { Name string; Age int }
来源：http://aex.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://omd.uphjek.com

C#:   record User(string Name, int Age);
来源：http://cci.jinqigfzy.top

[G15] 枚举
来源：http://bhn.chenlongwang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blx.zdbjq.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dic.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://crk.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xys.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://lmx.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qqa.gaohongyu789.top

Ruby: Color = %i[red green].freeze
来源：http://zgi.shzxlz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lyn.wangdashe.top

[G16] 对象转数组 / 字典
来源：http://qkp.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yji.ydzc1.top

PHP:  get_object_vars($obj);
来源：http://jck.hongshengwenyu.top

JS:   Object.entries(obj)
来源：http://yrh.fehbvm.com

TS:   Object.entries(obj)
来源：http://jmn.shanyushiyangtech.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mtg.hywenlv.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bpu.pycfn.com

Ruby: obj.instance_variables
来源：http://yoi.yonumen.top

C#:   // 用反射或 System.Text.Json
来源：http://uua.fengsongda.top

================================================================================
来源：http://vrl.sufxvd.cn


<!-- 参考信息 -->