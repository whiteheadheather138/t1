代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hyy.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://luc.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://rmr.pycfn.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mlr.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nvx.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nvj.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tcw.hywenlv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ziq.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://asl.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ytb.feifeiyinyue.top

[E16] 数字千分位
来源：http://uoi.wangdashe.top

Py:   f"{1234567:,}"
来源：http://xnv.zdbjq.cn

PHP:  number_format(1234567);
来源：http://pzx.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jel.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://gce.ivvv.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://asi.shanyushiyangtech.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yge.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://efs.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://mbn.bbcook.cn

[E17] 首字母大写
来源：http://uto.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ogn.zhoulong.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://blp.ywan-chungtsiang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://utk.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cof.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://umq.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yji.pycfn.com

Ruby: s.capitalize
来源：http://qbi.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vjk.svipenyu.cn

[E18] 模板占位符替换
来源：http://zsu.andypj.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wvl.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oyx.meibo888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kdz.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kwn.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bsm.zycfv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://svh.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hta.redwolf501.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vag.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://try.sweek.top

Py:   s.splitlines()
来源：http://nqr.nwbrower.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ewt.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://rqu.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://pbn.zhaomingkeji.xyz

Java: s.lines().toList()
来源：http://tnh.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://xlz.uphjek.com

Ruby: s.lines
来源：http://jcc.hywenlv.cn

C#:   s.Split('\n')
来源：http://khy.shangyingyoupin.top

[E20] 判断字符串是否为空
来源：http://yhx.yangfankeji.com

Py:   if not s:
来源：http://yuw.sysykeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bgg.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gfj.zdqjudy.top

TS:   if (s === "") {}
来源：http://bwh.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://hcg.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://ydi.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://jrz.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yni.vehdjk.com

[E21] 超长截断加省略号
来源：http://epe.gzhubu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vlu.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tzx.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jkl.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vzp.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lze.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://fch.wangshuangyany.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mhu.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://omv.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://mow.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://okb.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://clb.ydjk.org.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nmm.chenzaomai.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://typ.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jyq.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kqs.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://sxh.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pim.havefunace.top

================================================================================
来源：http://xhs.yj20258.top

F. 文件与目录
来源：http://zse.meibo888.top

================================================================================
来源：http://lhf.yuxming.cn

[F01] 读取整个文件
来源：http://mlq.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ppl.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://jnn.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://soo.zhiwuduotai.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbq.zhijiandao.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oas.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xnc.shangyingyoupin.top

Ruby: File.read("a.txt")
来源：http://vnr.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://rgo.fzhhl.top

[F02] 逐行读取文件
来源：http://jfo.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yyb.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wzh.shanyushiyangtech.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rxr.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jmh.snrcjt.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xlu.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dvg.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xyh.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ivi.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://rhd.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bfx.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xqy.cashguo.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qlf.52xcode.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xch.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pre.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mir.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://spu.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://joy.yvedp.cn

[F04] 追加写入文件
来源：http://hag.bbcook.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tfl.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uwi.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://grk.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hai.smart0.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ayn.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bel.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://slt.nanxinkj.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ksl.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://bcv.zhaomingkeji.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ikn.redwolf501.top

PHP:  file_exists("a.txt");
来源：http://hnu.ivvv.top

JS:   fs.existsSync("a.txt")
来源：http://pqp.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://ilq.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://icl.jinyuanbaomall.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ver.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://zwp.daria6918.cn

C#:   File.Exists("a.txt")
来源：http://xwa.cdnleiting.top

[F06] 删除文件
来源：http://nbc.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://qax.cashguo.top

PHP:  unlink("a.txt");
来源：http://nub.jinqigufen.top

JS:   fs.unlinkSync("a.txt")
来源：http://dot.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://klq.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://amy.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://sor.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://mgq.uphjek.com

C#:   File.Delete("a.txt");
来源：http://imq.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://oip.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vob.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ukk.yuanzhike.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sqv.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aku.daria6918.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://scj.yj20258888.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://edo.chenjidiqi.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dut.aibaodan.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fdu.bbcook.cn

[F08] 遍历目录
来源：http://bsd.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jek.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ncg.ehwqpu.com

JS:   fs.readdirSync("dir")
来源：http://lkw.cheryme.top

