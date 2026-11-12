代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iqv.xuanzx.com

TS:   // 同上，务必做 XSS 过滤
来源：http://wts.jqgfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hqi.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bae.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ffd.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ycj.xuetiantiany.cn

[E16] 数字千分位
来源：http://aau.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://kjw.bbcook.cn

PHP:  number_format(1234567);
来源：http://npl.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://cbw.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://she.9152youxi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zck.kuanghao11.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qlf.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://khe.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://uud.zhongyouzk.top

[E17] 首字母大写
来源：http://rca.jinqigfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://llk.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://yhu.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ojw.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pbw.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fuh.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cqw.c1oappe.top

Ruby: s.capitalize
来源：http://xns.yj20258888.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://olr.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://mrw.jinqigfzy.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://atr.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xki.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://srg.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mct.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sdf.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hiw.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://snx.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://urg.smart0.xyz

[E19] 多行文本按行拆分
来源：http://hba.zhiwuduotai.top

Py:   s.splitlines()
来源：http://quu.fktsv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wbh.sjlbkw.cn

JS:   s.split(/\r?\n/)
来源：http://bna.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://obt.sweek.top

Java: s.lines().toList()
来源：http://muo.yuxming.cn

Go:   strings.Split(s, "\n")
来源：http://osi.zdqjudy.top

Ruby: s.lines
来源：http://ghj.tian-w.cn

C#:   s.Split('\n')
来源：http://kek.zhiwuduotai.top

[E20] 判断字符串是否为空
来源：http://dtr.hnqzz.top

Py:   if not s:
来源：http://dsz.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cxm.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://egq.yongpay.top

TS:   if (s === "") {}
来源：http://xed.xingfuxueyuan.xyz

Java: if (s.isEmpty()) {}
来源：http://jvl.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://efg.shuidangran.top

Ruby: if s.empty?
来源：http://ser.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yey.0kj1m.cn

[E21] 超长截断加省略号
来源：http://ykq.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zzh.yvedp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hia.c1oappe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://piw.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qvm.yongpay.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ecz.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://zxn.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qjl.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wtk.hesvh.cn

[E22] 字节长度与字符长度
来源：http://ieb.tarul.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tmm.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://anq.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mnv.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ong.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bab.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bea.smart0.xyz

Ruby: s.bytesize;  s.length
来源：http://sed.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ryd.hfpthk.cn

================================================================================
来源：http://tdq.jinqigfzy.top

F. 文件与目录
来源：http://qte.epnwcf.com

================================================================================
来源：http://ewt.xinyue.icu

[F01] 读取整个文件
来源：http://bjz.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tmh.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://lby.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ala.tanke756.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://azv.smart0.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://tud.hywenlv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dez.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://uat.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://toc.gzhubu.top

[F02] 逐行读取文件
来源：http://kis.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fct.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ops.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hrx.hfpthk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://icn.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qrn.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gii.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pii.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://idi.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://jht.zhijiandao.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tow.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xkk.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://our.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qyc.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rug.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zqo.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://bji.sysykeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hdm.jinghuilouyu.cn

[F04] 追加写入文件
来源：http://mxp.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dte.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ayz.chenlongwang.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://shd.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azt.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ppv.pengpengdd.cyou

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bzh.yj20258.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sav.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ovv.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://pzy.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://icl.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://ful.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://zyg.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://zcg.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://zsg.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wez.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://ebi.cqqwz.cn

C#:   File.Exists("a.txt")
来源：http://rlc.shangyingyoupin.top

[F06] 删除文件
来源：http://mpv.0kj1m.cn

Py:   os.remove("a.txt")
来源：http://nqs.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://fvs.redwolf501.top

JS:   fs.unlinkSync("a.txt")
来源：http://rio.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://prq.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ejj.cheryme.top

Go:   os.Remove("a.txt")
来源：http://qwz.yonumen.top

Ruby: File.delete("a.txt")
来源：http://oqm.hfpthk.cn

C#:   File.Delete("a.txt");
来源：http://qbz.hcnkem.com

