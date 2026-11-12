代发 wailian999

[E18] 模板占位符替换
来源：http://sxa.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ggb.zhongyouzk.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://poq.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://seh.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vcx.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jyt.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hfv.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ulk.zdqjudy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wvd.andypj.xyz

[E19] 多行文本按行拆分
来源：http://jzr.316326.xyz

Py:   s.splitlines()
来源：http://dxz.tian-w.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://evf.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://icn.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://dsp.svipenyu.cn

Java: s.lines().toList()
来源：http://oiw.sxryk.cn

Go:   strings.Split(s, "\n")
来源：http://mpk.guannengcc.top

Ruby: s.lines
来源：http://pkg.yonumen.top

C#:   s.Split('\n')
来源：http://qzx.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://lrp.zhengqikj.top

Py:   if not s:
来源：http://zoc.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xmb.gotoacloud.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qpu.nanxuanxn.top

TS:   if (s === "") {}
来源：http://hqh.sweek.top

Java: if (s.isEmpty()) {}
来源：http://itk.nwbrower.top

Go:   if s == "" {}
来源：http://tmn.bjfxy.top

Ruby: if s.empty?
来源：http://ccg.yanxiufei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bmm.chenzaomai.com

[E21] 超长截断加省略号
来源：http://icy.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xye.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qpu.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nlk.tianlin.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xpr.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uvf.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://exe.cheryme.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aze.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://frv.smart0.xyz

[E22] 字节长度与字符长度
来源：http://hmx.hysaishi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://djk.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uho.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pea.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nds.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gjd.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cug.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://khn.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pik.yuanzhike.top

================================================================================
来源：http://roq.yj20258888.top

F. 文件与目录
来源：http://kgz.jqgfzy.top

================================================================================
来源：http://ctq.xylfe.cn

[F01] 读取整个文件
来源：http://hgz.bbcook.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jao.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://awl.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aop.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://brd.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bcb.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xrf.iojbl.cn

Ruby: File.read("a.txt")
来源：http://tlc.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://din.cashguo.top

[F02] 逐行读取文件
来源：http://tmk.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kuy.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ntd.andypj.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bxs.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ndy.zhixingplan.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zlc.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fud.zhijiandao.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hzw.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://isc.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://ebi.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zyl.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://zxb.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zdn.birdmap.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vpg.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lcj.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://poz.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://gsd.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://whq.aibaodan.cn

[F04] 追加写入文件
来源：http://ina.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xbr.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rjf.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfi.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gel.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zwi.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cvy.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://caj.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nwj.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://bxs.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vdh.zhoulong.xyz

PHP:  file_exists("a.txt");
来源：http://ibc.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://crp.tarul.cn

TS:   fs.existsSync("a.txt")
来源：http://yeq.ctjpmb.com

Java: Files.exists(Path.of("a.txt"))
来源：http://uba.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zdg.guannengcc.top

Ruby: File.exist?("a.txt")
来源：http://tng.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://jwq.hammf.cn

[F06] 删除文件
来源：http://vjg.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://yap.zhongyouzk.top

PHP:  unlink("a.txt");
来源：http://kph.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fkb.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nlo.yj20258.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xph.tarul.cn

Go:   os.Remove("a.txt")
来源：http://waf.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://qyi.tarul.cn

C#:   File.Delete("a.txt");
来源：http://gek.mhx1999.top

[F07] 创建目录（含多级）
来源：http://jql.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gvq.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xyv.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://osu.yj202588.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eqm.yanxiufei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://frs.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yvl.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fdv.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hra.vehdjk.com

[F08] 遍历目录
来源：http://nfd.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://gfg.bjfxy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blc.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://lxt.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://qoi.yvedp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cst.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lpa.pycfn.com

Ruby: Dir.children("dir")
来源：http://miq.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://sie.zhixingplan.top

[F09] 获取文件大小
来源：http://fuw.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://dxz.yj20258.top

PHP:  filesize("a.txt");
来源：http://xqb.yangfankeji.com

JS:   fs.statSync("a.txt").size
来源：http://chu.bbcook.cn

TS:   fs.statSync("a.txt").size
来源：http://sht.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bfe.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ita.yueranfly.top

