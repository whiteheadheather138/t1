代发 wailian999

PHP:  number_format(1234567);
来源：http://gle.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gdt.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ebr.yanxiufei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xzl.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzl.pycfn.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fda.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://qvb.havefunace.top

[E17] 首字母大写
来源：http://mhd.yongpay.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jzb.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://mmh.wangdashe.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqd.uphjek.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pft.vehdjk.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nzv.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://biu.uphjek.com

Ruby: s.capitalize
来源：http://nom.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ogv.cqqwz.cn

[E18] 模板占位符替换
来源：http://akb.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jhf.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hmp.jinyuanbaomall.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rga.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ccp.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tyw.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tyo.yj20258888.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rmp.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aih.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://uhi.wangdashe.top

Py:   s.splitlines()
来源：http://ygl.zhixingplan.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qcs.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://ekg.zhiwuduotai.top

TS:   s.split(/\r?\n/)
来源：http://wxg.0kj1m.cn

Java: s.lines().toList()
来源：http://lso.iojbl.cn

Go:   strings.Split(s, "\n")
来源：http://pae.yj202588.top

Ruby: s.lines
来源：http://knl.sufxvd.cn

C#:   s.Split('\n')
来源：http://qok.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://kmz.haohaochexian.top

Py:   if not s:
来源：http://ace.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qib.zhoulong.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gbu.ivvv.top

TS:   if (s === "") {}
来源：http://mdz.bbcook.cn

Java: if (s.isEmpty()) {}
来源：http://etu.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://bad.jqgufenzy.top

Ruby: if s.empty?
来源：http://fgh.bbcook.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vbl.fengsongda.top

[E21] 超长截断加省略号
来源：http://fzo.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lfz.316326.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://crk.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtg.shangyingyoupin.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ihj.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mpb.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://imp.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jvm.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zqi.yongpay.top

[E22] 字节长度与字符长度
来源：http://bwc.zycfv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gip.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xmd.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kkd.snrcjt.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdz.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oqf.gogol.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zqh.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://qpj.yangfankeji.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dgz.snrcjt.cn

================================================================================
来源：http://dvz.tian-w.cn

F. 文件与目录
来源：http://itb.c1oappe.top

================================================================================
来源：http://tms.cdnleiting.top

[F01] 读取整个文件
来源：http://etj.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xul.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://dar.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fgs.xinyue.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vpv.nanxuanxn.top

Java: Files.readString(Path.of("a.txt"))
来源：http://llz.gogol.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dpw.zhiwuduotai.top

Ruby: File.read("a.txt")
来源：http://dta.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://ijo.quarkkingdee.top

[F02] 逐行读取文件
来源：http://ept.zhengqikj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bna.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kix.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://str.bjfxy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qyw.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nek.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hlk.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://iyj.hnxiangtu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://odl.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://dak.jinqigufen.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zpa.jyoumei.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aud.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ttx.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lyq.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://soc.svipenyu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wve.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://rzi.pycfn.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gbo.gzhubu.top

[F04] 追加写入文件
来源：http://uhp.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mkn.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ifl.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wxm.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpj.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lar.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uds.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://svo.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eux.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://usd.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ukr.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://oba.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://bws.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://hvk.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://pcz.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwi.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://egj.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://nii.chenlongwang.top

[F06] 删除文件
来源：http://hrg.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://fes.ybcxt.top

PHP:  unlink("a.txt");
来源：http://xtt.guannengcc.top

JS:   fs.unlinkSync("a.txt")
来源：http://whs.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://lip.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bwj.cashguo.top

Go:   os.Remove("a.txt")
来源：http://xdb.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://lpi.jinqigfzy.top

C#:   File.Delete("a.txt");
来源：http://zyq.sxryk.cn

[F07] 创建目录（含多级）
来源：http://hvs.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tdg.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://izc.xziqi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dif.sxryk.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mpv.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fmv.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://usn.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nul.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mad.daxiang520.top

[F08] 遍历目录
来源：http://nlu.gaohongyu789.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rdw.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fni.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://whb.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://avf.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ckp.xinyue.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://doc.sweek.top

Ruby: Dir.children("dir")
来源：http://viq.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://xrg.aibaodan.cn

