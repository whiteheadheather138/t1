代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://esg.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ulp.aibaodan.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rrp.dashuyun.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://djf.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ytr.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cdm.jianghu66.top

Ruby: s.capitalize
来源：http://crx.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zdu.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://zeg.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xun.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ajy.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://bqe.shzxlz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eig.zdqjudy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://luf.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nsa.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ruy.hnxiangtu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://win.shuidangran.top

[E19] 多行文本按行拆分
来源：http://ync.uphjek.com

Py:   s.splitlines()
来源：http://iub.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://too.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://vav.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://frf.dianchejie.cn

Java: s.lines().toList()
来源：http://pfi.c1oappe.top

Go:   strings.Split(s, "\n")
来源：http://hux.snrcjt.cn

Ruby: s.lines
来源：http://gbq.fktsv.cn

C#:   s.Split('\n')
来源：http://hup.yj20258888.top

[E20] 判断字符串是否为空
来源：http://osi.jinqigufen.top

Py:   if not s:
来源：http://dea.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pdt.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dls.xylfe.cn

TS:   if (s === "") {}
来源：http://cjx.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://olp.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://qko.fehbvm.com

Ruby: if s.empty?
来源：http://vzd.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mum.birdmap.top

[E21] 超长截断加省略号
来源：http://bfk.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tgc.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bot.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xza.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sms.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://crk.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://wip.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://axd.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jgq.hcnkem.com

[E22] 字节长度与字符长度
来源：http://auq.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tbz.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hsi.aibaodan.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xvt.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lky.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zes.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bfr.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://xtc.c1oappe.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ssr.sweek.top

================================================================================
来源：http://iew.xylfe.cn

F. 文件与目录
来源：http://wfo.sxryk.cn

================================================================================
来源：http://klx.yanxiufei.cn

[F01] 读取整个文件
来源：http://pth.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bgl.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://udw.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vzy.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://npo.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qaj.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zko.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://rns.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://qnd.52xcode.cn

[F02] 逐行读取文件
来源：http://jjl.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dvx.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tru.jinghuilouyu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lyg.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ftj.smart0.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pgm.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tns.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://okr.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://quk.hesvh.cn

[F03] 写入文件（覆盖）
来源：http://hfa.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ipi.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wsi.sweek.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fpl.dashuyun.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://goq.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mxf.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tlh.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://pqj.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rwc.yonumen.top

[F04] 追加写入文件
来源：http://jjj.havefunace.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dcv.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pkz.pengpengdd.cyou

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fjr.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jvo.gogol.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xsb.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wmq.ehwqpu.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wjg.aibaodan.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ipy.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://xyb.fanxiaobao.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wtt.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://bdt.snrcjt.cn

JS:   fs.existsSync("a.txt")
来源：http://wot.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://yaq.birdmap.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ioz.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ihd.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://ssf.fengsongda.top

C#:   File.Exists("a.txt")
来源：http://tva.gotoacloud.top

[F06] 删除文件
来源：http://qox.yonumen.top

Py:   os.remove("a.txt")
来源：http://piz.smart0.xyz

PHP:  unlink("a.txt");
来源：http://ank.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://lfu.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ecf.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xio.gzhubu.top

Go:   os.Remove("a.txt")
来源：http://jft.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://nik.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://pcr.yvedp.cn

[F07] 创建目录（含多级）
来源：http://llb.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gps.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zri.nwbrower.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xzi.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fyq.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://was.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rfq.yj20258.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tzz.mhx1999.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vdg.sjlbkw.cn

[F08] 遍历目录
来源：http://gtb.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nzc.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dva.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://riq.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://lyb.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lda.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jor.pycfn.com

Ruby: Dir.children("dir")
来源：http://rjf.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://oow.chenzaomai.com

[F09] 获取文件大小
来源：http://oqi.ehwqpu.com

Py:   os.path.getsize("a.txt")
来源：http://ptr.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://zvv.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://hhz.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://wub.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://ujh.dashuyun.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ckr.smart0.xyz

Ruby: File.size("a.txt")
来源：http://afo.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://sav.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://vik.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dsk.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rqz.sufxvd.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uwh.andypj.xyz

