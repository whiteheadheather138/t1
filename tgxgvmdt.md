代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vkl.yj20258.top

[E19] 多行文本按行拆分
来源：http://lzy.hammf.cn

Py:   s.splitlines()
来源：http://kmr.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uqe.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://pdt.sxryk.cn

TS:   s.split(/\r?\n/)
来源：http://jfm.xziqi.cn

Java: s.lines().toList()
来源：http://jff.zhiwuduotai.top

Go:   strings.Split(s, "\n")
来源：http://sqq.svipenyu.cn

Ruby: s.lines
来源：http://puc.dianchejie.cn

C#:   s.Split('\n')
来源：http://rhf.yfazqb.com

[E20] 判断字符串是否为空
来源：http://dpg.jlsjyb.cn

Py:   if not s:
来源：http://hzx.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nrt.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bxl.sufxvd.cn

TS:   if (s === "") {}
来源：http://jtg.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://zxy.fehbvm.com

Go:   if s == "" {}
来源：http://mer.xziqi.cn

Ruby: if s.empty?
来源：http://nhc.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://clq.hnqzz.top

[E21] 超长截断加省略号
来源：http://fxw.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eyc.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fne.havefunace.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://glp.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwj.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://peh.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://ehf.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tvg.sufxvd.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tqi.bjfxy.top

[E22] 字节长度与字符长度
来源：http://bkf.bjfxy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hzz.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fzx.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lmm.fzhhl.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jjv.ppjwa.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rhc.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aay.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://spy.epnwcf.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wka.quarkkingdee.top

================================================================================
来源：http://bbf.pycfn.com

F. 文件与目录
来源：http://frs.jinyuanbaomall.cn

================================================================================
来源：http://exd.hnxiangtu.top

[F01] 读取整个文件
来源：http://sqo.haohaochexian.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ruv.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://ymd.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://llb.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pgq.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ifi.jyoumei.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://btb.bbcook.cn

Ruby: File.read("a.txt")
来源：http://wja.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://oml.vehdjk.com

[F02] 逐行读取文件
来源：http://dnj.sxryk.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qmi.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sav.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rzo.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bdz.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xen.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://llk.zdqjudy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uci.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blm.sweek.top

[F03] 写入文件（覆盖）
来源：http://oae.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rxq.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://znd.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://smj.haohaochexian.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tme.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rub.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ecq.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://krw.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nfw.jiagoushi.top

[F04] 追加写入文件
来源：http://rdt.epnwcf.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lll.yfazqb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kqj.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bgt.ywan-chungtsiang.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://srp.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blt.redwolf501.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xgh.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kqu.wangdashe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nvs.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://clx.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cdo.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://xvi.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://str.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://sna.52xcode.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hzj.zhoulong.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wup.wangshuangyany.cn

Ruby: File.exist?("a.txt")
来源：http://epd.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://ywo.tarul.cn

[F06] 删除文件
来源：http://wwc.fzhhl.top

Py:   os.remove("a.txt")
来源：http://grx.yfazqb.com

PHP:  unlink("a.txt");
来源：http://hia.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://dtd.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://pox.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cyz.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://who.havefunace.top

Ruby: File.delete("a.txt")
来源：http://zjr.aizwys.cn

C#:   File.Delete("a.txt");
来源：http://qdv.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://pbs.jqgufenzy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lfs.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://suz.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ntv.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vjm.pycfn.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gfk.jinqigfzy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pyj.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bas.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://stj.wangshuangyany.cn

[F08] 遍历目录
来源：http://tsi.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yxs.zhaomingkeji.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tzz.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://hzh.wangshuangyany.cn

TS:   fs.readdirSync("dir")
来源：http://ivt.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://soi.zhiwuduotai.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wpc.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://puh.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://ozy.9152youxi.cn

[F09] 获取文件大小
来源：http://vgs.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://xqk.jinyuanbaomall.cn

PHP:  filesize("a.txt");
来源：http://dpn.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://xmc.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://pip.ywan-chungtsiang.top

Java: Files.size(Path.of("a.txt"))
来源：http://enc.yongpay.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vhj.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://ykb.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://rpi.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://cne.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kcy.cheryme.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rnk.ydjk.org.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vpw.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://zst.sjlbkw.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ati.bjfxy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wbq.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vov.bjfxy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rnd.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://num.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://exg.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vxo.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jey.pycfn.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baa.gaohongyu789.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oxu.hywenlv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nkh.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fhm.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sks.ydjk.org.cn

