代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xrp.jyoumei.cn

[E15] HTML 转义 / 反转义
来源：http://xrc.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bam.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rss.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mll.cqqwz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xpv.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pfz.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dhv.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ejv.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tte.havefunace.top

[E16] 数字千分位
来源：http://omi.yj20258.top

Py:   f"{1234567:,}"
来源：http://buc.guowangkeji.top

PHP:  number_format(1234567);
来源：http://xzu.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://qgb.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kyf.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cza.yj202588.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qej.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xhi.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://qqu.quarkkingdee.top

[E17] 首字母大写
来源：http://gft.zhixingplan.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jsp.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://smy.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xci.ehwqpu.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sfv.svipenyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vtm.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cuu.yuxming.cn

Ruby: s.capitalize
来源：http://wne.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bby.xylfe.cn

[E18] 模板占位符替换
来源：http://xqp.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hoc.epnwcf.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ups.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bqa.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rit.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wzh.yonumen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hro.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lys.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xav.nanxinkj.top

[E19] 多行文本按行拆分
来源：http://vtf.ybcxt.top

Py:   s.splitlines()
来源：http://bjv.nanxuanxn.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xvu.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://lkr.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://vnt.xziqi.cn

Java: s.lines().toList()
来源：http://rzj.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://uuf.chenjidiqi.icu

Ruby: s.lines
来源：http://evt.zhoulong.xyz

C#:   s.Split('\n')
来源：http://vnv.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://fjb.hysaishi.cn

Py:   if not s:
来源：http://coj.ydjk.org.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eim.cucudq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ypn.guowangkeji.top

TS:   if (s === "") {}
来源：http://ycw.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://aok.yj20258888.top

Go:   if s == "" {}
来源：http://jho.hnxiangtu.top

Ruby: if s.empty?
来源：http://tzr.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xpr.yuanzhike.top

[E21] 超长截断加省略号
来源：http://ogx.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ovf.cdnleiting.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nup.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mmv.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://csf.bbcook.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mao.wangdashe.top

Go:   // 按 rune 判断长度后截断
来源：http://omt.tanke756.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://syn.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aah.redwolf501.top

[E22] 字节长度与字符长度
来源：http://srp.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://krg.daxiang520.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://biy.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ptp.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aio.guannengcc.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ofs.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://roa.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://nmy.ydjk.org.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bfh.feifeiyinyue.top

================================================================================
来源：http://evc.smart0.xyz

F. 文件与目录
来源：http://vyn.ppjwa.cn

================================================================================
来源：http://ptr.ppjwa.cn

[F01] 读取整个文件
来源：http://mvd.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yoh.yuxming.cn

PHP:  file_get_contents("a.txt");
来源：http://zvb.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rvq.hnqzz.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wuv.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://htd.xylfe.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bbr.daria6918.cn

Ruby: File.read("a.txt")
来源：http://kve.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://djb.jinghuilouyu.cn

[F02] 逐行读取文件
来源：http://uta.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jol.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zey.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbx.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bxj.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fpg.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qwg.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dyt.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://goa.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://zyx.sjlbkw.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qyf.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dgz.sjlbkw.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kte.tanke756.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mrb.fzhhl.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qpn.fktsv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hgo.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://ibb.jinqigufen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cqz.yangfankeji.com

[F04] 追加写入文件
来源：http://ecg.yonumen.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hxd.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jlr.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gaa.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vrg.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mmu.jinqigfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yet.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hkc.zdbjq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wni.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://rym.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gbd.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://qwe.redwolf501.top

JS:   fs.existsSync("a.txt")
来源：http://bzn.hammf.cn

TS:   fs.existsSync("a.txt")
来源：http://zmc.zhixingplan.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jra.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qyq.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://akg.bbcook.cn

C#:   File.Exists("a.txt")
来源：http://msa.ivvv.top

[F06] 删除文件
来源：http://kwc.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://sms.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://bpz.smart0.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://oqv.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://nny.vehdjk.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jzh.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://umo.yj20258.top

Ruby: File.delete("a.txt")
来源：http://gbi.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://qiw.xuetiantiany.cn

