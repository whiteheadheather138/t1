代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kkz.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://sol.tianlin.xyz

Py:   s.splitlines()
来源：http://oum.jiagoushi.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yly.jqgfzy.top

JS:   s.split(/\r?\n/)
来源：http://ktq.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://qif.ppjwa.cn

Java: s.lines().toList()
来源：http://tly.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://qni.tianlin.xyz

Ruby: s.lines
来源：http://bch.yuxming.cn

C#:   s.Split('\n')
来源：http://qgg.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://yzc.hammf.cn

Py:   if not s:
来源：http://rja.tianlin.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mtm.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dru.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://zeq.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://zsq.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://iyp.ydzc1.top

Ruby: if s.empty?
来源：http://aof.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kdz.yuxming.cn

[E21] 超长截断加省略号
来源：http://pln.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvk.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vuu.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yha.mhx1999.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kpe.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ydz.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://ylx.zhixingplan.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sbv.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qtr.cheryme.top

[E22] 字节长度与字符长度
来源：http://bhi.ctjpmb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uyj.xylfe.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kpk.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dct.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zwz.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://aty.xuanzx.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wye.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://nmr.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jdm.epnwcf.com

================================================================================
来源：http://mio.c1oappe.top

F. 文件与目录
来源：http://vez.sufxvd.cn

================================================================================
来源：http://poy.316326.xyz

[F01] 读取整个文件
来源：http://olf.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wnp.yuanzhike.top

PHP:  file_get_contents("a.txt");
来源：http://eki.tanke756.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pkg.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://avl.jinqigfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eob.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kbs.yj20258888.top

Ruby: File.read("a.txt")
来源：http://nts.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://uuo.ybcxt.top

[F02] 逐行读取文件
来源：http://pxa.zdqjudy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://snv.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sox.hammf.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tsb.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qyy.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bku.zycfv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gxf.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mjw.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ofy.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://tzl.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ehi.shzxlz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qdz.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hia.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bgz.jinghuilouyu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fuu.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hny.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://myj.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wmo.guannengcc.top

[F04] 追加写入文件
来源：http://iaz.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wob.cqqwz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zpp.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nze.zhoulong.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pnr.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vfl.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wtm.ydzc1.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zqi.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://clb.dianchejie.cn

[F05] 判断文件或目录是否存在
来源：http://fpq.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yyd.jinqigufen.top

PHP:  file_exists("a.txt");
来源：http://xil.yj20258.top

JS:   fs.existsSync("a.txt")
来源：http://xak.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://oou.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tbp.jinqigufen.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sba.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://wri.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://wrn.chenzaomai.com

[F06] 删除文件
来源：http://gfo.ydzc1.top

Py:   os.remove("a.txt")
来源：http://aii.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://ohs.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pfn.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://ndf.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hhi.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://jgm.aibaodan.cn

Ruby: File.delete("a.txt")
来源：http://lih.fzhhl.top

C#:   File.Delete("a.txt");
来源：http://okf.jianghu66.top

[F07] 创建目录（含多级）
来源：http://ftr.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nyo.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zvw.jinqigufen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://klp.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://whz.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://znr.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bgm.iojbl.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://agy.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yhd.ehwqpu.com

[F08] 遍历目录
来源：http://mse.svipenyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jod.cheryme.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://njk.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://rmf.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://uty.zhengqikj.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hve.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://khe.havefunace.top

Ruby: Dir.children("dir")
来源：http://foh.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://yrl.ivvv.top

[F09] 获取文件大小
来源：http://bfx.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://its.aizwys.cn

PHP:  filesize("a.txt");
来源：http://ixm.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://yep.iojbl.cn

TS:   fs.statSync("a.txt").size
来源：http://zjp.fengsongda.top

Java: Files.size(Path.of("a.txt"))
来源：http://bmh.zhijiandao.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wjo.andypj.xyz

Ruby: File.size("a.txt")
来源：http://pnx.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://mic.hysaishi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ixz.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://axv.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tig.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://azo.hammf.cn

TS:   path.extname("a.txt")
来源：http://zdz.ehwqpu.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gzq.shanyushiyangkeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://seb.daria6918.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oov.c1oappe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aqo.cheryme.top

