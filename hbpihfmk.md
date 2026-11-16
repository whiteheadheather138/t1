代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wtg.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zsd.hfpthk.cn

[E16] 数字千分位
来源：http://dxx.nwbrower.top

Py:   f"{1234567:,}"
来源：http://gna.guannengcc.top

PHP:  number_format(1234567);
来源：http://bqt.daxiang520.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ctt.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://soy.bjfxy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fbf.hongshengwenyu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vjd.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ekd.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://swb.aizwys.cn

[E17] 首字母大写
来源：http://txr.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ddd.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://znp.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yzh.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gcd.chenlongwang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nri.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ust.cheryme.top

Ruby: s.capitalize
来源：http://shq.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ffh.jqgfzy.top

[E18] 模板占位符替换
来源：http://plk.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bzm.havefunace.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vce.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dgr.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ukd.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xgz.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hge.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://guo.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://exd.gotoacloud.top

[E19] 多行文本按行拆分
来源：http://uan.ydzc1.top

Py:   s.splitlines()
来源：http://rcp.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zry.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://yqy.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://vne.meibo888.top

Java: s.lines().toList()
来源：http://dsp.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://ovl.zycfv.cn

Ruby: s.lines
来源：http://xvj.jqgufenzy.top

C#:   s.Split('\n')
来源：http://rtq.jqgfzy.top

[E20] 判断字符串是否为空
来源：http://crx.cdnleiting.top

Py:   if not s:
来源：http://dga.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://adt.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://skz.jlsjyb.cn

TS:   if (s === "") {}
来源：http://dod.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://mwb.cqqwz.cn

Go:   if s == "" {}
来源：http://xgz.guannengcc.top

Ruby: if s.empty?
来源：http://ofy.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yap.haohaochexian.top

[E21] 超长截断加省略号
来源：http://zaq.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://khx.snrcjt.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://txo.yj202588.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://emy.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kkq.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ffg.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://zek.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qvh.yfazqb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://epa.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://nds.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kqx.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ijv.bbcook.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hnp.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://scg.gzhubu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jnj.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qbu.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://ppn.hnqzz.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lrs.shuidangran.top

================================================================================
来源：http://onl.hysaishi.cn

F. 文件与目录
来源：http://mok.andypj.xyz

================================================================================
来源：http://psf.cashguo.top

[F01] 读取整个文件
来源：http://oiq.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tmy.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://arv.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fsa.dianchejie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hif.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ive.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jqh.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://kut.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://xck.hongshengwenyu.top

[F02] 逐行读取文件
来源：http://tjb.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ccg.yonumen.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jtq.wangdashe.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://twf.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rml.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fkr.zdbjq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mzk.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vqb.bjfxy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://foo.jinqigfzy.top

[F03] 写入文件（覆盖）
来源：http://afj.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://frv.bbcook.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jjg.yueranfly.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mrv.hysaishi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://npp.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vxz.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://srr.daxiang520.top

Ruby: File.write("a.txt", "hi")
来源：http://ynq.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dia.quarkkingdee.top

[F04] 追加写入文件
来源：http://lsd.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rnf.dashuyun.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fyk.fktsv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kzo.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jja.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qub.cucudq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gmy.epnwcf.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://evn.tianlin.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kkq.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://gpk.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vra.hnxiangtu.top

PHP:  file_exists("a.txt");
来源：http://yig.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://gvj.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://rln.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ksa.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yri.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://cgw.yj20258.top

C#:   File.Exists("a.txt")
来源：http://lfo.tianlin.xyz

[F06] 删除文件
来源：http://xax.iojbl.cn

Py:   os.remove("a.txt")
来源：http://vpc.redwolf501.top

PHP:  unlink("a.txt");
来源：http://hzk.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mql.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vro.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rkd.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://vri.birdmap.top

Ruby: File.delete("a.txt")
来源：http://fnm.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://xbb.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://pga.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://swg.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://stq.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ndi.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vlr.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://duc.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hsk.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wjy.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://roo.9152youxi.cn

