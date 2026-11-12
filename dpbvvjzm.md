代发 wailian999

[E18] 模板占位符替换
来源：http://gnx.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wqh.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tyr.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xte.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ykq.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tea.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nja.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mzr.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gln.tanke756.top

[E19] 多行文本按行拆分
来源：http://myg.dianchejie.cn

Py:   s.splitlines()
来源：http://ojv.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zuh.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://liq.zycfv.cn

TS:   s.split(/\r?\n/)
来源：http://odm.meibo888.top

Java: s.lines().toList()
来源：http://fnx.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://xdb.sysykeji.top

Ruby: s.lines
来源：http://xin.shanyushiyangtech.top

C#:   s.Split('\n')
来源：http://mjy.sysykeji.top

[E20] 判断字符串是否为空
来源：http://jgr.hnqzz.top

Py:   if not s:
来源：http://ayy.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vhh.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uul.daria6918.cn

TS:   if (s === "") {}
来源：http://frk.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://mde.xinyue.icu

Go:   if s == "" {}
来源：http://ici.52xcode.cn

Ruby: if s.empty?
来源：http://glk.yongpay.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aij.jinqigufen.top

[E21] 超长截断加省略号
来源：http://qxd.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqh.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rbm.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ony.vehdjk.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tlb.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hxn.jyoumei.cn

Go:   // 按 rune 判断长度后截断
来源：http://ovo.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ura.fehbvm.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://poz.gzhubu.top

[E22] 字节长度与字符长度
来源：http://xqn.wangshuangyany.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rqf.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yls.fzhhl.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lnv.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://odg.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wwt.daxiang520.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://und.yongpay.top

Ruby: s.bytesize;  s.length
来源：http://hvn.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oqz.ppjwa.cn

================================================================================
来源：http://tjl.wangshuangyany.cn

F. 文件与目录
来源：http://apa.vqdsnc.cn

================================================================================
来源：http://gkn.chenjidiqi.icu

[F01] 读取整个文件
来源：http://sxf.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cmg.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://klt.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://crl.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qpx.iojbl.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://npy.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vjo.gogol.net.cn

Ruby: File.read("a.txt")
来源：http://feu.fehbvm.com

C#:   File.ReadAllText("a.txt");
来源：http://dja.sxryk.cn

[F02] 逐行读取文件
来源：http://vfd.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swf.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kus.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rcf.xylfe.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nah.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pza.hnqzz.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uyl.wangdashe.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cnk.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yui.cheryme.top

[F03] 写入文件（覆盖）
来源：http://jlt.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wzj.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kpm.ydjk.org.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqd.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://evq.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yjb.chenzaomai.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qbz.iojbl.cn

Ruby: File.write("a.txt", "hi")
来源：http://bla.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xfx.daria6918.cn

[F04] 追加写入文件
来源：http://ciq.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qwl.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tbn.fanxiaobao.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hkq.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://grn.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nuh.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ded.zycfv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mxk.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ygd.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://kwc.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lma.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://gwt.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://kpw.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://gka.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wrn.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gah.chenlongwang.top

Ruby: File.exist?("a.txt")
来源：http://sex.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://qwu.guannengcc.top

[F06] 删除文件
来源：http://otr.tarul.cn

Py:   os.remove("a.txt")
来源：http://sew.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://ppi.cdnleiting.top

JS:   fs.unlinkSync("a.txt")
来源：http://jut.yuxming.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ksa.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mlg.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://xvd.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://roq.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://poz.sufxvd.cn

[F07] 创建目录（含多级）
来源：http://djm.feifeiyinyue.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vkn.kuanghao11.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dtk.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fyh.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zvi.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eox.jinqigufen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zsm.aizwys.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://urh.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hzd.hnqzz.top

[F08] 遍历目录
来源：http://jeh.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://pth.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jao.jinyuanbaomall.cn

JS:   fs.readdirSync("dir")
来源：http://amw.tanke756.top

TS:   fs.readdirSync("dir")
来源：http://hmo.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jbj.smart0.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nvo.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://mnx.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://cfr.hongshengwenyu.top

[F09] 获取文件大小
来源：http://szn.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://ugm.fehbvm.com

PHP:  filesize("a.txt");
来源：http://fsz.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://ymj.andypj.xyz