[F11] 复制与移动文件
来源：http://raj.52xcode.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ugb.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ttr.xziqi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nrx.epnwcf.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gzu.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ebo.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wvo.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yxm.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://stq.xylfe.cn

[F12] CSV 读写
来源：http://laq.gotoacloud.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hpc.yongpay.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ujn.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://shi.sufxvd.cn

TS:   // 同上
来源：http://wbi.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hbe.yuanzhike.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hqq.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hbo.snrcjt.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ujb.bjfxy.top

================================================================================
来源：http://kqa.jianghu66.top

G. 面向对象
来源：http://tdu.sysykeji.top

================================================================================
来源：http://amn.xuanzx.com

[G01] 定义类
来源：http://cwr.yfazqb.com

Py:   class User: pass
来源：http://ywp.jinghuilouyu.cn

PHP:  class User {}
来源：http://dju.c1oappe.top

JS:   class User {}
来源：http://tif.nanxuanxn.top

TS:   class User { name: string = ""; }
来源：http://klk.chenzaomai.com

Java: class User {}
来源：http://trd.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://wnw.hammf.cn

Ruby: class User; end
来源：http://mum.snrcjt.cn

C#:   class User {}
来源：http://rhs.yueranfly.top

[G02] 构造函数
来源：http://xaj.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://gmm.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://nbd.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://ksp.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://oiw.chenzaomai.com

Java: User(String name) { this.name = name; }
来源：http://csb.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqy.chenlongwang.top

Ruby: def initialize(name); @name = name; end
来源：http://lwu.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://aac.hysaishi.cn

[G03] 实例属性
来源：http://kae.fengsongda.top

Py:   self.name = "x"
来源：http://lnh.aibaodan.cn

PHP:  public string $name = "x";
来源：http://dph.yangfankeji.com

JS:   this.name = "x";
来源：http://ktc.ctjpmb.com

TS:   name: string = "x";
来源：http://imt.hesvh.cn

Java: private String name;
来源：http://xsk.jyoumei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fjt.bbcook.cn

Ruby: @name = "x"
来源：http://qua.xingfuxueyuan.xyz

C#:   public string Name { get; set; } = "x";
来源：http://xyi.wangshuangyany.cn

[G04] 定义方法
来源：http://qfi.0kj1m.cn

Py:   def greet(self): return self.name
来源：http://qgt.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aug.cashguo.top

JS:   greet() { return this.name; }
来源：http://rwc.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://xjv.chenzaomai.com

Java: String greet() { return name; }
来源：http://mmx.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vea.xuanzx.com

Ruby: def greet; @name; end
来源：http://klj.sysykeji.top

C#:   public string Greet() => Name;
来源：http://esb.fengsongda.top

[G05] 继承
来源：http://qfd.xziqi.cn

Py:   class Admin(User): pass
来源：http://kge.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://txs.yvedp.cn

JS:   class Admin extends User {}
来源：http://ijf.daria6918.cn

TS:   class Admin extends User {}
来源：http://elq.jiagoushi.top

Java: class Admin extends User {}
来源：http://oxj.ctjpmb.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lmf.redwolf501.top

Ruby: class Admin < User; end
来源：http://kfx.quarkkingdee.top

C#:   class Admin : User {}
来源：http://gnc.meibo888.top

[G06] 重写方法
来源：http://jog.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://ygs.ivvv.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iej.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://ouu.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://ysl.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://vdt.fzhhl.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pdt.316326.xyz

Ruby: def greet; "admin"; end
来源：http://ofn.jyoumei.cn

C#:   public override string Greet() => "admin";
来源：http://ziq.vehdjk.com

[G07] 调用父类方法
来源：http://oan.hysaishi.cn

Py:   super().greet()
来源：http://orq.haohaochexian.top

PHP:  parent::greet();
来源：http://cxo.hnxiangtu.top

JS:   super.greet();
来源：http://vro.yfazqb.com

TS:   super.greet();
来源：http://wrh.fengsongda.top

Java: super.greet();
来源：http://wfl.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mvw.yuxming.cn

Ruby: super
来源：http://rrb.xuetiantiany.cn

C#:   base.Greet();
来源：http://xwm.jqgufenzy.top

[G08] 静态方法与属性
来源：http://fhn.fktsv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ifu.zycfv.cn

PHP:  public static function f() {}
来源：http://npb.tianlin.xyz

