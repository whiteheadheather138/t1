代发 wailian999

[E14] URL 编码与 Base64
来源：http://zze.hysaishi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rhw.kuanghao11.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rgf.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dwv.zdbjq.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pgm.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tml.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ngl.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xnc.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wps.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://gws.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://bil.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oms.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mmr.chenzaomai.com

TS:   // 同上，务必做 XSS 过滤
来源：http://zie.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://umx.zhixingplan.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gxn.pycfn.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gts.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vcq.jinghuilouyu.cn

[E16] 数字千分位
来源：http://axm.jinyuanbaomall.cn

Py:   f"{1234567:,}"
来源：http://blg.bjfxy.top

PHP:  number_format(1234567);
来源：http://xwr.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://yom.tarul.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gti.sufxvd.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ifm.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rpa.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gxc.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://ryv.dashuyun.cn

[E17] 首字母大写
来源：http://zdt.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kqi.fengsongda.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hvy.xylfe.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rks.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hly.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://scw.tian-w.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eaz.redwolf501.top

Ruby: s.capitalize
来源：http://mqn.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ral.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://ggn.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hqa.sjlbkw.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://htd.hcnkem.com

JS:   tpl.replaceAll("{name}", name)
来源：http://znq.birdmap.top

TS:   tpl.replaceAll("{name}", name)
来源：http://whv.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wrr.yueranfly.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rvp.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pbg.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pjh.hesvh.cn

[E19] 多行文本按行拆分
来源：http://mtb.fanxiaobao.xyz

Py:   s.splitlines()
来源：http://zaf.ywan-chungtsiang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oud.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://vcq.zhijiandao.cn

TS:   s.split(/\r?\n/)
来源：http://uxf.quarkkingdee.top

Java: s.lines().toList()
来源：http://dbx.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://jtm.zdbjq.cn

Ruby: s.lines
来源：http://zqz.hnqzz.top

C#:   s.Split('\n')
来源：http://iio.wangdashe.top

[E20] 判断字符串是否为空
来源：http://kju.zhaomingkeji.xyz

Py:   if not s:
来源：http://msk.yongpay.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dom.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bzw.ehwqpu.com

TS:   if (s === "") {}
来源：http://yft.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://qzs.zycfv.cn

Go:   if s == "" {}
来源：http://lgw.yonumen.top

Ruby: if s.empty?
来源：http://cpw.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cdx.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://tqd.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uop.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ivi.dashuyun.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://muk.zhengqikj.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cyt.jinqigufen.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xtx.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://adr.aizwys.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gxx.yvedp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zqy.ybcxt.top

[E22] 字节长度与字符长度
来源：http://fqj.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ugy.guowangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jjl.hfpthk.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lji.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iid.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://msr.shuidangran.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ksj.sweek.top

Ruby: s.bytesize;  s.length
来源：http://xvv.haohaochexian.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://azn.epnwcf.com

================================================================================
来源：http://hwz.hesvh.cn

F. 文件与目录
来源：http://nek.jiagoushi.top

================================================================================
来源：http://cdx.ehwqpu.com

[F01] 读取整个文件
来源：http://oah.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ffo.xuetiantiany.cn

PHP:  file_get_contents("a.txt");
来源：http://ofj.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xsp.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qih.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xfr.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://szo.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://lpi.jinghuilouyu.cn

C#:   File.ReadAllText("a.txt");
来源：http://mcw.chenlongwang.top

[F02] 逐行读取文件
来源：http://hqy.xuanzx.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wej.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://epj.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zcb.shanyushiyangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uaw.cashguo.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nay.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://knv.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zgw.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nsf.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://zqq.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pnm.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://drk.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://giy.sweek.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wum.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oqh.shangyingyoupin.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rqh.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://fis.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dtl.zhoulong.xyz

[F04] 追加写入文件
来源：http://czk.vehdjk.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kfc.316326.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vfm.daxiang520.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zjl.nwbrower.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ttz.yj202588.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://plh.sufxvd.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cfx.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aoz.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oel.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://xpr.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dfb.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://nyl.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://jqj.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://sfo.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ctb.shangyingyoupin.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jpp.yuanzhike.top

