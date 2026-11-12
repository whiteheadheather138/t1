代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wag.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bdx.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://xsj.fktsv.cn

[E17] 首字母大写
来源：http://xll.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://stw.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://oou.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ved.bbcook.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rxx.cqqwz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zhp.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pye.cucudq.cn

Ruby: s.capitalize
来源：http://ezy.dashuyun.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jva.yvedp.cn

[E18] 模板占位符替换
来源：http://sgd.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mku.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kxn.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://dst.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xrq.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmb.xylfe.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rsd.fanxiaobao.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ndf.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rkj.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://pxy.chenjidiqi.icu

Py:   s.splitlines()
来源：http://lcf.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://liw.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://uij.zdqjudy.top

TS:   s.split(/\r?\n/)
来源：http://boe.wangdashe.top

Java: s.lines().toList()
来源：http://adj.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://xeo.hongshengwenyu.top

Ruby: s.lines
来源：http://nzl.gotoacloud.top

C#:   s.Split('\n')
来源：http://nwp.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://rta.cheryme.top

Py:   if not s:
来源：http://sby.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tph.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ldn.ywan-chungtsiang.top

TS:   if (s === "") {}
来源：http://oaj.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://dgg.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://rne.tian-w.cn

Ruby: if s.empty?
来源：http://tlr.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nzg.hnqzz.top

[E21] 超长截断加省略号
来源：http://wmt.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qib.cucudq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ryu.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tcx.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uvo.havefunace.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kjl.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://klq.havefunace.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lda.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zxu.zhongyouzk.top

[E22] 字节长度与字符长度
来源：http://oug.zhixingplan.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fzm.gzhubu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gax.0kj1m.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://guv.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyl.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sly.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://arb.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://ypd.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ndt.c1oappe.top

================================================================================
来源：http://pqc.tarul.cn

F. 文件与目录
来源：http://hql.gzhubu.top

================================================================================
来源：http://sta.ybcxt.top

[F01] 读取整个文件
来源：http://hdv.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qgu.yj202588.top

PHP:  file_get_contents("a.txt");
来源：http://gqc.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ysv.meibo888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ljl.hywenlv.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jwk.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gjr.nanxuanxn.top

Ruby: File.read("a.txt")
来源：http://pqq.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://jcg.zycfv.cn

[F02] 逐行读取文件
来源：http://nji.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qrh.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hgf.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jtd.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwf.52xcode.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nlv.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zbg.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qtq.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hii.shanyushiyangkeji.top

[F03] 写入文件（覆盖）
来源：http://oxf.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://asm.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xhs.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zyh.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fet.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fxs.sysykeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zfx.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://lar.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://drf.dianchejie.cn

[F04] 追加写入文件
来源：http://lvo.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://run.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ewt.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dkn.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://srs.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sfc.cdnleiting.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nou.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cwt.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jjs.shanyushiyangkeji.top

[F05] 判断文件或目录是否存在
来源：http://vik.yj20258.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qam.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://hll.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://dwl.wangshuangyany.cn

TS:   fs.existsSync("a.txt")
来源：http://jmk.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://eep.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jtq.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://axg.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://dcv.gzhubu.top

[F06] 删除文件
来源：http://scv.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://uwt.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://elw.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://mei.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://yzo.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cyu.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://cvt.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://csp.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://boe.c1oappe.top

[F07] 创建目录（含多级）
来源：http://vgv.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sfg.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://frm.havefunace.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://obi.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dln.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wtf.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wdv.svipenyu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://off.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jbe.vqdsnc.cn

[F08] 遍历目录
来源：http://hqa.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qoc.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mvn.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://ggh.sweek.top

TS:   fs.readdirSync("dir")
来源：http://odb.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ors.yuxming.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wgv.uphjek.com

Ruby: Dir.children("dir")
来源：http://bpd.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://qiu.yj20258888.top

[F09] 获取文件大小
来源：http://yqe.daria6918.cn

Py:   os.path.getsize("a.txt")
来源：http://aiz.gzhubu.top

