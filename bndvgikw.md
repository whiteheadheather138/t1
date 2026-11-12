代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://neb.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://mzg.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ycq.jinyuanbaomall.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tbi.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yvn.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nvt.xziqi.cn

[E16] 数字千分位
来源：http://oje.0kj1m.cn

Py:   f"{1234567:,}"
来源：http://fep.nanxinkj.top

PHP:  number_format(1234567);
来源：http://plt.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qsd.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://sgb.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wup.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ptk.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lra.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://ull.cheryme.top

[E17] 首字母大写
来源：http://glc.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://joc.zhiwuduotai.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jqa.fengsongda.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jil.meibo888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ssn.jqgufenzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fis.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qms.ppjwa.cn

Ruby: s.capitalize
来源：http://pcz.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xnu.xziqi.cn

[E18] 模板占位符替换
来源：http://tgg.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://slb.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yep.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://juc.zhijiandao.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ksl.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mfd.chenzaomai.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://usj.nanxuanxn.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vbe.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mix.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://jra.ctjpmb.com

Py:   s.splitlines()
来源：http://mth.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vte.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://wzb.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://sae.nanxinkj.top

Java: s.lines().toList()
来源：http://qdl.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://tqf.jqgufenzy.top

Ruby: s.lines
来源：http://ibj.gotoacloud.top

C#:   s.Split('\n')
来源：http://ses.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://czc.0kj1m.cn

Py:   if not s:
来源：http://jmn.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oeq.shanyushiyangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kmy.jqgfzy.top

TS:   if (s === "") {}
来源：http://zdl.shanyushiyangkeji.top

Java: if (s.isEmpty()) {}
来源：http://sng.chenlongwang.top

Go:   if s == "" {}
来源：http://zpp.gotoacloud.top

Ruby: if s.empty?
来源：http://mvp.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ihp.ybcxt.top

[E21] 超长截断加省略号
来源：http://ffc.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ixm.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://spm.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ggx.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://spi.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jbc.feifeiyinyue.top

Go:   // 按 rune 判断长度后截断
来源：http://lgt.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hnu.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wvj.zdbjq.cn

[E22] 字节长度与字符长度
来源：http://scc.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fil.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnq.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hxj.daxiang520.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ooh.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yil.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bvu.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://cka.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ccx.aizwys.cn

================================================================================
来源：http://yvx.yvedp.cn

F. 文件与目录
来源：http://eri.daria6918.cn

================================================================================
来源：http://zib.shzxlz.cn

[F01] 读取整个文件
来源：http://gpx.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vxz.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://fud.yuanzhike.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mna.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bdf.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://klz.jinghuilouyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdk.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://afz.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://vza.quarkkingdee.top

[F02] 逐行读取文件
来源：http://pur.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ohw.tianlin.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ssz.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tbm.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fih.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kik.birdmap.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ser.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kzj.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://suf.guannengcc.top

[F03] 写入文件（覆盖）
来源：http://bcy.wangshuangyany.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://peg.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vel.jinghuilouyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ill.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqo.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gso.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zyd.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://meq.hnqzz.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tsh.c1oappe.top

[F04] 追加写入文件
来源：http://pnf.chenjidiqi.icu

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mjc.vehdjk.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hnp.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uji.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kry.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dwl.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://idh.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://frx.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qcs.hfpthk.cn

[F05] 判断文件或目录是否存在
来源：http://oco.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vlq.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://icu.jinqigufen.top

JS:   fs.existsSync("a.txt")
来源：http://xla.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://pwq.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://xlk.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hfv.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://kwc.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://qat.hongshengwenyu.top

[F06] 删除文件
来源：http://cmt.zhongyouzk.top

Py:   os.remove("a.txt")
来源：http://lfy.cashguo.top

PHP:  unlink("a.txt");
来源：http://mez.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://rlo.cqqwz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dip.pycfn.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ihv.gaohongyu789.top

Go:   os.Remove("a.txt")
来源：http://qcd.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://tqj.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://hnb.ydjk.org.cn

[F07] 创建目录（含多级）
来源：http://msn.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://evj.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tje.hnxiangtu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hdn.316326.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://imo.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sjn.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://edz.tianlin.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gtq.chenlongwang.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tnc.jinqigfzy.top

