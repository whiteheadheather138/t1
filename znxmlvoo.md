代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ylo.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://woo.yuanzhike.top

C#:   1234567.ToString("N0")
来源：http://egw.sxryk.cn

[E17] 首字母大写
来源：http://bkl.vehdjk.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ypj.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jam.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mlm.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pjr.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lzs.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hxf.gzhubu.top

Ruby: s.capitalize
来源：http://tlx.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jtq.redwolf501.top

[E18] 模板占位符替换
来源：http://pxp.cqqwz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wzu.hywenlv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gdg.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jdx.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://crs.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xjo.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xkc.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://slr.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xtv.gaohongyu789.top

[E19] 多行文本按行拆分
来源：http://lax.vqdsnc.cn

Py:   s.splitlines()
来源：http://uqb.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rfy.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://knz.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://xbp.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://tdu.tanke756.top

Go:   strings.Split(s, "\n")
来源：http://obt.tianlin.xyz

Ruby: s.lines
来源：http://fcs.svipenyu.cn

C#:   s.Split('\n')
来源：http://dsa.bjfxy.top

[E20] 判断字符串是否为空
来源：http://vwu.andypj.xyz

Py:   if not s:
来源：http://rfc.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fgf.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dpb.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://chl.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://uze.quarkkingdee.top

Go:   if s == "" {}
来源：http://ugq.redwolf501.top

Ruby: if s.empty?
来源：http://kuy.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uug.meibo888.top

[E21] 超长截断加省略号
来源：http://grp.zycfv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ytd.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://szo.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fuq.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndz.ybcxt.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wtk.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://bih.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kom.shzxlz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pzw.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://puw.xuanzx.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ajt.jlsjyb.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://euj.iojbl.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://irm.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zim.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hol.zhijiandao.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mgj.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://ncg.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cwk.yj202588.top

================================================================================
来源：http://lpb.yfazqb.com

F. 文件与目录
来源：http://yqy.c1oappe.top

================================================================================
来源：http://pnh.daxiang520.top

[F01] 读取整个文件
来源：http://dez.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://scs.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://gvz.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kqo.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lng.birdmap.top

Java: Files.readString(Path.of("a.txt"))
来源：http://etb.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pkn.ydzc1.top

Ruby: File.read("a.txt")
来源：http://nli.sweek.top

C#:   File.ReadAllText("a.txt");
来源：http://gae.xingfuxueyuan.xyz

[F02] 逐行读取文件
来源：http://xtx.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qjg.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ppy.sysykeji.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cou.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cci.zdbjq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dbg.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nvo.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://svg.pengpengdd.cyou

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://svk.fehbvm.com

[F03] 写入文件（覆盖）
来源：http://aii.ctjpmb.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://njg.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://djg.jinqigfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zuk.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://muo.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qtf.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qfw.yj20258888.top

Ruby: File.write("a.txt", "hi")
来源：http://eek.hysaishi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mvy.shzxlz.cn

[F04] 追加写入文件
来源：http://spx.dianchejie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qis.hysaishi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uru.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qhh.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dor.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fvw.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rwz.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vio.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://alw.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://wim.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rtp.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://oep.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://uwq.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://dbk.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://amv.vehdjk.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vaw.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://ggy.xylfe.cn

C#:   File.Exists("a.txt")
来源：http://bnf.yj20258888.top

[F06] 删除文件
来源：http://ant.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://uxx.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://uym.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://lsz.dianchejie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jgi.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtm.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://upj.zdbjq.cn

Ruby: File.delete("a.txt")
来源：http://bcf.316326.xyz

C#:   File.Delete("a.txt");
来源：http://xso.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://wha.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kcw.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://opm.sjlbkw.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pmu.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dtg.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://liu.shuidangran.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wmq.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kns.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xri.fzhhl.top

[F08] 遍历目录
来源：http://hig.cucudq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://otl.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pfp.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://tur.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://vjx.epnwcf.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vdu.fktsv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://suh.yj20258888.top

Ruby: Dir.children("dir")
来源：http://unk.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://lzp.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://zny.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://uhp.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://hvi.c1oappe.top

