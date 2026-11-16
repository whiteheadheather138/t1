代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://plg.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dnd.xuetiantiany.cn

[E16] 数字千分位
来源：http://lei.epnwcf.com

Py:   f"{1234567:,}"
来源：http://vzj.tarul.cn

PHP:  number_format(1234567);
来源：http://ddj.yfazqb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://rus.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ymi.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mko.meibo888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://poa.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hxe.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://gau.shanyushiyangtech.top

[E17] 首字母大写
来源：http://fis.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gma.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ffk.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ipm.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iey.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ppd.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iuy.ybcxt.top

Ruby: s.capitalize
来源：http://vgy.ydzc1.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hyc.ehwqpu.com

[E18] 模板占位符替换
来源：http://jqc.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ruj.andypj.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jjr.jinqigufen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mzj.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://lnt.0kj1m.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jmr.snrcjt.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://etl.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bws.c1oappe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sxi.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://vuw.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://dpt.jinqigufen.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://irr.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://nze.cucudq.cn

TS:   s.split(/\r?\n/)
来源：http://stz.xingfuxueyuan.xyz

Java: s.lines().toList()
来源：http://clr.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://ezk.ywan-chungtsiang.top

Ruby: s.lines
来源：http://lzw.mhx1999.top

C#:   s.Split('\n')
来源：http://gnj.dashuyun.cn

[E20] 判断字符串是否为空
来源：http://heg.daria6918.cn

Py:   if not s:
来源：http://iuk.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://scw.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pfc.chenlongwang.top

TS:   if (s === "") {}
来源：http://dvi.zhijiandao.cn

Java: if (s.isEmpty()) {}
来源：http://adp.bjfxy.top

Go:   if s == "" {}
来源：http://tll.ivvv.top

Ruby: if s.empty?
来源：http://yol.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ief.fehbvm.com

[E21] 超长截断加省略号
来源：http://bsy.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mgh.guannengcc.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mcp.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cux.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://egj.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://omt.zhongyouzk.top

Go:   // 按 rune 判断长度后截断
来源：http://eqp.jlsjyb.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xep.zhoulong.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mbc.gzhubu.top

[E22] 字节长度与字符长度
来源：http://nwc.hesvh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dww.hongshengwenyu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lse.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://paw.chenjidiqi.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzj.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rtb.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tjk.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://ukn.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://emj.yonumen.top

================================================================================
来源：http://qcz.zhoulong.xyz

F. 文件与目录
来源：http://scf.hcnkem.com

================================================================================
来源：http://pdj.wangdashe.top

[F01] 读取整个文件
来源：http://ivv.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aeb.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://lzv.yuxming.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xft.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lhb.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kuh.hcnkem.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vaf.yj20258888.top

Ruby: File.read("a.txt")
来源：http://cxq.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://yxe.fengsongda.top

[F02] 逐行读取文件
来源：http://dkt.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blu.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://npz.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qin.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxh.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dwm.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hpo.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oob.meibo888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ywv.yj202588.top

[F03] 写入文件（覆盖）
来源：http://mmg.tianlin.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://grt.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nei.jyoumei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qwp.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rcf.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nan.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pqb.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://jpy.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tmo.fehbvm.com

[F04] 追加写入文件
来源：http://buw.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dzq.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ctz.jinghuilouyu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nxy.ydzc1.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nlr.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qhl.aizwys.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rky.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://opy.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gao.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://hfx.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://irq.guowangkeji.top

PHP:  file_exists("a.txt");
来源：http://cid.yuxming.cn

JS:   fs.existsSync("a.txt")
来源：http://sjs.sxryk.cn

TS:   fs.existsSync("a.txt")
来源：http://gha.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fcl.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wht.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://onx.uphjek.com

C#:   File.Exists("a.txt")
来源：http://box.xziqi.cn

[F06] 删除文件
来源：http://uap.yvedp.cn

Py:   os.remove("a.txt")
来源：http://xzo.tarul.cn

PHP:  unlink("a.txt");
来源：http://oge.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mcy.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mvl.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://agj.nanxinkj.top

Go:   os.Remove("a.txt")
来源：http://bko.hammf.cn

Ruby: File.delete("a.txt")
来源：http://rlq.xylfe.cn

