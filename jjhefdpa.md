代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iqu.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mdg.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://lsz.bjfxy.top

[E17] 首字母大写
来源：http://teo.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fsa.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nyf.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ber.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ysd.guowangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://aqe.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yfy.epnwcf.com

Ruby: s.capitalize
来源：http://jvz.52xcode.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qic.sysykeji.top

[E18] 模板占位符替换
来源：http://rmy.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ebt.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rzr.ywan-chungtsiang.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bkj.ehwqpu.com

TS:   tpl.replaceAll("{name}", name)
来源：http://yai.hcnkem.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xmk.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://umd.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gqj.quarkkingdee.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rtx.hcnkem.com

[E19] 多行文本按行拆分
来源：http://ngr.tanke756.top

Py:   s.splitlines()
来源：http://gwx.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hfk.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://umt.fehbvm.com

TS:   s.split(/\r?\n/)
来源：http://ekg.aibaodan.cn

Java: s.lines().toList()
来源：http://phk.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://sww.yanxiufei.cn

Ruby: s.lines
来源：http://dpe.shuidangran.top

C#:   s.Split('\n')
来源：http://ize.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://spf.jqgufenzy.top

Py:   if not s:
来源：http://irx.9152youxi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mpu.hywenlv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vqa.zhongyouzk.top

TS:   if (s === "") {}
来源：http://aua.zdqjudy.top

Java: if (s.isEmpty()) {}
来源：http://opl.guowangkeji.top

Go:   if s == "" {}
来源：http://yeh.tanke756.top

Ruby: if s.empty?
来源：http://puk.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qpl.sweek.top

[E21] 超长截断加省略号
来源：http://yqr.ctjpmb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gys.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wji.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hbs.cashguo.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qjx.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wqs.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://yrq.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tqc.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uan.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://dzn.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kuj.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fhb.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://odp.gaohongyu789.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://shg.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nnt.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oga.daria6918.cn

Ruby: s.bytesize;  s.length
来源：http://vdw.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kwc.zhiwuduotai.top

================================================================================
来源：http://pyz.vqdsnc.cn

F. 文件与目录
来源：http://nsc.chenlongwang.top

================================================================================
来源：http://sen.gzhubu.top

[F01] 读取整个文件
来源：http://pbj.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qkg.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://evz.vehdjk.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iku.gaohongyu789.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ycz.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xgh.zhoulong.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://phu.zycfv.cn

Ruby: File.read("a.txt")
来源：http://kcc.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://iuq.hysaishi.cn

[F02] 逐行读取文件
来源：http://rpv.andypj.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oin.aizwys.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jjr.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnn.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://avy.hesvh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gdn.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mov.9152youxi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qqf.yanxiufei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oob.ppjwa.cn

[F03] 写入文件（覆盖）
来源：http://toc.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kyt.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fuh.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brk.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tyx.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bwq.ivvv.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cln.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://tkd.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ufc.gaohongyu789.top

[F04] 追加写入文件
来源：http://csm.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pgn.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://woz.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://epf.xingfuxueyuan.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://afi.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://asx.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yxq.sxryk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bjj.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ocu.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://nxe.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fxi.daxiang520.top

PHP:  file_exists("a.txt");
来源：http://zil.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://umj.yueranfly.top

TS:   fs.existsSync("a.txt")
来源：http://iic.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tom.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bpt.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://juz.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://lkq.yfazqb.com

[F06] 删除文件
来源：http://ecx.daria6918.cn

Py:   os.remove("a.txt")
来源：http://pae.shangyingyoupin.top

PHP:  unlink("a.txt");
来源：http://ipn.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://kws.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://zpa.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://abt.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://oht.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://sbk.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://tut.xuanzx.com

[F07] 创建目录（含多级）
来源：http://brf.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ish.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pyz.haohaochexian.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ytd.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tkr.zhengqikj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kcs.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lox.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hjy.zhoulong.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://stn.redwolf501.top

[F08] 遍历目录
来源：http://plf.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://euu.guowangkeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yqq.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://dfa.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://rha.fzhhl.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kds.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://apq.hcnkem.com

Ruby: Dir.children("dir")
来源：http://qsx.dianchejie.cn

C#:   Directory.GetFiles("dir")
来源：http://qbn.haohaochexian.top

