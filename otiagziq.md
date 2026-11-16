代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://kzz.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wzk.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://opu.bbcook.cn

[E17] 首字母大写
来源：http://afq.aibaodan.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nbs.fzhhl.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://afk.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nsl.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovw.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lvg.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zry.ydzc1.top

Ruby: s.capitalize
来源：http://ylr.jlsjyb.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wze.svipenyu.cn

[E18] 模板占位符替换
来源：http://ojg.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kmh.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wjd.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ubu.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kaz.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ofm.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bfu.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zjw.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://erv.yj20258.top

[E19] 多行文本按行拆分
来源：http://wcj.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://sbu.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://onf.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://qjz.hcnkem.com

TS:   s.split(/\r?\n/)
来源：http://idb.zhongyouzk.top

Java: s.lines().toList()
来源：http://pkw.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://zms.chenzaomai.com

Ruby: s.lines
来源：http://fca.yangfankeji.com

C#:   s.Split('\n')
来源：http://tdi.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://rml.bjfxy.top

Py:   if not s:
来源：http://gxc.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://drl.snrcjt.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://htd.jlsjyb.cn

TS:   if (s === "") {}
来源：http://kui.hongshengwenyu.top

Java: if (s.isEmpty()) {}
来源：http://etn.yj20258.top

Go:   if s == "" {}
来源：http://sje.jianghu66.top

Ruby: if s.empty?
来源：http://wao.xinyue.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://foj.aizwys.cn

[E21] 超长截断加省略号
来源：http://wtd.andypj.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ktj.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zbt.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hsa.316326.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mzy.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vky.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://blr.jianghu66.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uce.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ghd.xylfe.cn

[E22] 字节长度与字符长度
来源：http://xev.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lao.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dxy.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xsd.zhengqikj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://amj.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wjv.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jjx.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://mjh.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ahg.xylfe.cn

================================================================================
来源：http://hpf.hnxiangtu.top

F. 文件与目录
来源：http://dxl.ywan-chungtsiang.top

================================================================================
来源：http://tji.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://fuo.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oqg.epnwcf.com

PHP:  file_get_contents("a.txt");
来源：http://ugq.nwbrower.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://eto.ydjk.org.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mrx.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gwi.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kyz.shuidangran.top

Ruby: File.read("a.txt")
来源：http://yrb.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ctf.smart0.xyz

[F02] 逐行读取文件
来源：http://mfj.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://edc.uphjek.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pdf.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://siz.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://paz.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kcx.jinghuilouyu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ifz.snrcjt.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fpp.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lzd.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://dqn.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gsr.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wyc.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dix.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dje.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mfq.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eyt.fktsv.cn

Ruby: File.write("a.txt", "hi")
来源：http://imw.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cja.yfazqb.com

[F04] 追加写入文件
来源：http://fgo.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xui.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://htm.xuetiantiany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://izc.andypj.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yas.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fjc.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://irk.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hzj.chenzaomai.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aai.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://dam.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fqx.meibo888.top

PHP:  file_exists("a.txt");
来源：http://rtn.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://mma.yonumen.top

TS:   fs.existsSync("a.txt")
来源：http://kzz.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jjp.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mfm.zdqjudy.top

Ruby: File.exist?("a.txt")
来源：http://wgx.hammf.cn

C#:   File.Exists("a.txt")
来源：http://epv.sjlbkw.cn

[F06] 删除文件
来源：http://zfg.zycfv.cn

Py:   os.remove("a.txt")
来源：http://vmp.316326.xyz

PHP:  unlink("a.txt");
来源：http://pxz.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://lpx.kuanghao11.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gpd.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sec.vqdsnc.cn

Go:   os.Remove("a.txt")
来源：http://soy.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://twu.jianghu66.top

C#:   File.Delete("a.txt");
来源：http://yim.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://npn.52xcode.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nbc.dianchejie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kuq.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aun.cdnleiting.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xyh.52xcode.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://khd.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ong.yueranfly.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mst.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cjn.nwbrower.top