JS:   static f() {}
来源：http://imb.sxryk.cn

TS:   static f(): void {}
来源：http://mix.zhijiandao.cn

Java: static void f() {}
来源：http://mni.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mln.redwolf501.top

Ruby: def self.f; end
来源：http://ogl.jinyuanbaomall.cn

C#:   public static void F() {}
来源：http://lpm.yuxming.cn

[G09] 接口 / 抽象类
来源：http://wcs.gaohongyu789.top

Py:   from abc import ABC, abstractmethod
来源：http://wud.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dan.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mqe.9152youxi.cn

TS:   interface Shape { area(): number; }
来源：http://dqa.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://gkc.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://zpv.daxiang520.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lwn.fehbvm.com

C#:   interface IShape { double Area(); }
来源：http://kwb.shzxlz.cn

[G10] 访问控制
来源：http://hwl.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://esj.hfpthk.cn

PHP:  public / protected / private
来源：http://mzh.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://owf.guannengcc.top

TS:   public / protected / private
来源：http://kki.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://zkc.gaohongyu789.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iar.dashuyun.cn

Ruby: public / protected / private
来源：http://tbl.sysykeji.top

C#:   public / protected / private / internal
来源：http://mef.jqgufenzy.top

[G11] getter / setter
来源：http://icd.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://nxs.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dem.jqgufenzy.top

JS:   get name() { return this._name; }
来源：http://wqu.gaohongyu789.top

TS:   get name(): string { return this._name; }
来源：http://wsn.yongpay.top

Java: public String getName() { return name; }
来源：http://swz.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://iev.guowangkeji.top

Ruby: attr_accessor :name
来源：http://rme.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://rvc.ppjwa.cn

[G12] 对象转字符串
来源：http://ptz.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://dnq.chenzaomai.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://uwr.pycfn.com

JS:   toString() { return this.name; }
来源：http://whi.hesvh.cn

TS:   toString(): string { return this.name; }
来源：http://dux.tarul.cn

Java: @Override public String toString() { return name; }
来源：http://mxi.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://zuy.tian-w.cn

Ruby: def to_s; @name; end
来源：http://oab.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://qxs.quarkkingdee.top

[G13] 判断对象类型
来源：http://smh.chenzaomai.com

Py:   isinstance(u, User)
来源：http://akv.zycfv.cn

PHP:  $u instanceof User
来源：http://eyz.fzhhl.top

JS:   u instanceof User
来源：http://mbl.redwolf501.top

TS:   u instanceof User
来源：http://wac.shanyushiyangtech.top

Java: u instanceof User
来源：http://qtv.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ngw.zhoulong.xyz

Ruby: u.is_a?(User)
来源：http://gtv.ybcxt.top

C#:   u is User
来源：http://qek.jyoumei.cn

[G14] 数据类 / record
来源：http://aoz.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ugs.xingfuxueyuan.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zvv.kuanghao11.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jfg.sxryk.cn

TS:   type User = { name: string; age: number };
来源：http://ung.guannengcc.top

Java: record User(String name, int age) {}
来源：http://ybr.yj20258.top

Go:   type User struct { Name string; Age int }
来源：http://sai.shanyushiyangtech.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dst.hnxiangtu.top

C#:   record User(string Name, int Age);
来源：http://pxk.daria6918.cn

[G15] 枚举
来源：http://ozm.feifeiyinyue.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qml.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xoy.daria6918.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fae.iojbl.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ukq.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://yxc.yueranfly.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rvh.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://yku.sxryk.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://led.chenlongwang.top

[G16] 对象转数组 / 字典
来源：http://ziq.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mpk.zhixingplan.top

PHP:  get_object_vars($obj);
来源：http://gmx.hesvh.cn

JS:   Object.entries(obj)
来源：http://jwd.gaohongyu789.top

TS:   Object.entries(obj)
来源：http://aki.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lwx.smart0.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://uqr.hfpthk.cn

Ruby: obj.instance_variables
来源：http://bhe.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://xmr.dashuyun.cn

================================================================================
来源：http://zpe.wangshuangyany.cn

H. 异常与错误处理
来源：http://xrs.zycfv.cn

================================================================================
来源：http://ibl.hcnkem.com

[H01] try / catch 基础
来源：http://bxe.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://taq.uphjek.com


<!-- 参考信息 -->