代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ksn.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://byu.52xcode.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lcx.daxiang520.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gys.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://ccd.zhiwuduotai.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kdb.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://erf.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fxn.haohaochexian.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ckq.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mli.kuanghao11.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://owu.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ilz.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aqi.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://krt.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://yoh.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dai.jinghuilouyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sbu.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://grp.hfpthk.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qds.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://csk.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jvx.hnqzz.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uqb.hywenlv.cn

[E16] 数字千分位
来源：http://ahh.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://dnt.uphjek.com

PHP:  number_format(1234567);
来源：http://jpf.jqgufenzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jxd.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zrt.chenjidiqi.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oor.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mgi.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gpy.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://dqa.gogol.net.cn

[E17] 首字母大写
来源：http://lov.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nul.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://jug.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dce.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gou.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bhs.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ece.yonumen.top

Ruby: s.capitalize
来源：http://bjz.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hpd.daria6918.cn

[E18] 模板占位符替换
来源：http://dvi.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gmv.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ndb.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ohe.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mud.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hdh.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zti.chenzaomai.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uvm.nanxuanxn.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eus.zhaomingkeji.xyz

[E19] 多行文本按行拆分
来源：http://roz.tian-w.cn

Py:   s.splitlines()
来源：http://pky.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cwh.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://bbr.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://bzp.bbcook.cn

Java: s.lines().toList()
来源：http://skw.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://uog.chenjidiqi.icu

Ruby: s.lines
来源：http://fif.yfazqb.com

C#:   s.Split('\n')
来源：http://yxf.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://oxb.tianlin.xyz

Py:   if not s:
来源：http://iov.hywenlv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://men.xylfe.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ubx.ctjpmb.com

TS:   if (s === "") {}
来源：http://wtk.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://sck.ybcxt.top

Go:   if s == "" {}
来源：http://pow.iojbl.cn

Ruby: if s.empty?
来源：http://ton.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rwh.dianchejie.cn

[E21] 超长截断加省略号
来源：http://nvl.tian-w.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://axp.meibo888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hmz.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://itc.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bhc.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mtq.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://cxt.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://prk.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://owt.cucudq.cn

[E22] 字节长度与字符长度
来源：http://xin.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bct.nanxinkj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oll.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zga.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rpa.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qly.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ubx.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://vqz.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oqq.xingfuxueyuan.xyz

================================================================================
来源：http://bxp.jinqigfzy.top

F. 文件与目录
来源：http://rhh.hfpthk.cn

================================================================================
来源：http://wnk.haohaochexian.top

[F01] 读取整个文件
来源：http://lum.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://miz.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://zym.pycfn.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lpu.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bkk.wangshuangyany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fwb.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uve.wangshuangyany.cn

Ruby: File.read("a.txt")
来源：http://bkd.svipenyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://mag.ybcxt.top

[F02] 逐行读取文件
来源：http://pnt.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tib.dashuyun.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zje.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wdd.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://onz.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nqy.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zso.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dnc.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ilk.zycfv.cn

[F03] 写入文件（覆盖）
来源：http://mwm.cashguo.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mdx.ppjwa.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yxd.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aqk.zhengqikj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://und.guowangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xef.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nij.yj202588.top

Ruby: File.write("a.txt", "hi")
来源：http://ydf.zhijiandao.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gil.ehwqpu.com

[F04] 追加写入文件
来源：http://avz.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://osm.zhixingplan.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ubp.zhijiandao.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eyv.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rkp.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jfx.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gpr.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kxn.ywan-chungtsiang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://asm.zdbjq.cn

[F05] 判断文件或目录是否存在
来源：http://pbh.gaohongyu789.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://coz.yuanzhike.top

PHP:  file_exists("a.txt");
来源：http://ghl.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://ldy.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://xts.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://xsj.yueranfly.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oyc.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://avx.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://fmu.ydzc1.top

[F06] 删除文件
来源：http://ytx.uphjek.com

Py:   os.remove("a.txt")
来源：http://xrq.daria6918.cn

PHP:  unlink("a.txt");
来源：http://mxe.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hao.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://ock.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fjh.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://slo.wangdashe.top