[F08] 遍历目录
来源：http://pot.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sic.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vdk.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://ehs.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://mtd.jqgfzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pvl.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jbd.zdbjq.cn

Ruby: Dir.children("dir")
来源：http://esd.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://tkm.havefunace.top

[F09] 获取文件大小
来源：http://ovd.cheryme.top

Py:   os.path.getsize("a.txt")
来源：http://gyk.fehbvm.com

PHP:  filesize("a.txt");
来源：http://mjc.jianghu66.top

JS:   fs.statSync("a.txt").size
来源：http://iak.xuetiantiany.cn

TS:   fs.statSync("a.txt").size
来源：http://bzj.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://vjh.guannengcc.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rjr.mhx1999.top

Ruby: File.size("a.txt")
来源：http://iys.jianghu66.top

C#:   new FileInfo("a.txt").Length
来源：http://nnr.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://pia.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xwt.fengsongda.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bfo.hnqzz.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pfc.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://mti.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://izr.cashguo.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gmm.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://skd.hcnkem.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qen.hnqzz.top

[F11] 复制与移动文件
来源：http://zzr.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sfg.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://des.jinqigfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wue.cashguo.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jrr.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rzb.ivvv.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://abz.shuidangran.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uaj.hysaishi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cdo.jinqigfzy.top

[F12] CSV 读写
来源：http://kqk.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lfr.tanke756.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jgm.sweek.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://aqg.gzhubu.top

TS:   // 同上
来源：http://web.havefunace.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sen.zhiwuduotai.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pqq.shanyushiyangtech.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yob.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://msl.nwbrower.top

================================================================================
来源：http://wiy.vehdjk.com

G. 面向对象
来源：http://gsu.sufxvd.cn

================================================================================
来源：http://noi.tianlin.xyz

[G01] 定义类
来源：http://ida.havefunace.top

Py:   class User: pass
来源：http://pbh.gaohongyu789.top

PHP:  class User {}
来源：http://nud.shanyushiyangkeji.top

JS:   class User {}
来源：http://nwl.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://zsk.shangyingyoupin.top

Java: class User {}
来源：http://won.shzxlz.cn

Go:   type User struct { Name string }
来源：http://kgk.redwolf501.top

Ruby: class User; end
来源：http://yqn.xylfe.cn

C#:   class User {}
来源：http://quq.yj20258.top

[G02] 构造函数
来源：http://ema.jqgfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://dra.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://iqq.yuxming.cn

JS:   constructor(name) { this.name = name; }
来源：http://yvz.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://kho.nwbrower.top

Java: User(String name) { this.name = name; }
来源：http://bbb.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bzj.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://ues.cqqwz.cn

C#:   public User(string name) { Name = name; }
来源：http://dwi.hnqzz.top

[G03] 实例属性
来源：http://scr.shuidangran.top

Py:   self.name = "x"
来源：http://vmc.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://wgq.yfazqb.com

JS:   this.name = "x";
来源：http://rlb.yonumen.top

TS:   name: string = "x";
来源：http://xch.aizwys.cn

Java: private String name;
来源：http://duw.tian-w.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ilt.c1oappe.top

Ruby: @name = "x"
来源：http://rdu.hcnkem.com

C#:   public string Name { get; set; } = "x";
来源：http://iji.redwolf501.top

[G04] 定义方法
来源：http://fah.fehbvm.com

Py:   def greet(self): return self.name
来源：http://kij.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ftm.fktsv.cn

JS:   greet() { return this.name; }
来源：http://bga.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://ael.zycfv.cn

Java: String greet() { return name; }
来源：http://uum.iojbl.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aeg.guowangkeji.top

Ruby: def greet; @name; end
来源：http://zoo.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://kmg.hammf.cn

[G05] 继承
来源：http://wwo.tanke756.top

Py:   class Admin(User): pass
来源：http://lpq.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://fyb.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://hmh.gogol.net.cn

TS:   class Admin extends User {}
来源：http://vka.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://mlg.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ayw.dianchejie.cn

Ruby: class Admin < User; end
来源：http://xgq.zhoulong.xyz