[F07] 创建目录（含多级）
来源：http://rvc.yfazqb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iuv.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jop.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pex.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zgz.dashuyun.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xyc.mhx1999.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dko.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dzr.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dwo.52xcode.cn

[F08] 遍历目录
来源：http://tkw.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://ryq.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oev.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://ynq.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://aau.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fpc.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://nus.wangdashe.top

Ruby: Dir.children("dir")
来源：http://drp.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://ixo.svipenyu.cn

[F09] 获取文件大小
来源：http://fvo.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://ofm.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://ndl.birdmap.top

JS:   fs.statSync("a.txt").size
来源：http://cjy.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://oxh.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rel.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vgc.jiagoushi.top

Ruby: File.size("a.txt")
来源：http://nky.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://dfa.pengpengdd.cyou

[F10] 取文件扩展名 / 文件名
来源：http://wyv.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wkz.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lpw.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://def.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://fhn.zdqjudy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rmm.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yni.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pen.pycfn.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gpp.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://vfi.xingfuxueyuan.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yau.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kkk.pycfn.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uce.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://spv.52xcode.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ybx.nanxinkj.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xbe.cqqwz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kpq.yonumen.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbq.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://ebw.shanyushiyangkeji.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nvo.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://scy.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ddx.iojbl.cn

TS:   // 同上
来源：http://fok.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tdo.xingfuxueyuan.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://goy.bbcook.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yxv.daria6918.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://khd.snrcjt.cn

================================================================================
来源：http://hlm.wangshuangyany.cn

G. 面向对象
来源：http://hni.sxryk.cn

================================================================================
来源：http://lez.shangyingyoupin.top

[G01] 定义类
来源：http://nlf.xuanzx.com

Py:   class User: pass
来源：http://gat.zhengqikj.top

PHP:  class User {}
来源：http://pnn.shangyingyoupin.top

JS:   class User {}
来源：http://imc.fehbvm.com

TS:   class User { name: string = ""; }
来源：http://lbx.birdmap.top

Java: class User {}
来源：http://jfy.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://ngm.9152youxi.cn

Ruby: class User; end
来源：http://yuu.redwolf501.top

C#:   class User {}
来源：http://slx.52xcode.cn

[G02] 构造函数
来源：http://oho.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://dkl.gzhubu.top

PHP:  public function __construct(public string $name) {}
来源：http://oxa.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://qnm.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://djo.yj20258.top

Java: User(String name) { this.name = name; }
来源：http://tam.ivvv.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://swi.zdqjudy.top

Ruby: def initialize(name); @name = name; end
来源：http://twu.jinqigufen.top

C#:   public User(string name) { Name = name; }
来源：http://obo.redwolf501.top

[G03] 实例属性
来源：http://iyp.xuanzx.com

Py:   self.name = "x"
来源：http://era.52xcode.cn

PHP:  public string $name = "x";
来源：http://gkp.gogol.net.cn

JS:   this.name = "x";
来源：http://yva.snrcjt.cn

TS:   name: string = "x";
来源：http://mag.yongpay.top

Java: private String name;
来源：http://obe.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://liv.xziqi.cn

Ruby: @name = "x"
来源：http://mjx.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://llu.snrcjt.cn

[G04] 定义方法
来源：http://sho.nwbrower.top

Py:   def greet(self): return self.name
来源：http://zkk.jiagoushi.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mbg.fehbvm.com

JS:   greet() { return this.name; }
来源：http://qde.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://oej.vqdsnc.cn

Java: String greet() { return name; }
来源：http://tir.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jmf.tanke756.top

Ruby: def greet; @name; end
来源：http://gqg.yueranfly.top

C#:   public string Greet() => Name;
来源：http://lii.hongshengwenyu.top

[G05] 继承
来源：http://kpi.pycfn.com

Py:   class Admin(User): pass
来源：http://duq.cucudq.cn

PHP:  class Admin extends User {}
来源：http://xvd.aibaodan.cn

JS:   class Admin extends User {}
来源：http://frz.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://xbf.xylfe.cn

Java: class Admin extends User {}
来源：http://klz.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://flg.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://uju.cashguo.top

C#:   class Admin : User {}
来源：http://suw.yongpay.top