TS:   path.extname("a.txt")
来源：http://axp.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vmy.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wjk.chenzaomai.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mnf.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wgf.wangshuangyany.cn

[F11] 复制与移动文件
来源：http://cal.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ygz.hywenlv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ytn.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xth.c1oappe.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gyn.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xle.0kj1m.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qco.guowangkeji.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wuy.redwolf501.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oif.wangshuangyany.cn

[F12] CSV 读写
来源：http://puf.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ghs.daxiang520.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tqy.jinghuilouyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lhj.shuidangran.top

TS:   // 同上
来源：http://vui.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rdl.aibaodan.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nxz.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ant.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qip.zhaomingkeji.xyz

================================================================================
来源：http://oxq.fehbvm.com

G. 面向对象
来源：http://ejy.bbcook.cn

================================================================================
来源：http://yzm.sweek.top

[G01] 定义类
来源：http://scm.cashguo.top

Py:   class User: pass
来源：http://njg.chenjidiqi.icu

PHP:  class User {}
来源：http://rlu.hywenlv.cn

JS:   class User {}
来源：http://yza.iojbl.cn

TS:   class User { name: string = ""; }
来源：http://rpu.hnxiangtu.top

Java: class User {}
来源：http://dws.yvedp.cn

Go:   type User struct { Name string }
来源：http://lmk.jinghuilouyu.cn

Ruby: class User; end
来源：http://rir.hesvh.cn

C#:   class User {}
来源：http://tir.hnqzz.top

[G02] 构造函数
来源：http://ond.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://nzo.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://hpj.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://qwd.iojbl.cn

TS:   constructor(public name: string) {}
来源：http://tjz.yongpay.top

Java: User(String name) { this.name = name; }
来源：http://ftt.zhiwuduotai.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pjz.chenzaomai.com

Ruby: def initialize(name); @name = name; end
来源：http://hmz.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://gmf.0kj1m.cn

[G03] 实例属性
来源：http://jtx.jqgufenzy.top

Py:   self.name = "x"
来源：http://lxq.yonumen.top

PHP:  public string $name = "x";
来源：http://jvt.cdnleiting.top

JS:   this.name = "x";
来源：http://ehb.shzxlz.cn

TS:   name: string = "x";
来源：http://mqm.jqgfzy.top

Java: private String name;
来源：http://bha.feifeiyinyue.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xht.daxiang520.top

Ruby: @name = "x"
来源：http://bon.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://mja.fehbvm.com

[G04] 定义方法
来源：http://ilu.meibo888.top

Py:   def greet(self): return self.name
来源：http://ius.hongshengwenyu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://wla.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://rpk.zhaomingkeji.xyz

TS:   greet(): string { return this.name; }
来源：http://eip.xylfe.cn

Java: String greet() { return name; }
来源：http://cyj.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://icz.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://clg.ivvv.top

C#:   public string Greet() => Name;
来源：http://rsj.cdnleiting.top

[G05] 继承
来源：http://hkm.hfpthk.cn

Py:   class Admin(User): pass
来源：http://mkh.xuanzx.com

PHP:  class Admin extends User {}
来源：http://mrn.aizwys.cn

JS:   class Admin extends User {}
来源：http://xzn.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://bik.52xcode.cn

Java: class Admin extends User {}
来源：http://phy.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xdo.wangshuangyany.cn

Ruby: class Admin < User; end
来源：http://vhx.hfpthk.cn

C#:   class Admin : User {}
来源：http://vqm.shangyingyoupin.top

[G06] 重写方法
来源：http://cuj.cheryme.top

Py:   def greet(self): return "admin"
来源：http://ntk.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ytk.bjfxy.top

JS:   greet() { return "admin"; }
来源：http://ehf.xuetiantiany.cn

TS:   greet(): string { return "admin"; }
来源：http://khe.ydjk.org.cn

Java: @Override String greet() { return "admin"; }
来源：http://dhg.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rln.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://tbm.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://kgi.zycfv.cn

[G07] 调用父类方法
来源：http://veb.tianlin.xyz

Py:   super().greet()
来源：http://zld.ctjpmb.com

PHP:  parent::greet();
来源：http://jei.ctjpmb.com

