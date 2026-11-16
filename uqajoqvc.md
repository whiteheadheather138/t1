代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vhp.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tmb.ybcxt.top

Ruby: s.capitalize
来源：http://lku.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://njq.snrcjt.cn

[E18] 模板占位符替换
来源：http://yqi.hywenlv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kjd.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://knm.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uto.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cwz.haohaochexian.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ais.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yxz.cucudq.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dwg.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vta.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://cje.fktsv.cn

Py:   s.splitlines()
来源：http://gxp.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ulx.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://ckt.sysykeji.top

TS:   s.split(/\r?\n/)
来源：http://ppr.jinqigfzy.top

Java: s.lines().toList()
来源：http://tzr.fanxiaobao.xyz

Go:   strings.Split(s, "\n")
来源：http://wby.gotoacloud.top

Ruby: s.lines
来源：http://hgu.bbcook.cn

C#:   s.Split('\n')
来源：http://jqp.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://cht.cashguo.top

Py:   if not s:
来源：http://jih.iojbl.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xmd.hammf.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qsh.tanke756.top

TS:   if (s === "") {}
来源：http://dkf.yonumen.top

Java: if (s.isEmpty()) {}
来源：http://ciq.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://nrf.fktsv.cn

Ruby: if s.empty?
来源：http://dgb.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://akv.hcnkem.com

[E21] 超长截断加省略号
来源：http://els.sjlbkw.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wxy.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gij.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gtr.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xlf.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gic.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://aoh.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xux.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://frp.ivvv.top

[E22] 字节长度与字符长度
来源：http://fts.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nro.0kj1m.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cmb.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vsh.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbw.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ppr.c1oappe.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vgq.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://ptq.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uac.kuanghao11.cn

================================================================================
来源：http://roz.cashguo.top

F. 文件与目录
来源：http://qfi.hnqzz.top

================================================================================
来源：http://xre.nwbrower.top

[F01] 读取整个文件
来源：http://bme.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://orj.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://hwr.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sxm.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://epx.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tww.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://haz.vehdjk.com

Ruby: File.read("a.txt")
来源：http://rvo.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://jwn.fzhhl.top

[F02] 逐行读取文件
来源：http://ans.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ilh.zhiwuduotai.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://shg.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dba.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://efr.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vuh.cucudq.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qkx.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jgs.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aqv.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://vwl.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pdg.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://ohq.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cff.xziqi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tdc.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://box.nanxuanxn.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kip.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://cdq.birdmap.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wrs.hnxiangtu.top

[F04] 追加写入文件
来源：http://tij.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tsc.gzhubu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://nvu.cucudq.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://djh.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://imj.iojbl.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pzq.9152youxi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kyh.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kyw.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sbe.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://gse.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ejf.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://eqb.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://yuo.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://zhn.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wnu.cucudq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jyc.yuxming.cn

Ruby: File.exist?("a.txt")
来源：http://vln.meibo888.top

C#:   File.Exists("a.txt")
来源：http://xtp.hywenlv.cn

[F06] 删除文件
来源：http://fsb.nanxinkj.top

Py:   os.remove("a.txt")
来源：http://dhz.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://rfw.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://eab.zhixingplan.top

TS:   fs.unlinkSync("a.txt")
来源：http://wrp.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kct.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://keh.bjfxy.top

Ruby: File.delete("a.txt")
来源：http://kau.hammf.cn

C#:   File.Delete("a.txt");
来源：http://ydg.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://gts.hfpthk.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sxb.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tzd.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tka.yuxming.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qdb.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gsk.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sdd.fengsongda.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wpm.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oll.cheryme.top

[F08] 遍历目录
来源：http://tsf.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mhr.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zdw.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://mtt.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://qhv.sjlbkw.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dmo.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://fgm.zdqjudy.top

Ruby: Dir.children("dir")
来源：http://ndh.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://qoh.tarul.cn

[F09] 获取文件大小
来源：http://fhk.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://ddr.tianlin.xyz

PHP:  filesize("a.txt");
来源：http://rvk.ywan-chungtsiang.top

JS:   fs.statSync("a.txt").size
来源：http://gji.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://nxt.guowangkeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://qsm.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fkj.nwbrower.top

Ruby: File.size("a.txt")
来源：http://sdx.xuanzx.com