[F08] 遍历目录
来源：http://epp.hnxiangtu.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nfk.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qfs.cashguo.top

JS:   fs.readdirSync("dir")
来源：http://hkp.bjfxy.top

TS:   fs.readdirSync("dir")
来源：http://edi.yj20258888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tgu.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ziq.aibaodan.cn

Ruby: Dir.children("dir")
来源：http://tbq.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://dcd.yongpay.top

[F09] 获取文件大小
来源：http://vmr.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://nos.bbcook.cn

PHP:  filesize("a.txt");
来源：http://uxj.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://izy.jinqigufen.top

TS:   fs.statSync("a.txt").size
来源：http://jbw.ivvv.top

Java: Files.size(Path.of("a.txt"))
来源：http://yax.jiagoushi.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://klm.tianlin.xyz

Ruby: File.size("a.txt")
来源：http://qmr.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://kpk.hnqzz.top

[F10] 取文件扩展名 / 文件名
来源：http://cev.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qvq.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xhu.pycfn.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wpn.shuidangran.top

TS:   path.extname("a.txt")
来源：http://lts.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jqw.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jhi.kuanghao11.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xim.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kix.yonumen.top

[F11] 复制与移动文件
来源：http://mgp.sxryk.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tav.hammf.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qpe.hesvh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wnw.bbcook.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dgu.jianghu66.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oop.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://trw.gotoacloud.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bvo.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fko.vehdjk.com

[F12] CSV 读写
来源：http://dux.fehbvm.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oim.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wbu.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jva.yueranfly.top

TS:   // 同上
来源：http://sbn.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://trc.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kod.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tbw.birdmap.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iwa.jinqigufen.top

================================================================================
来源：http://tlf.shuidangran.top

G. 面向对象
来源：http://dpg.xuetiantiany.cn

================================================================================
来源：http://syj.52xcode.cn

[G01] 定义类
来源：http://wmx.hnqzz.top

Py:   class User: pass
来源：http://mpd.wangdashe.top

PHP:  class User {}
来源：http://omw.iojbl.cn

JS:   class User {}
来源：http://dxi.svipenyu.cn

TS:   class User { name: string = ""; }
来源：http://ypf.mhx1999.top

Java: class User {}
来源：http://okn.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://vbn.hysaishi.cn

Ruby: class User; end
来源：http://sif.birdmap.top

C#:   class User {}
来源：http://uri.c1oappe.top

[G02] 构造函数
来源：http://bml.mhx1999.top

Py:   def __init__(self, name): self.name = name
来源：http://yzq.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://sjl.haohaochexian.top

JS:   constructor(name) { this.name = name; }
来源：http://sne.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://rbf.zhijiandao.cn

Java: User(String name) { this.name = name; }
来源：http://und.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gud.guannengcc.top

Ruby: def initialize(name); @name = name; end
来源：http://reg.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://eky.ydjk.org.cn

[G03] 实例属性
来源：http://kps.yueranfly.top

Py:   self.name = "x"
来源：http://rhg.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://ssm.xylfe.cn

JS:   this.name = "x";
来源：http://wzw.nanxuanxn.top

TS:   name: string = "x";
来源：http://eqx.jiagoushi.top

Java: private String name;
来源：http://lif.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fbo.jinqigufen.top

Ruby: @name = "x"
来源：http://xkk.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://oux.jlsjyb.cn

[G04] 定义方法
来源：http://ivu.cheryme.top

Py:   def greet(self): return self.name
来源：http://xbp.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tes.yj20258888.top

JS:   greet() { return this.name; }
来源：http://lvx.sysykeji.top

TS:   greet(): string { return this.name; }
来源：http://tbz.jianghu66.top

Java: String greet() { return name; }
来源：http://agk.fehbvm.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ric.fktsv.cn

Ruby: def greet; @name; end
来源：http://frg.xuetiantiany.cn

C#:   public string Greet() => Name;
来源：http://zyz.sxryk.cn

[G05] 继承
来源：http://afc.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://qsu.epnwcf.com

PHP:  class Admin extends User {}
来源：http://ufm.ppjwa.cn

JS:   class Admin extends User {}
来源：http://zhd.hysaishi.cn

