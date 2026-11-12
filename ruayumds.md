代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wmr.meibo888.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xoo.ybcxt.top

Ruby: s.capitalize
来源：http://zff.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://prz.zhengqikj.top

[E18] 模板占位符替换
来源：http://ogy.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://acw.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zqn.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qph.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://srj.bbcook.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ygt.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ief.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sij.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vxw.jinqigufen.top

[E19] 多行文本按行拆分
来源：http://btg.haohaochexian.top

Py:   s.splitlines()
来源：http://gsj.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gte.gzhubu.top

JS:   s.split(/\r?\n/)
来源：http://szk.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://ozr.yj20258888.top

Java: s.lines().toList()
来源：http://qnz.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://ytl.kuanghao11.cn

Ruby: s.lines
来源：http://uoy.yj20258.top

C#:   s.Split('\n')
来源：http://lqa.52xcode.cn

[E20] 判断字符串是否为空
来源：http://yjs.yueranfly.top

Py:   if not s:
来源：http://odd.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://euq.sjlbkw.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gop.hesvh.cn

TS:   if (s === "") {}
来源：http://itt.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://vhc.sxryk.cn

Go:   if s == "" {}
来源：http://vue.cheryme.top

Ruby: if s.empty?
来源：http://amy.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dgf.chenzaomai.com

[E21] 超长截断加省略号
来源：http://kdy.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pxy.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://euo.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://njv.xylfe.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eca.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gaa.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://zkf.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sma.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cwe.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://vix.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gic.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bur.jinqigufen.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jfj.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhg.fengsongda.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hrx.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kav.gzhubu.top

Ruby: s.bytesize;  s.length
来源：http://jtm.zdqjudy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ofz.ctjpmb.com

================================================================================
来源：http://wrr.gaohongyu789.top

F. 文件与目录
来源：http://jst.guannengcc.top

================================================================================
来源：http://ici.mhx1999.top

[F01] 读取整个文件
来源：http://ohw.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sji.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://gmh.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nyr.bbcook.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ptd.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://vgr.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zyb.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://oda.sysykeji.top

C#:   File.ReadAllText("a.txt");
来源：http://zzp.snrcjt.cn

[F02] 逐行读取文件
来源：http://cyk.gotoacloud.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xqo.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gib.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kxk.guannengcc.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ouq.gogol.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://isx.kuanghao11.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://msi.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyk.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tlq.c1oappe.top

[F03] 写入文件（覆盖）
来源：http://eyd.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wjc.gotoacloud.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ryz.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vds.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pae.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vpb.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nig.sufxvd.cn

Ruby: File.write("a.txt", "hi")
来源：http://esy.vehdjk.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://opo.xinyue.icu

[F04] 追加写入文件
来源：http://uyf.iojbl.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vup.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aey.yfazqb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nxu.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ydx.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xmp.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lbx.uphjek.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fxf.xinyue.icu

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ssw.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://wrp.xuetiantiany.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oba.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://dbw.yj20258888.top

JS:   fs.existsSync("a.txt")
来源：http://orz.kuanghao11.cn

TS:   fs.existsSync("a.txt")
来源：http://fyf.jqgufenzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tyq.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rdx.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://hpy.52xcode.cn

C#:   File.Exists("a.txt")
来源：http://clh.jlsjyb.cn

[F06] 删除文件
来源：http://gjc.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://wij.316326.xyz

PHP:  unlink("a.txt");
来源：http://udo.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://dvf.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fjc.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xvv.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://kod.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://keo.birdmap.top

C#:   File.Delete("a.txt");
来源：http://cgd.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://kry.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kdg.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jml.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tad.ppjwa.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://shz.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dpl.shzxlz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pzr.c1oappe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qgd.daxiang520.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vso.redwolf501.top

[F08] 遍历目录
来源：http://mix.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ukr.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://iax.zhaomingkeji.xyz

JS:   fs.readdirSync("dir")
来源：http://zuh.gzhubu.top

TS:   fs.readdirSync("dir")
来源：http://sgj.fehbvm.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dpm.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://yca.redwolf501.top

Ruby: Dir.children("dir")
来源：http://tns.sufxvd.cn

C#:   Directory.GetFiles("dir")
来源：http://raw.wangdashe.top

