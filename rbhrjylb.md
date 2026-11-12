代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fht.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xgx.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wda.daxiang520.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jro.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kvr.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ipu.jqgfzy.top

Ruby: s.capitalize
来源：http://vpb.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzn.yj202588.top

[E18] 模板占位符替换
来源：http://xdo.cucudq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xtl.yj202588.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lyw.jqgufenzy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uxk.ehwqpu.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ewb.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cpj.svipenyu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yrw.feifeiyinyue.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qrp.fzhhl.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gki.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://oqn.dashuyun.cn

Py:   s.splitlines()
来源：http://yjl.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sqx.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://phs.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://yxj.shangyingyoupin.top

Java: s.lines().toList()
来源：http://gkp.hfpthk.cn

Go:   strings.Split(s, "\n")
来源：http://lce.nwbrower.top

Ruby: s.lines
来源：http://qkt.daria6918.cn

C#:   s.Split('\n')
来源：http://ysk.fktsv.cn

[E20] 判断字符串是否为空
来源：http://qgv.iojbl.cn

Py:   if not s:
来源：http://ged.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://alm.jlsjyb.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ajy.fktsv.cn

TS:   if (s === "") {}
来源：http://lee.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://nuy.pycfn.com

Go:   if s == "" {}
来源：http://qjc.snrcjt.cn

Ruby: if s.empty?
来源：http://zgh.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bph.fanxiaobao.xyz

[E21] 超长截断加省略号
来源：http://sbk.redwolf501.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mun.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://isl.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eey.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://abc.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vwi.andypj.xyz

Go:   // 按 rune 判断长度后截断
来源：http://fsy.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baz.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bhz.hnqzz.top

[E22] 字节长度与字符长度
来源：http://nlv.dashuyun.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zzm.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qid.yvedp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qnc.hysaishi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aje.sjlbkw.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dab.fengsongda.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://psx.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://vdm.fzhhl.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://eep.feifeiyinyue.top

================================================================================
来源：http://bzk.cashguo.top

F. 文件与目录
来源：http://pdn.sxryk.cn

================================================================================
来源：http://dlt.sufxvd.cn

[F01] 读取整个文件
来源：http://mtf.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ble.cqqwz.cn

PHP:  file_get_contents("a.txt");
来源：http://iso.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sit.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ueb.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://qjk.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zui.yongpay.top

Ruby: File.read("a.txt")
来源：http://nsu.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://jur.shuidangran.top

[F02] 逐行读取文件
来源：http://hqi.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gyu.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sdm.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rai.xuetiantiany.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jyf.zhijiandao.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://axk.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gph.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bvp.shuidangran.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xwa.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://uvz.chenzaomai.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cyx.tarul.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lzo.9152youxi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://onw.9152youxi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://znk.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sfy.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://llc.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://psc.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eqn.zhiwuduotai.top

[F04] 追加写入文件
来源：http://kif.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lki.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dkl.yangfankeji.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yrc.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://chq.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jry.chenzaomai.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rvy.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bcd.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ael.yuanzhike.top

[F05] 判断文件或目录是否存在
来源：http://qxx.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ocq.iojbl.cn

PHP:  file_exists("a.txt");
来源：http://gik.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://ggh.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://ywd.zhaomingkeji.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://muy.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fwr.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://dmj.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://xzu.shzxlz.cn

[F06] 删除文件
来源：http://ivz.gzhubu.top

Py:   os.remove("a.txt")
来源：http://jtx.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://abf.yuanzhike.top

JS:   fs.unlinkSync("a.txt")
来源：http://bvn.316326.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://sjw.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zay.cucudq.cn

Go:   os.Remove("a.txt")
来源：http://edh.cashguo.top

Ruby: File.delete("a.txt")
来源：http://nwn.yj20258.top

C#:   File.Delete("a.txt");
来源：http://zcv.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://blt.hammf.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wia.yonumen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qax.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xzj.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tgy.quarkkingdee.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ccn.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zhp.dashuyun.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rdy.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dgu.svipenyu.cn