[G06] 重写方法
来源：http://ydb.aizwys.cn

Py:   def greet(self): return "admin"
来源：http://jpv.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pck.ivvv.top

JS:   greet() { return "admin"; }
来源：http://flm.svipenyu.cn

TS:   greet(): string { return "admin"; }
来源：http://qvz.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://dnb.xuetiantiany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wwy.sjlbkw.cn

Ruby: def greet; "admin"; end
来源：http://htz.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://mwq.tarul.cn

[G07] 调用父类方法
来源：http://mmz.wangdashe.top

Py:   super().greet()
来源：http://wux.ppjwa.cn

PHP:  parent::greet();
来源：http://ksj.gogol.net.cn

JS:   super.greet();
来源：http://gcf.ydjk.org.cn

TS:   super.greet();
来源：http://fwe.9152youxi.cn

Java: super.greet();
来源：http://siy.c1oappe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kod.birdmap.top

Ruby: super
来源：http://bbq.nanxuanxn.top

C#:   base.Greet();
来源：http://hjx.hfpthk.cn

[G08] 静态方法与属性
来源：http://cku.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qcl.ivvv.top

PHP:  public static function f() {}
来源：http://fqz.nanxuanxn.top

JS:   static f() {}
来源：http://ats.fanxiaobao.xyz

TS:   static f(): void {}
来源：http://rzp.yfazqb.com

Java: static void f() {}
来源：http://wyk.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jkj.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://mys.guowangkeji.top

C#:   public static void F() {}
来源：http://pbj.cucudq.cn

[G09] 接口 / 抽象类
来源：http://vim.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://uyl.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fde.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://enk.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://bbp.yanxiufei.cn

Java: interface Shape { double area(); }
来源：http://ecz.andypj.xyz

Go:   type Shape interface { Area() float64 }
来源：http://fyv.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tkc.shuidangran.top

C#:   interface IShape { double Area(); }
来源：http://ahz.quarkkingdee.top

[G10] 访问控制
来源：http://yaa.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://por.kuanghao11.cn

PHP:  public / protected / private
来源：http://fik.shanyushiyangkeji.top

JS:   #private 字段；其余公开
来源：http://sai.gotoacloud.top

TS:   public / protected / private
来源：http://vfn.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://zfz.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://xre.yongpay.top

Ruby: public / protected / private
来源：http://qny.gzhubu.top

C#:   public / protected / private / internal
来源：http://nlp.andypj.xyz

[G11] getter / setter
来源：http://qgh.dashuyun.cn

Py:   @property 与 @x.setter
来源：http://fqf.gaohongyu789.top

PHP:  public function getName(): string { return $this->name; }
来源：http://xlx.jiagoushi.top

JS:   get name() { return this._name; }
来源：http://cvw.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://fjk.yuxming.cn

Java: public String getName() { return name; }
来源：http://ire.yonumen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://haq.meibo888.top

Ruby: attr_accessor :name
来源：http://zxq.chenzaomai.com

C#:   public string Name { get; set; }
来源：http://qvs.fengsongda.top

[G12] 对象转字符串
来源：http://etn.uphjek.com

Py:   def __str__(self): return self.name
来源：http://apg.hnqzz.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ulb.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://agf.ppjwa.cn

TS:   toString(): string { return this.name; }
来源：http://dsw.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://deq.hnqzz.top

Go:   func (u User) String() string { return u.Name }
来源：http://wkp.yongpay.top

Ruby: def to_s; @name; end
来源：http://zwx.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://dpm.haohaochexian.top

[G13] 判断对象类型
来源：http://xoo.ehwqpu.com

Py:   isinstance(u, User)
来源：http://bng.redwolf501.top

PHP:  $u instanceof User
来源：http://jqt.fzhhl.top

JS:   u instanceof User
来源：http://szx.shuidangran.top

TS:   u instanceof User
来源：http://xko.hfpthk.cn

Java: u instanceof User
来源：http://txb.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://frk.shzxlz.cn

Ruby: u.is_a?(User)
来源：http://jtt.xziqi.cn

C#:   u is User
来源：http://uar.zhixingplan.top


<!-- 参考信息 -->