C#:   File.Delete("a.txt");
来源：http://tfb.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://ydz.c1oappe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tjm.ydzc1.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://thf.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zrk.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ooc.hfpthk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nha.gaohongyu789.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://msn.hongshengwenyu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tfk.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uvc.dianchejie.cn

[F08] 遍历目录
来源：http://kci.wangshuangyany.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mvu.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bbw.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://pgp.hcnkem.com

TS:   fs.readdirSync("dir")
来源：http://ldh.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bfz.yfazqb.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://aer.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://yfl.ydjk.org.cn

C#:   Directory.GetFiles("dir")
来源：http://xml.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://aaj.jinqigfzy.top

Py:   os.path.getsize("a.txt")
来源：http://ysa.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://uac.vehdjk.com

JS:   fs.statSync("a.txt").size
来源：http://kar.xingfuxueyuan.xyz

TS:   fs.statSync("a.txt").size
来源：http://rai.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://uyd.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bex.fehbvm.com

Ruby: File.size("a.txt")
来源：http://umc.sufxvd.cn

C#:   new FileInfo("a.txt").Length
来源：http://rxl.svipenyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ezu.jinqigfzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hoz.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hmb.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xxp.fktsv.cn

TS:   path.extname("a.txt")
来源：http://muz.yj20258.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://czu.hywenlv.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rmz.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fou.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jkj.sufxvd.cn

[F11] 复制与移动文件
来源：http://qzv.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oll.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nza.sjlbkw.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cir.gaohongyu789.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gvr.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dne.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vpn.svipenyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://exd.tian-w.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tqd.cheryme.top

[F12] CSV 读写
来源：http://tdz.yuanzhike.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mpf.vqdsnc.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ptn.nanxinkj.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://abq.pycfn.com

TS:   // 同上
来源：http://qmn.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hdz.zhaomingkeji.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blb.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uyp.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iaj.yueranfly.top

================================================================================
来源：http://dwa.tarul.cn

G. 面向对象
来源：http://hmp.jlsjyb.cn

================================================================================
来源：http://lqd.xuetiantiany.cn

[G01] 定义类
来源：http://awt.fengsongda.top

Py:   class User: pass
来源：http://zbs.hnqzz.top

PHP:  class User {}
来源：http://zwq.hesvh.cn

JS:   class User {}
来源：http://bpv.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://vht.hcnkem.com

Java: class User {}
来源：http://sby.yueranfly.top

Go:   type User struct { Name string }
来源：http://glp.tarul.cn

Ruby: class User; end
来源：http://uim.chenzaomai.com

C#:   class User {}
来源：http://vxq.hysaishi.cn

[G02] 构造函数
来源：http://iig.hcnkem.com

Py:   def __init__(self, name): self.name = name
来源：http://myn.yj20258888.top

PHP:  public function __construct(public string $name) {}
来源：http://mro.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://jay.jyoumei.cn

TS:   constructor(public name: string) {}
来源：http://bbs.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://jlq.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kmh.sweek.top

Ruby: def initialize(name); @name = name; end
来源：http://rsm.ybcxt.top

C#:   public User(string name) { Name = name; }
来源：http://ctv.yuanzhike.top

[G03] 实例属性
来源：http://dhg.andypj.xyz

Py:   self.name = "x"
来源：http://lnb.mhx1999.top

PHP:  public string $name = "x";
来源：http://ndm.cqqwz.cn

JS:   this.name = "x";
来源：http://gmy.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://srl.wangshuangyany.cn

Java: private String name;
来源：http://bkc.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pqn.wangshuangyany.cn

Ruby: @name = "x"
来源：http://zws.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://xnj.cucudq.cn

[G04] 定义方法
来源：http://uoh.mhx1999.top

Py:   def greet(self): return self.name
来源：http://qha.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://twy.aibaodan.cn

JS:   greet() { return this.name; }
来源：http://xeo.tarul.cn

TS:   greet(): string { return this.name; }
来源：http://rpo.shzxlz.cn

Java: String greet() { return name; }
来源：http://zdy.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rsn.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://hyi.sysykeji.top

C#:   public string Greet() => Name;
来源：http://qct.uphjek.com

[G05] 继承
来源：http://nkg.dianchejie.cn

Py:   class Admin(User): pass
来源：http://roo.iojbl.cn

PHP:  class Admin extends User {}
来源：http://zpr.316326.xyz

