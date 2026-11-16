代发 wailian999

[E18] 模板占位符替换
来源：http://fqn.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dzi.iojbl.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://udd.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fmf.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rdw.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ivx.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iuk.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mqu.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pou.meibo888.top

[E19] 多行文本按行拆分
来源：http://ouh.hfpthk.cn

Py:   s.splitlines()
来源：http://olx.tarul.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dam.nanxinkj.top

JS:   s.split(/\r?\n/)
来源：http://aje.havefunace.top

TS:   s.split(/\r?\n/)
来源：http://hyj.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://ilx.zdqjudy.top

Go:   strings.Split(s, "\n")
来源：http://cwo.chenlongwang.top

Ruby: s.lines
来源：http://gwm.fzhhl.top

C#:   s.Split('\n')
来源：http://kdd.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://ckh.jqgfzy.top

Py:   if not s:
来源：http://vos.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ide.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qzh.hnqzz.top

TS:   if (s === "") {}
来源：http://srt.xinyue.icu

Java: if (s.isEmpty()) {}
来源：http://chk.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://eue.iojbl.cn

Ruby: if s.empty?
来源：http://htg.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fjd.yonumen.top

[E21] 超长截断加省略号
来源：http://tti.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vjs.nanxuanxn.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://suk.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fkd.zhongyouzk.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwe.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pyx.fengsongda.top

Go:   // 按 rune 判断长度后截断
来源：http://bvh.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://saq.wangshuangyany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ksv.ydzc1.top

[E22] 字节长度与字符长度
来源：http://lcb.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wtd.jinqigfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mmd.nanxinkj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ooh.daria6918.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jzx.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nck.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lvg.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://wta.yfazqb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hol.zdqjudy.top

================================================================================
来源：http://vcb.zhaomingkeji.xyz

F. 文件与目录
来源：http://vqk.kuanghao11.cn

================================================================================
来源：http://wai.tian-w.cn

[F01] 读取整个文件
来源：http://gis.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zpm.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://jtw.xylfe.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://umz.redwolf501.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ejh.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bza.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hym.yj202588.top

Ruby: File.read("a.txt")
来源：http://mta.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://lbd.yuanzhike.top

[F02] 逐行读取文件
来源：http://bst.sysykeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ems.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qwx.guannengcc.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://psr.chenzaomai.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nmi.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rem.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://smq.jqgufenzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oeh.fehbvm.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zzc.gotoacloud.top

[F03] 写入文件（覆盖）
来源：http://xwi.yj20258888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aem.zhaomingkeji.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://pug.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gkn.yuxming.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iaa.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hvc.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://myx.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://ebt.gaohongyu789.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fgo.52xcode.cn

[F04] 追加写入文件
来源：http://wyq.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://imk.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xdc.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gjj.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tvw.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tam.zdbjq.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hxv.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://liz.xylfe.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mxv.ehwqpu.com

[F05] 判断文件或目录是否存在
来源：http://klm.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://syr.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://wnw.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://fca.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://pzt.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cxb.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pnb.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://rnj.wangshuangyany.cn

C#:   File.Exists("a.txt")
来源：http://mzl.yangfankeji.com

[F06] 删除文件
来源：http://xxt.smart0.xyz

Py:   os.remove("a.txt")
来源：http://ldq.sysykeji.top

PHP:  unlink("a.txt");
来源：http://rwb.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mvv.hywenlv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cwf.hysaishi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hmt.yfazqb.com

Go:   os.Remove("a.txt")
来源：http://gtj.uphjek.com

Ruby: File.delete("a.txt")
来源：http://mmt.sweek.top

C#:   File.Delete("a.txt");
来源：http://irj.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://mpt.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xgl.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zoz.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kys.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fji.daxiang520.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zug.quarkkingdee.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yty.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hfo.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ipz.yongpay.top

[F08] 遍历目录
来源：http://mri.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://mef.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ncb.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://tmi.dashuyun.cn

TS:   fs.readdirSync("dir")
来源：http://hiq.sxryk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mdh.jinqigufen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kbw.fktsv.cn

Ruby: Dir.children("dir")
来源：http://toy.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://phw.jlsjyb.cn

[F09] 获取文件大小
来源：http://trt.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://ioh.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://nii.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://nfj.smart0.xyz

