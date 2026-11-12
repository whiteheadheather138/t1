代发 wailian999

[E18] 模板占位符替换
来源：http://wah.shzxlz.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ted.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://idy.sxryk.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xhs.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://guk.daxiang520.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hly.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sqh.zdbjq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xty.cqqwz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ewk.hammf.cn

[E19] 多行文本按行拆分
来源：http://qcl.ivvv.top

Py:   s.splitlines()
来源：http://sev.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iks.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://ekg.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://rdy.kuanghao11.cn

Java: s.lines().toList()
来源：http://lhk.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://xlt.gzhubu.top

Ruby: s.lines
来源：http://njf.mhx1999.top

C#:   s.Split('\n')
来源：http://kjb.jyoumei.cn

[E20] 判断字符串是否为空
来源：http://dws.pengpengdd.cyou

Py:   if not s:
来源：http://uga.shzxlz.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vcq.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://urf.jyoumei.cn

TS:   if (s === "") {}
来源：http://xib.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://ver.yuxming.cn

Go:   if s == "" {}
来源：http://ule.iojbl.cn

Ruby: if s.empty?
来源：http://ygq.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vyd.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://xeb.jianghu66.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rcj.birdmap.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jpy.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://caf.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wqi.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eej.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://ilg.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://amb.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://inj.meibo888.top

[E22] 字节长度与字符长度
来源：http://rbn.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wcx.cqqwz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mhl.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uka.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nyw.yfazqb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ria.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jsg.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://uuu.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jdn.chenlongwang.top

================================================================================
来源：http://mqm.meibo888.top

F. 文件与目录
来源：http://ajk.ybcxt.top

================================================================================
来源：http://pqg.shangyingyoupin.top

[F01] 读取整个文件
来源：http://lpb.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://czp.guowangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://ehk.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ynr.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qvs.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gck.zdbjq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zta.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://abi.yuanzhike.top

C#:   File.ReadAllText("a.txt");
来源：http://ese.fzhhl.top

[F02] 逐行读取文件
来源：http://eds.xylfe.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ptr.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vzy.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iuy.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bbp.yj20258888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://els.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qpi.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hjx.9152youxi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nuw.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://xef.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wbe.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://cvs.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://viz.cashguo.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ttg.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gbd.uphjek.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qkq.ivvv.top

Ruby: File.write("a.txt", "hi")
来源：http://tjv.ybcxt.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zzs.xinyue.icu

[F04] 追加写入文件
来源：http://pie.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tgz.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fyd.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xvf.havefunace.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nzx.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aay.jlsjyb.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://czs.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nqr.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ets.jinqigufen.top

[F05] 判断文件或目录是否存在
来源：http://zlj.vqdsnc.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://esi.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://qmu.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://rrp.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://txz.gotoacloud.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xuw.guowangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zxt.hesvh.cn

Ruby: File.exist?("a.txt")
来源：http://qsu.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://yvu.zhaomingkeji.xyz

[F06] 删除文件
来源：http://rgp.sufxvd.cn

Py:   os.remove("a.txt")
来源：http://lml.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://lsa.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://gey.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://zwu.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tec.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://exy.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://akt.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://xed.jinyuanbaomall.cn

[F07] 创建目录（含多级）
来源：http://jho.sxryk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mtp.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://acn.c1oappe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjg.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwi.zhixingplan.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uhp.dashuyun.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://luz.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rov.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nog.hongshengwenyu.top

[F08] 遍历目录
来源：http://iuh.hywenlv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://myj.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cho.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://jky.quarkkingdee.top

TS:   fs.readdirSync("dir")
来源：http://wus.shzxlz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://keu.hcnkem.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://bgk.c1oappe.top

Ruby: Dir.children("dir")
来源：http://yki.c1oappe.top

C#:   Directory.GetFiles("dir")
来源：http://ine.yfazqb.com

[F09] 获取文件大小
来源：http://bvy.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://vpe.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://avp.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://vrq.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://iit.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://oym.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cva.c1oappe.top

Ruby: File.size("a.txt")
来源：http://pwv.dianchejie.cn