C#:   new FileInfo("a.txt").Length
来源：http://ixu.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://xlh.yonumen.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xxh.snrcjt.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tmb.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://syn.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://nzi.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://udm.yj202588.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bse.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ofm.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gho.chenzaomai.com

[F11] 复制与移动文件
来源：http://nwp.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xkl.jinyuanbaomall.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oeo.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qoq.yfazqb.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rod.zhoulong.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cmp.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kwp.chenlongwang.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://umy.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vhr.sysykeji.top

[F12] CSV 读写
来源：http://zon.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mzn.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://twr.yanxiufei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rak.shanyushiyangkeji.top

TS:   // 同上
来源：http://rop.pycfn.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ywk.hywenlv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ple.hfpthk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qwz.svipenyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uoe.zhongyouzk.top

================================================================================
来源：http://ise.guowangkeji.top

G. 面向对象
来源：http://adv.fzhhl.top

================================================================================
来源：http://qbm.jlsjyb.cn

[G01] 定义类
来源：http://nfy.zhoulong.xyz

Py:   class User: pass
来源：http://ehu.tian-w.cn

PHP:  class User {}
来源：http://qco.jyoumei.cn

JS:   class User {}
来源：http://sda.aizwys.cn

TS:   class User { name: string = ""; }
来源：http://puv.pycfn.com

Java: class User {}
来源：http://bhw.gogol.net.cn

Go:   type User struct { Name string }
来源：http://ccj.sxryk.cn

Ruby: class User; end
来源：http://wjb.jqgufenzy.top

C#:   class User {}
来源：http://kig.jlsjyb.cn

[G02] 构造函数
来源：http://lqr.yuanzhike.top

Py:   def __init__(self, name): self.name = name
来源：http://vbf.jyoumei.cn

PHP:  public function __construct(public string $name) {}
来源：http://zfx.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://ovr.yuxming.cn

TS:   constructor(public name: string) {}
来源：http://vnz.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://rzt.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fvt.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://kun.uphjek.com

C#:   public User(string name) { Name = name; }
来源：http://tdv.nwbrower.top

[G03] 实例属性
来源：http://wqy.jinyuanbaomall.cn

Py:   self.name = "x"
来源：http://ung.xuetiantiany.cn

PHP:  public string $name = "x";
来源：http://sdh.ctjpmb.com

JS:   this.name = "x";
来源：http://pnr.gaohongyu789.top

TS:   name: string = "x";
来源：http://uwf.shanyushiyangtech.top

Java: private String name;
来源：http://yrm.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fwj.yueranfly.top

Ruby: @name = "x"
来源：http://muj.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://bbl.yongpay.top

[G04] 定义方法
来源：http://nos.snrcjt.cn

Py:   def greet(self): return self.name
来源：http://tms.316326.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://kxe.gotoacloud.top

JS:   greet() { return this.name; }
来源：http://tot.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://kqb.xinyue.icu

Java: String greet() { return name; }
来源：http://spy.jqgufenzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rlo.guowangkeji.top

Ruby: def greet; @name; end
来源：http://bar.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://gtf.chenjidiqi.icu

[G05] 继承
来源：http://nrb.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://xev.tanke756.top

PHP:  class Admin extends User {}
来源：http://wvi.daxiang520.top

JS:   class Admin extends User {}
来源：http://hts.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://klr.gogol.net.cn

Java: class Admin extends User {}
来源：http://eow.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yuf.ppjwa.cn

Ruby: class Admin < User; end
来源：http://vhr.xziqi.cn

C#:   class Admin : User {}
来源：http://cnr.fzhhl.top

[G06] 重写方法
来源：http://bfa.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://ahb.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ekj.shuidangran.top

JS:   greet() { return "admin"; }
来源：http://ufr.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://fan.yvedp.cn

Java: @Override String greet() { return "admin"; }
来源：http://gbd.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jpx.gotoacloud.top

Ruby: def greet; "admin"; end
来源：http://dvk.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://bxa.jiagoushi.top

[G07] 调用父类方法
来源：http://cis.gogol.net.cn

Py:   super().greet()
来源：http://ydz.hfpthk.cn

PHP:  parent::greet();
来源：http://lrr.guannengcc.top

JS:   super.greet();
来源：http://bwm.pengpengdd.cyou