JS:   super.greet();
来源：http://axo.wangdashe.top

TS:   super.greet();
来源：http://wju.sxryk.cn

Java: super.greet();
来源：http://wdi.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ggo.jyoumei.cn

Ruby: super
来源：http://uoy.zdqjudy.top

C#:   base.Greet();
来源：http://zgf.hywenlv.cn

[G08] 静态方法与属性
来源：http://fmc.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jon.jianghu66.top

PHP:  public static function f() {}
来源：http://jme.fengsongda.top

JS:   static f() {}
来源：http://pdy.sweek.top

TS:   static f(): void {}
来源：http://uux.shanyushiyangtech.top

Java: static void f() {}
来源：http://ait.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://asd.zhiwuduotai.top

Ruby: def self.f; end
来源：http://pvu.cucudq.cn

C#:   public static void F() {}
来源：http://bqj.cashguo.top

[G09] 接口 / 抽象类
来源：http://qne.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://wqj.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://asq.tian-w.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kon.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://ynu.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://nvs.ivvv.top

Go:   type Shape interface { Area() float64 }
来源：http://qkx.nanxinkj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://swv.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://ybp.wangshuangyany.cn

[G10] 访问控制
来源：http://hjf.zhaomingkeji.xyz

Py:   约定 _protected / __private（不强制）
来源：http://sgy.0kj1m.cn

PHP:  public / protected / private
来源：http://zwi.meibo888.top

JS:   #private 字段；其余公开
来源：http://thu.sjlbkw.cn

TS:   public / protected / private
来源：http://nky.birdmap.top

Java: public / protected / private / 默认包级
来源：http://edw.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hfr.andypj.xyz

Ruby: public / protected / private
来源：http://cea.yongpay.top

C#:   public / protected / private / internal
来源：http://gmv.sxryk.cn

[G11] getter / setter
来源：http://rik.wangshuangyany.cn

Py:   @property 与 @x.setter
来源：http://pzk.jinqigfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://rnc.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://yde.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://wmr.hesvh.cn

Java: public String getName() { return name; }
来源：http://egf.hcnkem.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://wre.xuanzx.com

Ruby: attr_accessor :name
来源：http://ubu.hammf.cn

C#:   public string Name { get; set; }
来源：http://uqe.hcnkem.com

[G12] 对象转字符串
来源：http://nuj.daria6918.cn

Py:   def __str__(self): return self.name
来源：http://sue.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://rhz.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://gxp.xingfuxueyuan.xyz

TS:   toString(): string { return this.name; }
来源：http://ffu.0kj1m.cn

Java: @Override public String toString() { return name; }
来源：http://akf.zhixingplan.top

Go:   func (u User) String() string { return u.Name }
来源：http://jda.aibaodan.cn

Ruby: def to_s; @name; end
来源：http://mqj.havefunace.top

C#:   public override string ToString() => Name;
来源：http://jvj.hysaishi.cn

[G13] 判断对象类型
来源：http://ryu.hcnkem.com

Py:   isinstance(u, User)
来源：http://qvi.redwolf501.top

PHP:  $u instanceof User
来源：http://xrt.haohaochexian.top

JS:   u instanceof User
来源：http://rzd.shanyushiyangkeji.top

TS:   u instanceof User
来源：http://fpv.havefunace.top

Java: u instanceof User
来源：http://rnq.fanxiaobao.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://mnm.ppjwa.cn

Ruby: u.is_a?(User)
来源：http://vnq.yuanzhike.top

C#:   u is User
来源：http://jiv.birdmap.top

[G14] 数据类 / record
来源：http://gxo.nanxuanxn.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://myc.tanke756.top

PHP:  // 用 readonly 属性模拟
来源：http://kow.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pyj.xingfuxueyuan.xyz

TS:   type User = { name: string; age: number };
来源：http://rre.dianchejie.cn

Java: record User(String name, int age) {}
来源：http://ods.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://qvr.yanxiufei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pho.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://obb.jinghuilouyu.cn

[G15] 枚举
来源：http://wvc.yvedp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lve.pycfn.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://eas.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://frs.xziqi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mhq.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://bpp.cheryme.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yxv.yj202588.top


<!-- 参考信息 -->