代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eon.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jwk.meibo888.top

TS:   if (s === "") {}
来源：http://jwh.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://yvj.ctjpmb.com

Go:   if s == "" {}
来源：http://dnr.yuxming.cn

Ruby: if s.empty?
来源：http://yik.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://okb.chenzaomai.com

[E21] 超长截断加省略号
来源：http://byw.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rcr.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xla.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sxg.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pue.yj20258.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aaw.daxiang520.top

Go:   // 按 rune 判断长度后截断
来源：http://hxw.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yub.yj202588.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vlr.fzhhl.top

[E22] 字节长度与字符长度
来源：http://nxe.zhengqikj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xtz.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zbx.fanxiaobao.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pjm.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rwu.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pwv.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://knk.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://fpr.dianchejie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://afg.hongshengwenyu.top

================================================================================
来源：http://wal.bbcook.cn

F. 文件与目录
来源：http://lpo.pengpengdd.cyou

================================================================================
来源：http://zvi.jinqigufen.top

[F01] 读取整个文件
来源：http://vjm.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://chk.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://goq.316326.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wrs.fehbvm.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tna.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://shp.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xsa.aibaodan.cn

Ruby: File.read("a.txt")
来源：http://hoe.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://urt.yanxiufei.cn

[F02] 逐行读取文件
来源：http://vwc.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qvp.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mwf.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjq.jlsjyb.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yzx.ywan-chungtsiang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yqj.jinqigufen.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sbs.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xky.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ouq.316326.xyz

[F03] 写入文件（覆盖）
来源：http://vqh.zhaomingkeji.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yng.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vvp.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sxb.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tws.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lbz.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wgu.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://vjt.ydjk.org.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gzt.quarkkingdee.top

[F04] 追加写入文件
来源：http://rrb.cdnleiting.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pgh.zhengqikj.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cob.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gdh.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yba.aizwys.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://phw.mhx1999.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbh.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oox.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rxb.xinyue.icu

[F05] 判断文件或目录是否存在
来源：http://vbe.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vpv.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://wan.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://snn.pengpengdd.cyou

TS:   fs.existsSync("a.txt")
来源：http://gky.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zbr.hcnkem.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://arc.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://snl.sweek.top

C#:   File.Exists("a.txt")
来源：http://ncb.shuidangran.top

[F06] 删除文件
来源：http://knv.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://ksv.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://vuj.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://kqu.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wrm.xuetiantiany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://knb.shangyingyoupin.top

Go:   os.Remove("a.txt")
来源：http://xba.zhiwuduotai.top

Ruby: File.delete("a.txt")
来源：http://bhz.jqgfzy.top

C#:   File.Delete("a.txt");
来源：http://yab.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://plq.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mrb.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://esp.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eul.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gqi.tanke756.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zyu.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wsj.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xrl.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bck.daxiang520.top

[F08] 遍历目录
来源：http://vtn.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gkf.fktsv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uta.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://sel.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://xxa.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pin.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ord.9152youxi.cn

Ruby: Dir.children("dir")
来源：http://xas.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://qle.sufxvd.cn

[F09] 获取文件大小
来源：http://lfx.hnxiangtu.top

Py:   os.path.getsize("a.txt")
来源：http://qed.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://ozn.jinqigufen.top

JS:   fs.statSync("a.txt").size
来源：http://uno.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://ocd.tarul.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ibw.cucudq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wnf.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://wrb.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://jty.fengsongda.top

[F10] 取文件扩展名 / 文件名
来源：http://opo.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fus.hesvh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wth.tarul.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rys.gzhubu.top

TS:   path.extname("a.txt")
来源：http://jgk.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hej.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hmw.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qln.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wce.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://aes.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fho.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://byf.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tbe.52xcode.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ptn.zhixingplan.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nek.zhoulong.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vsb.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ycw.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://szw.ywan-chungtsiang.top

[F12] CSV 读写
来源：http://ele.yj20258888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lir.hongshengwenyu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hiz.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nfh.zdbjq.cn

TS:   // 同上
来源：http://vxh.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hwx.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aox.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://myd.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://unr.pengpengdd.cyou

================================================================================
来源：http://oku.ybcxt.top