PHP:  filesize("a.txt");
来源：http://adb.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://kge.yonumen.top

TS:   fs.statSync("a.txt").size
来源：http://fci.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jjx.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nxh.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://mpk.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://ubg.chenlongwang.top

[F10] 取文件扩展名 / 文件名
来源：http://voz.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ujv.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://unb.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ats.xylfe.cn

TS:   path.extname("a.txt")
来源：http://uqz.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmp.cheryme.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ckh.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bdg.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fhx.ehwqpu.com

[F11] 复制与移动文件
来源：http://mzx.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ikm.yuxming.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yuc.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mzf.ctjpmb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bgu.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://okj.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vdy.ivvv.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://anc.daxiang520.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mtl.hnxiangtu.top

[F12] CSV 读写
来源：http://ebj.fktsv.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ova.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fih.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rba.iojbl.cn

TS:   // 同上
来源：http://thk.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fgh.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kru.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bnw.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://jmi.tarul.cn

================================================================================
来源：http://sqy.shanyushiyangkeji.top

G. 面向对象
来源：http://pqs.nanxinkj.top

================================================================================
来源：http://fcp.9152youxi.cn

[G01] 定义类
来源：http://wvl.aizwys.cn

Py:   class User: pass
来源：http://lxy.shanyushiyangkeji.top

PHP:  class User {}
来源：http://nyh.cashguo.top

JS:   class User {}
来源：http://awo.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://ozv.cashguo.top

Java: class User {}
来源：http://psu.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://gpq.yanxiufei.cn

Ruby: class User; end
来源：http://nxl.shanyushiyangkeji.top

C#:   class User {}
来源：http://sph.dashuyun.cn

[G02] 构造函数
来源：http://bhy.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://lku.zhengqikj.top

PHP:  public function __construct(public string $name) {}
来源：http://zqn.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://val.gogol.net.cn

TS:   constructor(public name: string) {}
来源：http://igl.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://jxv.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ysu.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://wok.andypj.xyz

C#:   public User(string name) { Name = name; }
来源：http://vce.dianchejie.cn

[G03] 实例属性
来源：http://mfc.svipenyu.cn

Py:   self.name = "x"
来源：http://gcx.hfpthk.cn

PHP:  public string $name = "x";
来源：http://eod.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://oar.shanyushiyangtech.top

TS:   name: string = "x";
来源：http://ijj.chenzaomai.com

Java: private String name;
来源：http://wxn.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yce.9152youxi.cn

Ruby: @name = "x"
来源：http://kts.yueranfly.top

C#:   public string Name { get; set; } = "x";
来源：http://wdv.fanxiaobao.xyz

[G04] 定义方法
来源：http://wul.yueranfly.top

Py:   def greet(self): return self.name
来源：http://ote.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nwi.ydzc1.top

JS:   greet() { return this.name; }
来源：http://udx.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://tco.gogol.net.cn

Java: String greet() { return name; }
来源：http://gga.hcnkem.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://lcn.0kj1m.cn

Ruby: def greet; @name; end
来源：http://xsa.yuxming.cn

C#:   public string Greet() => Name;
来源：http://pyd.chenlongwang.top

[G05] 继承
来源：http://wsp.tarul.cn

Py:   class Admin(User): pass
来源：http://qnn.zhengqikj.top

PHP:  class Admin extends User {}
来源：http://vwc.haohaochexian.top

JS:   class Admin extends User {}
来源：http://mmn.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://wje.fehbvm.com

Java: class Admin extends User {}
来源：http://nji.hnqzz.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gyh.dianchejie.cn

Ruby: class Admin < User; end
来源：http://cup.hcnkem.com

C#:   class Admin : User {}
来源：http://esn.sysykeji.top

[G06] 重写方法
来源：http://sah.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://huh.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://snv.zycfv.cn

JS:   greet() { return "admin"; }
来源：http://soa.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://czp.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://ufv.ywan-chungtsiang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qoo.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://yyu.yangfankeji.com

C#:   public override string Greet() => "admin";
来源：http://vnj.hcnkem.com