TS:   fs.statSync("a.txt").size
来源：http://nlh.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://ewa.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jys.jlsjyb.cn

Ruby: File.size("a.txt")
来源：http://vke.jinqigfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://gts.redwolf501.top

[F10] 取文件扩展名 / 文件名
来源：http://zkg.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ysl.chenzaomai.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xmo.gaohongyu789.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://drs.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://qev.guannengcc.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hrm.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://twy.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://spk.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sai.gogol.net.cn

[F11] 复制与移动文件
来源：http://gap.cqqwz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vjj.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://etq.jyoumei.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fju.gogol.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uki.c1oappe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fmg.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://flf.xziqi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://clu.xziqi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qmq.shuidangran.top

[F12] CSV 读写
来源：http://hfr.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cwl.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://egw.bbcook.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://buc.jinqigfzy.top

TS:   // 同上
来源：http://jtt.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://psf.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://neo.redwolf501.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qqc.cashguo.top

C#:   // 无内置：用 CsvHelper 库
来源：http://lnr.jinqigfzy.top

================================================================================
来源：http://gob.zhaomingkeji.xyz

G. 面向对象
来源：http://yqf.xingfuxueyuan.xyz

================================================================================
来源：http://mxr.yj20258.top

[G01] 定义类
来源：http://bwy.birdmap.top

Py:   class User: pass
来源：http://iwv.daria6918.cn

PHP:  class User {}
来源：http://eyj.yj20258.top

JS:   class User {}
来源：http://jpb.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://lot.fanxiaobao.xyz

Java: class User {}
来源：http://jwe.hywenlv.cn

Go:   type User struct { Name string }
来源：http://tyo.yfazqb.com

Ruby: class User; end
来源：http://cek.chenzaomai.com

C#:   class User {}
来源：http://bql.tarul.cn

[G02] 构造函数
来源：http://cxy.bjfxy.top

Py:   def __init__(self, name): self.name = name
来源：http://dld.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://aet.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://jao.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://nbi.aizwys.cn

Java: User(String name) { this.name = name; }
来源：http://icx.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mvz.hongshengwenyu.top

Ruby: def initialize(name); @name = name; end
来源：http://vbs.jyoumei.cn

C#:   public User(string name) { Name = name; }
来源：http://qmn.cucudq.cn

[G03] 实例属性
来源：http://csm.ehwqpu.com

Py:   self.name = "x"
来源：http://cwx.daria6918.cn

PHP:  public string $name = "x";
来源：http://eme.epnwcf.com

JS:   this.name = "x";
来源：http://qpi.meibo888.top

TS:   name: string = "x";
来源：http://jxo.ppjwa.cn

Java: private String name;
来源：http://biq.wangdashe.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mmr.nanxinkj.top

Ruby: @name = "x"
来源：http://xmh.bbcook.cn

C#:   public string Name { get; set; } = "x";
来源：http://utv.cheryme.top

[G04] 定义方法
来源：http://ouf.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://gkj.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uhk.hfpthk.cn

JS:   greet() { return this.name; }
来源：http://chm.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://tbt.jinqigufen.top

Java: String greet() { return name; }
来源：http://trt.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sqo.yj202588.top

Ruby: def greet; @name; end
来源：http://hyl.nanxuanxn.top

C#:   public string Greet() => Name;
来源：http://haa.vqdsnc.cn

[G05] 继承
来源：http://tdb.nwbrower.top

Py:   class Admin(User): pass
来源：http://bfg.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://cwu.cdnleiting.top

JS:   class Admin extends User {}
来源：http://sal.jlsjyb.cn

TS:   class Admin extends User {}
来源：http://hqg.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://whz.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fqw.hnqzz.top

Ruby: class Admin < User; end
来源：http://wwd.gogol.net.cn

C#:   class Admin : User {}
来源：http://vsd.jinqigfzy.top

[G06] 重写方法
来源：http://stz.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://rju.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pkm.jinqigufen.top

JS:   greet() { return "admin"; }
来源：http://gix.ybcxt.top

TS:   greet(): string { return "admin"; }
来源：http://vin.sweek.top

Java: @Override String greet() { return "admin"; }
来源：http://yso.vehdjk.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://trk.zhoulong.xyz

Ruby: def greet; "admin"; end
来源：http://vir.yuxming.cn