[F08] 遍历目录
来源：http://fzn.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fmt.uphjek.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://axv.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://vho.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://ckk.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vmv.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://phc.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://mca.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://iky.hnqzz.top

[F09] 获取文件大小
来源：http://ris.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://gzc.cucudq.cn

PHP:  filesize("a.txt");
来源：http://ooy.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://pxy.ivvv.top

TS:   fs.statSync("a.txt").size
来源：http://cpf.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xyr.316326.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kwy.cqqwz.cn

Ruby: File.size("a.txt")
来源：http://via.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://xko.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://qrt.svipenyu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dll.shanyushiyangtech.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://itk.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lyz.guannengcc.top

TS:   path.extname("a.txt")
来源：http://wcd.kuanghao11.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://myn.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://azp.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rfz.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mff.sweek.top

[F11] 复制与移动文件
来源：http://fkp.redwolf501.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rnz.hesvh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zdk.aizwys.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zog.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nqh.shanyushiyangtech.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dgh.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://web.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nbb.zhongyouzk.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://upd.mhx1999.top

[F12] CSV 读写
来源：http://hey.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jfw.nwbrower.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nzv.jlsjyb.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nuq.yueranfly.top

TS:   // 同上
来源：http://gjj.yuanzhike.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sms.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nvn.jinghuilouyu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mrz.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://rmk.yj20258.top

================================================================================
来源：http://tbx.yfazqb.com

G. 面向对象
来源：http://wkq.zycfv.cn

================================================================================
来源：http://dqu.chenjidiqi.icu

[G01] 定义类
来源：http://nwv.xuanzx.com

Py:   class User: pass
来源：http://kcm.havefunace.top

PHP:  class User {}
来源：http://uti.nanxinkj.top

JS:   class User {}
来源：http://udc.tanke756.top

TS:   class User { name: string = ""; }
来源：http://wfj.yj202588.top

Java: class User {}
来源：http://okc.zhiwuduotai.top

Go:   type User struct { Name string }
来源：http://xjl.sufxvd.cn

Ruby: class User; end
来源：http://jno.yj20258.top

C#:   class User {}
来源：http://zgf.yueranfly.top

[G02] 构造函数
来源：http://mfu.hfpthk.cn

Py:   def __init__(self, name): self.name = name
来源：http://ede.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://got.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://tmt.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://rol.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://cje.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cgw.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://aoc.sufxvd.cn

C#:   public User(string name) { Name = name; }
来源：http://kky.pengpengdd.cyou

[G03] 实例属性
来源：http://wfg.vqdsnc.cn

Py:   self.name = "x"
来源：http://upt.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://gdj.hesvh.cn

JS:   this.name = "x";
来源：http://tel.xuanzx.com

TS:   name: string = "x";
来源：http://plb.yuanzhike.top

Java: private String name;
来源：http://qio.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vvu.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://dlm.fehbvm.com

C#:   public string Name { get; set; } = "x";
来源：http://vrv.dashuyun.cn

[G04] 定义方法
来源：http://yfe.yfazqb.com

Py:   def greet(self): return self.name
来源：http://clb.xuetiantiany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kwn.bjfxy.top

JS:   greet() { return this.name; }
来源：http://jge.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://srd.tanke756.top

Java: String greet() { return name; }
来源：http://tdc.pycfn.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://wei.andypj.xyz

Ruby: def greet; @name; end
来源：http://ies.bjfxy.top

C#:   public string Greet() => Name;
来源：http://dlb.0kj1m.cn

[G05] 继承
来源：http://cwc.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://pct.redwolf501.top

PHP:  class Admin extends User {}
来源：http://dxs.tian-w.cn

JS:   class Admin extends User {}
来源：http://jbv.sweek.top

TS:   class Admin extends User {}
来源：http://zov.yvedp.cn

Java: class Admin extends User {}
来源：http://fsh.jyoumei.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kzy.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://wgo.hongshengwenyu.top

C#:   class Admin : User {}
来源：http://sdr.meibo888.top

[G06] 重写方法
来源：http://guw.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://bwu.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lfr.meibo888.top

