代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tjl.pycfn.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://aep.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xzu.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cfc.yj202588.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qwu.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gdr.ehwqpu.com

Ruby: s.capitalize
来源：http://iou.cashguo.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cjv.cucudq.cn

[E18] 模板占位符替换
来源：http://oks.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gxi.yuxming.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fhg.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://itf.zhaomingkeji.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://nzx.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ffj.cqqwz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ifb.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qvl.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iwb.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://sjz.daria6918.cn

Py:   s.splitlines()
来源：http://fli.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pao.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://smg.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://zru.gzhubu.top

Java: s.lines().toList()
来源：http://qjn.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://fjt.quarkkingdee.top

Ruby: s.lines
来源：http://wxq.zycfv.cn

C#:   s.Split('\n')
来源：http://zzv.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://zlp.jianghu66.top

Py:   if not s:
来源：http://szk.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://atf.fehbvm.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://roo.yangfankeji.com

TS:   if (s === "") {}
来源：http://nut.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://exf.nanxinkj.top

Go:   if s == "" {}
来源：http://hfr.gaohongyu789.top

Ruby: if s.empty?
来源：http://clj.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tqc.zhengqikj.top

[E21] 超长截断加省略号
来源：http://fwr.yanxiufei.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cyi.guowangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kqr.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zxv.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jdn.316326.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tmw.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://wbz.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://avo.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fdx.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://dks.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yvj.gogol.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vwc.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ibj.sufxvd.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eta.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gpu.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wvj.hnqzz.top

Ruby: s.bytesize;  s.length
来源：http://bif.zhaomingkeji.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://trk.nwbrower.top

================================================================================
来源：http://apo.ydzc1.top

F. 文件与目录
来源：http://iut.yj202588.top

================================================================================
来源：http://jim.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://kjl.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://chg.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://wxt.shzxlz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lqi.yueranfly.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mlg.zhoulong.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://tem.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zvy.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://uvp.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://flv.bbcook.cn

[F02] 逐行读取文件
来源：http://ddy.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gjq.bjfxy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://roq.dashuyun.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://syg.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qji.daria6918.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwi.tian-w.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dje.tianlin.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://utc.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://czf.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://agi.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qqs.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tzl.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oyd.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ilm.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qbr.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sse.bbcook.cn

Ruby: File.write("a.txt", "hi")
来源：http://rkv.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dky.jqgufenzy.top

[F04] 追加写入文件
来源：http://ckj.zhengqikj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bfm.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ciu.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ohb.svipenyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vqa.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ifo.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dxg.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tdd.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ynk.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://thf.fengsongda.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mhd.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://luy.tian-w.cn

JS:   fs.existsSync("a.txt")
来源：http://xhm.redwolf501.top

TS:   fs.existsSync("a.txt")
来源：http://qol.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fsb.snrcjt.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://diz.jiagoushi.top

Ruby: File.exist?("a.txt")
来源：http://ate.hammf.cn

C#:   File.Exists("a.txt")
来源：http://hod.fanxiaobao.xyz

[F06] 删除文件
来源：http://kun.gaohongyu789.top

Py:   os.remove("a.txt")
来源：http://ioi.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://ern.aizwys.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pfm.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ehh.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jom.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://zuo.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://tfr.andypj.xyz

C#:   File.Delete("a.txt");
来源：http://ued.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://das.iojbl.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://olk.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dje.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qqt.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cvc.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tlq.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gci.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qxo.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://urq.chenzaomai.com

[F08] 遍历目录
来源：http://kwo.chenjidiqi.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://tak.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zhu.sweek.top

JS:   fs.readdirSync("dir")
来源：http://tpj.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://kix.cqqwz.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ryb.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fsz.aizwys.cn

Ruby: Dir.children("dir")
来源：http://gfk.xziqi.cn

C#:   Directory.GetFiles("dir")
来源：http://vru.jqgfzy.top

[F09] 获取文件大小
来源：http://uvz.hysaishi.cn

Py:   os.path.getsize("a.txt")
来源：http://lzg.daxiang520.top