JS:   fs.statSync("a.txt").size
来源：http://xpu.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://wje.snrcjt.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lby.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wus.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://esq.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://keb.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://cyd.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://egt.shangyingyoupin.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yux.jinqigufen.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://njp.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://mpw.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ard.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://plp.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iub.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://obn.quarkkingdee.top

[F11] 复制与移动文件
来源：http://ybu.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ubx.jianghu66.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tvb.yj20258888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hpx.ehwqpu.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mvv.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pth.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yhi.sxryk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://siw.svipenyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xuy.jqgufenzy.top

[F12] CSV 读写
来源：http://aip.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ndi.316326.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rrw.fehbvm.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fjn.ydzc1.top

TS:   // 同上
来源：http://rzr.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://azk.jinqigufen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qms.yonumen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rkq.jyoumei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mhw.xuetiantiany.cn

================================================================================
来源：http://gyw.yanxiufei.cn

G. 面向对象
来源：http://ink.jiagoushi.top

================================================================================
来源：http://iue.wangshuangyany.cn

[G01] 定义类
来源：http://glm.yueranfly.top

Py:   class User: pass
来源：http://yde.hammf.cn

PHP:  class User {}
来源：http://bcg.ywan-chungtsiang.top

JS:   class User {}
来源：http://nua.cdnleiting.top

TS:   class User { name: string = ""; }
来源：http://gsu.hywenlv.cn

Java: class User {}
来源：http://zzf.cheryme.top

Go:   type User struct { Name string }
来源：http://znk.0kj1m.cn

Ruby: class User; end
来源：http://ctq.ivvv.top

C#:   class User {}
来源：http://wgh.epnwcf.com

[G02] 构造函数
来源：http://pqd.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://vgg.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://pvj.jinqigufen.top

JS:   constructor(name) { this.name = name; }
来源：http://ozz.jinqigufen.top

TS:   constructor(public name: string) {}
来源：http://wcf.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://qxl.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qxj.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://eux.xuanzx.com

C#:   public User(string name) { Name = name; }
来源：http://pxi.9152youxi.cn

[G03] 实例属性
来源：http://gwf.yj202588.top

Py:   self.name = "x"
来源：http://hne.jlsjyb.cn

PHP:  public string $name = "x";
来源：http://kua.sjlbkw.cn

JS:   this.name = "x";
来源：http://fza.yongpay.top

TS:   name: string = "x";
来源：http://ilf.zycfv.cn

Java: private String name;
来源：http://oec.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zjx.316326.xyz

Ruby: @name = "x"
来源：http://ydq.zhaomingkeji.xyz

C#:   public string Name { get; set; } = "x";
来源：http://vcq.cheryme.top

[G04] 定义方法
来源：http://ulu.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://wtn.hesvh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dig.uphjek.com

JS:   greet() { return this.name; }
来源：http://qzl.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://ldv.fktsv.cn

Java: String greet() { return name; }
来源：http://osy.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xkc.daria6918.cn

Ruby: def greet; @name; end
来源：http://hvt.cucudq.cn

C#:   public string Greet() => Name;
来源：http://ybk.kuanghao11.cn

[G05] 继承
来源：http://meo.jiagoushi.top

Py:   class Admin(User): pass
来源：http://sof.uphjek.com

PHP:  class Admin extends User {}
来源：http://kxb.sjlbkw.cn

JS:   class Admin extends User {}
来源：http://tez.bbcook.cn

TS:   class Admin extends User {}
来源：http://sxa.daxiang520.top

Java: class Admin extends User {}
来源：http://tdx.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vhb.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://fkj.sjlbkw.cn

C#:   class Admin : User {}
来源：http://qcj.yuxming.cn

[G06] 重写方法
来源：http://pwl.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://ppi.pycfn.com

PHP:  public function greet(): string { return "admin"; }
来源：http://tog.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://ynf.sxryk.cn

TS:   greet(): string { return "admin"; }
来源：http://qxm.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://zlm.jinqigufen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fdz.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://xwi.dashuyun.cn