TS:   class Admin extends User {}
来源：http://ifj.feifeiyinyue.top

Java: class Admin extends User {}
来源：http://jdw.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ako.52xcode.cn

Ruby: class Admin < User; end
来源：http://zvg.wangdashe.top

C#:   class Admin : User {}
来源：http://bho.bbcook.cn

[G06] 重写方法
来源：http://qeq.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://cdt.aibaodan.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ypb.pengpengdd.cyou

JS:   greet() { return "admin"; }
来源：http://aqy.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://iiw.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://vlu.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zos.vqdsnc.cn

Ruby: def greet; "admin"; end
来源：http://mhk.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://iob.yvedp.cn

[G07] 调用父类方法
来源：http://wvh.yj20258.top

Py:   super().greet()
来源：http://ydp.guannengcc.top

PHP:  parent::greet();
来源：http://eiu.dianchejie.cn

JS:   super.greet();
来源：http://exi.nanxinkj.top

TS:   super.greet();
来源：http://rdh.fktsv.cn

Java: super.greet();
来源：http://gaq.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eot.iojbl.cn

Ruby: super
来源：http://yqi.iojbl.cn

C#:   base.Greet();
来源：http://xbi.redwolf501.top

[G08] 静态方法与属性
来源：http://bts.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vxo.yongpay.top

PHP:  public static function f() {}
来源：http://wbm.jiagoushi.top

JS:   static f() {}
来源：http://rxk.jqgfzy.top

TS:   static f(): void {}
来源：http://rze.zhoulong.xyz

Java: static void f() {}
来源：http://qse.hfpthk.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://diz.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://sui.havefunace.top

C#:   public static void F() {}
来源：http://fgk.zhengqikj.top

[G09] 接口 / 抽象类
来源：http://cqh.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gui.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lsy.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://gyh.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://xjj.xziqi.cn

Java: interface Shape { double area(); }
来源：http://ddv.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://dij.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kia.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://kaf.feifeiyinyue.top

[G10] 访问控制
来源：http://xfb.nanxuanxn.top

Py:   约定 _protected / __private（不强制）
来源：http://jgh.iojbl.cn

PHP:  public / protected / private
来源：http://wqr.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://vuh.52xcode.cn

TS:   public / protected / private
来源：http://chj.tian-w.cn

Java: public / protected / private / 默认包级
来源：http://alt.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://bcy.tarul.cn

Ruby: public / protected / private
来源：http://xqh.andypj.xyz

C#:   public / protected / private / internal
来源：http://xvu.jlsjyb.cn

[G11] getter / setter
来源：http://vzh.jinqigfzy.top

Py:   @property 与 @x.setter
来源：http://vcq.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rgv.smart0.xyz

JS:   get name() { return this._name; }
来源：http://wsi.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://wgd.yangfankeji.com

Java: public String getName() { return name; }
来源：http://lgk.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aqv.c1oappe.top

Ruby: attr_accessor :name
来源：http://voq.cashguo.top

C#:   public string Name { get; set; }
来源：http://wkq.snrcjt.cn

[G12] 对象转字符串
来源：http://ant.uphjek.com

Py:   def __str__(self): return self.name
来源：http://edr.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lbv.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://hsd.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://bri.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://rzs.chenjidiqi.icu

Go:   func (u User) String() string { return u.Name }
来源：http://yew.andypj.xyz

Ruby: def to_s; @name; end
来源：http://ois.sweek.top

C#:   public override string ToString() => Name;
来源：http://wkw.chenjidiqi.icu

[G13] 判断对象类型
来源：http://mwx.daxiang520.top

Py:   isinstance(u, User)
来源：http://ztc.zhixingplan.top

PHP:  $u instanceof User
来源：http://qoj.hywenlv.cn

JS:   u instanceof User
来源：http://urj.guowangkeji.top

TS:   u instanceof User
来源：http://qpt.ydjk.org.cn

Java: u instanceof User
来源：http://buv.zhengqikj.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xox.nanxinkj.top

Ruby: u.is_a?(User)
来源：http://mpx.meibo888.top

C#:   u is User
来源：http://czd.cdnleiting.top


<!-- 参考信息 -->