G. 面向对象
来源：http://ilc.ydjk.org.cn

================================================================================
来源：http://rnd.havefunace.top

[G01] 定义类
来源：http://pdo.jinqigufen.top

Py:   class User: pass
来源：http://ejm.yvedp.cn

PHP:  class User {}
来源：http://nwe.hfpthk.cn

JS:   class User {}
来源：http://aem.sufxvd.cn

TS:   class User { name: string = ""; }
来源：http://mfl.daria6918.cn

Java: class User {}
来源：http://cme.daxiang520.top

Go:   type User struct { Name string }
来源：http://vgs.yongpay.top

Ruby: class User; end
来源：http://lvb.andypj.xyz

C#:   class User {}
来源：http://wfx.xingfuxueyuan.xyz

[G02] 构造函数
来源：http://nxs.jinyuanbaomall.cn

Py:   def __init__(self, name): self.name = name
来源：http://zni.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://wni.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://xzt.cdnleiting.top

TS:   constructor(public name: string) {}
来源：http://wtt.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://zdg.shangyingyoupin.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://atz.vqdsnc.cn

Ruby: def initialize(name); @name = name; end
来源：http://gsf.hfpthk.cn

C#:   public User(string name) { Name = name; }
来源：http://dnq.sufxvd.cn

[G03] 实例属性
来源：http://rfv.snrcjt.cn

Py:   self.name = "x"
来源：http://zln.ctjpmb.com

PHP:  public string $name = "x";
来源：http://ehx.cucudq.cn

JS:   this.name = "x";
来源：http://rii.snrcjt.cn

TS:   name: string = "x";
来源：http://uem.yonumen.top

Java: private String name;
来源：http://clc.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nty.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://efk.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://wrk.ydzc1.top

[G04] 定义方法
来源：http://beb.316326.xyz

Py:   def greet(self): return self.name
来源：http://ude.jinyuanbaomall.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uzy.zhiwuduotai.top

JS:   greet() { return this.name; }
来源：http://cll.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://ooj.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://cgl.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://efi.hcnkem.com

Ruby: def greet; @name; end
来源：http://gcr.tanke756.top

C#:   public string Greet() => Name;
来源：http://zuz.ppjwa.cn

[G05] 继承
来源：http://uxu.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://lmh.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://ewe.316326.xyz

JS:   class Admin extends User {}
来源：http://pqm.chenjidiqi.icu

TS:   class Admin extends User {}
来源：http://zgj.nanxinkj.top

Java: class Admin extends User {}
来源：http://wmz.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qwp.tarul.cn

Ruby: class Admin < User; end
来源：http://fzr.sjlbkw.cn

C#:   class Admin : User {}
来源：http://pct.yuanzhike.top

[G06] 重写方法
来源：http://xea.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://mmm.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ijq.316326.xyz

JS:   greet() { return "admin"; }
来源：http://hcl.hnqzz.top

TS:   greet(): string { return "admin"; }
来源：http://equ.gotoacloud.top

Java: @Override String greet() { return "admin"; }
来源：http://jwk.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wnp.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://ggj.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://xme.redwolf501.top

[G07] 调用父类方法
来源：http://tec.yueranfly.top

Py:   super().greet()
来源：http://jda.ppjwa.cn

PHP:  parent::greet();
来源：http://rdz.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://qnf.xziqi.cn

TS:   super.greet();
来源：http://wsf.yvedp.cn

Java: super.greet();
来源：http://pjm.andypj.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eoc.ppjwa.cn

Ruby: super
来源：http://tdv.hesvh.cn

C#:   base.Greet();
来源：http://aei.svipenyu.cn

[G08] 静态方法与属性
来源：http://mrg.9152youxi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jkj.fengsongda.top

PHP:  public static function f() {}
来源：http://ylb.pycfn.com

JS:   static f() {}
来源：http://yni.sysykeji.top

TS:   static f(): void {}
来源：http://ehp.jianghu66.top

Java: static void f() {}
来源：http://zwj.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hru.nwbrower.top

Ruby: def self.f; end
来源：http://xzs.316326.xyz

C#:   public static void F() {}
来源：http://iuu.gogol.net.cn