[F08] 遍历目录
来源：http://yrf.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dye.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kyx.zhoulong.xyz

JS:   fs.readdirSync("dir")
来源：http://mlk.ctjpmb.com

TS:   fs.readdirSync("dir")
来源：http://bdq.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zew.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgk.tarul.cn

Ruby: Dir.children("dir")
来源：http://arh.smart0.xyz

C#:   Directory.GetFiles("dir")
来源：http://zux.jinyuanbaomall.cn

[F09] 获取文件大小
来源：http://cuh.uphjek.com

Py:   os.path.getsize("a.txt")
来源：http://soc.gzhubu.top

PHP:  filesize("a.txt");
来源：http://jhq.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://vew.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://prr.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wnk.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xuu.pengpengdd.cyou

Ruby: File.size("a.txt")
来源：http://okh.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://hvw.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://zsi.dashuyun.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cdw.fzhhl.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tfb.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qlr.andypj.xyz

TS:   path.extname("a.txt")
来源：http://edn.sysykeji.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qww.dianchejie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://khe.cdnleiting.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dlh.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ipt.xinyue.icu

[F11] 复制与移动文件
来源：http://txc.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kmz.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uqf.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sin.ydjk.org.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mav.yvedp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qtx.shuidangran.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vft.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gdx.pycfn.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nbp.mhx1999.top

[F12] CSV 读写
来源：http://bzn.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dvs.jiagoushi.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nsn.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pvv.yanxiufei.cn

TS:   // 同上
来源：http://poz.shuidangran.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qyz.hesvh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://swc.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cny.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://mgb.jianghu66.top

================================================================================
来源：http://gwk.c1oappe.top

G. 面向对象
来源：http://xff.yj20258.top

================================================================================
来源：http://tba.hcnkem.com

[G01] 定义类
来源：http://bbv.hnxiangtu.top

Py:   class User: pass
来源：http://pss.nanxinkj.top

PHP:  class User {}
来源：http://ore.redwolf501.top

JS:   class User {}
来源：http://efc.yangfankeji.com

TS:   class User { name: string = ""; }
来源：http://vpb.316326.xyz

Java: class User {}
来源：http://fzs.uphjek.com

Go:   type User struct { Name string }
来源：http://lyf.bbcook.cn

Ruby: class User; end
来源：http://ion.andypj.xyz

C#:   class User {}
来源：http://swi.ppjwa.cn

[G02] 构造函数
来源：http://yvo.nanxinkj.top

Py:   def __init__(self, name): self.name = name
来源：http://fzm.guannengcc.top

PHP:  public function __construct(public string $name) {}
来源：http://wtr.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://mml.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://dgv.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://lfw.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gcu.shanyushiyangtech.top

Ruby: def initialize(name); @name = name; end
来源：http://eps.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://ulc.fzhhl.top

[G03] 实例属性
来源：http://kxy.fehbvm.com

Py:   self.name = "x"
来源：http://api.birdmap.top

PHP:  public string $name = "x";
来源：http://sha.yonumen.top

JS:   this.name = "x";
来源：http://lyz.daria6918.cn

TS:   name: string = "x";
来源：http://zpu.epnwcf.com

Java: private String name;
来源：http://rsf.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vvb.aibaodan.cn

Ruby: @name = "x"
来源：http://qby.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://jpl.zhixingplan.top

[G04] 定义方法
来源：http://ted.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://bja.zhixingplan.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ldt.yongpay.top

JS:   greet() { return this.name; }
来源：http://ayn.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://xgy.chenlongwang.top

Java: String greet() { return name; }
来源：http://ueu.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://eeg.guowangkeji.top

Ruby: def greet; @name; end
来源：http://jzz.shuidangran.top

C#:   public string Greet() => Name;
来源：http://ujx.haohaochexian.top

[G05] 继承
来源：http://moy.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://gio.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://glh.ehwqpu.com

JS:   class Admin extends User {}
来源：http://twe.zhongyouzk.top

TS:   class Admin extends User {}
来源：http://yvz.cucudq.cn