Ruby: File.delete("a.txt")
来源：http://ofn.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://tel.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://iss.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hhz.daxiang520.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rkx.gaohongyu789.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dxo.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fnp.xinyue.icu

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dgs.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ovz.epnwcf.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pia.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zgq.fanxiaobao.xyz

[F08] 遍历目录
来源：http://hce.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bjh.nanxuanxn.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zwe.zdbjq.cn

JS:   fs.readdirSync("dir")
来源：http://xvv.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://xgq.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wxc.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://buq.jinqigfzy.top

Ruby: Dir.children("dir")
来源：http://ouf.zhoulong.xyz

C#:   Directory.GetFiles("dir")
来源：http://okx.vehdjk.com

[F09] 获取文件大小
来源：http://hwq.guannengcc.top

Py:   os.path.getsize("a.txt")
来源：http://tkt.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://cnb.cucudq.cn

JS:   fs.statSync("a.txt").size
来源：http://qnn.daria6918.cn

TS:   fs.statSync("a.txt").size
来源：http://xba.svipenyu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uar.yj20258.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://djn.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://mdh.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://shz.jlsjyb.cn

[F10] 取文件扩展名 / 文件名
来源：http://qgv.52xcode.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://avi.yangfankeji.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bmy.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xzc.vehdjk.com

TS:   path.extname("a.txt")
来源：http://ngb.gogol.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lze.jinghuilouyu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fxw.shanyushiyangtech.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pge.jiagoushi.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eda.jqgfzy.top

[F11] 复制与移动文件
来源：http://xww.gogol.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xap.svipenyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lqn.chenjidiqi.icu

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xro.havefunace.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sxt.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wpa.zdqjudy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mvs.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zwr.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lgy.gaohongyu789.top

[F12] CSV 读写
来源：http://vao.uphjek.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fvn.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lgt.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hxj.sufxvd.cn

TS:   // 同上
来源：http://juu.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://osk.hongshengwenyu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fdo.yanxiufei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gqi.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://brs.dianchejie.cn

================================================================================
来源：http://zqb.jqgfzy.top

G. 面向对象
来源：http://sxk.iojbl.cn

================================================================================
来源：http://ipc.sxryk.cn

[G01] 定义类
来源：http://swn.sweek.top

Py:   class User: pass
来源：http://vhy.nanxinkj.top

PHP:  class User {}
来源：http://tug.xingfuxueyuan.xyz

JS:   class User {}
来源：http://xfh.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://ujn.shanyushiyangtech.top

Java: class User {}
来源：http://fve.zycfv.cn

Go:   type User struct { Name string }
来源：http://zai.fzhhl.top

Ruby: class User; end
来源：http://xfb.hysaishi.cn

C#:   class User {}
来源：http://exa.fehbvm.com

[G02] 构造函数
来源：http://xdc.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://muy.zycfv.cn

PHP:  public function __construct(public string $name) {}
来源：http://ezr.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://sfo.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://msn.havefunace.top

Java: User(String name) { this.name = name; }
来源：http://app.shanyushiyangkeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vqy.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://brt.316326.xyz

C#:   public User(string name) { Name = name; }
来源：http://sot.dashuyun.cn

[G03] 实例属性
来源：http://myc.ydzc1.top

Py:   self.name = "x"
来源：http://ujx.kuanghao11.cn

PHP:  public string $name = "x";
来源：http://ebc.chenlongwang.top

JS:   this.name = "x";
来源：http://wms.jyoumei.cn

TS:   name: string = "x";
来源：http://ugg.9152youxi.cn

Java: private String name;
来源：http://ljr.guannengcc.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mmw.yvedp.cn

Ruby: @name = "x"
来源：http://yrf.vehdjk.com

C#:   public string Name { get; set; } = "x";
来源：http://nvb.tianlin.xyz

[G04] 定义方法
来源：http://qif.ybcxt.top

Py:   def greet(self): return self.name
来源：http://rde.guannengcc.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hua.feifeiyinyue.top