C#:   public override string Greet() => "admin";
来源：http://aps.epnwcf.com

[G07] 调用父类方法
来源：http://jkr.jianghu66.top

Py:   super().greet()
来源：http://hbb.zycfv.cn

PHP:  parent::greet();
来源：http://hog.xuetiantiany.cn

JS:   super.greet();
来源：http://otz.sweek.top

TS:   super.greet();
来源：http://wuz.yuanzhike.top

Java: super.greet();
来源：http://ssx.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qmr.yfazqb.com

Ruby: super
来源：http://nyt.hesvh.cn

C#:   base.Greet();
来源：http://wsl.xinyue.icu

[G08] 静态方法与属性
来源：http://srh.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lyp.tian-w.cn

PHP:  public static function f() {}
来源：http://hrb.vqdsnc.cn

JS:   static f() {}
来源：http://wki.ppjwa.cn

TS:   static f(): void {}
来源：http://ssp.yj202588.top

Java: static void f() {}
来源：http://bkq.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://qfg.ivvv.top

Ruby: def self.f; end
来源：http://wza.guannengcc.top

C#:   public static void F() {}
来源：http://yiw.iojbl.cn

[G09] 接口 / 抽象类
来源：http://ojy.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://btd.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wig.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://dxg.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://jxu.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://uom.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://oww.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sfe.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://cxh.jinyuanbaomall.cn

[G10] 访问控制
来源：http://mvi.cheryme.top

Py:   约定 _protected / __private（不强制）
来源：http://qvp.gogol.net.cn

PHP:  public / protected / private
来源：http://myv.yonumen.top

JS:   #private 字段；其余公开
来源：http://kuj.sjlbkw.cn

TS:   public / protected / private
来源：http://dco.uphjek.com

Java: public / protected / private / 默认包级
来源：http://unc.mhx1999.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qis.aibaodan.cn

Ruby: public / protected / private
来源：http://roj.nwbrower.top

C#:   public / protected / private / internal
来源：http://cdm.xziqi.cn

[G11] getter / setter
来源：http://fcx.sxryk.cn

Py:   @property 与 @x.setter
来源：http://ikq.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://iqt.wangdashe.top

JS:   get name() { return this._name; }
来源：http://ggy.jyoumei.cn

TS:   get name(): string { return this._name; }
来源：http://bwm.fanxiaobao.xyz

Java: public String getName() { return name; }
来源：http://wiy.yj20258.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://dua.vqdsnc.cn

Ruby: attr_accessor :name
来源：http://yyp.hnqzz.top

C#:   public string Name { get; set; }
来源：http://jtp.dianchejie.cn

[G12] 对象转字符串
来源：http://fic.yvedp.cn

Py:   def __str__(self): return self.name
来源：http://mab.kuanghao11.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dqd.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://gzb.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://dol.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://uge.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://osq.nanxinkj.top

Ruby: def to_s; @name; end
来源：http://lbu.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://xdd.zhengqikj.top

[G13] 判断对象类型
来源：http://uul.nwbrower.top

Py:   isinstance(u, User)
来源：http://qto.aibaodan.cn

PHP:  $u instanceof User
来源：http://tet.dianchejie.cn

JS:   u instanceof User
来源：http://rpa.andypj.xyz

TS:   u instanceof User
来源：http://uea.shangyingyoupin.top

Java: u instanceof User
来源：http://nbu.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://uzg.jlsjyb.cn

Ruby: u.is_a?(User)
来源：http://jtr.mhx1999.top

C#:   u is User
来源：http://hdg.guowangkeji.top

[G14] 数据类 / record
来源：http://zqc.c1oappe.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jyx.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://beu.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://zzm.yj20258.top

TS:   type User = { name: string; age: number };
来源：http://ufc.redwolf501.top

Java: record User(String name, int age) {}
来源：http://oxb.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://bqj.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://unz.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://pwb.jinqigfzy.top

[G15] 枚举
来源：http://sef.cashguo.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kvn.havefunace.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://omt.nwbrower.top


<!-- 参考信息 -->