Java: class Admin extends User {}
来源：http://saj.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rla.birdmap.top

Ruby: class Admin < User; end
来源：http://xqx.chenzaomai.com

C#:   class Admin : User {}
来源：http://psi.smart0.xyz

[G06] 重写方法
来源：http://ljx.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://bkl.hysaishi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://smm.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://wej.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://qph.jiagoushi.top

Java: @Override String greet() { return "admin"; }
来源：http://ztd.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ive.bbcook.cn

Ruby: def greet; "admin"; end
来源：http://vud.sjlbkw.cn

C#:   public override string Greet() => "admin";
来源：http://ooj.tarul.cn

[G07] 调用父类方法
来源：http://dpw.fengsongda.top

Py:   super().greet()
来源：http://yvq.fktsv.cn

PHP:  parent::greet();
来源：http://kjq.ctjpmb.com

JS:   super.greet();
来源：http://zdd.gogol.net.cn

TS:   super.greet();
来源：http://tye.guowangkeji.top

Java: super.greet();
来源：http://adw.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fdy.zdbjq.cn

Ruby: super
来源：http://ivq.52xcode.cn

C#:   base.Greet();
来源：http://cld.bjfxy.top

[G08] 静态方法与属性
来源：http://sry.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zrp.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://wmq.tanke756.top

JS:   static f() {}
来源：http://ukx.hywenlv.cn

TS:   static f(): void {}
来源：http://pfi.shanyushiyangkeji.top

Java: static void f() {}
来源：http://zlf.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rky.yuxming.cn

Ruby: def self.f; end
来源：http://kaq.chenjidiqi.icu

C#:   public static void F() {}
来源：http://bfa.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://yzs.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://scl.wangshuangyany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zax.zhijiandao.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pqw.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://ttl.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://mmy.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://caa.aizwys.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fdk.wangdashe.top

C#:   interface IShape { double Area(); }
来源：http://xbd.bjfxy.top

[G10] 访问控制
来源：http://xnb.wangdashe.top

Py:   约定 _protected / __private（不强制）
来源：http://jcl.ybcxt.top

PHP:  public / protected / private
来源：http://cxj.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://ioo.xziqi.cn

TS:   public / protected / private
来源：http://cfs.meibo888.top

Java: public / protected / private / 默认包级
来源：http://mre.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://quz.smart0.xyz

Ruby: public / protected / private
来源：http://moy.pycfn.com

C#:   public / protected / private / internal
来源：http://pwe.hongshengwenyu.top

[G11] getter / setter
来源：http://wbz.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://mth.jlsjyb.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yig.yueranfly.top

JS:   get name() { return this._name; }
来源：http://ujv.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://ewq.haohaochexian.top

Java: public String getName() { return name; }
来源：http://gjs.kuanghao11.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rcb.hesvh.cn

Ruby: attr_accessor :name
来源：http://uiz.cdnleiting.top

C#:   public string Name { get; set; }
来源：http://nki.cucudq.cn

[G12] 对象转字符串
来源：http://cbv.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://ifz.hammf.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://efq.sysykeji.top

JS:   toString() { return this.name; }
来源：http://cyl.daxiang520.top

TS:   toString(): string { return this.name; }
来源：http://ihi.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://ttg.cucudq.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bhs.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://fgq.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://viq.ehwqpu.com

[G13] 判断对象类型
来源：http://jdd.xuanzx.com

Py:   isinstance(u, User)
来源：http://dog.nwbrower.top

PHP:  $u instanceof User
来源：http://pmq.redwolf501.top

JS:   u instanceof User
来源：http://nlf.yuxming.cn

TS:   u instanceof User
来源：http://ryw.pycfn.com

Java: u instanceof User
来源：http://uab.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://iad.cucudq.cn

Ruby: u.is_a?(User)
来源：http://fna.zhixingplan.top

C#:   u is User
来源：http://foo.zhijiandao.cn

[G14] 数据类 / record
来源：http://ref.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yde.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://qtb.smart0.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://ejf.tian-w.cn


<!-- 参考信息 -->