Ruby: File.size("a.txt")
来源：http://atv.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://pvd.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://rmr.nwbrower.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gzr.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ozr.zhijiandao.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://njn.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://rxj.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rrz.316326.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gwx.jinghuilouyu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kwr.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lot.ctjpmb.com

[F11] 复制与移动文件
来源：http://hfw.iojbl.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fus.ybcxt.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://agu.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://els.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bud.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pwa.xuetiantiany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lah.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rhz.hywenlv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ttw.hesvh.cn

[F12] CSV 读写
来源：http://ssf.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://plu.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lwn.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://boj.bbcook.cn

TS:   // 同上
来源：http://aiz.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lui.tian-w.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://smj.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lej.cheryme.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bga.daria6918.cn

================================================================================
来源：http://sjf.yj20258.top

G. 面向对象
来源：http://xsc.jinqigufen.top

================================================================================
来源：http://ldu.cqqwz.cn

[G01] 定义类
来源：http://xwx.jinqigfzy.top

Py:   class User: pass
来源：http://dto.yueranfly.top

PHP:  class User {}
来源：http://wzh.cucudq.cn

JS:   class User {}
来源：http://yti.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://sky.shanyushiyangtech.top

Java: class User {}
来源：http://zjh.xziqi.cn

Go:   type User struct { Name string }
来源：http://byq.gogol.net.cn

Ruby: class User; end
来源：http://pza.sxryk.cn

C#:   class User {}
来源：http://eqp.gzhubu.top

[G02] 构造函数
来源：http://fue.fanxiaobao.xyz

Py:   def __init__(self, name): self.name = name
来源：http://eca.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://vyy.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://iih.jiagoushi.top

TS:   constructor(public name: string) {}
来源：http://axz.gzhubu.top

Java: User(String name) { this.name = name; }
来源：http://fwy.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://twc.uphjek.com

Ruby: def initialize(name); @name = name; end
来源：http://anl.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://jao.fehbvm.com

[G03] 实例属性
来源：http://yau.guannengcc.top

Py:   self.name = "x"
来源：http://bad.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://ond.gogol.net.cn

JS:   this.name = "x";
来源：http://oqm.tarul.cn

TS:   name: string = "x";
来源：http://nlx.zdbjq.cn

Java: private String name;
来源：http://ugi.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hip.chenzaomai.com

Ruby: @name = "x"
来源：http://syf.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://efw.kuanghao11.cn

[G04] 定义方法
来源：http://jam.yangfankeji.com

Py:   def greet(self): return self.name
来源：http://bzh.birdmap.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kfi.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://xyq.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://ldf.yuxming.cn

Java: String greet() { return name; }
来源：http://yyc.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uhb.pycfn.com

Ruby: def greet; @name; end
来源：http://lyg.sysykeji.top

C#:   public string Greet() => Name;
来源：http://qls.xuanzx.com

[G05] 继承
来源：http://ook.cqqwz.cn

Py:   class Admin(User): pass
来源：http://fte.yonumen.top

PHP:  class Admin extends User {}
来源：http://gho.jyoumei.cn

JS:   class Admin extends User {}
来源：http://hix.zhengqikj.top

TS:   class Admin extends User {}
来源：http://llq.vqdsnc.cn

Java: class Admin extends User {}
来源：http://mec.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://twf.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://udl.meibo888.top

C#:   class Admin : User {}
来源：http://oca.zhixingplan.top

[G06] 重写方法
来源：http://hqa.jianghu66.top

Py:   def greet(self): return "admin"
来源：http://duf.uphjek.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kdu.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://cky.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://inn.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://sck.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ijx.ehwqpu.com

Ruby: def greet; "admin"; end
来源：http://mbn.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://fvz.hysaishi.cn

[G07] 调用父类方法
来源：http://mqy.svipenyu.cn

Py:   super().greet()
来源：http://auk.hongshengwenyu.top

PHP:  parent::greet();
来源：http://iek.fanxiaobao.xyz

JS:   super.greet();
来源：http://zuh.tian-w.cn

TS:   super.greet();
来源：http://qwe.gaohongyu789.top

Java: super.greet();
来源：http://icv.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ner.fehbvm.com