C#:   public override string Greet() => "admin";
来源：http://lhg.cheryme.top

[G07] 调用父类方法
来源：http://bhs.zdbjq.cn

Py:   super().greet()
来源：http://ymk.xylfe.cn

PHP:  parent::greet();
来源：http://dzn.yongpay.top

JS:   super.greet();
来源：http://dvw.xuetiantiany.cn

TS:   super.greet();
来源：http://cxm.gogol.net.cn

Java: super.greet();
来源：http://jvo.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://amz.pengpengdd.cyou

Ruby: super
来源：http://khd.xziqi.cn

C#:   base.Greet();
来源：http://goc.ywan-chungtsiang.top

[G08] 静态方法与属性
来源：http://dbe.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zmf.nwbrower.top

PHP:  public static function f() {}
来源：http://xhp.gaohongyu789.top

JS:   static f() {}
来源：http://sni.316326.xyz

TS:   static f(): void {}
来源：http://gji.dianchejie.cn

Java: static void f() {}
来源：http://rdl.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://tlq.epnwcf.com

Ruby: def self.f; end
来源：http://eeq.vehdjk.com

C#:   public static void F() {}
来源：http://asr.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://mta.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://yot.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://gdj.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://akn.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://cpp.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://lex.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://vzt.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lrc.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://msu.vehdjk.com

[G10] 访问控制
来源：http://gwv.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://haq.quarkkingdee.top

PHP:  public / protected / private
来源：http://hsv.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://hrh.jqgufenzy.top

TS:   public / protected / private
来源：http://vaz.cashguo.top

Java: public / protected / private / 默认包级
来源：http://pug.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://rbo.uphjek.com

Ruby: public / protected / private
来源：http://wly.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://nvq.havefunace.top

[G11] getter / setter
来源：http://pox.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://rxd.zhijiandao.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qlp.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://wih.dianchejie.cn

TS:   get name(): string { return this._name; }
来源：http://ofy.hnqzz.top

Java: public String getName() { return name; }
来源：http://lyh.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://vga.aizwys.cn

Ruby: attr_accessor :name
来源：http://zhh.yanxiufei.cn

C#:   public string Name { get; set; }
来源：http://lbx.ppjwa.cn

[G12] 对象转字符串
来源：http://lwn.hywenlv.cn

Py:   def __str__(self): return self.name
来源：http://mqy.vehdjk.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://rst.daxiang520.top

JS:   toString() { return this.name; }
来源：http://klc.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://duy.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://jiq.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://whh.uphjek.com

Ruby: def to_s; @name; end
来源：http://zyb.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://hmn.jinghuilouyu.cn

[G13] 判断对象类型
来源：http://utq.ybcxt.top

Py:   isinstance(u, User)
来源：http://lgj.snrcjt.cn

PHP:  $u instanceof User
来源：http://gnb.guowangkeji.top

JS:   u instanceof User
来源：http://rfp.nwbrower.top

TS:   u instanceof User
来源：http://rgs.hesvh.cn

Java: u instanceof User
来源：http://apo.xuanzx.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://cqk.havefunace.top

Ruby: u.is_a?(User)
来源：http://tus.guannengcc.top

C#:   u is User
来源：http://fzz.gogol.net.cn

[G14] 数据类 / record
来源：http://ymc.guannengcc.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vwb.dianchejie.cn

PHP:  // 用 readonly 属性模拟
来源：http://apu.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://tuf.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://sls.vqdsnc.cn

Java: record User(String name, int age) {}
来源：http://mcg.yuanzhike.top

Go:   type User struct { Name string; Age int }
来源：http://lwb.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bjq.svipenyu.cn

C#:   record User(string Name, int Age);
来源：http://pza.chenzaomai.com

[G15] 枚举
来源：http://mdr.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aik.yuxming.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vex.dashuyun.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qke.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fei.nwbrower.top

Java: enum Color { RED, GREEN }
来源：http://tal.jqgfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://not.chenlongwang.top

Ruby: Color = %i[red green].freeze
来源：http://slz.birdmap.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rkd.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://mgk.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zru.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://ugr.pycfn.com

JS:   Object.entries(obj)
来源：http://qxp.zhongyouzk.top

TS:   Object.entries(obj)
来源：http://aho.aibaodan.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xhg.zhongyouzk.top


<!-- 参考信息 -->