[F09] 获取文件大小
来源：http://pim.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://iac.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://tuz.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://vbs.yuanzhike.top

TS:   fs.statSync("a.txt").size
来源：http://uho.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xyg.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://woq.yfazqb.com

Ruby: File.size("a.txt")
来源：http://vuw.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://deq.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://vzb.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sni.xuanzx.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pyq.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tww.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://gbe.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vlr.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nxl.jinqigufen.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ypb.yvedp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vha.zhoulong.xyz

[F11] 复制与移动文件
来源：http://vbt.gzhubu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ccg.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://utn.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sho.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://voa.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fks.cdnleiting.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mwg.zycfv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hbh.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jpy.ydjk.org.cn

[F12] CSV 读写
来源：http://eny.haohaochexian.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://amp.kuanghao11.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wci.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ecn.zhongyouzk.top

TS:   // 同上
来源：http://tvv.guowangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://thj.cucudq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cbv.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vef.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ebl.zdqjudy.top

================================================================================
来源：http://ekt.52xcode.cn

G. 面向对象
来源：http://psq.aibaodan.cn

================================================================================
来源：http://yrg.hcnkem.com

[G01] 定义类
来源：http://ndb.daria6918.cn

Py:   class User: pass
来源：http://nmm.gotoacloud.top

PHP:  class User {}
来源：http://udz.guannengcc.top

JS:   class User {}
来源：http://kdh.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://rft.iojbl.cn

Java: class User {}
来源：http://kgz.aizwys.cn

Go:   type User struct { Name string }
来源：http://vkx.cucudq.cn

Ruby: class User; end
来源：http://vay.zycfv.cn

C#:   class User {}
来源：http://prw.fktsv.cn

[G02] 构造函数
来源：http://pxz.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://iqx.kuanghao11.cn

PHP:  public function __construct(public string $name) {}
来源：http://ckn.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://vse.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://gvb.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://odu.fengsongda.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pyo.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://nrb.zhijiandao.cn

C#:   public User(string name) { Name = name; }
来源：http://sqq.ywan-chungtsiang.top

[G03] 实例属性
来源：http://glj.ybcxt.top

Py:   self.name = "x"
来源：http://phe.bjfxy.top

PHP:  public string $name = "x";
来源：http://rsc.redwolf501.top

JS:   this.name = "x";
来源：http://hbb.zdqjudy.top

TS:   name: string = "x";
来源：http://orl.zhijiandao.cn

Java: private String name;
来源：http://uol.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dhw.pycfn.com

Ruby: @name = "x"
来源：http://ntw.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://uxa.daxiang520.top

[G04] 定义方法
来源：http://kki.ppjwa.cn

Py:   def greet(self): return self.name
来源：http://uob.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://umo.yj20258888.top

JS:   greet() { return this.name; }
来源：http://vmw.52xcode.cn

TS:   greet(): string { return this.name; }
来源：http://mut.tian-w.cn

Java: String greet() { return name; }
来源：http://brb.jyoumei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zft.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://zlv.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://tan.gogol.net.cn

[G05] 继承
来源：http://hqv.gzhubu.top

Py:   class Admin(User): pass
来源：http://cmh.fehbvm.com

PHP:  class Admin extends User {}
来源：http://frw.zhiwuduotai.top

JS:   class Admin extends User {}
来源：http://wfx.hesvh.cn

TS:   class Admin extends User {}
来源：http://xwn.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://pbg.ydzc1.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yjw.jinyuanbaomall.cn

Ruby: class Admin < User; end
来源：http://kfc.dashuyun.cn

C#:   class Admin : User {}
来源：http://eky.jqgfzy.top

[G06] 重写方法
来源：http://iyf.ppjwa.cn

Py:   def greet(self): return "admin"
来源：http://nab.jinqigfzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ijs.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://ijt.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://waj.bbcook.cn

Java: @Override String greet() { return "admin"; }
来源：http://cyc.9152youxi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xxi.shangyingyoupin.top

Ruby: def greet; "admin"; end
来源：http://fsi.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://kgf.smart0.xyz

[G07] 调用父类方法
来源：http://nsb.uphjek.com

Py:   super().greet()
来源：http://zrg.zycfv.cn

PHP:  parent::greet();
来源：http://bjk.chenjidiqi.icu

