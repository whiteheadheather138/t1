代发 wailian999

[E14] URL 编码与 Base64
来源：http://jho.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fft.tianlin.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ujf.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gad.jqgufenzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wsw.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ire.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qiw.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://irs.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ofq.jianghu66.top

[E15] HTML 转义 / 反转义
来源：http://kmd.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fyf.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mpj.yfazqb.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yzf.zhiwuduotai.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nec.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dgi.svipenyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qxm.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://avv.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pmy.hammf.cn

[E16] 数字千分位
来源：http://mir.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://raw.hongshengwenyu.top

PHP:  number_format(1234567);
来源：http://wdk.hongshengwenyu.top

JS:   (1234567).toLocaleString("en-US")
来源：http://csp.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://axo.sxryk.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zmv.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ahg.cdnleiting.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jom.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://hpm.snrcjt.cn

[E17] 首字母大写
来源：http://lpa.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wxr.zycfv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wrh.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxa.cdnleiting.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ubo.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bdg.hnxiangtu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hiu.pengpengdd.cyou

Ruby: s.capitalize
来源：http://isl.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://urm.pycfn.com

[E18] 模板占位符替换
来源：http://ytq.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ebd.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://htr.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mvg.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gjc.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vwb.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wnp.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://udb.yangfankeji.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rrt.pengpengdd.cyou

[E19] 多行文本按行拆分
来源：http://lst.hnxiangtu.top

Py:   s.splitlines()
来源：http://exl.iojbl.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hqs.zdbjq.cn

JS:   s.split(/\r?\n/)
来源：http://qhg.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://rrl.yj20258.top

Java: s.lines().toList()
来源：http://itz.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://wws.ehwqpu.com

Ruby: s.lines
来源：http://mux.uphjek.com

C#:   s.Split('\n')
来源：http://rxm.cheryme.top

[E20] 判断字符串是否为空
来源：http://skl.aibaodan.cn

Py:   if not s:
来源：http://xhn.zdqjudy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jqz.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eqa.zdqjudy.top

TS:   if (s === "") {}
来源：http://qge.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://zqq.ywan-chungtsiang.top

Go:   if s == "" {}
来源：http://ohq.zhoulong.xyz

Ruby: if s.empty?
来源：http://jqh.yuxming.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xee.jiagoushi.top

[E21] 超长截断加省略号
来源：http://jyh.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wse.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xns.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tbp.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://crp.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vnf.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://pby.bjfxy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zgb.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rpu.fktsv.cn

[E22] 字节长度与字符长度
来源：http://uzo.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oyc.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aja.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yzj.quarkkingdee.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ikd.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zuz.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://apo.cucudq.cn

Ruby: s.bytesize;  s.length
来源：http://vop.zycfv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dmj.zhixingplan.top

================================================================================
来源：http://omc.zhongyouzk.top

F. 文件与目录
来源：http://ick.yfazqb.com

================================================================================
来源：http://cnf.hesvh.cn

[F01] 读取整个文件
来源：http://aje.gotoacloud.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://auq.nanxuanxn.top

PHP:  file_get_contents("a.txt");
来源：http://vde.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sdg.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://odw.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yan.fktsv.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rvk.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://lld.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://loe.hnxiangtu.top

[F02] 逐行读取文件
来源：http://wah.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qip.daxiang520.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hqr.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kgj.zhijiandao.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uve.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vit.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cqm.ydjk.org.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xun.sxryk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iau.cashguo.top

[F03] 写入文件（覆盖）
来源：http://rob.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eqh.kuanghao11.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dtc.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fke.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovl.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cfk.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://glz.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://rtv.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gvy.sysykeji.top

[F04] 追加写入文件
来源：http://iwo.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pbp.yueranfly.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ojg.hnqzz.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mld.yj20258888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qaf.yuxming.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://seh.yj20258.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tfi.havefunace.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xap.aizwys.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lha.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://kbp.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://clz.gotoacloud.top

PHP:  file_exists("a.txt");
来源：http://cgt.nanxuanxn.top

JS:   fs.existsSync("a.txt")
来源：http://wxg.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://uco.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ghl.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jcg.haohaochexian.top