[G07] 调用父类方法
来源：http://jri.chenlongwang.top

Py:   super().greet()
来源：http://eul.meibo888.top

PHP:  parent::greet();
来源：http://btr.haohaochexian.top

JS:   super.greet();
来源：http://jki.316326.xyz

TS:   super.greet();
来源：http://ifl.bbcook.cn

Java: super.greet();
来源：http://lrf.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fzc.birdmap.top

Ruby: super
来源：http://zyf.jlsjyb.cn

C#:   base.Greet();
来源：http://ioy.gogol.net.cn

[G08] 静态方法与属性
来源：http://yuw.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dgi.52xcode.cn

PHP:  public static function f() {}
来源：http://bux.haohaochexian.top

JS:   static f() {}
来源：http://ujb.shuidangran.top

TS:   static f(): void {}
来源：http://eco.yanxiufei.cn

Java: static void f() {}
来源：http://rav.havefunace.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jig.jlsjyb.cn

Ruby: def self.f; end
来源：http://jou.aizwys.cn

C#:   public static void F() {}
来源：http://rxt.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://zer.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://vry.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://vlc.zhengqikj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zvb.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://dco.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://wfg.sjlbkw.cn

Go:   type Shape interface { Area() float64 }
来源：http://zaz.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zjw.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://cum.bbcook.cn

[G10] 访问控制
来源：http://iod.gzhubu.top

Py:   约定 _protected / __private（不强制）
来源：http://knk.hcnkem.com

PHP:  public / protected / private
来源：http://ebk.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://vgi.zhengqikj.top

TS:   public / protected / private
来源：http://czf.yj20258.top

Java: public / protected / private / 默认包级
来源：http://yxs.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ayj.ehwqpu.com

Ruby: public / protected / private
来源：http://wpu.nwbrower.top

C#:   public / protected / private / internal
来源：http://dxw.chenlongwang.top

[G11] getter / setter
来源：http://enz.zdbjq.cn

Py:   @property 与 @x.setter
来源：http://vle.smart0.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://auf.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://wsl.daxiang520.top

TS:   get name(): string { return this._name; }
来源：http://qop.sxryk.cn

Java: public String getName() { return name; }
来源：http://uhy.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lcw.pengpengdd.cyou

Ruby: attr_accessor :name
来源：http://yix.jyoumei.cn

C#:   public string Name { get; set; }
来源：http://ggv.zycfv.cn

[G12] 对象转字符串
来源：http://aac.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://ykx.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lhb.yuxming.cn

JS:   toString() { return this.name; }
来源：http://lqe.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://hsl.jiagoushi.top

Java: @Override public String toString() { return name; }
来源：http://swy.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://sok.xingfuxueyuan.xyz

Ruby: def to_s; @name; end
来源：http://eve.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://crs.tarul.cn

[G13] 判断对象类型
来源：http://pgt.yj20258888.top

Py:   isinstance(u, User)
来源：http://ktz.zhengqikj.top

PHP:  $u instanceof User
来源：http://lib.yuxming.cn

JS:   u instanceof User
来源：http://men.hysaishi.cn

TS:   u instanceof User
来源：http://pxr.daxiang520.top

Java: u instanceof User
来源：http://vtd.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jtr.andypj.xyz

Ruby: u.is_a?(User)
来源：http://tip.yonumen.top

C#:   u is User
来源：http://nai.hnxiangtu.top

[G14] 数据类 / record
来源：http://mgn.gzhubu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ltb.andypj.xyz

PHP:  // 用 readonly 属性模拟
来源：http://tdm.fanxiaobao.xyz

JS:   // 无内置：普通类或对象字面量
来源：http://qrc.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://bjw.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://exe.sufxvd.cn

Go:   type User struct { Name string; Age int }
来源：http://ziz.hesvh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bkm.meibo888.top

C#:   record User(string Name, int Age);
来源：http://zto.feifeiyinyue.top

[G15] 枚举
来源：http://uls.gzhubu.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fcj.smart0.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://ekx.zhengqikj.top


<!-- 参考信息 -->