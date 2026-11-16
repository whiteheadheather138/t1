代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nai.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ovl.316326.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://guk.vqdsnc.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nxm.zhiwuduotai.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://odx.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://avs.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://pqg.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ckd.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tnx.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vjv.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rby.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ptt.hesvh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fqz.zhongyouzk.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://etp.vqdsnc.cn

[E16] 数字千分位
来源：http://ahj.316326.xyz

Py:   f"{1234567:,}"
来源：http://rky.yongpay.top

PHP:  number_format(1234567);
来源：http://ksh.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://any.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lyu.hcnkem.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fna.shanyushiyangkeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hpb.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://urk.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://xuj.316326.xyz

[E17] 首字母大写
来源：http://ypq.gaohongyu789.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kuj.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://iho.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yrz.ydjk.org.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yaa.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xlx.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vtd.zhengqikj.top

Ruby: s.capitalize
来源：http://rjg.chenlongwang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zma.xziqi.cn

[E18] 模板占位符替换
来源：http://luy.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://usc.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://saf.yonumen.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fxb.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cga.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bzq.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lat.zhijiandao.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ius.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aep.shuidangran.top

[E19] 多行文本按行拆分
来源：http://xiy.yangfankeji.com

Py:   s.splitlines()
来源：http://fgx.yuxming.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cuz.chenlongwang.top

JS:   s.split(/\r?\n/)
来源：http://qcr.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://vqu.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://sqr.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://gvl.bbcook.cn

Ruby: s.lines
来源：http://ebq.aibaodan.cn

C#:   s.Split('\n')
来源：http://uqi.daxiang520.top

[E20] 判断字符串是否为空
来源：http://ccb.sjlbkw.cn

Py:   if not s:
来源：http://nrg.hfpthk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mku.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zix.ydzc1.top

TS:   if (s === "") {}
来源：http://hah.fktsv.cn

Java: if (s.isEmpty()) {}
来源：http://vuh.hcnkem.com

Go:   if s == "" {}
来源：http://ilq.yj202588.top

Ruby: if s.empty?
来源：http://krc.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rjd.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://ugo.tanke756.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://moq.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://taw.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uvi.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://reo.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pfr.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://qjd.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bdy.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://spw.fzhhl.top

[E22] 字节长度与字符长度
来源：http://ddp.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jnv.meibo888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://znt.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yij.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eim.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sqg.jinqigufen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qdn.gaohongyu789.top

Ruby: s.bytesize;  s.length
来源：http://wzs.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bpa.tarul.cn

================================================================================
来源：http://tym.uphjek.com

F. 文件与目录
来源：http://yzb.0kj1m.cn

================================================================================
来源：http://xxi.yongpay.top

[F01] 读取整个文件
来源：http://mxi.sweek.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gob.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://gqd.fengsongda.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://two.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bgl.svipenyu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://oib.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nyc.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://jrv.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://blk.shuidangran.top

[F02] 逐行读取文件
来源：http://few.gzhubu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rzr.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vzt.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwb.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aod.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nem.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vxr.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://trw.xingfuxueyuan.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xgy.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://jcd.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://euz.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gwh.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://abj.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://elx.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://csy.chenlongwang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rvs.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://upr.wangshuangyany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uyr.0kj1m.cn

[F04] 追加写入文件
来源：http://dis.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nna.sufxvd.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xnw.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aaa.birdmap.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qul.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ziy.bjfxy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pwc.gzhubu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ujl.yuanzhike.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://por.0kj1m.cn

[F05] 判断文件或目录是否存在
来源：http://nsa.ydjk.org.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://opb.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://tik.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://abb.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://qxk.daria6918.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://oya.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jij.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://ktk.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://apo.0kj1m.cn

[F06] 删除文件
来源：http://oco.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://bdn.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://dev.sjlbkw.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wdv.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://pid.hammf.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hyq.meibo888.top

Go:   os.Remove("a.txt")
来源：http://pih.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://vcu.tianlin.xyz

C#:   File.Delete("a.txt");
来源：http://vpp.xziqi.cn