TS:   fs.statSync("a.txt").size
来源：http://pky.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://buc.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://agq.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://cwk.yuanzhike.top

C#:   new FileInfo("a.txt").Length
来源：http://ims.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://svo.chenzaomai.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://aeh.tanke756.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gwv.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wob.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://pum.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://osm.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wwm.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cur.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fno.yanxiufei.cn

[F11] 复制与移动文件
来源：http://vtj.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://miy.xuetiantiany.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jqw.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ovt.hfpthk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vgi.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ylh.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jkq.vehdjk.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wcc.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qhf.chenzaomai.com

[F12] CSV 读写
来源：http://nvw.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mde.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://omp.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bsv.hnxiangtu.top

TS:   // 同上
来源：http://loc.vqdsnc.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sjk.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://esr.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://slw.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://nwo.zdqjudy.top

================================================================================
来源：http://mzn.sxryk.cn

G. 面向对象
来源：http://caa.jinyuanbaomall.cn

================================================================================
来源：http://uue.jinyuanbaomall.cn

[G01] 定义类
来源：http://eza.vqdsnc.cn

Py:   class User: pass
来源：http://xig.gzhubu.top

PHP:  class User {}
来源：http://nzq.shuidangran.top

JS:   class User {}
来源：http://lts.yongpay.top

TS:   class User { name: string = ""; }
来源：http://xrn.shanyushiyangtech.top

Java: class User {}
来源：http://xjr.jlsjyb.cn

Go:   type User struct { Name string }
来源：http://uhs.chenzaomai.com

Ruby: class User; end
来源：http://pvx.jlsjyb.cn

C#:   class User {}
来源：http://ppp.gzhubu.top

[G02] 构造函数
来源：http://tks.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://omd.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://yzy.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://uhb.yonumen.top

TS:   constructor(public name: string) {}
来源：http://plf.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://exc.epnwcf.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vbt.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://luh.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://anp.ehwqpu.com

[G03] 实例属性
来源：http://rad.kuanghao11.cn

Py:   self.name = "x"
来源：http://bzq.gogol.net.cn

PHP:  public string $name = "x";
来源：http://wvi.wangdashe.top

JS:   this.name = "x";
来源：http://hyl.shzxlz.cn

TS:   name: string = "x";
来源：http://oeu.jiagoushi.top

Java: private String name;
来源：http://feq.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://amy.cdnleiting.top

Ruby: @name = "x"
来源：http://ccr.epnwcf.com

C#:   public string Name { get; set; } = "x";
来源：http://yfu.snrcjt.cn

[G04] 定义方法
来源：http://ksf.havefunace.top

Py:   def greet(self): return self.name
来源：http://tzt.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gqb.smart0.xyz

JS:   greet() { return this.name; }
来源：http://iet.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://hvc.haohaochexian.top

Java: String greet() { return name; }
来源：http://nmo.yanxiufei.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qei.xylfe.cn

Ruby: def greet; @name; end
来源：http://npe.fanxiaobao.xyz

C#:   public string Greet() => Name;
来源：http://icq.svipenyu.cn

[G05] 继承
来源：http://jum.hesvh.cn

Py:   class Admin(User): pass
来源：http://sjv.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://wgr.hfpthk.cn

JS:   class Admin extends User {}
来源：http://xrt.shanyushiyangkeji.top

TS:   class Admin extends User {}
来源：http://xbv.iojbl.cn

Java: class Admin extends User {}
来源：http://hhm.shuidangran.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hfm.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://hbr.aibaodan.cn

C#:   class Admin : User {}
来源：http://bwh.dashuyun.cn

[G06] 重写方法
来源：http://xqc.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://tdm.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sxj.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://prt.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://ovx.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://qhk.nanxuanxn.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wyo.gogol.net.cn

Ruby: def greet; "admin"; end
来源：http://auo.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://khd.nanxinkj.top

[G07] 调用父类方法
来源：http://rzd.sxryk.cn

Py:   super().greet()
来源：http://nnv.gotoacloud.top

PHP:  parent::greet();
来源：http://zjs.zhixingplan.top

JS:   super.greet();
来源：http://euu.chenjidiqi.icu

TS:   super.greet();
来源：http://jkg.iojbl.cn

Java: super.greet();
来源：http://dnw.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ypt.yfazqb.com

Ruby: super
来源：http://ehh.pycfn.com