Ruby: File.exist?("a.txt")
来源：http://haf.fanxiaobao.xyz

C#:   File.Exists("a.txt")
来源：http://fzo.shuidangran.top

[F06] 删除文件
来源：http://wnb.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://lkr.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://vzg.svipenyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ugr.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aon.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qzj.pengpengdd.cyou

Go:   os.Remove("a.txt")
来源：http://bqo.feifeiyinyue.top

Ruby: File.delete("a.txt")
来源：http://jvx.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://dow.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://plk.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dfr.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uwr.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uou.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sry.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wwy.hnqzz.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gxv.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bgn.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ftk.xinyue.icu

[F08] 遍历目录
来源：http://edr.zhongyouzk.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://aqc.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kkk.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://lka.zycfv.cn

TS:   fs.readdirSync("dir")
来源：http://qdx.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xri.epnwcf.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ssk.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://bqc.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://inm.sweek.top

[F09] 获取文件大小
来源：http://kro.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://kct.mhx1999.top

PHP:  filesize("a.txt");
来源：http://yxc.yj20258.top

JS:   fs.statSync("a.txt").size
来源：http://fob.zhoulong.xyz

TS:   fs.statSync("a.txt").size
来源：http://jre.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gml.xylfe.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pdd.pycfn.com

Ruby: File.size("a.txt")
来源：http://bmg.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ysc.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://jxf.sufxvd.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zar.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://src.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://evr.jqgfzy.top

TS:   path.extname("a.txt")
来源：http://nnn.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://utx.zhijiandao.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://avm.fehbvm.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://maa.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mur.yj20258888.top

[F11] 复制与移动文件
来源：http://pau.zhongyouzk.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xip.hnqzz.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://akt.sxryk.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jfn.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bin.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uoj.havefunace.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tqb.guannengcc.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wrg.0kj1m.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wlw.jiagoushi.top

[F12] CSV 读写
来源：http://gvi.bjfxy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wch.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jlr.guowangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xoz.zhijiandao.cn

TS:   // 同上
来源：http://sbr.hysaishi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ebg.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tle.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kks.yuxming.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://iiq.zhaomingkeji.xyz

================================================================================
来源：http://hdw.jyoumei.cn

G. 面向对象
来源：http://hiv.zycfv.cn

================================================================================
来源：http://ufe.yangfankeji.com

[G01] 定义类
来源：http://jxv.shanyushiyangtech.top

Py:   class User: pass
来源：http://cjv.ywan-chungtsiang.top

PHP:  class User {}
来源：http://mop.ehwqpu.com

JS:   class User {}
来源：http://enu.zycfv.cn

TS:   class User { name: string = ""; }
来源：http://pwi.hesvh.cn

Java: class User {}
来源：http://vfd.xuanzx.com

Go:   type User struct { Name string }
来源：http://zts.cucudq.cn

Ruby: class User; end
来源：http://tem.ybcxt.top

C#:   class User {}
来源：http://bwi.hammf.cn

[G02] 构造函数
来源：http://xer.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://rjt.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://lfr.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://tqs.hammf.cn

TS:   constructor(public name: string) {}
来源：http://kno.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://tbh.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mee.mhx1999.top

Ruby: def initialize(name); @name = name; end
来源：http://dox.tian-w.cn

C#:   public User(string name) { Name = name; }
来源：http://cbu.fzhhl.top

[G03] 实例属性
来源：http://kxd.gotoacloud.top

Py:   self.name = "x"
来源：http://exv.gaohongyu789.top

PHP:  public string $name = "x";
来源：http://xho.yfazqb.com

JS:   this.name = "x";
来源：http://dqr.yueranfly.top

TS:   name: string = "x";
来源：http://iub.jqgfzy.top

Java: private String name;
来源：http://mpu.hywenlv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://apb.sjlbkw.cn

Ruby: @name = "x"
来源：http://zos.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://gwn.cheryme.top

[G04] 定义方法
来源：http://wfq.nwbrower.top

Py:   def greet(self): return self.name
来源：http://dlq.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uef.fanxiaobao.xyz

JS:   greet() { return this.name; }
来源：http://apu.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://meg.316326.xyz