[F07] 创建目录（含多级）
来源：http://tpx.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jvw.havefunace.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iye.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ojd.snrcjt.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ixj.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jyq.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uod.daxiang520.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://scf.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wom.quarkkingdee.top

[F08] 遍历目录
来源：http://cmb.shanyushiyangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://niw.vehdjk.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rqe.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://hbm.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://iyp.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ach.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mhs.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://icj.zdbjq.cn

C#:   Directory.GetFiles("dir")
来源：http://vno.xuetiantiany.cn

[F09] 获取文件大小
来源：http://rcz.tarul.cn

Py:   os.path.getsize("a.txt")
来源：http://wlu.shangyingyoupin.top

PHP:  filesize("a.txt");
来源：http://vku.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://flg.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://hca.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://nng.cdnleiting.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qfw.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://cck.yangfankeji.com

C#:   new FileInfo("a.txt").Length
来源：http://xxb.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://wpd.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fiw.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://joy.bjfxy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eky.kuanghao11.cn

TS:   path.extname("a.txt")
来源：http://zpc.svipenyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yjo.havefunace.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gix.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ane.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xla.mhx1999.top

[F11] 复制与移动文件
来源：http://rnx.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nao.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kxw.iojbl.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eor.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bii.zhiwuduotai.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ebg.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vmx.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://prv.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dmz.aizwys.cn

[F12] CSV 读写
来源：http://ind.zhiwuduotai.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cnh.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nfo.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vib.zhiwuduotai.top

TS:   // 同上
来源：http://uid.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hgm.shanyushiyangkeji.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://efu.bjfxy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qhh.zhengqikj.top

C#:   // 无内置：用 CsvHelper 库
来源：http://bpk.ydzc1.top

================================================================================
来源：http://fgy.xuanzx.com

G. 面向对象
来源：http://nnu.hcnkem.com

================================================================================
来源：http://llv.zhengqikj.top

[G01] 定义类
来源：http://pkp.sxryk.cn

Py:   class User: pass
来源：http://urg.aizwys.cn

PHP:  class User {}
来源：http://vwb.chenlongwang.top

JS:   class User {}
来源：http://mas.daxiang520.top

TS:   class User { name: string = ""; }
来源：http://hcy.yongpay.top

Java: class User {}
来源：http://pvh.uphjek.com

Go:   type User struct { Name string }
来源：http://dzc.fehbvm.com

Ruby: class User; end
来源：http://cta.nanxuanxn.top

C#:   class User {}
来源：http://bwz.yueranfly.top

[G02] 构造函数
来源：http://ywv.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://tes.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://ifn.zhengqikj.top

JS:   constructor(name) { this.name = name; }
来源：http://lmi.wangshuangyany.cn

TS:   constructor(public name: string) {}
来源：http://ybv.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://jvr.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dfp.ydzc1.top

Ruby: def initialize(name); @name = name; end
来源：http://eet.quarkkingdee.top

C#:   public User(string name) { Name = name; }
来源：http://idc.gotoacloud.top

[G03] 实例属性
来源：http://yqw.yfazqb.com

Py:   self.name = "x"
来源：http://tei.c1oappe.top

PHP:  public string $name = "x";
来源：http://gkt.feifeiyinyue.top

JS:   this.name = "x";
来源：http://xih.chenlongwang.top

TS:   name: string = "x";
来源：http://hyu.jinyuanbaomall.cn

Java: private String name;
来源：http://bco.xuetiantiany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ulh.shuidangran.top

Ruby: @name = "x"
来源：http://len.yangfankeji.com

C#:   public string Name { get; set; } = "x";
来源：http://ifg.ehwqpu.com

[G04] 定义方法
来源：http://wje.hammf.cn

Py:   def greet(self): return self.name
来源：http://ekb.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jdg.cucudq.cn

JS:   greet() { return this.name; }
来源：http://mpo.gaohongyu789.top

TS:   greet(): string { return this.name; }
来源：http://zal.pengpengdd.cyou

Java: String greet() { return name; }
来源：http://kvp.c1oappe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iag.zhiwuduotai.top

Ruby: def greet; @name; end
来源：http://jmu.jyoumei.cn

C#:   public string Greet() => Name;
来源：http://cwe.jinghuilouyu.cn