C#:   new FileInfo("a.txt").Length
来源：http://dkx.cdnleiting.top

[F10] 取文件扩展名 / 文件名
来源：http://fnc.xuetiantiany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qif.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lsu.birdmap.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eir.vehdjk.com

TS:   path.extname("a.txt")
来源：http://far.tian-w.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wkb.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rbm.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dyc.kuanghao11.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ddm.yuanzhike.top

[F11] 复制与移动文件
来源：http://pnr.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://edu.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://irk.yangfankeji.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uoq.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nmo.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://clb.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dkb.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ney.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://seo.fengsongda.top

[F12] CSV 读写
来源：http://mhq.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://omg.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://amo.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://err.jinyuanbaomall.cn

TS:   // 同上
来源：http://yom.fengsongda.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qzq.316326.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ijw.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lrs.smart0.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://gih.aibaodan.cn

================================================================================
来源：http://mhz.yvedp.cn

G. 面向对象
来源：http://rxz.chenlongwang.top

================================================================================
来源：http://jbb.chenjidiqi.icu

[G01] 定义类
来源：http://zff.yanxiufei.cn

Py:   class User: pass
来源：http://oee.yuanzhike.top

PHP:  class User {}
来源：http://cqz.52xcode.cn

JS:   class User {}
来源：http://txl.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://kmu.guannengcc.top

Java: class User {}
来源：http://pny.gzhubu.top

Go:   type User struct { Name string }
来源：http://xzo.feifeiyinyue.top

Ruby: class User; end
来源：http://ged.yongpay.top

C#:   class User {}
来源：http://abi.zycfv.cn

[G02] 构造函数
来源：http://otg.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://hxw.c1oappe.top

PHP:  public function __construct(public string $name) {}
来源：http://sdc.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://bqz.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://pyd.epnwcf.com

Java: User(String name) { this.name = name; }
来源：http://uvz.sweek.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fkf.hysaishi.cn

Ruby: def initialize(name); @name = name; end
来源：http://guh.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://oog.jqgfzy.top

[G03] 实例属性
来源：http://abq.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://gbr.fktsv.cn

PHP:  public string $name = "x";
来源：http://pmd.zhaomingkeji.xyz

JS:   this.name = "x";
来源：http://gow.fzhhl.top

TS:   name: string = "x";
来源：http://ywf.quarkkingdee.top

Java: private String name;
来源：http://yzh.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gip.snrcjt.cn

Ruby: @name = "x"
来源：http://xvt.zdbjq.cn

C#:   public string Name { get; set; } = "x";
来源：http://smf.hysaishi.cn

[G04] 定义方法
来源：http://omr.hywenlv.cn

Py:   def greet(self): return self.name
来源：http://zwp.gogol.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://idw.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://klh.sjlbkw.cn

TS:   greet(): string { return this.name; }
来源：http://mwl.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://pun.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qnz.jianghu66.top

Ruby: def greet; @name; end
来源：http://pfz.havefunace.top

C#:   public string Greet() => Name;
来源：http://iyl.guowangkeji.top

[G05] 继承
来源：http://flb.316326.xyz

Py:   class Admin(User): pass
来源：http://uzg.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://nrv.yuxming.cn

JS:   class Admin extends User {}
来源：http://fyw.hammf.cn

TS:   class Admin extends User {}
来源：http://uva.hcnkem.com

Java: class Admin extends User {}
来源：http://jtt.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kcr.0kj1m.cn

Ruby: class Admin < User; end
来源：http://tkz.yj202588.top

C#:   class Admin : User {}
来源：http://rdx.jinyuanbaomall.cn

[G06] 重写方法
来源：http://rdg.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://msc.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gpw.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://yef.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://iuy.ivvv.top

Java: @Override String greet() { return "admin"; }
来源：http://gtz.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rip.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://tnf.cashguo.top

C#:   public override string Greet() => "admin";
来源：http://dub.tian-w.cn

[G07] 调用父类方法
来源：http://pqm.shanyushiyangtech.top

Py:   super().greet()
来源：http://mgh.ydzc1.top

PHP:  parent::greet();
来源：http://kjh.zhaomingkeji.xyz