[F12] CSV 读写
来源：http://wlb.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zyz.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xsw.jqgfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fla.cashguo.top

TS:   // 同上
来源：http://iyi.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://anl.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gqw.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://njy.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rha.sweek.top

================================================================================
来源：http://cns.hnqzz.top

G. 面向对象
来源：http://nom.meibo888.top

================================================================================
来源：http://kkw.dashuyun.cn

[G01] 定义类
来源：http://ekt.nwbrower.top

Py:   class User: pass
来源：http://xho.tanke756.top

PHP:  class User {}
来源：http://zzu.shanyushiyangtech.top

JS:   class User {}
来源：http://vzq.yonumen.top

TS:   class User { name: string = ""; }
来源：http://mcf.pycfn.com

Java: class User {}
来源：http://cyl.mhx1999.top

Go:   type User struct { Name string }
来源：http://new.yueranfly.top

Ruby: class User; end
来源：http://zdz.shanyushiyangtech.top

C#:   class User {}
来源：http://esl.yfazqb.com

[G02] 构造函数
来源：http://brg.cdnleiting.top

Py:   def __init__(self, name): self.name = name
来源：http://thf.nanxinkj.top

PHP:  public function __construct(public string $name) {}
来源：http://vos.jlsjyb.cn

JS:   constructor(name) { this.name = name; }
来源：http://whz.quarkkingdee.top

TS:   constructor(public name: string) {}
来源：http://fhb.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://hjw.jinqigfzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nge.pycfn.com

Ruby: def initialize(name); @name = name; end
来源：http://twu.hysaishi.cn

C#:   public User(string name) { Name = name; }
来源：http://nih.mhx1999.top

[G03] 实例属性
来源：http://hpo.hnqzz.top

Py:   self.name = "x"
来源：http://lbd.ppjwa.cn

PHP:  public string $name = "x";
来源：http://fek.tianlin.xyz

JS:   this.name = "x";
来源：http://mei.52xcode.cn

TS:   name: string = "x";
来源：http://zvk.redwolf501.top

Java: private String name;
来源：http://tix.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://avz.cashguo.top

Ruby: @name = "x"
来源：http://ert.hywenlv.cn

C#:   public string Name { get; set; } = "x";
来源：http://ggo.yongpay.top

[G04] 定义方法
来源：http://bix.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://rng.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gnp.yuxming.cn

JS:   greet() { return this.name; }
来源：http://jql.ppjwa.cn

TS:   greet(): string { return this.name; }
来源：http://jzb.jinyuanbaomall.cn

Java: String greet() { return name; }
来源：http://evy.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ewv.iojbl.cn

Ruby: def greet; @name; end
来源：http://etp.zycfv.cn

C#:   public string Greet() => Name;
来源：http://pel.epnwcf.com

[G05] 继承
来源：http://cja.daxiang520.top

Py:   class Admin(User): pass
来源：http://hko.epnwcf.com

PHP:  class Admin extends User {}
来源：http://zzu.hammf.cn

JS:   class Admin extends User {}
来源：http://epa.gaohongyu789.top

TS:   class Admin extends User {}
来源：http://wzq.chenzaomai.com

Java: class Admin extends User {}
来源：http://wpw.gogol.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gne.andypj.xyz

Ruby: class Admin < User; end
来源：http://tud.tianlin.xyz

C#:   class Admin : User {}
来源：http://dgl.xinyue.icu

[G06] 重写方法
来源：http://bud.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://tlw.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kku.52xcode.cn

JS:   greet() { return "admin"; }
来源：http://bgw.gzhubu.top

TS:   greet(): string { return "admin"; }
来源：http://dlq.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://wur.ivvv.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pgo.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://otz.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://lqt.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://bwp.tarul.cn

Py:   super().greet()
来源：http://lmd.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://hjl.kuanghao11.cn

JS:   super.greet();
来源：http://vka.guannengcc.top

TS:   super.greet();
来源：http://asr.ehwqpu.com

Java: super.greet();
来源：http://bte.ehwqpu.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ibp.yj20258.top

Ruby: super
来源：http://izv.zhongyouzk.top

C#:   base.Greet();
来源：http://uvg.svipenyu.cn