Ruby: super
来源：http://jxg.guowangkeji.top

C#:   base.Greet();
来源：http://yhh.zdbjq.cn

[G08] 静态方法与属性
来源：http://kao.zhongyouzk.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tjy.cucudq.cn

PHP:  public static function f() {}
来源：http://hhs.meibo888.top

JS:   static f() {}
来源：http://jyb.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://mqo.daria6918.cn

Java: static void f() {}
来源：http://mwn.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://uwu.xinyue.icu

Ruby: def self.f; end
来源：http://pao.hcnkem.com

C#:   public static void F() {}
来源：http://biq.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://vfd.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gaj.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hvt.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://klg.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://rbb.fehbvm.com

Java: interface Shape { double area(); }
来源：http://oyk.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://pga.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tzg.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://hct.wangshuangyany.cn

[G10] 访问控制
来源：http://jdm.xylfe.cn

Py:   约定 _protected / __private（不强制）
来源：http://lpk.zycfv.cn

PHP:  public / protected / private
来源：http://ukg.jqgufenzy.top

JS:   #private 字段；其余公开
来源：http://dlc.aizwys.cn

TS:   public / protected / private
来源：http://ods.bbcook.cn

Java: public / protected / private / 默认包级
来源：http://pqb.chenjidiqi.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://ccn.xziqi.cn

Ruby: public / protected / private
来源：http://ohf.cdnleiting.top

C#:   public / protected / private / internal
来源：http://idn.snrcjt.cn

[G11] getter / setter
来源：http://gdf.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://ouw.jqgfzy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dtw.mhx1999.top

JS:   get name() { return this._name; }
来源：http://mmm.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://bdx.ivvv.top

Java: public String getName() { return name; }
来源：http://uob.316326.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://mne.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://mul.wangshuangyany.cn

C#:   public string Name { get; set; }
来源：http://aot.chenzaomai.com

[G12] 对象转字符串
来源：http://tks.shanyushiyangkeji.top

Py:   def __str__(self): return self.name
来源：http://cvn.zdbjq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://maq.zhijiandao.cn

JS:   toString() { return this.name; }
来源：http://gai.uphjek.com

TS:   toString(): string { return this.name; }
来源：http://xwm.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://ruz.hesvh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zqj.smart0.xyz

Ruby: def to_s; @name; end
来源：http://raz.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://bhk.nanxuanxn.top

[G13] 判断对象类型
来源：http://rih.jyoumei.cn

Py:   isinstance(u, User)
来源：http://xvt.xziqi.cn

PHP:  $u instanceof User
来源：http://gtf.pycfn.com

JS:   u instanceof User
来源：http://nhe.cheryme.top

TS:   u instanceof User
来源：http://ywp.zhixingplan.top

Java: u instanceof User
来源：http://mhz.aibaodan.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lzk.zdbjq.cn

Ruby: u.is_a?(User)
来源：http://qzi.jqgfzy.top

C#:   u is User
来源：http://oxs.yuxming.cn

[G14] 数据类 / record
来源：http://amt.zhijiandao.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://loa.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://arz.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://vut.cqqwz.cn

TS:   type User = { name: string; age: number };
来源：http://xox.daria6918.cn

Java: record User(String name, int age) {}
来源：http://aoq.xingfuxueyuan.xyz

Go:   type User struct { Name string; Age int }
来源：http://veb.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zpw.yonumen.top

C#:   record User(string Name, int Age);
来源：http://mnh.daxiang520.top

[G15] 枚举
来源：http://bdh.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bhk.pengpengdd.cyou

PHP:  enum Color: string { case Red = "red"; }
来源：http://lhb.hnqzz.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xlw.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kqy.yj20258.top

Java: enum Color { RED, GREEN }
来源：http://tij.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uta.fktsv.cn

Ruby: Color = %i[red green].freeze
来源：http://out.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ejt.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://mdj.jlsjyb.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oel.fzhhl.top

PHP:  get_object_vars($obj);
来源：http://egm.chenlongwang.top

JS:   Object.entries(obj)
来源：http://nxs.yonumen.top

TS:   Object.entries(obj)
来源：http://pxr.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wiq.tianlin.xyz


<!-- 参考信息 -->