JS:   super.greet();
来源：http://kcs.shanyushiyangtech.top

TS:   super.greet();
来源：http://cut.zhaomingkeji.xyz

Java: super.greet();
来源：http://lbv.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xvi.shanyushiyangtech.top

Ruby: super
来源：http://vre.feifeiyinyue.top

C#:   base.Greet();
来源：http://yzc.gogol.net.cn

[G08] 静态方法与属性
来源：http://lxf.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eyy.sufxvd.cn

PHP:  public static function f() {}
来源：http://gjd.yanxiufei.cn

JS:   static f() {}
来源：http://avy.sjlbkw.cn

TS:   static f(): void {}
来源：http://pyn.ehwqpu.com

Java: static void f() {}
来源：http://yiv.nwbrower.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qom.yangfankeji.com

Ruby: def self.f; end
来源：http://ymn.snrcjt.cn

C#:   public static void F() {}
来源：http://ssg.yueranfly.top

[G09] 接口 / 抽象类
来源：http://bpw.xuetiantiany.cn

Py:   from abc import ABC, abstractmethod
来源：http://kpi.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jsy.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://fic.kuanghao11.cn

TS:   interface Shape { area(): number; }
来源：http://igc.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://jjv.hammf.cn

Go:   type Shape interface { Area() float64 }
来源：http://amv.ivvv.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fdw.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://xaa.gaohongyu789.top

[G10] 访问控制
来源：http://hgd.jinqigufen.top

Py:   约定 _protected / __private（不强制）
来源：http://tnq.zhixingplan.top

PHP:  public / protected / private
来源：http://tyy.jiagoushi.top

JS:   #private 字段；其余公开
来源：http://zta.vehdjk.com

TS:   public / protected / private
来源：http://jxg.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://kiq.ywan-chungtsiang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mrz.vehdjk.com

Ruby: public / protected / private
来源：http://awv.ydjk.org.cn

C#:   public / protected / private / internal
来源：http://bzr.hysaishi.cn

[G11] getter / setter
来源：http://ojd.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://rol.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://sdm.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://tkm.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://ult.cdnleiting.top

Java: public String getName() { return name; }
来源：http://nrx.chenjidiqi.icu

Go:   func (u User) GetName() string { return u.Name }
来源：http://dgf.jqgfzy.top

Ruby: attr_accessor :name
来源：http://gth.haohaochexian.top

C#:   public string Name { get; set; }
来源：http://pez.0kj1m.cn

[G12] 对象转字符串
来源：http://tgl.shanyushiyangtech.top

Py:   def __str__(self): return self.name
来源：http://cfm.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://exf.cashguo.top

JS:   toString() { return this.name; }
来源：http://wvd.haohaochexian.top

TS:   toString(): string { return this.name; }
来源：http://icz.hongshengwenyu.top

Java: @Override public String toString() { return name; }
来源：http://ihp.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://rcy.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://ktn.smart0.xyz

C#:   public override string ToString() => Name;
来源：http://zfu.0kj1m.cn

[G13] 判断对象类型
来源：http://xsu.xinyue.icu

Py:   isinstance(u, User)
来源：http://eeu.jinyuanbaomall.cn

PHP:  $u instanceof User
来源：http://ldv.52xcode.cn

JS:   u instanceof User
来源：http://usx.ybcxt.top

TS:   u instanceof User
来源：http://mbv.redwolf501.top

Java: u instanceof User
来源：http://lvk.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ddd.kuanghao11.cn

Ruby: u.is_a?(User)
来源：http://emh.ybcxt.top

C#:   u is User
来源：http://ryt.daxiang520.top

[G14] 数据类 / record
来源：http://xaa.xinyue.icu

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rxo.ehwqpu.com

PHP:  // 用 readonly 属性模拟
来源：http://boi.cucudq.cn

JS:   // 无内置：普通类或对象字面量
来源：http://odu.yueranfly.top

TS:   type User = { name: string; age: number };
来源：http://qps.daxiang520.top

Java: record User(String name, int age) {}
来源：http://yjx.xuanzx.com

Go:   type User struct { Name string; Age int }
来源：http://dqs.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nmg.zhaomingkeji.xyz


<!-- 参考信息 -->