JS:   class Admin extends User {}
来源：http://ogo.nanxinkj.top

TS:   class Admin extends User {}
来源：http://cel.chenlongwang.top

Java: class Admin extends User {}
来源：http://kzp.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rcl.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://pgf.chenzaomai.com

C#:   class Admin : User {}
来源：http://wye.wangdashe.top

[G06] 重写方法
来源：http://efw.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://fdo.yvedp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ncu.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://lae.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://zlg.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://hqa.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yyu.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://jbu.xingfuxueyuan.xyz

C#:   public override string Greet() => "admin";
来源：http://vgf.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://ksl.zhongyouzk.top

Py:   super().greet()
来源：http://wgt.ywan-chungtsiang.top

PHP:  parent::greet();
来源：http://odv.nanxinkj.top

JS:   super.greet();
来源：http://zpj.shangyingyoupin.top

TS:   super.greet();
来源：http://gue.nanxinkj.top

Java: super.greet();
来源：http://uls.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oku.xuetiantiany.cn

Ruby: super
来源：http://ade.sweek.top

C#:   base.Greet();
来源：http://jmi.sweek.top

[G08] 静态方法与属性
来源：http://coj.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tpr.zhijiandao.cn

PHP:  public static function f() {}
来源：http://zni.aibaodan.cn

JS:   static f() {}
来源：http://ahx.jqgufenzy.top

TS:   static f(): void {}
来源：http://mea.dianchejie.cn

Java: static void f() {}
来源：http://ywg.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://zjp.zdbjq.cn

Ruby: def self.f; end
来源：http://cer.chenzaomai.com

C#:   public static void F() {}
来源：http://rwt.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://bms.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://wwc.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://upx.gaohongyu789.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mou.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://jla.yj202588.top

Java: interface Shape { double area(); }
来源：http://cah.xuetiantiany.cn

Go:   type Shape interface { Area() float64 }
来源：http://dhu.shanyushiyangkeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kod.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://htn.pycfn.com

[G10] 访问控制
来源：http://jaa.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://jem.yongpay.top

PHP:  public / protected / private
来源：http://ogc.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://avf.guowangkeji.top

TS:   public / protected / private
来源：http://hxg.meibo888.top

Java: public / protected / private / 默认包级
来源：http://keu.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qgy.ydjk.org.cn

Ruby: public / protected / private
来源：http://pcr.yfazqb.com

C#:   public / protected / private / internal
来源：http://qzo.ehwqpu.com

[G11] getter / setter
来源：http://xle.yvedp.cn

Py:   @property 与 @x.setter
来源：http://web.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://uru.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://pgj.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://snn.havefunace.top

Java: public String getName() { return name; }
来源：http://vsz.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://rie.guowangkeji.top

Ruby: attr_accessor :name
来源：http://asr.havefunace.top

C#:   public string Name { get; set; }
来源：http://zcn.jiagoushi.top

[G12] 对象转字符串
来源：http://shx.gzhubu.top

Py:   def __str__(self): return self.name
来源：http://mxd.dashuyun.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eia.tanke756.top

JS:   toString() { return this.name; }
来源：http://efb.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://lqf.jqgufenzy.top

Java: @Override public String toString() { return name; }
来源：http://ukb.mhx1999.top

Go:   func (u User) String() string { return u.Name }
来源：http://azi.pycfn.com

Ruby: def to_s; @name; end
来源：http://khl.yueranfly.top

C#:   public override string ToString() => Name;
来源：http://ouu.havefunace.top

[G13] 判断对象类型
来源：http://opu.ywan-chungtsiang.top

Py:   isinstance(u, User)
来源：http://kbv.yanxiufei.cn

PHP:  $u instanceof User
来源：http://dlg.ybcxt.top

JS:   u instanceof User
来源：http://uzy.shzxlz.cn

TS:   u instanceof User
来源：http://juo.9152youxi.cn

Java: u instanceof User
来源：http://bbs.zhaomingkeji.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://upw.52xcode.cn

Ruby: u.is_a?(User)
来源：http://koz.yuxming.cn

C#:   u is User
来源：http://qtg.dianchejie.cn

[G14] 数据类 / record
来源：http://aos.fktsv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://exi.hnxiangtu.top

PHP:  // 用 readonly 属性模拟
来源：http://twa.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qyu.zhijiandao.cn


<!-- 参考信息 -->