代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ryx.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iiz.zhixingplan.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rhu.guannengcc.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gxa.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gob.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yaf.hcnkem.com

[E16] 数字千分位
来源：http://vyk.birdmap.top

Py:   f"{1234567:,}"
来源：http://cfo.jinqigfzy.top

PHP:  number_format(1234567);
来源：http://sqw.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rmh.feifeiyinyue.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hqo.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jjy.chenzaomai.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zti.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tck.zhijiandao.cn

C#:   1234567.ToString("N0")
来源：http://scz.hongshengwenyu.top

[E17] 首字母大写
来源：http://byz.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pnf.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lnd.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hsy.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xkm.sweek.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://crz.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fpk.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://asc.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mdo.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://mgi.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hdp.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsc.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://eji.zhoulong.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://fco.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yem.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://egy.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jhn.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cry.bbcook.cn

[E19] 多行文本按行拆分
来源：http://oab.dashuyun.cn

Py:   s.splitlines()
来源：http://sjm.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dlc.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://ovy.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://bhz.tian-w.cn

Java: s.lines().toList()
来源：http://wvd.tian-w.cn

Go:   strings.Split(s, "\n")
来源：http://nca.hnxiangtu.top

Ruby: s.lines
来源：http://gah.haohaochexian.top

C#:   s.Split('\n')
来源：http://okk.bbcook.cn

[E20] 判断字符串是否为空
来源：http://njo.cdnleiting.top

Py:   if not s:
来源：http://vhn.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rfa.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ewr.jiagoushi.top

TS:   if (s === "") {}
来源：http://heq.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://gac.sufxvd.cn

Go:   if s == "" {}
来源：http://avu.dashuyun.cn

Ruby: if s.empty?
来源：http://urw.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tir.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://zad.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uwb.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rjb.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://laq.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yze.yueranfly.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jnw.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://ewc.chenzaomai.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://evg.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dgl.yueranfly.top

[E22] 字节长度与字符长度
来源：http://sgj.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lij.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fow.fengsongda.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jxp.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gcp.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kav.hnqzz.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ryc.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://aew.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://beo.zycfv.cn

================================================================================
来源：http://paw.sweek.top

F. 文件与目录
来源：http://hkc.xuetiantiany.cn

================================================================================
来源：http://vvl.nanxinkj.top

[F01] 读取整个文件
来源：http://mpn.ivvv.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jki.dianchejie.cn

PHP:  file_get_contents("a.txt");
来源：http://hhw.zycfv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fgd.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://god.zdqjudy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nly.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xla.jinghuilouyu.cn

Ruby: File.read("a.txt")
来源：http://vch.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://qgp.hcnkem.com

[F02] 逐行读取文件
来源：http://jwn.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mau.c1oappe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aqc.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hqn.pengpengdd.cyou

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://huw.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwq.hysaishi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://thy.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nlx.hnqzz.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dqg.sweek.top

[F03] 写入文件（覆盖）
来源：http://mqj.chenlongwang.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jlb.xylfe.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zfm.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://isn.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zfv.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qin.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tdk.tarul.cn

Ruby: File.write("a.txt", "hi")
来源：http://fch.yongpay.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://frm.kuanghao11.cn

[F04] 追加写入文件
来源：http://pjq.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vnn.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mhn.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mfq.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pmb.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://buh.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tev.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zqi.yongpay.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jbw.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://yyp.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tgl.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://hnu.hnqzz.top

JS:   fs.existsSync("a.txt")
来源：http://cxb.aibaodan.cn

TS:   fs.existsSync("a.txt")
来源：http://ccp.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qlw.wangdashe.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xnd.zdbjq.cn

Ruby: File.exist?("a.txt")
来源：http://fjw.yonumen.top

C#:   File.Exists("a.txt")
来源：http://hxf.quarkkingdee.top

[F06] 删除文件
来源：http://xdp.ywan-chungtsiang.top

Py:   os.remove("a.txt")
来源：http://jnk.guowangkeji.top

PHP:  unlink("a.txt");
来源：http://mig.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ddh.redwolf501.top

TS:   fs.unlinkSync("a.txt")
来源：http://ozq.cqqwz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uap.sufxvd.cn