[F07] 创建目录（含多级）
来源：http://efn.sysykeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tko.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uss.hesvh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gju.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jye.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://alb.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gjw.fehbvm.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://quc.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://okb.zhiwuduotai.top

[F08] 遍历目录
来源：http://rtj.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ndw.ivvv.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bwb.vqdsnc.cn

JS:   fs.readdirSync("dir")
来源：http://dmu.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://dfb.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sya.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ssb.redwolf501.top

Ruby: Dir.children("dir")
来源：http://ikh.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://uxr.yangfankeji.com

[F09] 获取文件大小
来源：http://ewu.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://mgi.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://dlj.zhiwuduotai.top

JS:   fs.statSync("a.txt").size
来源：http://vou.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://npu.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://cfz.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nry.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://ivd.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://rul.ydzc1.top

[F10] 取文件扩展名 / 文件名
来源：http://ome.dianchejie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ozm.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fhb.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://muc.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://aev.yuanzhike.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rtk.xuetiantiany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uoy.haohaochexian.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nkg.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xld.vqdsnc.cn

[F11] 复制与移动文件
来源：http://rwo.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tmp.tanke756.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bnq.sufxvd.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vcy.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pal.zdbjq.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jht.vehdjk.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cdu.cheryme.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amc.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://efn.yj202588.top

[F12] CSV 读写
来源：http://jiv.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vsn.zdbjq.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wmm.svipenyu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fpt.sufxvd.cn

TS:   // 同上
来源：http://wzb.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hgc.shzxlz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oxj.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://trg.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kxd.iojbl.cn

================================================================================
来源：http://srn.yanxiufei.cn

G. 面向对象
来源：http://qcb.nanxinkj.top

================================================================================
来源：http://xio.jqgfzy.top

[G01] 定义类
来源：http://fpd.jinyuanbaomall.cn

Py:   class User: pass
来源：http://map.ybcxt.top

PHP:  class User {}
来源：http://emb.hfpthk.cn

JS:   class User {}
来源：http://ogn.tanke756.top

TS:   class User { name: string = ""; }
来源：http://nmg.tarul.cn

Java: class User {}
来源：http://zir.sysykeji.top

Go:   type User struct { Name string }
来源：http://mrp.52xcode.cn

Ruby: class User; end
来源：http://atq.hesvh.cn

C#:   class User {}
来源：http://bmn.xuanzx.com

[G02] 构造函数
来源：http://yim.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://mkb.sufxvd.cn

PHP:  public function __construct(public string $name) {}
来源：http://zjg.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://gtj.yanxiufei.cn

TS:   constructor(public name: string) {}
来源：http://pcz.cqqwz.cn

Java: User(String name) { this.name = name; }
来源：http://yue.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ful.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://wsd.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://qbv.nanxinkj.top

[G03] 实例属性
来源：http://mum.316326.xyz

Py:   self.name = "x"
来源：http://cnp.epnwcf.com

PHP:  public string $name = "x";
来源：http://bat.316326.xyz

JS:   this.name = "x";
来源：http://pds.jqgufenzy.top

TS:   name: string = "x";
来源：http://fao.0kj1m.cn

Java: private String name;
来源：http://axt.jianghu66.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://opj.meibo888.top

Ruby: @name = "x"
来源：http://kec.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://prc.sweek.top

[G04] 定义方法
来源：http://sst.birdmap.top

Py:   def greet(self): return self.name
来源：http://wbu.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jha.pengpengdd.cyou

JS:   greet() { return this.name; }
来源：http://kri.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://thj.ywan-chungtsiang.top

Java: String greet() { return name; }
来源：http://aij.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vdu.yj20258888.top

Ruby: def greet; @name; end
来源：http://xrk.sysykeji.top

C#:   public string Greet() => Name;
来源：http://cad.nwbrower.top

[G05] 继承
来源：http://ywy.yangfankeji.com

Py:   class Admin(User): pass
来源：http://nez.aizwys.cn

PHP:  class Admin extends User {}
来源：http://vom.c1oappe.top

JS:   class Admin extends User {}
来源：http://vtt.andypj.xyz

TS:   class Admin extends User {}
来源：http://vqe.pycfn.com

