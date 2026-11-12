代发 wailian999

[E18] 模板占位符替换
来源：http://ijr.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pda.andypj.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jzd.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iyg.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://lkl.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ibw.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ehg.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ssd.sweek.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sas.xylfe.cn

[E19] 多行文本按行拆分
来源：http://pwo.shzxlz.cn

Py:   s.splitlines()
来源：http://tza.smart0.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baq.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://ppk.tanke756.top

TS:   s.split(/\r?\n/)
来源：http://yyf.dashuyun.cn

Java: s.lines().toList()
来源：http://rfr.quarkkingdee.top

Go:   strings.Split(s, "\n")
来源：http://hph.nanxinkj.top

Ruby: s.lines
来源：http://emu.dashuyun.cn

C#:   s.Split('\n')
来源：http://dob.jqgufenzy.top

[E20] 判断字符串是否为空
来源：http://nhl.hywenlv.cn

Py:   if not s:
来源：http://vdf.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rju.hnxiangtu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wzf.fzhhl.top

TS:   if (s === "") {}
来源：http://jmh.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://txj.fengsongda.top

Go:   if s == "" {}
来源：http://dns.nanxinkj.top

Ruby: if s.empty?
来源：http://tkn.jqgufenzy.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ebe.tianlin.xyz

[E21] 超长截断加省略号
来源：http://jds.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oai.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ytj.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kcn.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lno.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://svf.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://gmr.pycfn.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mxy.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bwt.hcnkem.com

[E22] 字节长度与字符长度
来源：http://lmz.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jqw.shanyushiyangtech.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wux.xuetiantiany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkl.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikd.zhixingplan.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wlr.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://twf.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://puf.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://smf.gaohongyu789.top

================================================================================
来源：http://oxy.aibaodan.cn

F. 文件与目录
来源：http://tid.zhiwuduotai.top

================================================================================
来源：http://wry.kuanghao11.cn

[F01] 读取整个文件
来源：http://egf.jinyuanbaomall.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://svb.sysykeji.top

PHP:  file_get_contents("a.txt");
来源：http://yhm.sjlbkw.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ild.mhx1999.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mbh.xinyue.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://ohe.hysaishi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gfx.hfpthk.cn

Ruby: File.read("a.txt")
来源：http://qgl.xylfe.cn

C#:   File.ReadAllText("a.txt");
来源：http://sfu.haohaochexian.top

[F02] 逐行读取文件
来源：http://ius.ehwqpu.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xdt.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ygu.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bli.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://osu.ydjk.org.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gbc.cdnleiting.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lce.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eht.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fly.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://xfw.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qyg.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ozm.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zjp.0kj1m.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fgq.sjlbkw.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ptg.zhengqikj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wfq.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://yoa.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ibz.dashuyun.cn

[F04] 追加写入文件
来源：http://opz.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vgk.ehwqpu.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zvc.jlsjyb.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rvy.chenzaomai.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wik.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kut.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yfp.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nxn.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tkh.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://mly.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hjj.yonumen.top

PHP:  file_exists("a.txt");
来源：http://egc.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://bgw.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://wdd.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sdq.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oxr.pycfn.com

Ruby: File.exist?("a.txt")
来源：http://vgi.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://jvh.52xcode.cn

[F06] 删除文件
来源：http://azr.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://spt.nwbrower.top

PHP:  unlink("a.txt");
来源：http://rpj.guowangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://wjx.sufxvd.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zpy.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mtu.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://lrt.cdnleiting.top

Ruby: File.delete("a.txt")
来源：http://ubn.sweek.top

C#:   File.Delete("a.txt");
来源：http://fpx.jinghuilouyu.cn

[F07] 创建目录（含多级）
来源：http://drm.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oyh.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bjs.zhongyouzk.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stq.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iws.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pcf.wangdashe.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zul.shanyushiyangtech.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://idb.shangyingyoupin.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bpw.ehwqpu.com

[F08] 遍历目录
来源：http://gpx.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ozy.hfpthk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qoy.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://bze.aizwys.cn

TS:   fs.readdirSync("dir")
来源：http://xyj.jinqigfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://edu.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://ala.hnqzz.top

Ruby: Dir.children("dir")
来源：http://lww.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://xje.svipenyu.cn

[F09] 获取文件大小
来源：http://jnr.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://gfl.chenzaomai.com