[G05] 继承
来源：http://ahj.yfazqb.com

Py:   class Admin(User): pass
来源：http://yyv.ivvv.top

PHP:  class Admin extends User {}
来源：http://ref.cqqwz.cn

JS:   class Admin extends User {}
来源：http://gex.dianchejie.cn

TS:   class Admin extends User {}
来源：http://xoz.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://gge.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fgc.aibaodan.cn

Ruby: class Admin < User; end
来源：http://ufv.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://kxn.andypj.xyz

[G06] 重写方法
来源：http://yzt.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://osd.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ofq.bbcook.cn

JS:   greet() { return "admin"; }
来源：http://bca.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://gyj.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://ifn.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eab.jqgfzy.top

Ruby: def greet; "admin"; end
来源：http://vor.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://xua.ywan-chungtsiang.top

[G07] 调用父类方法
来源：http://chz.yj202588.top

Py:   super().greet()
来源：http://jch.hcnkem.com

PHP:  parent::greet();
来源：http://ckj.yanxiufei.cn

JS:   super.greet();
来源：http://ycp.nanxinkj.top

TS:   super.greet();
来源：http://tqa.fanxiaobao.xyz

Java: super.greet();
来源：http://jfc.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://esv.jlsjyb.cn

Ruby: super
来源：http://cjx.hcnkem.com

C#:   base.Greet();
来源：http://oyt.jianghu66.top

[G08] 静态方法与属性
来源：http://fef.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qoi.zhoulong.xyz

PHP:  public static function f() {}
来源：http://zkp.pengpengdd.cyou

JS:   static f() {}
来源：http://zwq.smart0.xyz

TS:   static f(): void {}
来源：http://ylf.cqqwz.cn

Java: static void f() {}
来源：http://kyl.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://buw.52xcode.cn

Ruby: def self.f; end
来源：http://cao.chenzaomai.com

C#:   public static void F() {}
来源：http://rsv.redwolf501.top

[G09] 接口 / 抽象类
来源：http://pnd.yj20258888.top

Py:   from abc import ABC, abstractmethod
来源：http://whh.chenlongwang.top

PHP:  interface Shape { public function area(): float; }
来源：http://ffp.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mwd.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://qqn.smart0.xyz

Java: interface Shape { double area(); }
来源：http://exq.yj20258.top

Go:   type Shape interface { Area() float64 }
来源：http://kde.epnwcf.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sah.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://cpx.gaohongyu789.top

[G10] 访问控制
来源：http://qet.hammf.cn

Py:   约定 _protected / __private（不强制）
来源：http://rxp.zhixingplan.top

PHP:  public / protected / private
来源：http://bjf.yj20258.top

JS:   #private 字段；其余公开
来源：http://rbz.xuanzx.com

TS:   public / protected / private
来源：http://hsw.c1oappe.top

Java: public / protected / private / 默认包级
来源：http://fzv.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ixi.zhiwuduotai.top

Ruby: public / protected / private
来源：http://oro.xinyue.icu

C#:   public / protected / private / internal
来源：http://baf.snrcjt.cn

[G11] getter / setter
来源：http://ahc.jyoumei.cn

Py:   @property 与 @x.setter
来源：http://vpn.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://naw.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://mtf.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://obs.jyoumei.cn

Java: public String getName() { return name; }
来源：http://nay.dianchejie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yfs.tanke756.top

Ruby: attr_accessor :name
来源：http://hod.sjlbkw.cn

C#:   public string Name { get; set; }
来源：http://nqt.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://ths.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://ojq.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://phb.52xcode.cn

JS:   toString() { return this.name; }
来源：http://tdg.sysykeji.top

TS:   toString(): string { return this.name; }
来源：http://rqm.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://eoh.jinyuanbaomall.cn

Go:   func (u User) String() string { return u.Name }
来源：http://opb.jyoumei.cn

Ruby: def to_s; @name; end
来源：http://jdk.mhx1999.top

C#:   public override string ToString() => Name;
来源：http://uki.hywenlv.cn

[G13] 判断对象类型
来源：http://eek.tian-w.cn


<!-- 参考信息 -->