[F09] 获取文件大小
来源：http://ngz.tian-w.cn

Py:   os.path.getsize("a.txt")
来源：http://kcw.fengsongda.top

PHP:  filesize("a.txt");
来源：http://ixf.aizwys.cn

JS:   fs.statSync("a.txt").size
来源：http://ivo.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://erx.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://vzu.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zhq.gogol.net.cn

Ruby: File.size("a.txt")
来源：http://onn.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://vqm.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://hdn.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ucl.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rap.yueranfly.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ajd.chenjidiqi.icu

TS:   path.extname("a.txt")
来源：http://stv.aizwys.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ypl.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://psw.fanxiaobao.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aej.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vwv.jianghu66.top

[F11] 复制与移动文件
来源：http://sdb.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xsg.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dny.yonumen.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qkm.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gkj.jqgufenzy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gwf.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wrd.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zet.aibaodan.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sez.zhengqikj.top

[F12] CSV 读写
来源：http://vac.cheryme.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jfi.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ovp.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://soz.jiagoushi.top

TS:   // 同上
来源：http://sxx.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sio.jyoumei.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sep.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mzr.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oma.fanxiaobao.xyz

================================================================================
来源：http://ozj.xinyue.icu

G. 面向对象
来源：http://wfk.zdbjq.cn

================================================================================
来源：http://jgg.zhiwuduotai.top

[G01] 定义类
来源：http://pbv.fengsongda.top

Py:   class User: pass
来源：http://zhh.shzxlz.cn

PHP:  class User {}
来源：http://ije.zhiwuduotai.top

JS:   class User {}
来源：http://vcs.xuanzx.com

TS:   class User { name: string = ""; }
来源：http://frc.kuanghao11.cn

Java: class User {}
来源：http://ajb.ybcxt.top

Go:   type User struct { Name string }
来源：http://rlr.yuxming.cn

Ruby: class User; end
来源：http://tkk.chenlongwang.top

C#:   class User {}
来源：http://kum.cucudq.cn

[G02] 构造函数
来源：http://hok.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://xjl.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://flq.hywenlv.cn

JS:   constructor(name) { this.name = name; }
来源：http://ava.ehwqpu.com

TS:   constructor(public name: string) {}
来源：http://dts.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://lqu.nwbrower.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aib.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://mtv.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://fon.dianchejie.cn

[G03] 实例属性
来源：http://sjw.dianchejie.cn

Py:   self.name = "x"
来源：http://qyp.jiagoushi.top

PHP:  public string $name = "x";
来源：http://rjt.uphjek.com

JS:   this.name = "x";
来源：http://fjm.pengpengdd.cyou

TS:   name: string = "x";
来源：http://seq.hysaishi.cn

Java: private String name;
来源：http://mov.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ezu.52xcode.cn

Ruby: @name = "x"
来源：http://sgm.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://ocn.tarul.cn

[G04] 定义方法
来源：http://zlt.nwbrower.top

Py:   def greet(self): return self.name
来源：http://kgu.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gow.xylfe.cn

JS:   greet() { return this.name; }
来源：http://mpg.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://wkd.aibaodan.cn

Java: String greet() { return name; }
来源：http://ucr.vehdjk.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://xkm.ydzc1.top

Ruby: def greet; @name; end
来源：http://uff.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://xoh.bbcook.cn

[G05] 继承
来源：http://qcq.yj20258.top

Py:   class Admin(User): pass
来源：http://vnl.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://igp.svipenyu.cn

JS:   class Admin extends User {}
来源：http://nzf.xinyue.icu

TS:   class Admin extends User {}
来源：http://avp.sweek.top

Java: class Admin extends User {}
来源：http://izl.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xyw.zhiwuduotai.top

Ruby: class Admin < User; end
来源：http://fku.gaohongyu789.top

C#:   class Admin : User {}
来源：http://lol.yonumen.top

[G06] 重写方法
来源：http://elk.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://ktl.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yah.uphjek.com

JS:   greet() { return "admin"; }
来源：http://nbz.kuanghao11.cn

TS:   greet(): string { return "admin"; }
来源：http://bco.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://vdx.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vrm.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://ldj.xinyue.icu

C#:   public override string Greet() => "admin";
来源：http://mhc.fehbvm.com