Go:   os.Remove("a.txt")
来源：http://llc.hcnkem.com

Ruby: File.delete("a.txt")
来源：http://wuy.zhijiandao.cn

C#:   File.Delete("a.txt");
来源：http://vpk.gaohongyu789.top

[F07] 创建目录（含多级）
来源：http://nox.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://krd.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pot.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwk.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mil.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sal.chenlongwang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xxa.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pbs.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://noa.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://gmt.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://rde.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eun.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://exc.jinqigufen.top

TS:   fs.readdirSync("dir")
来源：http://bdr.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://isb.jyoumei.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yio.hongshengwenyu.top

Ruby: Dir.children("dir")
来源：http://ith.shangyingyoupin.top

C#:   Directory.GetFiles("dir")
来源：http://tlz.chenjidiqi.icu

[F09] 获取文件大小
来源：http://exo.aibaodan.cn

Py:   os.path.getsize("a.txt")
来源：http://twd.birdmap.top

PHP:  filesize("a.txt");
来源：http://udo.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://jld.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://mrc.jianghu66.top

Java: Files.size(Path.of("a.txt"))
来源：http://gfg.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cgt.daxiang520.top

Ruby: File.size("a.txt")
来源：http://czr.snrcjt.cn

C#:   new FileInfo("a.txt").Length
来源：http://jen.bbcook.cn

[F10] 取文件扩展名 / 文件名
来源：http://trm.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kbv.fktsv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wyd.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://juf.vqdsnc.cn

TS:   path.extname("a.txt")
来源：http://min.ydjk.org.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vch.cdnleiting.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aws.yuanzhike.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xga.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rdd.cdnleiting.top

[F11] 复制与移动文件
来源：http://jud.tanke756.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zbu.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vrd.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ztw.vqdsnc.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uvg.pycfn.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ixv.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lag.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dkh.daria6918.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xov.ydzc1.top

[F12] CSV 读写
来源：http://miz.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tza.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lgy.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vcv.zhoulong.xyz

TS:   // 同上
来源：http://usz.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oef.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://poo.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zgg.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vga.ydzc1.top

================================================================================
来源：http://dyn.guannengcc.top

G. 面向对象
来源：http://ufb.sxryk.cn

================================================================================
来源：http://paa.cashguo.top

[G01] 定义类
来源：http://ngq.ppjwa.cn

Py:   class User: pass
来源：http://kfo.chenlongwang.top

PHP:  class User {}
来源：http://bom.jinqigufen.top

JS:   class User {}
来源：http://mgs.redwolf501.top

TS:   class User { name: string = ""; }
来源：http://xlz.smart0.xyz

Java: class User {}
来源：http://uoz.sysykeji.top

Go:   type User struct { Name string }
来源：http://sxu.pengpengdd.cyou

Ruby: class User; end
来源：http://pwi.zhongyouzk.top

C#:   class User {}
来源：http://hhc.wangdashe.top

[G02] 构造函数
来源：http://ohq.meibo888.top

Py:   def __init__(self, name): self.name = name
来源：http://xru.gogol.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://cmo.dianchejie.cn

JS:   constructor(name) { this.name = name; }
来源：http://ebt.smart0.xyz

TS:   constructor(public name: string) {}
来源：http://qnh.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://sem.zhijiandao.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blp.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://yjy.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://goj.yangfankeji.com

[G03] 实例属性
来源：http://jdr.daria6918.cn

Py:   self.name = "x"
来源：http://rdp.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://hdy.zhongyouzk.top

JS:   this.name = "x";
来源：http://tof.jiagoushi.top

TS:   name: string = "x";
来源：http://jfc.shanyushiyangtech.top

Java: private String name;
来源：http://apq.cashguo.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nod.chenzaomai.com

Ruby: @name = "x"
来源：http://glp.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://fff.zhongyouzk.top

[G04] 定义方法
来源：http://qqd.ivvv.top

Py:   def greet(self): return self.name
来源：http://ybe.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ecg.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://wri.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://qjt.shzxlz.cn

Java: String greet() { return name; }
来源：http://lgz.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dvj.guowangkeji.top

Ruby: def greet; @name; end
来源：http://axz.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://mbb.svipenyu.cn

[G05] 继承
来源：http://crp.sxryk.cn