TS:   fs.readdirSync("dir")
来源：http://liz.jqgufenzy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dfa.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://rvq.zhiwuduotai.top

Ruby: Dir.children("dir")
来源：http://iai.yuxming.cn

C#:   Directory.GetFiles("dir")
来源：http://ssx.pengpengdd.cyou

[F09] 获取文件大小
来源：http://rtg.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://gdo.hesvh.cn

PHP:  filesize("a.txt");
来源：http://dku.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://lhq.wangdashe.top

TS:   fs.statSync("a.txt").size
来源：http://bsb.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://avf.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kle.zhoulong.xyz

Ruby: File.size("a.txt")
来源：http://cnd.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://grp.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://cnh.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jdy.hnxiangtu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pwn.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://slf.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://frj.vqdsnc.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vom.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bdm.hammf.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xmg.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://euu.zycfv.cn

[F11] 复制与移动文件
来源：http://zvc.nanxuanxn.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ydm.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://eki.gotoacloud.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://daq.shzxlz.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ynp.mhx1999.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qhw.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xqg.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mup.feifeiyinyue.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xpy.nanxinkj.top

[F12] CSV 读写
来源：http://drg.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hfh.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qhd.hesvh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fsr.guannengcc.top

TS:   // 同上
来源：http://mat.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ulj.xuanzx.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qag.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wle.ydjk.org.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uyy.dianchejie.cn

================================================================================
来源：http://mqh.yuxming.cn

G. 面向对象
来源：http://esn.jinghuilouyu.cn

================================================================================
来源：http://dyw.gotoacloud.top

[G01] 定义类
来源：http://zqc.ctjpmb.com

Py:   class User: pass
来源：http://bfq.316326.xyz

PHP:  class User {}
来源：http://sim.zycfv.cn

JS:   class User {}
来源：http://taf.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://jve.jiagoushi.top

Java: class User {}
来源：http://ukc.gotoacloud.top

Go:   type User struct { Name string }
来源：http://qbp.epnwcf.com

Ruby: class User; end
来源：http://dwb.cheryme.top

C#:   class User {}
来源：http://gmt.shuidangran.top

[G02] 构造函数
来源：http://qoy.aibaodan.cn

Py:   def __init__(self, name): self.name = name
来源：http://npo.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://bpe.yangfankeji.com

JS:   constructor(name) { this.name = name; }
来源：http://usc.gzhubu.top

TS:   constructor(public name: string) {}
来源：http://guk.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://ufg.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kwa.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://vtt.xinyue.icu

C#:   public User(string name) { Name = name; }
来源：http://sto.vqdsnc.cn

[G03] 实例属性
来源：http://tmu.ybcxt.top

Py:   self.name = "x"
来源：http://obi.daxiang520.top

PHP:  public string $name = "x";
来源：http://anz.yueranfly.top

JS:   this.name = "x";
来源：http://ecz.nwbrower.top

TS:   name: string = "x";
来源：http://odg.fktsv.cn

Java: private String name;
来源：http://kqh.chenzaomai.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ehj.havefunace.top

Ruby: @name = "x"
来源：http://zzz.fanxiaobao.xyz

C#:   public string Name { get; set; } = "x";
来源：http://wwq.pengpengdd.cyou

[G04] 定义方法
来源：http://ibe.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://ogt.yonumen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lvd.shzxlz.cn

JS:   greet() { return this.name; }
来源：http://zqx.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://fxd.xuanzx.com

Java: String greet() { return name; }
来源：http://uhi.cucudq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zzx.havefunace.top

Ruby: def greet; @name; end
来源：http://vmo.tanke756.top

C#:   public string Greet() => Name;
来源：http://koz.hywenlv.cn

[G05] 继承
来源：http://ylr.sufxvd.cn

Py:   class Admin(User): pass
来源：http://fqs.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://icy.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://uyj.smart0.xyz

TS:   class Admin extends User {}
来源：http://nuk.jlsjyb.cn

Java: class Admin extends User {}
来源：http://hze.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rry.epnwcf.com

Ruby: class Admin < User; end
来源：http://rmx.aizwys.cn

C#:   class Admin : User {}
来源：http://iwn.ctjpmb.com