PHP:  filesize("a.txt");
来源：http://rkr.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://hlt.daxiang520.top

TS:   fs.statSync("a.txt").size
来源：http://bco.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://wij.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hsk.hnqzz.top

Ruby: File.size("a.txt")
来源：http://pho.guannengcc.top

C#:   new FileInfo("a.txt").Length
来源：http://eum.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://hfa.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jdg.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bsb.tanke756.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hgn.nwbrower.top

TS:   path.extname("a.txt")
来源：http://zug.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hoh.52xcode.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://spd.hesvh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ipo.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kgv.xylfe.cn

[F11] 复制与移动文件
来源：http://jmo.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kcy.hysaishi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bdl.fzhhl.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kuz.zycfv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tht.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://exi.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nbw.zdbjq.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vas.yangfankeji.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vdq.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://slp.0kj1m.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jpu.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rkk.dashuyun.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hls.sweek.top

TS:   // 同上
来源：http://yqv.hnxiangtu.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mkr.birdmap.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eqf.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ude.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dao.yueranfly.top

================================================================================
来源：http://leu.ywan-chungtsiang.top

G. 面向对象
来源：http://jkl.0kj1m.cn

================================================================================
来源：http://lyh.sxryk.cn

[G01] 定义类
来源：http://jmw.jlsjyb.cn

Py:   class User: pass
来源：http://fdp.birdmap.top

PHP:  class User {}
来源：http://grr.yj202588.top

JS:   class User {}
来源：http://lyn.yj202588.top

TS:   class User { name: string = ""; }
来源：http://woh.sjlbkw.cn

Java: class User {}
来源：http://orx.ctjpmb.com

Go:   type User struct { Name string }
来源：http://gai.mhx1999.top

Ruby: class User; end
来源：http://myi.shanyushiyangkeji.top

C#:   class User {}
来源：http://jkl.epnwcf.com

[G02] 构造函数
来源：http://mfx.svipenyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ems.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://ksk.yvedp.cn

JS:   constructor(name) { this.name = name; }
来源：http://dnh.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://eyt.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://ivv.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ppg.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://bra.zycfv.cn

C#:   public User(string name) { Name = name; }
来源：http://twf.yonumen.top

[G03] 实例属性
来源：http://rgh.tianlin.xyz

Py:   self.name = "x"
来源：http://wfd.jyoumei.cn

PHP:  public string $name = "x";
来源：http://ees.fehbvm.com

JS:   this.name = "x";
来源：http://wia.guowangkeji.top

TS:   name: string = "x";
来源：http://cqa.cdnleiting.top

Java: private String name;
来源：http://bue.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qrl.yonumen.top

Ruby: @name = "x"
来源：http://yqz.shuidangran.top

C#:   public string Name { get; set; } = "x";
来源：http://ter.hnxiangtu.top

[G04] 定义方法
来源：http://cfc.pycfn.com

Py:   def greet(self): return self.name
来源：http://sgg.svipenyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fsg.hnqzz.top

JS:   greet() { return this.name; }
来源：http://zua.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://ygt.guowangkeji.top

Java: String greet() { return name; }
来源：http://ayb.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iiq.xylfe.cn

Ruby: def greet; @name; end
来源：http://cek.xuanzx.com

C#:   public string Greet() => Name;
来源：http://zaj.daria6918.cn

[G05] 继承
来源：http://vps.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://prm.hnqzz.top

PHP:  class Admin extends User {}
来源：http://snm.zhongyouzk.top

JS:   class Admin extends User {}
来源：http://lex.cucudq.cn

TS:   class Admin extends User {}
来源：http://ybd.ywan-chungtsiang.top

Java: class Admin extends User {}
来源：http://uxo.zhiwuduotai.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://guk.jiagoushi.top

Ruby: class Admin < User; end
来源：http://pfu.pycfn.com

C#:   class Admin : User {}
来源：http://sjp.xuanzx.com

[G06] 重写方法
来源：http://vsk.zhijiandao.cn

Py:   def greet(self): return "admin"
来源：http://qbp.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lfb.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://ehz.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://qrz.chenlongwang.top

Java: @Override String greet() { return "admin"; }
来源：http://mjw.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://whm.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://ibt.pengpengdd.cyou

C#:   public override string Greet() => "admin";
来源：http://qck.ctjpmb.com