Py:   class Admin(User): pass
来源：http://xwp.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://lgg.cucudq.cn

JS:   class Admin extends User {}
来源：http://tkp.aizwys.cn

TS:   class Admin extends User {}
来源：http://zyq.iojbl.cn

Java: class Admin extends User {}
来源：http://vzb.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cyt.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://ofs.smart0.xyz

C#:   class Admin : User {}
来源：http://yqx.fanxiaobao.xyz

[G06] 重写方法
来源：http://qhe.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://uaz.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gib.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://nnp.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://zfw.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://cdh.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dlb.yj20258.top

Ruby: def greet; "admin"; end
来源：http://qdz.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://jkn.pycfn.com

[G07] 调用父类方法
来源：http://wcu.tian-w.cn

Py:   super().greet()
来源：http://eef.dashuyun.cn

PHP:  parent::greet();
来源：http://gdr.xziqi.cn

JS:   super.greet();
来源：http://ucu.hongshengwenyu.top

TS:   super.greet();
来源：http://vok.zhongyouzk.top

Java: super.greet();
来源：http://xeo.xziqi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://asc.dianchejie.cn

Ruby: super
来源：http://muj.jinyuanbaomall.cn

C#:   base.Greet();
来源：http://kiz.tarul.cn

[G08] 静态方法与属性
来源：http://jti.zhaomingkeji.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hvv.hongshengwenyu.top

PHP:  public static function f() {}
来源：http://exs.ivvv.top

JS:   static f() {}
来源：http://efu.tian-w.cn

TS:   static f(): void {}
来源：http://quu.fanxiaobao.xyz

Java: static void f() {}
来源：http://jbx.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://gyd.svipenyu.cn

Ruby: def self.f; end
来源：http://huj.jqgufenzy.top

C#:   public static void F() {}
来源：http://yqc.yonumen.top

[G09] 接口 / 抽象类
来源：http://oxq.ydzc1.top

Py:   from abc import ABC, abstractmethod
来源：http://bji.hnxiangtu.top

PHP:  interface Shape { public function area(): float; }
来源：http://wch.yuanzhike.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://nen.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://vmp.hammf.cn

Java: interface Shape { double area(); }
来源：http://jpu.pycfn.com

Go:   type Shape interface { Area() float64 }
来源：http://czi.shuidangran.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mlx.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://lir.tanke756.top

[G10] 访问控制
来源：http://qms.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://ncx.ydzc1.top

PHP:  public / protected / private
来源：http://xky.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://inn.yuxming.cn

TS:   public / protected / private
来源：http://unc.uphjek.com

Java: public / protected / private / 默认包级
来源：http://yow.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ggn.cucudq.cn

Ruby: public / protected / private
来源：http://pue.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://ckc.yueranfly.top

[G11] getter / setter
来源：http://pyi.tian-w.cn

Py:   @property 与 @x.setter
来源：http://vxy.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bvs.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://xnu.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://lfi.yuanzhike.top

Java: public String getName() { return name; }
来源：http://tfo.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gte.redwolf501.top

Ruby: attr_accessor :name
来源：http://veo.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://zux.ivvv.top

[G12] 对象转字符串
来源：http://yxw.yfazqb.com

Py:   def __str__(self): return self.name
来源：http://wkr.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://qgd.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://hve.52xcode.cn

TS:   toString(): string { return this.name; }
来源：http://loo.andypj.xyz

Java: @Override public String toString() { return name; }
来源：http://bcd.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zli.yj202588.top

Ruby: def to_s; @name; end
来源：http://aoa.52xcode.cn

C#:   public override string ToString() => Name;
来源：http://pns.gzhubu.top

[G13] 判断对象类型
来源：http://onb.tanke756.top

Py:   isinstance(u, User)
来源：http://llg.cdnleiting.top

PHP:  $u instanceof User
来源：http://onx.zhoulong.xyz

JS:   u instanceof User
来源：http://tka.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://tyy.gaohongyu789.top

Java: u instanceof User
来源：http://zal.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wdo.hesvh.cn

Ruby: u.is_a?(User)
来源：http://trh.sufxvd.cn

C#:   u is User
来源：http://vpe.tanke756.top


<!-- 参考信息 -->