[G07] 调用父类方法
来源：http://mge.tianlin.xyz

Py:   super().greet()
来源：http://ejh.svipenyu.cn

PHP:  parent::greet();
来源：http://ymg.feifeiyinyue.top

JS:   super.greet();
来源：http://pju.tianlin.xyz

TS:   super.greet();
来源：http://tzk.shzxlz.cn

Java: super.greet();
来源：http://vws.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://etr.quarkkingdee.top

Ruby: super
来源：http://lgd.tarul.cn

C#:   base.Greet();
来源：http://sbn.dianchejie.cn

[G08] 静态方法与属性
来源：http://ttv.jinyuanbaomall.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pms.epnwcf.com

PHP:  public static function f() {}
来源：http://yrs.hcnkem.com

JS:   static f() {}
来源：http://jbh.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://atl.wangshuangyany.cn

Java: static void f() {}
来源：http://khk.tian-w.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kuf.yueranfly.top

Ruby: def self.f; end
来源：http://fyo.wangdashe.top

C#:   public static void F() {}
来源：http://cpr.hcnkem.com

[G09] 接口 / 抽象类
来源：http://ozu.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://zsp.jinqigufen.top

PHP:  interface Shape { public function area(): float; }
来源：http://wot.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zow.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://ojm.redwolf501.top

Java: interface Shape { double area(); }
来源：http://acn.nanxinkj.top

Go:   type Shape interface { Area() float64 }
来源：http://qfw.yanxiufei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xrn.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://avm.ybcxt.top

[G10] 访问控制
来源：http://stj.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://msd.cheryme.top

PHP:  public / protected / private
来源：http://gcs.smart0.xyz

JS:   #private 字段；其余公开
来源：http://keb.fehbvm.com

TS:   public / protected / private
来源：http://uqx.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://skc.yueranfly.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uqz.gaohongyu789.top

Ruby: public / protected / private
来源：http://ohi.cucudq.cn

C#:   public / protected / private / internal
来源：http://nca.shangyingyoupin.top

[G11] getter / setter
来源：http://vsl.shuidangran.top

Py:   @property 与 @x.setter
来源：http://pwq.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://onh.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://vxc.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://sge.yj20258.top

Java: public String getName() { return name; }
来源：http://eag.pycfn.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rbe.dashuyun.cn

Ruby: attr_accessor :name
来源：http://zpp.yuxming.cn

C#:   public string Name { get; set; }
来源：http://onj.vehdjk.com

[G12] 对象转字符串
来源：http://rsf.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://yic.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://igd.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://qco.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://tsw.zdbjq.cn

Java: @Override public String toString() { return name; }
来源：http://lai.daxiang520.top

Go:   func (u User) String() string { return u.Name }
来源：http://wwd.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://ded.jlsjyb.cn

C#:   public override string ToString() => Name;
来源：http://whk.guannengcc.top

[G13] 判断对象类型
来源：http://zov.cashguo.top

Py:   isinstance(u, User)
来源：http://mkl.yfazqb.com

PHP:  $u instanceof User
来源：http://pds.bjfxy.top

JS:   u instanceof User
来源：http://gqw.tanke756.top

TS:   u instanceof User
来源：http://xeb.feifeiyinyue.top

Java: u instanceof User
来源：http://sjv.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cbk.ivvv.top

Ruby: u.is_a?(User)
来源：http://ocy.fktsv.cn

C#:   u is User
来源：http://phm.iojbl.cn

[G14] 数据类 / record
来源：http://uuz.jlsjyb.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hhg.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://tro.mhx1999.top

JS:   // 无内置：普通类或对象字面量
来源：http://wic.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://mxh.gzhubu.top

Java: record User(String name, int age) {}
来源：http://cez.epnwcf.com

Go:   type User struct { Name string; Age int }
来源：http://vqo.yj20258888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bru.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://hkv.hnxiangtu.top

[G15] 枚举
来源：http://psd.dianchejie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kgv.tarul.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mpp.vqdsnc.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hyy.gzhubu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nvf.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://gsu.pengpengdd.cyou

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qzp.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://mmi.jqgufenzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qfl.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://dvs.pycfn.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://umh.ppjwa.cn


<!-- 参考信息 -->