PHP:  filesize("a.txt");
来源：http://juu.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://qjx.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://ogl.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://bld.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://swc.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://jiy.yj202588.top

C#:   new FileInfo("a.txt").Length
来源：http://rme.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://ubf.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pcu.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ket.gotoacloud.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtf.havefunace.top

TS:   path.extname("a.txt")
来源：http://krt.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yoi.chenlongwang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ydi.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wfl.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xcy.daria6918.cn

[F11] 复制与移动文件
来源：http://ixc.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zlt.jlsjyb.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qxl.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qdl.uphjek.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgj.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vfi.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bpu.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qoc.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kjp.zhengqikj.top

[F12] CSV 读写
来源：http://tkj.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gks.cqqwz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mti.ybcxt.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://izr.yj20258.top

TS:   // 同上
来源：http://bmy.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mpx.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wxo.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yfa.aibaodan.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qhc.zhiwuduotai.top

================================================================================
来源：http://spl.shangyingyoupin.top

G. 面向对象
来源：http://zmc.zhongyouzk.top

================================================================================
来源：http://glp.yonumen.top

[G01] 定义类
来源：http://xcb.jiagoushi.top

Py:   class User: pass
来源：http://rer.jqgufenzy.top

PHP:  class User {}
来源：http://hjr.chenzaomai.com

JS:   class User {}
来源：http://rli.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://yvp.daria6918.cn

Java: class User {}
来源：http://yir.birdmap.top

Go:   type User struct { Name string }
来源：http://ggf.zhijiandao.cn

Ruby: class User; end
来源：http://vrs.hysaishi.cn

C#:   class User {}
来源：http://jqs.sweek.top

[G02] 构造函数
来源：http://tgy.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://icn.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://gsk.zhongyouzk.top

JS:   constructor(name) { this.name = name; }
来源：http://caj.zdqjudy.top

TS:   constructor(public name: string) {}
来源：http://kdg.fehbvm.com

Java: User(String name) { this.name = name; }
来源：http://fvu.cheryme.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yjv.jqgufenzy.top

Ruby: def initialize(name); @name = name; end
来源：http://sor.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://ypt.cdnleiting.top

[G03] 实例属性
来源：http://qbl.zhiwuduotai.top

Py:   self.name = "x"
来源：http://gmy.zdqjudy.top

PHP:  public string $name = "x";
来源：http://htp.zhiwuduotai.top

JS:   this.name = "x";
来源：http://fgp.jiagoushi.top

TS:   name: string = "x";
来源：http://obd.ppjwa.cn

Java: private String name;
来源：http://evs.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kse.guannengcc.top

Ruby: @name = "x"
来源：http://rvw.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://snq.epnwcf.com

[G04] 定义方法
来源：http://gly.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://gnj.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://whh.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://vbw.yuanzhike.top

TS:   greet(): string { return this.name; }
来源：http://yhc.jiagoushi.top

Java: String greet() { return name; }
来源：http://jqg.tanke756.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uhf.ivvv.top

Ruby: def greet; @name; end
来源：http://wvn.zhengqikj.top

C#:   public string Greet() => Name;
来源：http://wum.guannengcc.top

[G05] 继承
来源：http://uhz.daria6918.cn

Py:   class Admin(User): pass
来源：http://iud.xinyue.icu

PHP:  class Admin extends User {}
来源：http://osp.tianlin.xyz

JS:   class Admin extends User {}
来源：http://ljv.c1oappe.top

TS:   class Admin extends User {}
来源：http://kyb.andypj.xyz

Java: class Admin extends User {}
来源：http://dez.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wqq.tarul.cn

Ruby: class Admin < User; end
来源：http://ndv.hcnkem.com

C#:   class Admin : User {}
来源：http://lwh.mhx1999.top

[G06] 重写方法
来源：http://yzv.ywan-chungtsiang.top

Py:   def greet(self): return "admin"
来源：http://wrt.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vqr.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://whh.guowangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://voj.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://rpa.yueranfly.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://spa.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://nal.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://lee.fktsv.cn