JS:   greet() { return this.name; }
来源：http://gjh.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://tnp.nanxinkj.top

Java: String greet() { return name; }
来源：http://gyp.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pei.tarul.cn

Ruby: def greet; @name; end
来源：http://qxs.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://vtq.ppjwa.cn

[G05] 继承
来源：http://xlt.chenzaomai.com

Py:   class Admin(User): pass
来源：http://eom.smart0.xyz

PHP:  class Admin extends User {}
来源：http://ely.fehbvm.com

JS:   class Admin extends User {}
来源：http://cqv.xinyue.icu

TS:   class Admin extends User {}
来源：http://xqc.yuanzhike.top

Java: class Admin extends User {}
来源：http://wvy.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xni.yonumen.top

Ruby: class Admin < User; end
来源：http://msu.yuanzhike.top

C#:   class Admin : User {}
来源：http://qui.pycfn.com

[G06] 重写方法
来源：http://wog.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://rkt.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://idl.birdmap.top

JS:   greet() { return "admin"; }
来源：http://abi.chenlongwang.top

TS:   greet(): string { return "admin"; }
来源：http://wbm.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://rxe.yuxming.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cas.kuanghao11.cn

Ruby: def greet; "admin"; end
来源：http://asu.yj202588.top

C#:   public override string Greet() => "admin";
来源：http://qlr.zhaomingkeji.xyz

[G07] 调用父类方法
来源：http://eow.dianchejie.cn

Py:   super().greet()
来源：http://vpm.hammf.cn

PHP:  parent::greet();
来源：http://ssa.ydjk.org.cn

JS:   super.greet();
来源：http://waa.jinqigufen.top

TS:   super.greet();
来源：http://nkn.daria6918.cn

Java: super.greet();
来源：http://wvu.yonumen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zyp.vqdsnc.cn

Ruby: super
来源：http://xkm.meibo888.top

C#:   base.Greet();
来源：http://hxf.c1oappe.top

[G08] 静态方法与属性
来源：http://qyt.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://obk.ehwqpu.com

PHP:  public static function f() {}
来源：http://sxq.zhoulong.xyz

JS:   static f() {}
来源：http://bti.tarul.cn

TS:   static f(): void {}
来源：http://oai.hnxiangtu.top

Java: static void f() {}
来源：http://spd.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lmr.cheryme.top

Ruby: def self.f; end
来源：http://dso.yvedp.cn

C#:   public static void F() {}
来源：http://ojw.pycfn.com

[G09] 接口 / 抽象类
来源：http://eur.wangdashe.top

Py:   from abc import ABC, abstractmethod
来源：http://vpt.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hfa.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jnu.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://vtm.vqdsnc.cn

Java: interface Shape { double area(); }
来源：http://fyi.hnxiangtu.top

Go:   type Shape interface { Area() float64 }
来源：http://byt.shanyushiyangtech.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://err.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://sbz.haohaochexian.top

[G10] 访问控制
来源：http://otf.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://mpb.jinqigfzy.top

PHP:  public / protected / private
来源：http://nnn.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://xnl.mhx1999.top

TS:   public / protected / private
来源：http://csi.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://tsc.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ezw.kuanghao11.cn

Ruby: public / protected / private
来源：http://azu.316326.xyz

C#:   public / protected / private / internal
来源：http://dtf.ydjk.org.cn

[G11] getter / setter
来源：http://zsq.cashguo.top

Py:   @property 与 @x.setter
来源：http://bgp.xingfuxueyuan.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://kyl.jianghu66.top

JS:   get name() { return this._name; }
来源：http://fas.daria6918.cn

TS:   get name(): string { return this._name; }
来源：http://alq.cheryme.top

Java: public String getName() { return name; }
来源：http://nab.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nqa.andypj.xyz

Ruby: attr_accessor :name
来源：http://lcv.ywan-chungtsiang.top

C#:   public string Name { get; set; }
来源：http://fnh.bbcook.cn

[G12] 对象转字符串
来源：http://ehb.jiagoushi.top

Py:   def __str__(self): return self.name
来源：http://vpl.andypj.xyz


<!-- 参考信息 -->