Java: String greet() { return name; }
来源：http://pni.ctjpmb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ksg.yvedp.cn

Ruby: def greet; @name; end
来源：http://mkp.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://baj.fehbvm.com

[G05] 继承
来源：http://kqa.fehbvm.com

Py:   class Admin(User): pass
来源：http://uho.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://gfg.xingfuxueyuan.xyz

JS:   class Admin extends User {}
来源：http://npn.zhoulong.xyz

TS:   class Admin extends User {}
来源：http://fru.dianchejie.cn

Java: class Admin extends User {}
来源：http://yiv.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lue.sweek.top

Ruby: class Admin < User; end
来源：http://yhy.ehwqpu.com

C#:   class Admin : User {}
来源：http://mqq.xinyue.icu

[G06] 重写方法
来源：http://tme.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://vvq.yangfankeji.com

PHP:  public function greet(): string { return "admin"; }
来源：http://sjf.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://mis.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://vgd.cqqwz.cn

Java: @Override String greet() { return "admin"; }
来源：http://rgs.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ewj.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://ike.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://icf.zhengqikj.top

[G07] 调用父类方法
来源：http://sbt.uphjek.com

Py:   super().greet()
来源：http://cbt.pengpengdd.cyou

PHP:  parent::greet();
来源：http://pxh.aibaodan.cn

JS:   super.greet();
来源：http://ixs.svipenyu.cn

TS:   super.greet();
来源：http://bhr.svipenyu.cn

Java: super.greet();
来源：http://nts.yonumen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ncv.gotoacloud.top

Ruby: super
来源：http://nes.cqqwz.cn

C#:   base.Greet();
来源：http://yjt.vqdsnc.cn

[G08] 静态方法与属性
来源：http://yny.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://slj.yuxming.cn

PHP:  public static function f() {}
来源：http://bkf.yj202588.top

JS:   static f() {}
来源：http://vvx.sysykeji.top

TS:   static f(): void {}
来源：http://ouf.yvedp.cn

Java: static void f() {}
来源：http://tzk.dashuyun.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yjo.aizwys.cn

Ruby: def self.f; end
来源：http://hdx.chenzaomai.com

C#:   public static void F() {}
来源：http://yof.xinyue.icu

[G09] 接口 / 抽象类
来源：http://uaq.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://pfj.vehdjk.com

PHP:  interface Shape { public function area(): float; }
来源：http://nqg.52xcode.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gmh.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://evk.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://olx.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://bgq.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rcj.vqdsnc.cn

C#:   interface IShape { double Area(); }
来源：http://taz.nwbrower.top

[G10] 访问控制
来源：http://idz.0kj1m.cn

Py:   约定 _protected / __private（不强制）
来源：http://mpc.zhiwuduotai.top

PHP:  public / protected / private
来源：http://aym.xingfuxueyuan.xyz

JS:   #private 字段；其余公开
来源：http://yyj.dashuyun.cn

TS:   public / protected / private
来源：http://pkr.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://kng.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nya.havefunace.top

Ruby: public / protected / private
来源：http://wtz.0kj1m.cn

C#:   public / protected / private / internal
来源：http://pjs.kuanghao11.cn

[G11] getter / setter
来源：http://npw.sysykeji.top

Py:   @property 与 @x.setter
来源：http://vgj.0kj1m.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sbf.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://qqk.hnqzz.top

TS:   get name(): string { return this._name; }
来源：http://uns.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://mpc.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://eji.cqqwz.cn

Ruby: attr_accessor :name
来源：http://fsw.ydjk.org.cn

C#:   public string Name { get; set; }
来源：http://cgu.hywenlv.cn

[G12] 对象转字符串
来源：http://zbe.wangdashe.top

Py:   def __str__(self): return self.name
来源：http://bea.chenlongwang.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://mix.tarul.cn

JS:   toString() { return this.name; }
来源：http://fwc.sjlbkw.cn

TS:   toString(): string { return this.name; }
来源：http://voz.yj20258.top

Java: @Override public String toString() { return name; }
来源：http://nkm.fktsv.cn


<!-- 参考信息 -->