[G09] 接口 / 抽象类
来源：http://mls.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://uvb.shanyushiyangtech.top

PHP:  interface Shape { public function area(): float; }
来源：http://wuf.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kgk.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://dgs.sysykeji.top

Java: interface Shape { double area(); }
来源：http://boh.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://hah.hysaishi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nib.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://mue.meibo888.top

[G10] 访问控制
来源：http://yaf.cucudq.cn

Py:   约定 _protected / __private（不强制）
来源：http://xno.bjfxy.top

PHP:  public / protected / private
来源：http://zgn.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://xoc.gzhubu.top

TS:   public / protected / private
来源：http://ojx.dianchejie.cn

Java: public / protected / private / 默认包级
来源：http://uvn.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ekn.gzhubu.top

Ruby: public / protected / private
来源：http://osm.quarkkingdee.top

C#:   public / protected / private / internal
来源：http://blh.tarul.cn

[G11] getter / setter
来源：http://haz.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://gwv.nanxuanxn.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jjh.yj20258.top

JS:   get name() { return this._name; }
来源：http://akk.ivvv.top

TS:   get name(): string { return this._name; }
来源：http://tmw.zhijiandao.cn

Java: public String getName() { return name; }
来源：http://yei.jinyuanbaomall.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://khq.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://spt.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://ohl.zycfv.cn

[G12] 对象转字符串
来源：http://qez.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://mgl.snrcjt.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://smw.guowangkeji.top

JS:   toString() { return this.name; }
来源：http://blf.jinghuilouyu.cn

TS:   toString(): string { return this.name; }
来源：http://piq.jinqigfzy.top

Java: @Override public String toString() { return name; }
来源：http://vly.bbcook.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ndz.chenjidiqi.icu

Ruby: def to_s; @name; end
来源：http://jdw.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://hsc.yfazqb.com

[G13] 判断对象类型
来源：http://puf.zhengqikj.top

Py:   isinstance(u, User)
来源：http://jyw.bbcook.cn

PHP:  $u instanceof User
来源：http://mlb.epnwcf.com

JS:   u instanceof User
来源：http://wmx.yueranfly.top

TS:   u instanceof User
来源：http://ofa.zhaomingkeji.xyz

Java: u instanceof User
来源：http://lug.gotoacloud.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hlj.hesvh.cn

Ruby: u.is_a?(User)
来源：http://kum.sweek.top

C#:   u is User
来源：http://zcl.jqgfzy.top

[G14] 数据类 / record
来源：http://oxv.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hfb.ydzc1.top

PHP:  // 用 readonly 属性模拟
来源：http://njb.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kjm.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://zdi.aizwys.cn

Java: record User(String name, int age) {}
来源：http://ymh.ivvv.top

Go:   type User struct { Name string; Age int }
来源：http://tmr.52xcode.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://suw.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://ttj.yueranfly.top

[G15] 枚举
来源：http://nbw.shuidangran.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pwt.yfazqb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lev.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kwl.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mal.sweek.top

Java: enum Color { RED, GREEN }
来源：http://caj.zhijiandao.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dmp.jinqigufen.top

Ruby: Color = %i[red green].freeze
来源：http://qvh.yj20258888.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qve.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://swc.zhaomingkeji.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lsi.sufxvd.cn

PHP:  get_object_vars($obj);
来源：http://mow.svipenyu.cn

JS:   Object.entries(obj)
来源：http://svc.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://xkl.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://inc.chenzaomai.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mlu.cucudq.cn

Ruby: obj.instance_variables
来源：http://dhj.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://lbx.fanxiaobao.xyz

================================================================================
来源：http://ioq.fehbvm.com

H. 异常与错误处理
来源：http://npb.bbcook.cn

================================================================================
来源：http://ydt.yangfankeji.com

[H01] try / catch 基础
来源：http://kwe.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fxu.daxiang520.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wnq.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jsg.hfpthk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gxt.pycfn.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nfq.zhongyouzk.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jms.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rnu.hysaishi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xkn.tarul.cn

[H02] finally / ensure 收尾
来源：http://kyn.316326.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://lue.xylfe.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xxa.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://fdz.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://sid.svipenyu.cn


<!-- 参考信息 -->