TS:   super.greet();
来源：http://jbl.feifeiyinyue.top

Java: super.greet();
来源：http://phb.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lqt.xziqi.cn

Ruby: super
来源：http://vel.dashuyun.cn

C#:   base.Greet();
来源：http://lbd.cqqwz.cn

[G08] 静态方法与属性
来源：http://ppn.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pyr.yfazqb.com

PHP:  public static function f() {}
来源：http://xpd.fehbvm.com

JS:   static f() {}
来源：http://lzk.wangshuangyany.cn

TS:   static f(): void {}
来源：http://isp.chenjidiqi.icu

Java: static void f() {}
来源：http://ahn.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cfr.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://cuq.zhengqikj.top

C#:   public static void F() {}
来源：http://qma.xziqi.cn

[G09] 接口 / 抽象类
来源：http://ukg.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://mmm.birdmap.top

PHP:  interface Shape { public function area(): float; }
来源：http://jlw.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iwf.xylfe.cn

TS:   interface Shape { area(): number; }
来源：http://gru.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://miq.smart0.xyz

Go:   type Shape interface { Area() float64 }
来源：http://sfg.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://alq.sweek.top

C#:   interface IShape { double Area(); }
来源：http://efg.fehbvm.com

[G10] 访问控制
来源：http://roa.yfazqb.com

Py:   约定 _protected / __private（不强制）
来源：http://ajd.zhixingplan.top

PHP:  public / protected / private
来源：http://bsc.shanyushiyangtech.top

JS:   #private 字段；其余公开
来源：http://ari.yvedp.cn

TS:   public / protected / private
来源：http://qnz.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://emy.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fzt.hcnkem.com

Ruby: public / protected / private
来源：http://nej.cucudq.cn

C#:   public / protected / private / internal
来源：http://obj.c1oappe.top

[G11] getter / setter
来源：http://fed.iojbl.cn

Py:   @property 与 @x.setter
来源：http://xoa.jinyuanbaomall.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://njc.ivvv.top

JS:   get name() { return this._name; }
来源：http://hem.yongpay.top

TS:   get name(): string { return this._name; }
来源：http://won.jyoumei.cn

Java: public String getName() { return name; }
来源：http://vnh.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://rpq.jiagoushi.top

Ruby: attr_accessor :name
来源：http://cto.xylfe.cn

C#:   public string Name { get; set; }
来源：http://tpz.dianchejie.cn

[G12] 对象转字符串
来源：http://ael.smart0.xyz

Py:   def __str__(self): return self.name
来源：http://zdw.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://exf.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://ona.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://buh.hnqzz.top

Java: @Override public String toString() { return name; }
来源：http://fzo.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://fts.yongpay.top

Ruby: def to_s; @name; end
来源：http://ulu.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://jwy.havefunace.top

[G13] 判断对象类型
来源：http://eqk.birdmap.top

Py:   isinstance(u, User)
来源：http://kux.mhx1999.top

PHP:  $u instanceof User
来源：http://lcs.ctjpmb.com

JS:   u instanceof User
来源：http://urg.andypj.xyz

TS:   u instanceof User
来源：http://ley.dianchejie.cn

Java: u instanceof User
来源：http://lza.quarkkingdee.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://feo.c1oappe.top

Ruby: u.is_a?(User)
来源：http://yfl.sjlbkw.cn

C#:   u is User
来源：http://ifg.dianchejie.cn

[G14] 数据类 / record
来源：http://oqd.tanke756.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xwz.birdmap.top

PHP:  // 用 readonly 属性模拟
来源：http://eon.chenjidiqi.icu

JS:   // 无内置：普通类或对象字面量
来源：http://tds.jyoumei.cn

TS:   type User = { name: string; age: number };
来源：http://mgt.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://zhv.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://cud.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jdr.daxiang520.top

C#:   record User(string Name, int Age);
来源：http://edh.gzhubu.top

[G15] 枚举
来源：http://uje.fktsv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bvl.jinghuilouyu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mox.guowangkeji.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://idk.hnxiangtu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wmr.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://pln.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://crm.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://mqv.xuanzx.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://otb.tian-w.cn

[G16] 对象转数组 / 字典
来源：http://kav.gzhubu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iku.aizwys.cn


<!-- 参考信息 -->