C#:   class Admin : User {}
来源：http://tzn.hcnkem.com

[G06] 重写方法
来源：http://tcu.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://qnd.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ozl.hnqzz.top

JS:   greet() { return "admin"; }
来源：http://adm.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://zdp.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://zce.dashuyun.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kxb.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://dwh.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://mhd.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://cfk.jianghu66.top

Py:   super().greet()
来源：http://owc.shanyushiyangkeji.top

PHP:  parent::greet();
来源：http://nma.daria6918.cn

JS:   super.greet();
来源：http://tpj.guowangkeji.top

TS:   super.greet();
来源：http://tfr.meibo888.top

Java: super.greet();
来源：http://ptu.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lxq.xylfe.cn

Ruby: super
来源：http://wkw.jinqigufen.top

C#:   base.Greet();
来源：http://nlo.sjlbkw.cn

[G08] 静态方法与属性
来源：http://zka.zdbjq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cus.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://lzq.zhoulong.xyz

JS:   static f() {}
来源：http://wgs.jinqigufen.top

TS:   static f(): void {}
来源：http://adt.chenzaomai.com

Java: static void f() {}
来源：http://uex.yj202588.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dta.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://uzm.sxryk.cn

C#:   public static void F() {}
来源：http://nkw.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://ihs.cashguo.top

Py:   from abc import ABC, abstractmethod
来源：http://xlf.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://jfb.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wan.hcnkem.com

TS:   interface Shape { area(): number; }
来源：http://ipx.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://uet.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ilo.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://keb.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://ymf.fehbvm.com

[G10] 访问控制
来源：http://uko.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://ztv.316326.xyz

PHP:  public / protected / private
来源：http://rtm.pycfn.com

JS:   #private 字段；其余公开
来源：http://pzh.hesvh.cn

TS:   public / protected / private
来源：http://ngh.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://uef.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gxv.gotoacloud.top

Ruby: public / protected / private
来源：http://kow.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://bqx.cqqwz.cn

[G11] getter / setter
来源：http://jhr.jinghuilouyu.cn

Py:   @property 与 @x.setter
来源：http://bpn.epnwcf.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fqe.yj20258.top

JS:   get name() { return this._name; }
来源：http://sji.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://enh.zhixingplan.top

Java: public String getName() { return name; }
来源：http://ngx.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://npd.cashguo.top

Ruby: attr_accessor :name
来源：http://arh.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://xgc.ehwqpu.com

[G12] 对象转字符串
来源：http://mag.316326.xyz

Py:   def __str__(self): return self.name
来源：http://loc.aizwys.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vjk.ydjk.org.cn

JS:   toString() { return this.name; }
来源：http://nfc.cheryme.top

TS:   toString(): string { return this.name; }
来源：http://bsz.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://jxx.shanyushiyangtech.top

Go:   func (u User) String() string { return u.Name }
来源：http://iqp.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://vvw.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://cfl.yongpay.top

[G13] 判断对象类型
来源：http://hfy.ctjpmb.com

Py:   isinstance(u, User)
来源：http://par.shangyingyoupin.top

PHP:  $u instanceof User
来源：http://xnb.ywan-chungtsiang.top

JS:   u instanceof User
来源：http://btq.cqqwz.cn

TS:   u instanceof User
来源：http://mlm.zhiwuduotai.top

Java: u instanceof User
来源：http://vqj.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vdg.gzhubu.top

Ruby: u.is_a?(User)
来源：http://nfy.chenlongwang.top

C#:   u is User
来源：http://bwh.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://xpo.cheryme.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bwh.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://uwt.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://wye.hnqzz.top

TS:   type User = { name: string; age: number };
来源：http://cxx.andypj.xyz

Java: record User(String name, int age) {}
来源：http://jyr.sxryk.cn

Go:   type User struct { Name string; Age int }
来源：http://ysd.birdmap.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://urh.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://ycu.yfazqb.com

[G15] 枚举
来源：http://uww.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rgw.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://spa.zdbjq.cn


<!-- 参考信息 -->