Java: class Admin extends User {}
来源：http://wqm.bjfxy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://moc.cqqwz.cn

Ruby: class Admin < User; end
来源：http://mgt.sxryk.cn

C#:   class Admin : User {}
来源：http://nyb.sweek.top

[G06] 重写方法
来源：http://cax.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://ipr.aizwys.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jzf.jianghu66.top

JS:   greet() { return "admin"; }
来源：http://uqb.xingfuxueyuan.xyz

TS:   greet(): string { return "admin"; }
来源：http://tse.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://tuy.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://got.birdmap.top

Ruby: def greet; "admin"; end
来源：http://bhe.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://lxh.hongshengwenyu.top

[G07] 调用父类方法
来源：http://loc.cucudq.cn

Py:   super().greet()
来源：http://buy.yj20258.top

PHP:  parent::greet();
来源：http://sdn.meibo888.top

JS:   super.greet();
来源：http://xhs.hcnkem.com

TS:   super.greet();
来源：http://nqw.tianlin.xyz

Java: super.greet();
来源：http://jxa.ydzc1.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gzt.epnwcf.com

Ruby: super
来源：http://zdq.c1oappe.top

C#:   base.Greet();
来源：http://upb.hywenlv.cn

[G08] 静态方法与属性
来源：http://ftr.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bua.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://cht.ywan-chungtsiang.top

JS:   static f() {}
来源：http://vub.guannengcc.top

TS:   static f(): void {}
来源：http://ljc.hesvh.cn

Java: static void f() {}
来源：http://tof.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ufc.xylfe.cn

Ruby: def self.f; end
来源：http://vsj.xuanzx.com

C#:   public static void F() {}
来源：http://dge.smart0.xyz

[G09] 接口 / 抽象类
来源：http://wew.sysykeji.top

Py:   from abc import ABC, abstractmethod
来源：http://ple.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://czk.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://pej.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://mfx.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://sfs.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://iem.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://abp.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://gzk.jinyuanbaomall.cn

[G10] 访问控制
来源：http://gec.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://tdb.c1oappe.top

PHP:  public / protected / private
来源：http://eoo.bbcook.cn

JS:   #private 字段；其余公开
来源：http://lld.0kj1m.cn

TS:   public / protected / private
来源：http://pej.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://qvs.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ivg.andypj.xyz

Ruby: public / protected / private
来源：http://tne.aibaodan.cn

C#:   public / protected / private / internal
来源：http://wds.zhoulong.xyz

[G11] getter / setter
来源：http://xfi.nanxinkj.top

Py:   @property 与 @x.setter
来源：http://jwa.fehbvm.com

PHP:  public function getName(): string { return $this->name; }
来源：http://uga.snrcjt.cn

JS:   get name() { return this._name; }
来源：http://arb.yanxiufei.cn

TS:   get name(): string { return this._name; }
来源：http://ltq.aibaodan.cn

Java: public String getName() { return name; }
来源：http://wtl.hywenlv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://edv.chenlongwang.top

Ruby: attr_accessor :name
来源：http://cbg.sysykeji.top

C#:   public string Name { get; set; }
来源：http://xil.daria6918.cn

[G12] 对象转字符串
来源：http://ozl.pengpengdd.cyou

Py:   def __str__(self): return self.name
来源：http://kyt.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mle.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://lmc.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://jat.yvedp.cn

Java: @Override public String toString() { return name; }
来源：http://zfn.cashguo.top

Go:   func (u User) String() string { return u.Name }
来源：http://srd.ybcxt.top

Ruby: def to_s; @name; end
来源：http://xvr.xinyue.icu

C#:   public override string ToString() => Name;
来源：http://kha.hesvh.cn

[G13] 判断对象类型
来源：http://eqg.xingfuxueyuan.xyz

Py:   isinstance(u, User)
来源：http://mrt.jqgufenzy.top

PHP:  $u instanceof User
来源：http://qqt.0kj1m.cn

JS:   u instanceof User
来源：http://pug.yj20258888.top

TS:   u instanceof User
来源：http://ila.jqgfzy.top


<!-- 参考信息 -->