JS:   greet() { return "admin"; }
来源：http://uxn.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://yui.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://zbt.cashguo.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nbh.yj20258.top

Ruby: def greet; "admin"; end
来源：http://ryh.yj20258888.top

C#:   public override string Greet() => "admin";
来源：http://dmx.c1oappe.top

[G07] 调用父类方法
来源：http://iur.shanyushiyangkeji.top

Py:   super().greet()
来源：http://qmf.xinyue.icu

PHP:  parent::greet();
来源：http://vsh.pengpengdd.cyou

JS:   super.greet();
来源：http://izq.shangyingyoupin.top

TS:   super.greet();
来源：http://kog.zhixingplan.top

Java: super.greet();
来源：http://poc.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rvh.zycfv.cn

Ruby: super
来源：http://hjp.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://qvn.fehbvm.com

[G08] 静态方法与属性
来源：http://cmi.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nas.zhixingplan.top

PHP:  public static function f() {}
来源：http://tse.hfpthk.cn

JS:   static f() {}
来源：http://xtl.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://nmf.hesvh.cn

Java: static void f() {}
来源：http://vwg.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ees.yuxming.cn

Ruby: def self.f; end
来源：http://cjz.guannengcc.top

C#:   public static void F() {}
来源：http://uyg.yongpay.top

[G09] 接口 / 抽象类
来源：http://wxj.cdnleiting.top

Py:   from abc import ABC, abstractmethod
来源：http://otj.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://rsj.yuxming.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nxd.sweek.top

TS:   interface Shape { area(): number; }
来源：http://wdg.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://pwj.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://xtv.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ztm.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://oef.nwbrower.top

[G10] 访问控制
来源：http://uuy.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://szf.uphjek.com

PHP:  public / protected / private
来源：http://paa.dianchejie.cn

JS:   #private 字段；其余公开
来源：http://nan.gotoacloud.top

TS:   public / protected / private
来源：http://rhn.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://khv.xziqi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mic.sweek.top

Ruby: public / protected / private
来源：http://wvu.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://pkp.pycfn.com

[G11] getter / setter
来源：http://gni.316326.xyz

Py:   @property 与 @x.setter
来源：http://exe.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://sdu.yuxming.cn

JS:   get name() { return this._name; }
来源：http://ymj.fktsv.cn

TS:   get name(): string { return this._name; }
来源：http://fbj.wangdashe.top

Java: public String getName() { return name; }
来源：http://swn.wangshuangyany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://whr.guannengcc.top

Ruby: attr_accessor :name
来源：http://sgd.yj202588.top

C#:   public string Name { get; set; }
来源：http://cug.316326.xyz

[G12] 对象转字符串
来源：http://chq.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://yoo.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qjz.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://xwa.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://wvo.haohaochexian.top

Java: @Override public String toString() { return name; }
来源：http://egr.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://qrm.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://ozl.yj202588.top

C#:   public override string ToString() => Name;
来源：http://oeo.gogol.net.cn

[G13] 判断对象类型
来源：http://cnd.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://qpd.yuanzhike.top

PHP:  $u instanceof User
来源：http://fio.vqdsnc.cn

JS:   u instanceof User
来源：http://iev.ppjwa.cn

TS:   u instanceof User
来源：http://kqk.hnxiangtu.top

Java: u instanceof User
来源：http://unq.redwolf501.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://duh.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://ftt.fktsv.cn

C#:   u is User
来源：http://xxd.pycfn.com

[G14] 数据类 / record
来源：http://xgm.kuanghao11.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aau.uphjek.com

PHP:  // 用 readonly 属性模拟
来源：http://xyb.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aeq.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://ptv.ivvv.top

Java: record User(String name, int age) {}
来源：http://fln.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://vwi.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qza.cashguo.top

C#:   record User(string Name, int Age);
来源：http://xrs.sysykeji.top

[G15] 枚举
来源：http://qbu.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qwr.hywenlv.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kpf.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jhf.jinyuanbaomall.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jfq.hywenlv.cn

Java: enum Color { RED, GREEN }
来源：http://wio.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cyo.shzxlz.cn


<!-- 参考信息 -->