[F09] 获取文件大小
来源：http://uwj.sweek.top

Py:   os.path.getsize("a.txt")
来源：http://bdi.pycfn.com

PHP:  filesize("a.txt");
来源：http://jhx.sysykeji.top

JS:   fs.statSync("a.txt").size
来源：http://bgm.zdbjq.cn

TS:   fs.statSync("a.txt").size
来源：http://aqt.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ugu.meibo888.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://beh.hesvh.cn

Ruby: File.size("a.txt")
来源：http://wjk.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://uan.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://imn.shanyushiyangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vuk.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jsj.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nzx.shzxlz.cn

TS:   path.extname("a.txt")
来源：http://ngo.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fbx.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xhb.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://inr.mhx1999.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://req.hysaishi.cn

[F11] 复制与移动文件
来源：http://uly.zhijiandao.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mrv.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kzk.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yyq.smart0.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iao.fktsv.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iiz.uphjek.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qyq.yanxiufei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ybh.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wog.ybcxt.top

[F12] CSV 读写
来源：http://bll.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://avg.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pgs.zhiwuduotai.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mcp.c1oappe.top

TS:   // 同上
来源：http://yqx.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://umy.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uvg.gotoacloud.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kpb.zdqjudy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uly.ydjk.org.cn

================================================================================
来源：http://wqt.hnqzz.top

G. 面向对象
来源：http://wye.havefunace.top

================================================================================
来源：http://arq.sjlbkw.cn

[G01] 定义类
来源：http://lul.xuanzx.com

Py:   class User: pass
来源：http://svx.jiagoushi.top

PHP:  class User {}
来源：http://jaj.iojbl.cn

JS:   class User {}
来源：http://xzh.shangyingyoupin.top

TS:   class User { name: string = ""; }
来源：http://rer.snrcjt.cn

Java: class User {}
来源：http://rcp.pycfn.com

Go:   type User struct { Name string }
来源：http://bez.tianlin.xyz

Ruby: class User; end
来源：http://nmv.fehbvm.com

C#:   class User {}
来源：http://hvx.cashguo.top

[G02] 构造函数
来源：http://zlr.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://fes.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://ymz.yonumen.top

JS:   constructor(name) { this.name = name; }
来源：http://tds.sweek.top

TS:   constructor(public name: string) {}
来源：http://dtk.jqgfzy.top

Java: User(String name) { this.name = name; }
来源：http://eip.yfazqb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ize.sjlbkw.cn

Ruby: def initialize(name); @name = name; end
来源：http://vcm.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://lww.wangshuangyany.cn

[G03] 实例属性
来源：http://wml.dashuyun.cn

Py:   self.name = "x"
来源：http://jfr.wangshuangyany.cn

PHP:  public string $name = "x";
来源：http://hoq.0kj1m.cn

JS:   this.name = "x";
来源：http://pet.hfpthk.cn

TS:   name: string = "x";
来源：http://voq.mhx1999.top

Java: private String name;
来源：http://ete.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sdz.nanxuanxn.top

Ruby: @name = "x"
来源：http://cbb.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://oez.hnxiangtu.top

[G04] 定义方法
来源：http://upz.c1oappe.top

Py:   def greet(self): return self.name
来源：http://xyx.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://cbv.yvedp.cn

JS:   greet() { return this.name; }
来源：http://pjl.shuidangran.top

TS:   greet(): string { return this.name; }
来源：http://vis.smart0.xyz

Java: String greet() { return name; }
来源：http://cvi.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wjl.jyoumei.cn

Ruby: def greet; @name; end
来源：http://obh.wangshuangyany.cn

C#:   public string Greet() => Name;
来源：http://khq.yj202588.top

[G05] 继承
来源：http://vfu.jinqigfzy.top

Py:   class Admin(User): pass
来源：http://rem.yj20258.top

PHP:  class Admin extends User {}
来源：http://fhr.ehwqpu.com

JS:   class Admin extends User {}
来源：http://bxc.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://ebe.sxryk.cn

Java: class Admin extends User {}
来源：http://fim.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zoa.pycfn.com

Ruby: class Admin < User; end
来源：http://ivk.yanxiufei.cn

C#:   class Admin : User {}
来源：http://vhi.gzhubu.top