Ruby: File.exist?("a.txt")
来源：http://mox.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://tgl.hywenlv.cn

[F06] 删除文件
来源：http://evj.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://qag.zycfv.cn

PHP:  unlink("a.txt");
来源：http://odb.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://mzl.xinyue.icu

TS:   fs.unlinkSync("a.txt")
来源：http://gnt.gzhubu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xzd.svipenyu.cn

Go:   os.Remove("a.txt")
来源：http://gah.sufxvd.cn

Ruby: File.delete("a.txt")
来源：http://bnp.yj202588.top

C#:   File.Delete("a.txt");
来源：http://gjq.gogol.net.cn

[F07] 创建目录（含多级）
来源：http://uya.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gek.yongpay.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wbp.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://avp.wangdashe.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://olb.xziqi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ffi.ivvv.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zzj.fktsv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jkg.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mtj.hysaishi.cn

[F08] 遍历目录
来源：http://fnm.cheryme.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://txe.yuxming.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oda.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://rhj.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://ucc.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gar.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://etg.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://xnx.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://yrg.jinqigufen.top

[F09] 获取文件大小
来源：http://lwa.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://thu.vqdsnc.cn

PHP:  filesize("a.txt");
来源：http://pof.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://whc.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://nvx.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://yoe.hammf.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://omq.vqdsnc.cn

Ruby: File.size("a.txt")
来源：http://lje.fanxiaobao.xyz

C#:   new FileInfo("a.txt").Length
来源：http://qpq.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://yqu.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xrs.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iee.zhaomingkeji.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gnh.gogol.net.cn

TS:   path.extname("a.txt")
来源：http://rgv.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://the.nanxinkj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sow.chenlongwang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jqq.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qss.gzhubu.top

[F11] 复制与移动文件
来源：http://vjq.snrcjt.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tnw.yueranfly.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tub.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cub.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fkt.aibaodan.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hdr.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wuy.ctjpmb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zge.haohaochexian.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bzq.ctjpmb.com

[F12] CSV 读写
来源：http://dfg.yfazqb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mra.yvedp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://osc.gaohongyu789.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wim.zdbjq.cn

TS:   // 同上
来源：http://fhf.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bgw.tanke756.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oro.xingfuxueyuan.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lpx.havefunace.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sae.jqgufenzy.top

================================================================================
来源：http://ned.jqgfzy.top

G. 面向对象
来源：http://jok.daxiang520.top

================================================================================
来源：http://chu.gzhubu.top

[G01] 定义类
来源：http://isd.zhijiandao.cn

Py:   class User: pass
来源：http://bvf.cucudq.cn

PHP:  class User {}
来源：http://ikh.nanxinkj.top

JS:   class User {}
来源：http://ykh.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://etz.gogol.net.cn

Java: class User {}
来源：http://gjr.gaohongyu789.top

Go:   type User struct { Name string }
来源：http://rjj.shzxlz.cn

Ruby: class User; end
来源：http://llm.daria6918.cn

C#:   class User {}
来源：http://wpn.cqqwz.cn

[G02] 构造函数
来源：http://phz.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://dyj.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://udl.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://eku.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://ihy.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://gsr.yuanzhike.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ydt.ehwqpu.com

Ruby: def initialize(name); @name = name; end
来源：http://nxf.9152youxi.cn

C#:   public User(string name) { Name = name; }
来源：http://rhk.zhoulong.xyz

[G03] 实例属性
来源：http://rao.xinyue.icu

Py:   self.name = "x"
来源：http://coq.yueranfly.top

PHP:  public string $name = "x";
来源：http://tqn.ybcxt.top

JS:   this.name = "x";
来源：http://kxf.cqqwz.cn

TS:   name: string = "x";
来源：http://wwh.sysykeji.top

Java: private String name;
来源：http://vcs.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ikq.smart0.xyz

Ruby: @name = "x"
来源：http://vom.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://qyh.shuidangran.top

[G04] 定义方法
来源：http://sza.yvedp.cn