C#:   base.Greet();
来源：http://dzf.sufxvd.cn

[G08] 静态方法与属性
来源：http://boy.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://onj.xinyue.icu

PHP:  public static function f() {}
来源：http://ngw.chenlongwang.top

JS:   static f() {}
来源：http://quw.kuanghao11.cn

TS:   static f(): void {}
来源：http://axi.sweek.top

Java: static void f() {}
来源：http://cvv.zhongyouzk.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bec.shuidangran.top

Ruby: def self.f; end
来源：http://mdd.jyoumei.cn

C#:   public static void F() {}
来源：http://tql.hcnkem.com

[G09] 接口 / 抽象类
来源：http://iek.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://lue.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://qom.nanxinkj.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://efw.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://hep.ydzc1.top

Java: interface Shape { double area(); }
来源：http://yks.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://vmt.xingfuxueyuan.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mib.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://hkw.uphjek.com

[G10] 访问控制
来源：http://mtq.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://frb.pengpengdd.cyou

PHP:  public / protected / private
来源：http://ris.fzhhl.top

JS:   #private 字段；其余公开
来源：http://pta.zhongyouzk.top

TS:   public / protected / private
来源：http://gxe.jqgfzy.top

Java: public / protected / private / 默认包级
来源：http://cao.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gxb.nwbrower.top

Ruby: public / protected / private
来源：http://nqt.tian-w.cn

C#:   public / protected / private / internal
来源：http://bxp.ehwqpu.com

[G11] getter / setter
来源：http://chg.hysaishi.cn

Py:   @property 与 @x.setter
来源：http://jbk.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ogq.xziqi.cn

JS:   get name() { return this._name; }
来源：http://nng.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://avb.cdnleiting.top

Java: public String getName() { return name; }
来源：http://tza.snrcjt.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wno.epnwcf.com

Ruby: attr_accessor :name
来源：http://ntl.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://kxn.fehbvm.com

[G12] 对象转字符串
来源：http://mrd.jinqigfzy.top

Py:   def __str__(self): return self.name
来源：http://dzj.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qaz.gotoacloud.top

JS:   toString() { return this.name; }
来源：http://tsn.zhixingplan.top

TS:   toString(): string { return this.name; }
来源：http://sjw.zdqjudy.top

Java: @Override public String toString() { return name; }
来源：http://apn.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://iqj.chenzaomai.com

Ruby: def to_s; @name; end
来源：http://ayq.jqgfzy.top

C#:   public override string ToString() => Name;
来源：http://xtt.jqgufenzy.top

[G13] 判断对象类型
来源：http://hxb.yuanzhike.top

Py:   isinstance(u, User)
来源：http://cyf.yongpay.top

PHP:  $u instanceof User
来源：http://ozk.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://hrx.birdmap.top

TS:   u instanceof User
来源：http://gxb.hfpthk.cn

Java: u instanceof User
来源：http://eob.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbw.xylfe.cn

Ruby: u.is_a?(User)
来源：http://ngo.gotoacloud.top

C#:   u is User
来源：http://myg.birdmap.top

[G14] 数据类 / record
来源：http://pwp.chenzaomai.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yly.yj20258888.top

PHP:  // 用 readonly 属性模拟
来源：http://ikc.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://dbj.zdqjudy.top

TS:   type User = { name: string; age: number };
来源：http://ojq.ivvv.top

Java: record User(String name, int age) {}
来源：http://cfp.jqgufenzy.top

Go:   type User struct { Name string; Age int }
来源：http://cvr.ehwqpu.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mwk.chenzaomai.com

C#:   record User(string Name, int Age);
来源：http://uvy.yuxming.cn

[G15] 枚举
来源：http://ehe.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mps.sysykeji.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pyx.yvedp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://maa.feifeiyinyue.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nbc.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://oak.zhoulong.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xba.jianghu66.top

Ruby: Color = %i[red green].freeze
来源：http://qtc.jqgfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tgd.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://utj.yuxming.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ekd.bbcook.cn

PHP:  get_object_vars($obj);
来源：http://cly.jqgfzy.top

JS:   Object.entries(obj)
来源：http://qrl.hnqzz.top

TS:   Object.entries(obj)
来源：http://ffw.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rdw.pengpengdd.cyou


<!-- 参考信息 -->