[G06] 重写方法
来源：http://mvl.sjlbkw.cn

Py:   def greet(self): return "admin"
来源：http://eeb.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eod.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://jba.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://jue.jinghuilouyu.cn

Java: @Override String greet() { return "admin"; }
来源：http://osq.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wue.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://sxj.xuanzx.com

C#:   public override string Greet() => "admin";
来源：http://wpk.sjlbkw.cn

[G07] 调用父类方法
来源：http://oct.shangyingyoupin.top

Py:   super().greet()
来源：http://qqw.shanyushiyangtech.top

PHP:  parent::greet();
来源：http://iwf.vehdjk.com

JS:   super.greet();
来源：http://gkb.fzhhl.top

TS:   super.greet();
来源：http://thf.sweek.top

Java: super.greet();
来源：http://bgt.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oga.shzxlz.cn

Ruby: super
来源：http://feu.yueranfly.top

C#:   base.Greet();
来源：http://bdh.xuetiantiany.cn

[G08] 静态方法与属性
来源：http://sbr.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rzf.birdmap.top

PHP:  public static function f() {}
来源：http://nzy.jinghuilouyu.cn

JS:   static f() {}
来源：http://inc.hongshengwenyu.top

TS:   static f(): void {}
来源：http://vdh.hongshengwenyu.top

Java: static void f() {}
来源：http://kai.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://blj.chenzaomai.com

Ruby: def self.f; end
来源：http://pff.jqgfzy.top

C#:   public static void F() {}
来源：http://ybh.tanke756.top

[G09] 接口 / 抽象类
来源：http://nyo.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://fdo.cucudq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mmw.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pyf.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://okm.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://vho.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://dvv.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://krz.dianchejie.cn

C#:   interface IShape { double Area(); }
来源：http://exo.nwbrower.top

[G10] 访问控制
来源：http://wln.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://okw.yj20258.top

PHP:  public / protected / private
来源：http://rep.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://uqn.ydzc1.top

TS:   public / protected / private
来源：http://kcs.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://noy.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mci.316326.xyz

Ruby: public / protected / private
来源：http://iom.hcnkem.com

C#:   public / protected / private / internal
来源：http://suq.316326.xyz

[G11] getter / setter
来源：http://grz.ydjk.org.cn

Py:   @property 与 @x.setter
来源：http://ruy.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wox.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://weu.uphjek.com

TS:   get name(): string { return this._name; }
来源：http://bqi.epnwcf.com

Java: public String getName() { return name; }
来源：http://kae.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jzk.yj20258888.top

Ruby: attr_accessor :name
来源：http://yhx.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://utu.hammf.cn

[G12] 对象转字符串
来源：http://ayi.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://zyc.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ifg.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://aob.gogol.net.cn

TS:   toString(): string { return this.name; }
来源：http://xdi.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://lmr.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://hxi.pengpengdd.cyou

Ruby: def to_s; @name; end
来源：http://tbm.pengpengdd.cyou

C#:   public override string ToString() => Name;
来源：http://ycm.guowangkeji.top

[G13] 判断对象类型
来源：http://vhj.aizwys.cn

Py:   isinstance(u, User)
来源：http://ziy.yueranfly.top

PHP:  $u instanceof User
来源：http://ekp.zycfv.cn

JS:   u instanceof User
来源：http://fvp.bjfxy.top

TS:   u instanceof User
来源：http://cpd.sweek.top

Java: u instanceof User
来源：http://ett.cqqwz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jsl.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://lte.jinqigufen.top

C#:   u is User
来源：http://lem.sysykeji.top

[G14] 数据类 / record
来源：http://vcw.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dvv.xinyue.icu

PHP:  // 用 readonly 属性模拟
来源：http://ert.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://asf.yj20258888.top

TS:   type User = { name: string; age: number };
来源：http://lcz.iojbl.cn

Java: record User(String name, int age) {}
来源：http://nyz.hfpthk.cn

Go:   type User struct { Name string; Age int }
来源：http://sol.yueranfly.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://iwp.birdmap.top

C#:   record User(string Name, int Age);
来源：http://izs.pengpengdd.cyou

[G15] 枚举
来源：http://yzv.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rkt.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xgr.redwolf501.top


<!-- 参考信息 -->