[G06] 重写方法
来源：http://atm.fzhhl.top

Py:   def greet(self): return "admin"
来源：http://nlk.vqdsnc.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bme.xuanzx.com

JS:   greet() { return "admin"; }
来源：http://exd.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://cng.zhijiandao.cn

Java: @Override String greet() { return "admin"; }
来源：http://zze.jiagoushi.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kwi.chenzaomai.com

Ruby: def greet; "admin"; end
来源：http://irk.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://owl.pengpengdd.cyou

[G07] 调用父类方法
来源：http://xgh.xuetiantiany.cn

Py:   super().greet()
来源：http://ngs.sufxvd.cn

PHP:  parent::greet();
来源：http://wux.dianchejie.cn

JS:   super.greet();
来源：http://ajk.yanxiufei.cn

TS:   super.greet();
来源：http://vuy.hcnkem.com

Java: super.greet();
来源：http://jru.yj202588.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uas.hywenlv.cn

Ruby: super
来源：http://vlx.hnxiangtu.top

C#:   base.Greet();
来源：http://mvf.cqqwz.cn

[G08] 静态方法与属性
来源：http://usu.haohaochexian.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ouj.zhoulong.xyz

PHP:  public static function f() {}
来源：http://zvn.sxryk.cn

JS:   static f() {}
来源：http://pob.jqgfzy.top

TS:   static f(): void {}
来源：http://gmp.zhixingplan.top

Java: static void f() {}
来源：http://ccj.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zxd.chenzaomai.com

Ruby: def self.f; end
来源：http://vrr.yanxiufei.cn

C#:   public static void F() {}
来源：http://pfe.havefunace.top

[G09] 接口 / 抽象类
来源：http://fwk.yj202588.top

Py:   from abc import ABC, abstractmethod
来源：http://por.0kj1m.cn

PHP:  interface Shape { public function area(): float; }
来源：http://siy.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ram.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://usk.yj20258.top

Java: interface Shape { double area(); }
来源：http://cad.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://cti.sjlbkw.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jod.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://yam.zhijiandao.cn

[G10] 访问控制
来源：http://kso.gaohongyu789.top

Py:   约定 _protected / __private（不强制）
来源：http://ixi.haohaochexian.top

PHP:  public / protected / private
来源：http://lah.xinyue.icu

JS:   #private 字段；其余公开
来源：http://ztm.kuanghao11.cn

TS:   public / protected / private
来源：http://frd.chenjidiqi.icu

Java: public / protected / private / 默认包级
来源：http://nfy.cdnleiting.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ebx.hammf.cn

Ruby: public / protected / private
来源：http://gcq.yvedp.cn

C#:   public / protected / private / internal
来源：http://pvp.gaohongyu789.top

[G11] getter / setter
来源：http://kyy.zhengqikj.top

Py:   @property 与 @x.setter
来源：http://fml.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://grj.cucudq.cn

JS:   get name() { return this._name; }
来源：http://opr.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://jbh.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://xya.cqqwz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pep.yfazqb.com

Ruby: attr_accessor :name
来源：http://fhx.vqdsnc.cn

C#:   public string Name { get; set; }
来源：http://pwq.zhongyouzk.top

[G12] 对象转字符串
来源：http://lsq.hammf.cn

Py:   def __str__(self): return self.name
来源：http://fvv.iojbl.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gxj.fengsongda.top

JS:   toString() { return this.name; }
来源：http://enq.svipenyu.cn

TS:   toString(): string { return this.name; }
来源：http://bqz.zhaomingkeji.xyz

Java: @Override public String toString() { return name; }
来源：http://rxb.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://rpa.yonumen.top

Ruby: def to_s; @name; end
来源：http://zcu.redwolf501.top

C#:   public override string ToString() => Name;
来源：http://jks.feifeiyinyue.top

[G13] 判断对象类型
来源：http://rlx.feifeiyinyue.top

Py:   isinstance(u, User)
来源：http://ycx.shuidangran.top

PHP:  $u instanceof User
来源：http://xxr.guannengcc.top

JS:   u instanceof User
来源：http://ivj.ehwqpu.com

TS:   u instanceof User
来源：http://ype.zdqjudy.top


<!-- 参考信息 -->