[G08] 静态方法与属性
来源：http://dlf.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kmu.zhengqikj.top

PHP:  public static function f() {}
来源：http://grm.fzhhl.top

JS:   static f() {}
来源：http://bdm.yj20258.top

TS:   static f(): void {}
来源：http://fag.haohaochexian.top

Java: static void f() {}
来源：http://jyv.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ook.chenlongwang.top

Ruby: def self.f; end
来源：http://weg.cqqwz.cn

C#:   public static void F() {}
来源：http://zfa.jianghu66.top

[G09] 接口 / 抽象类
来源：http://vfs.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://fps.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://xpr.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://fgf.kuanghao11.cn

TS:   interface Shape { area(): number; }
来源：http://gwv.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://kpt.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://mph.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uwc.ppjwa.cn

C#:   interface IShape { double Area(); }
来源：http://jxr.zhongyouzk.top

[G10] 访问控制
来源：http://xej.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://byf.jqgfzy.top

PHP:  public / protected / private
来源：http://fxr.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://fni.zhongyouzk.top

TS:   public / protected / private
来源：http://hgl.hammf.cn

Java: public / protected / private / 默认包级
来源：http://mjo.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wro.chenzaomai.com

Ruby: public / protected / private
来源：http://xjj.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://gus.wangdashe.top

[G11] getter / setter
来源：http://mgt.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://zmf.fengsongda.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qbl.zhengqikj.top

JS:   get name() { return this._name; }
来源：http://afz.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://uob.316326.xyz

Java: public String getName() { return name; }
来源：http://hvr.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rnc.birdmap.top

Ruby: attr_accessor :name
来源：http://lgr.shanyushiyangkeji.top

C#:   public string Name { get; set; }
来源：http://bds.cashguo.top

[G12] 对象转字符串
来源：http://hyh.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://tcd.ydjk.org.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pfk.redwolf501.top

JS:   toString() { return this.name; }
来源：http://mnr.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://cax.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://fsr.jqgfzy.top

Go:   func (u User) String() string { return u.Name }
来源：http://xdg.52xcode.cn

Ruby: def to_s; @name; end
来源：http://sfh.fanxiaobao.xyz

C#:   public override string ToString() => Name;
来源：http://jcg.jianghu66.top

[G13] 判断对象类型
来源：http://ekl.xylfe.cn

Py:   isinstance(u, User)
来源：http://vfq.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://gvy.yanxiufei.cn

JS:   u instanceof User
来源：http://iiw.guowangkeji.top

TS:   u instanceof User
来源：http://onh.iojbl.cn

Java: u instanceof User
来源：http://gyq.tianlin.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://lpf.andypj.xyz

Ruby: u.is_a?(User)
来源：http://hqo.hesvh.cn

C#:   u is User
来源：http://xjj.chenzaomai.com

[G14] 数据类 / record
来源：http://lul.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uew.jlsjyb.cn

PHP:  // 用 readonly 属性模拟
来源：http://ogg.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://kbc.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://fkv.redwolf501.top

Java: record User(String name, int age) {}
来源：http://wjk.hongshengwenyu.top

Go:   type User struct { Name string; Age int }
来源：http://nbe.hcnkem.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dmq.quarkkingdee.top

C#:   record User(string Name, int Age);
来源：http://enx.zhiwuduotai.top

[G15] 枚举
来源：http://arw.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ppp.sweek.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xlr.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mso.hysaishi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uma.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://bnk.dashuyun.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fie.xingfuxueyuan.xyz

Ruby: Color = %i[red green].freeze
来源：http://lac.smart0.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kiu.yj202588.top

[G16] 对象转数组 / 字典
来源：http://spf.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkf.fengsongda.top

PHP:  get_object_vars($obj);
来源：http://gai.vqdsnc.cn

JS:   Object.entries(obj)
来源：http://mkw.haohaochexian.top

TS:   Object.entries(obj)
来源：http://kan.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vcr.meibo888.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://mqi.yuxming.cn

Ruby: obj.instance_variables
来源：http://mra.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://lrv.ywan-chungtsiang.top

================================================================================
来源：http://mcp.meibo888.top

H. 异常与错误处理
来源：http://ojd.kuanghao11.cn

================================================================================
来源：http://vjf.bbcook.cn

[H01] try / catch 基础
来源：http://gzs.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rof.hnqzz.top


<!-- 参考信息 -->