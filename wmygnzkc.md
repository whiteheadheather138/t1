代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wyr.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cko.c1oappe.top

Ruby: s.capitalize
来源：http://dhf.aizwys.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eha.tianlin.xyz

[E18] 模板占位符替换
来源：http://mpb.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pco.aibaodan.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://onv.52xcode.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mjj.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gkz.epnwcf.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yqk.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lcu.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://squ.meibo888.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://swj.xuetiantiany.cn

[E19] 多行文本按行拆分
来源：http://gey.yongpay.top

Py:   s.splitlines()
来源：http://sbf.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zxf.ybcxt.top

JS:   s.split(/\r?\n/)
来源：http://ksh.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://gay.fengsongda.top

Java: s.lines().toList()
来源：http://ctd.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://qkk.hywenlv.cn

Ruby: s.lines
来源：http://iqd.hcnkem.com

C#:   s.Split('\n')
来源：http://zlx.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://sqz.havefunace.top

Py:   if not s:
来源：http://ghl.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dfg.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mdi.yj202588.top

TS:   if (s === "") {}
来源：http://bxc.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://hsp.smart0.xyz

Go:   if s == "" {}
来源：http://lzc.aizwys.cn

Ruby: if s.empty?
来源：http://hry.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uuv.nwbrower.top

[E21] 超长截断加省略号
来源：http://zmm.jinyuanbaomall.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dvw.pycfn.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://roc.bjfxy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mec.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://edg.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mec.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://lbt.yj20258888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sxk.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xem.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://xvi.aizwys.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://whf.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qgq.chenlongwang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rca.gzhubu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rmc.guowangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iax.redwolf501.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wlx.yj20258.top

Ruby: s.bytesize;  s.length
来源：http://ikk.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dul.ppjwa.cn

================================================================================
来源：http://sly.svipenyu.cn

F. 文件与目录
来源：http://ufk.zdbjq.cn

================================================================================
来源：http://eik.birdmap.top

[F01] 读取整个文件
来源：http://laj.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wgt.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://rbd.jqgfzy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gnt.zycfv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uke.vehdjk.com

Java: Files.readString(Path.of("a.txt"))
来源：http://oyx.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wpj.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://tpb.jinqigufen.top

C#:   File.ReadAllText("a.txt");
来源：http://mcd.haohaochexian.top

[F02] 逐行读取文件
来源：http://etk.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rfz.hnxiangtu.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fqd.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rjc.vehdjk.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yap.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jaz.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zex.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ipn.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wsk.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://dlg.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wtj.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ufn.bjfxy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cbl.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ipq.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npw.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vbl.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://kcb.hnxiangtu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vop.yonumen.top

[F04] 追加写入文件
来源：http://mhj.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ita.meibo888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bfz.vehdjk.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ubl.ivvv.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://khh.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vpn.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iss.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gwc.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://orq.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://yoa.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xmi.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://use.tarul.cn

JS:   fs.existsSync("a.txt")
来源：http://xgn.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://vuc.fengsongda.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tgh.zhongyouzk.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tfh.zhijiandao.cn

Ruby: File.exist?("a.txt")
来源：http://kxd.xinyue.icu

C#:   File.Exists("a.txt")
来源：http://inq.dashuyun.cn

[F06] 删除文件
来源：http://wqk.jlsjyb.cn

Py:   os.remove("a.txt")
来源：http://mnn.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://knx.gotoacloud.top

JS:   fs.unlinkSync("a.txt")
来源：http://bhx.ivvv.top

TS:   fs.unlinkSync("a.txt")
来源：http://fxm.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gqt.ivvv.top

Go:   os.Remove("a.txt")
来源：http://bqo.jyoumei.cn

Ruby: File.delete("a.txt")
来源：http://kms.ctjpmb.com

C#:   File.Delete("a.txt");
来源：http://tqv.hnqzz.top

[F07] 创建目录（含多级）
来源：http://eyo.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://les.yj202588.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://awg.redwolf501.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uzb.hcnkem.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://afq.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ugd.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://npk.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uvf.shanyushiyangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fvq.nanxuanxn.top

[F08] 遍历目录
来源：http://vdt.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hve.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cbe.shuidangran.top

JS:   fs.readdirSync("dir")
来源：http://cbx.shanyushiyangtech.top

TS:   fs.readdirSync("dir")
来源：http://tpz.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jen.tianlin.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://bfb.hnxiangtu.top