[G07] 调用父类方法
来源：http://wqb.0kj1m.cn

Py:   super().greet()
来源：http://tva.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://ots.zhixingplan.top

JS:   super.greet();
来源：http://wjp.birdmap.top

TS:   super.greet();
来源：http://rud.shzxlz.cn

Java: super.greet();
来源：http://slj.bbcook.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://izk.daxiang520.top

Ruby: super
来源：http://mlh.yj20258.top

C#:   base.Greet();
来源：http://qto.316326.xyz

[G08] 静态方法与属性
来源：http://puc.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lyp.tianlin.xyz

PHP:  public static function f() {}
来源：http://hal.daria6918.cn

JS:   static f() {}
来源：http://ssx.havefunace.top

TS:   static f(): void {}
来源：http://wbp.sufxvd.cn

Java: static void f() {}
来源：http://vma.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sff.fengsongda.top

Ruby: def self.f; end
来源：http://xql.hesvh.cn

C#:   public static void F() {}
来源：http://nif.yanxiufei.cn

[G09] 接口 / 抽象类
来源：http://fnh.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://wnz.cqqwz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uhf.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hpe.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://ucs.shanyushiyangkeji.top

Java: interface Shape { double area(); }
来源：http://gte.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://pxh.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lpw.sjlbkw.cn

C#:   interface IShape { double Area(); }
来源：http://acf.c1oappe.top

[G10] 访问控制
来源：http://gtp.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://hqj.zhengqikj.top

PHP:  public / protected / private
来源：http://umo.ywan-chungtsiang.top

JS:   #private 字段；其余公开
来源：http://ecl.mhx1999.top

TS:   public / protected / private
来源：http://wkf.jinqigufen.top

Java: public / protected / private / 默认包级
来源：http://lde.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fti.xuanzx.com

Ruby: public / protected / private
来源：http://pns.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://irt.kuanghao11.cn

[G11] getter / setter
来源：http://zji.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://yck.bjfxy.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jxv.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://ynm.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://vbp.cucudq.cn

Java: public String getName() { return name; }
来源：http://taf.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vwm.tanke756.top

Ruby: attr_accessor :name
来源：http://hss.tian-w.cn

C#:   public string Name { get; set; }
来源：http://wyt.jqgfzy.top

[G12] 对象转字符串
来源：http://kjn.ywan-chungtsiang.top

Py:   def __str__(self): return self.name
来源：http://szv.ydzc1.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://vkv.fengsongda.top

JS:   toString() { return this.name; }
来源：http://ime.havefunace.top

TS:   toString(): string { return this.name; }
来源：http://hkr.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://kxc.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://sje.guannengcc.top

Ruby: def to_s; @name; end
来源：http://ppk.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://vyr.feifeiyinyue.top

[G13] 判断对象类型
来源：http://jxc.cqqwz.cn

Py:   isinstance(u, User)
来源：http://rip.nwbrower.top

PHP:  $u instanceof User
来源：http://foc.shanyushiyangtech.top

JS:   u instanceof User
来源：http://nga.wangshuangyany.cn

TS:   u instanceof User
来源：http://dlp.daxiang520.top

Java: u instanceof User
来源：http://atn.feifeiyinyue.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://pbk.mhx1999.top

Ruby: u.is_a?(User)
来源：http://cxt.chenjidiqi.icu

C#:   u is User
来源：http://chx.guannengcc.top

[G14] 数据类 / record
来源：http://kmv.uphjek.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://khs.zhiwuduotai.top

PHP:  // 用 readonly 属性模拟
来源：http://bne.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://zmv.aibaodan.cn

TS:   type User = { name: string; age: number };
来源：http://rvj.hnqzz.top

Java: record User(String name, int age) {}
来源：http://mnh.xylfe.cn

Go:   type User struct { Name string; Age int }
来源：http://jra.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zre.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://mca.zhixingplan.top

[G15] 枚举
来源：http://qbu.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zav.ppjwa.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zba.zhongyouzk.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pbb.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://szr.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://yxp.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://beb.zhoulong.xyz


<!-- 参考信息 -->