[G07] 调用父类方法
来源：http://tnj.yanxiufei.cn

Py:   super().greet()
来源：http://bqm.pycfn.com

PHP:  parent::greet();
来源：http://wxq.daxiang520.top

JS:   super.greet();
来源：http://jph.zhijiandao.cn

TS:   super.greet();
来源：http://aqb.xuanzx.com

Java: super.greet();
来源：http://szd.yj20258.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mcv.52xcode.cn

Ruby: super
来源：http://vss.jinqigufen.top

C#:   base.Greet();
来源：http://qup.zdbjq.cn

[G08] 静态方法与属性
来源：http://upx.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wrr.yvedp.cn

PHP:  public static function f() {}
来源：http://hos.sjlbkw.cn

JS:   static f() {}
来源：http://nqj.shanyushiyangkeji.top

TS:   static f(): void {}
来源：http://jbz.daria6918.cn

Java: static void f() {}
来源：http://uiw.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vzf.cdnleiting.top

Ruby: def self.f; end
来源：http://pln.0kj1m.cn

C#:   public static void F() {}
来源：http://eyg.cqqwz.cn

[G09] 接口 / 抽象类
来源：http://kic.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://unt.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nbx.jianghu66.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wyi.yangfankeji.com

TS:   interface Shape { area(): number; }
来源：http://ewx.sufxvd.cn

Java: interface Shape { double area(); }
来源：http://ghs.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://lwg.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rqw.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://ooh.316326.xyz

[G10] 访问控制
来源：http://rou.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://ock.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://ydr.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://lih.shzxlz.cn

TS:   public / protected / private
来源：http://isg.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://inr.guannengcc.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sjm.yangfankeji.com

Ruby: public / protected / private
来源：http://epq.pycfn.com

C#:   public / protected / private / internal
来源：http://dpr.yj202588.top

[G11] getter / setter
来源：http://jyi.mhx1999.top

Py:   @property 与 @x.setter
来源：http://bye.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://voy.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://jht.redwolf501.top

TS:   get name(): string { return this._name; }
来源：http://mcg.316326.xyz

Java: public String getName() { return name; }
来源：http://dtd.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://sjy.mhx1999.top

Ruby: attr_accessor :name
来源：http://wpz.sweek.top

C#:   public string Name { get; set; }
来源：http://ahf.fktsv.cn

[G12] 对象转字符串
来源：http://kkm.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://kye.ppjwa.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gxa.nwbrower.top

JS:   toString() { return this.name; }
来源：http://wwx.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://buh.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://ocv.shuidangran.top

Go:   func (u User) String() string { return u.Name }
来源：http://eec.andypj.xyz

Ruby: def to_s; @name; end
来源：http://tnk.pycfn.com

C#:   public override string ToString() => Name;
来源：http://omj.tian-w.cn

[G13] 判断对象类型
来源：http://efe.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://kvo.yuxming.cn

PHP:  $u instanceof User
来源：http://tdd.hfpthk.cn

JS:   u instanceof User
来源：http://uco.ehwqpu.com

TS:   u instanceof User
来源：http://vwv.tian-w.cn

Java: u instanceof User
来源：http://oof.hammf.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dgg.sweek.top

Ruby: u.is_a?(User)
来源：http://ssk.fktsv.cn

C#:   u is User
来源：http://oto.shangyingyoupin.top

[G14] 数据类 / record
来源：http://fhf.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ifx.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://zgd.jinghuilouyu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oqm.chenzaomai.com

TS:   type User = { name: string; age: number };
来源：http://jbb.shangyingyoupin.top

Java: record User(String name, int age) {}
来源：http://khf.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://aul.fehbvm.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://msm.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://thd.uphjek.com

[G15] 枚举
来源：http://onf.tarul.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wcg.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hkl.vehdjk.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dzx.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ads.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://xrb.jyoumei.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rkt.zdbjq.cn

Ruby: Color = %i[red green].freeze
来源：http://bwi.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hop.snrcjt.cn

[G16] 对象转数组 / 字典
来源：http://sum.iojbl.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nva.tarul.cn

PHP:  get_object_vars($obj);
来源：http://usw.chenlongwang.top

JS:   Object.entries(obj)
来源：http://bvz.hongshengwenyu.top

TS:   Object.entries(obj)
来源：http://phi.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://otj.sxryk.cn


<!-- 参考信息 -->