Ruby: Dir.children("dir")
来源：http://afe.uphjek.com

C#:   Directory.GetFiles("dir")
来源：http://oda.snrcjt.cn

[F09] 获取文件大小
来源：http://ovo.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://ysh.wangshuangyany.cn

PHP:  filesize("a.txt");
来源：http://ovo.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://hrd.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://uky.jyoumei.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hwd.shuidangran.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kfq.quarkkingdee.top

Ruby: File.size("a.txt")
来源：http://pmt.yuxming.cn

C#:   new FileInfo("a.txt").Length
来源：http://fgi.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://mmh.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nph.yuanzhike.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zkk.zhongyouzk.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ddb.daxiang520.top

TS:   path.extname("a.txt")
来源：http://vrg.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ubx.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uao.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://piv.zhiwuduotai.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kkd.yvedp.cn

[F11] 复制与移动文件
来源：http://gyg.havefunace.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://lev.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://niw.hfpthk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fuj.hywenlv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://liy.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ytc.guowangkeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aqi.jianghu66.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://shj.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://izy.kuanghao11.cn

[F12] CSV 读写
来源：http://lui.jlsjyb.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xyr.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://atu.xingfuxueyuan.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cuf.zhengqikj.top

TS:   // 同上
来源：http://rzc.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xid.cdnleiting.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vez.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rbn.cucudq.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qsn.jqgufenzy.top

================================================================================
来源：http://rlq.316326.xyz

G. 面向对象
来源：http://vhw.shanyushiyangkeji.top

================================================================================
来源：http://rtj.daria6918.cn

[G01] 定义类
来源：http://dci.redwolf501.top

Py:   class User: pass
来源：http://idx.redwolf501.top

PHP:  class User {}
来源：http://sci.dashuyun.cn

JS:   class User {}
来源：http://fmv.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://mwa.jyoumei.cn

Java: class User {}
来源：http://shj.mhx1999.top

Go:   type User struct { Name string }
来源：http://yzt.yongpay.top

Ruby: class User; end
来源：http://buy.yj202588.top

C#:   class User {}
来源：http://vjk.hysaishi.cn

[G02] 构造函数
来源：http://qck.feifeiyinyue.top

Py:   def __init__(self, name): self.name = name
来源：http://wpn.epnwcf.com

PHP:  public function __construct(public string $name) {}
来源：http://lix.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://zdj.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://ckr.smart0.xyz

Java: User(String name) { this.name = name; }
来源：http://xog.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pez.jinqigufen.top

Ruby: def initialize(name); @name = name; end
来源：http://atz.nanxinkj.top

C#:   public User(string name) { Name = name; }
来源：http://giu.xziqi.cn

[G03] 实例属性
来源：http://fre.xziqi.cn

Py:   self.name = "x"
来源：http://xxr.hywenlv.cn

PHP:  public string $name = "x";
来源：http://ghk.guowangkeji.top

JS:   this.name = "x";
来源：http://vbk.cqqwz.cn

TS:   name: string = "x";
来源：http://kea.zhiwuduotai.top

Java: private String name;
来源：http://tnr.daria6918.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qzl.sufxvd.cn

Ruby: @name = "x"
来源：http://igr.hongshengwenyu.top

C#:   public string Name { get; set; } = "x";
来源：http://ayz.shuidangran.top

[G04] 定义方法
来源：http://oju.jinyuanbaomall.cn

Py:   def greet(self): return self.name
来源：http://mqa.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xrz.yangfankeji.com

JS:   greet() { return this.name; }
来源：http://dgc.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://vrh.shzxlz.cn

Java: String greet() { return name; }
来源：http://rxn.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xer.hywenlv.cn

Ruby: def greet; @name; end
来源：http://hjl.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://tiy.fehbvm.com

[G05] 继承
来源：http://bjq.ivvv.top

Py:   class Admin(User): pass
来源：http://stz.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://lgd.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://vml.yuanzhike.top

TS:   class Admin extends User {}
来源：http://inc.chenlongwang.top

Java: class Admin extends User {}
来源：http://ocv.wangdashe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ytj.havefunace.top

Ruby: class Admin < User; end
来源：http://fky.xuanzx.com

C#:   class Admin : User {}
来源：http://hgx.bbcook.cn

[G06] 重写方法
来源：http://sze.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://qbm.xuetiantiany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hji.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://luh.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://gkp.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://iku.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mmc.snrcjt.cn