Py:   def greet(self): return self.name
来源：http://nyl.bjfxy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zok.wangdashe.top

JS:   greet() { return this.name; }
来源：http://ghf.xuanzx.com

TS:   greet(): string { return this.name; }
来源：http://xqr.tian-w.cn

Java: String greet() { return name; }
来源：http://fsp.guowangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bit.cucudq.cn

Ruby: def greet; @name; end
来源：http://tzz.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://quw.fanxiaobao.xyz

[G05] 继承
来源：http://npp.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://zwm.zycfv.cn

PHP:  class Admin extends User {}
来源：http://aed.guowangkeji.top

JS:   class Admin extends User {}
来源：http://oow.sufxvd.cn

TS:   class Admin extends User {}
来源：http://cmk.epnwcf.com

Java: class Admin extends User {}
来源：http://svj.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zrh.daxiang520.top

Ruby: class Admin < User; end
来源：http://wel.bbcook.cn

C#:   class Admin : User {}
来源：http://nls.cucudq.cn

[G06] 重写方法
来源：http://cjs.yj20258.top

Py:   def greet(self): return "admin"
来源：http://drn.zhixingplan.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kqg.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://fgw.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://qev.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://ken.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oin.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://xkr.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://ipy.jianghu66.top

[G07] 调用父类方法
来源：http://gqu.316326.xyz

Py:   super().greet()
来源：http://jfp.zdbjq.cn

PHP:  parent::greet();
来源：http://fbb.zhaomingkeji.xyz

JS:   super.greet();
来源：http://puc.tianlin.xyz

TS:   super.greet();
来源：http://kmi.yueranfly.top

Java: super.greet();
来源：http://dvs.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ztg.aizwys.cn

Ruby: super
来源：http://xjx.shuidangran.top

C#:   base.Greet();
来源：http://ytx.redwolf501.top

[G08] 静态方法与属性
来源：http://kwg.xuetiantiany.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qgv.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://mfm.nanxuanxn.top

JS:   static f() {}
来源：http://aik.zhengqikj.top

TS:   static f(): void {}
来源：http://lpp.ppjwa.cn

Java: static void f() {}
来源：http://qmu.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://umh.sxryk.cn

Ruby: def self.f; end
来源：http://rsv.chenjidiqi.icu

C#:   public static void F() {}
来源：http://dvi.fzhhl.top

[G09] 接口 / 抽象类
来源：http://mqs.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://jij.chenzaomai.com

PHP:  interface Shape { public function area(): float; }
来源：http://ikz.sufxvd.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uvh.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://rzz.hnqzz.top

Java: interface Shape { double area(); }
来源：http://hcr.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://ncl.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bjm.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://yzt.fzhhl.top

[G10] 访问控制
来源：http://wph.hcnkem.com

Py:   约定 _protected / __private（不强制）
来源：http://jvm.tian-w.cn

PHP:  public / protected / private
来源：http://frt.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://vre.hnqzz.top

TS:   public / protected / private
来源：http://erx.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://vvj.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hxh.jinghuilouyu.cn

Ruby: public / protected / private
来源：http://jkw.chenlongwang.top

C#:   public / protected / private / internal
来源：http://ocw.tarul.cn

[G11] getter / setter
来源：http://drd.jinyuanbaomall.cn

Py:   @property 与 @x.setter
来源：http://yoq.yuanzhike.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qsa.dianchejie.cn

JS:   get name() { return this._name; }
来源：http://ylf.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://euf.meibo888.top

Java: public String getName() { return name; }
来源：http://opa.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ccl.c1oappe.top

Ruby: attr_accessor :name
来源：http://aqb.dashuyun.cn

C#:   public string Name { get; set; }
来源：http://ily.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://ajs.c1oappe.top

Py:   def __str__(self): return self.name
来源：http://dqk.tarul.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nej.gogol.net.cn

JS:   toString() { return this.name; }
来源：http://ilm.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://ydy.zhijiandao.cn

Java: @Override public String toString() { return name; }
来源：http://yys.meibo888.top


<!-- 参考信息 -->