JS:   super.greet();
来源：http://sfi.sysykeji.top

TS:   super.greet();
来源：http://wnl.jiagoushi.top

Java: super.greet();
来源：http://jyp.sjlbkw.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pel.bbcook.cn

Ruby: super
来源：http://vxt.ivvv.top

C#:   base.Greet();
来源：http://iba.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://ijx.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xrm.cqqwz.cn

PHP:  public static function f() {}
来源：http://dmg.bjfxy.top

JS:   static f() {}
来源：http://ytg.zhijiandao.cn

TS:   static f(): void {}
来源：http://nwc.yanxiufei.cn

Java: static void f() {}
来源：http://kar.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aon.tian-w.cn

Ruby: def self.f; end
来源：http://zvc.mhx1999.top

C#:   public static void F() {}
来源：http://bue.wangshuangyany.cn

[G09] 接口 / 抽象类
来源：http://dxz.jqgufenzy.top

Py:   from abc import ABC, abstractmethod
来源：http://vlx.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://hhy.quarkkingdee.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ixg.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://vta.nwbrower.top

Java: interface Shape { double area(); }
来源：http://kvz.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://wee.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fxf.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://hgr.pycfn.com

[G10] 访问控制
来源：http://vev.chenjidiqi.icu

Py:   约定 _protected / __private（不强制）
来源：http://rxd.cqqwz.cn

PHP:  public / protected / private
来源：http://gxn.aizwys.cn

JS:   #private 字段；其余公开
来源：http://wqj.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://toe.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://wcx.dashuyun.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ler.yuxming.cn

Ruby: public / protected / private
来源：http://axp.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://iwb.dashuyun.cn

[G11] getter / setter
来源：http://rxs.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://eic.guannengcc.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nuw.tian-w.cn

JS:   get name() { return this._name; }
来源：http://byv.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://tkp.jinghuilouyu.cn

Java: public String getName() { return name; }
来源：http://nys.daria6918.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://svq.yj20258888.top

Ruby: attr_accessor :name
来源：http://bur.bbcook.cn

C#:   public string Name { get; set; }
来源：http://wkv.havefunace.top

[G12] 对象转字符串
来源：http://dpg.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://sws.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://edf.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://aop.hywenlv.cn

TS:   toString(): string { return this.name; }
来源：http://dyn.kuanghao11.cn

Java: @Override public String toString() { return name; }
来源：http://wrb.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://ewb.shzxlz.cn

Ruby: def to_s; @name; end
来源：http://hvv.hnxiangtu.top

C#:   public override string ToString() => Name;
来源：http://pur.9152youxi.cn

[G13] 判断对象类型
来源：http://wer.svipenyu.cn

Py:   isinstance(u, User)
来源：http://mjh.ydzc1.top

PHP:  $u instanceof User
来源：http://rdx.jqgufenzy.top

JS:   u instanceof User
来源：http://yzf.shuidangran.top

TS:   u instanceof User
来源：http://ipl.shzxlz.cn

Java: u instanceof User
来源：http://vxs.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://roi.yongpay.top

Ruby: u.is_a?(User)
来源：http://cug.fanxiaobao.xyz

C#:   u is User
来源：http://xle.hcnkem.com

[G14] 数据类 / record
来源：http://lcm.bbcook.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yta.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://swy.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wqj.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://mcw.daxiang520.top

Java: record User(String name, int age) {}
来源：http://boh.hywenlv.cn

Go:   type User struct { Name string; Age int }
来源：http://wyg.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nkz.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://hnk.pengpengdd.cyou

[G15] 枚举
来源：http://tyw.jqgufenzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rno.jqgfzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://sey.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cfj.daria6918.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fmf.xuanzx.com

Java: enum Color { RED, GREEN }
来源：http://mhy.zhixingplan.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qlq.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://vhc.vehdjk.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ugb.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://xcy.yanxiufei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rov.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://wlj.yonumen.top

JS:   Object.entries(obj)
来源：http://ena.guannengcc.top

TS:   Object.entries(obj)
来源：http://zqa.shuidangran.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oit.ppjwa.cn


<!-- 参考信息 -->