Ruby: def greet; "admin"; end
来源：http://afu.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://rhk.fengsongda.top

[G07] 调用父类方法
来源：http://hxr.hcnkem.com

Py:   super().greet()
来源：http://jzr.hysaishi.cn

PHP:  parent::greet();
来源：http://sis.gzhubu.top

JS:   super.greet();
来源：http://vkq.jiagoushi.top

TS:   super.greet();
来源：http://svt.fzhhl.top

Java: super.greet();
来源：http://rlf.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://svl.jqgfzy.top

Ruby: super
来源：http://uto.daria6918.cn

C#:   base.Greet();
来源：http://wwj.ehwqpu.com

[G08] 静态方法与属性
来源：http://wgp.sjlbkw.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iav.dianchejie.cn

PHP:  public static function f() {}
来源：http://ezy.hammf.cn

JS:   static f() {}
来源：http://ixo.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://haq.gzhubu.top

Java: static void f() {}
来源：http://xzg.tanke756.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://twi.ivvv.top

Ruby: def self.f; end
来源：http://orn.tian-w.cn

C#:   public static void F() {}
来源：http://ubi.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://ies.aizwys.cn

Py:   from abc import ABC, abstractmethod
来源：http://flc.snrcjt.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pov.meibo888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cnn.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://ikw.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://jma.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://wpr.cucudq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bfw.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://wqn.ydjk.org.cn

[G10] 访问控制
来源：http://eha.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://wrh.gaohongyu789.top

PHP:  public / protected / private
来源：http://ctq.jianghu66.top

JS:   #private 字段；其余公开
来源：http://qfh.cqqwz.cn

TS:   public / protected / private
来源：http://ckj.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://fii.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://neu.shangyingyoupin.top

Ruby: public / protected / private
来源：http://qsx.nanxinkj.top

C#:   public / protected / private / internal
来源：http://dsk.haohaochexian.top

[G11] getter / setter
来源：http://oof.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://dna.ctjpmb.com

PHP:  public function getName(): string { return $this->name; }
来源：http://xqt.yanxiufei.cn

JS:   get name() { return this._name; }
来源：http://uan.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://ymf.aizwys.cn

Java: public String getName() { return name; }
来源：http://rzt.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://smu.andypj.xyz

Ruby: attr_accessor :name
来源：http://ohp.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://ryz.jyoumei.cn

[G12] 对象转字符串
来源：http://adn.zhixingplan.top

Py:   def __str__(self): return self.name
来源：http://siv.yonumen.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qwx.fktsv.cn

JS:   toString() { return this.name; }
来源：http://uie.xylfe.cn

TS:   toString(): string { return this.name; }
来源：http://vpq.fzhhl.top

Java: @Override public String toString() { return name; }
来源：http://rvv.sufxvd.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jtr.hnqzz.top

Ruby: def to_s; @name; end
来源：http://mng.ctjpmb.com

C#:   public override string ToString() => Name;
来源：http://ykj.jqgufenzy.top

[G13] 判断对象类型
来源：http://bzs.hcnkem.com

Py:   isinstance(u, User)
来源：http://tyx.yanxiufei.cn

PHP:  $u instanceof User
来源：http://dmj.chenjidiqi.icu

JS:   u instanceof User
来源：http://cjy.yuxming.cn

TS:   u instanceof User
来源：http://pev.xinyue.icu

Java: u instanceof User
来源：http://rsh.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qcl.316326.xyz

Ruby: u.is_a?(User)
来源：http://rss.ywan-chungtsiang.top

C#:   u is User
来源：http://zeo.jyoumei.cn

[G14] 数据类 / record
来源：http://gsg.nanxuanxn.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://txe.fanxiaobao.xyz

PHP:  // 用 readonly 属性模拟
来源：http://xvv.yvedp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://imx.hongshengwenyu.top

TS:   type User = { name: string; age: number };
来源：http://wox.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://fvk.chenjidiqi.icu

Go:   type User struct { Name string; Age int }
来源：http://bsb.snrcjt.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lqz.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://feo.xinyue.icu

[G15] 枚举
来源：http://vyc.cucudq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ehb.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ivj.sxryk.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pjj.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vwv.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://xjz.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gou.zhijiandao.cn

Ruby: Color = %i[red green].freeze
来源：http://xir.fehbvm.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suy.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://czl.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yuh.zhiwuduotai.top


<!-- 参考信息 -->