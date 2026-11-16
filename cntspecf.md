代发 wailian999

[E14] URL 编码与 Base64
来源：http://veu.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nje.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eve.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wgt.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wvr.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ito.feifeiyinyue.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qzl.pycfn.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vzp.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wuv.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://mmr.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ikc.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dun.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://drz.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://aos.sufxvd.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xcp.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://myn.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fnr.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iva.svipenyu.cn

[E16] 数字千分位
来源：http://gzd.cheryme.top

Py:   f"{1234567:,}"
来源：http://jfg.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://cmy.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gwz.fktsv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xhr.redwolf501.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ril.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pov.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sgg.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://lrr.yongpay.top

[E17] 首字母大写
来源：http://dap.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gqj.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ure.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fqt.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jwu.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://umo.jinyuanbaomall.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bvt.ehwqpu.com

Ruby: s.capitalize
来源：http://lec.zhengqikj.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xnk.cqqwz.cn

[E18] 模板占位符替换
来源：http://qsk.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pgt.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sbl.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kum.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://deu.zhoulong.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bwl.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yhe.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bny.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lzc.daria6918.cn

[E19] 多行文本按行拆分
来源：http://hwf.andypj.xyz

Py:   s.splitlines()
来源：http://tuj.pycfn.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qgy.sweek.top

JS:   s.split(/\r?\n/)
来源：http://gph.tian-w.cn

TS:   s.split(/\r?\n/)
来源：http://wrb.pengpengdd.cyou

Java: s.lines().toList()
来源：http://wik.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://nkg.fengsongda.top

Ruby: s.lines
来源：http://scz.zhengqikj.top

C#:   s.Split('\n')
来源：http://sof.cheryme.top

[E20] 判断字符串是否为空
来源：http://opj.fengsongda.top

Py:   if not s:
来源：http://qpx.zhengqikj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ews.chenzaomai.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tls.cheryme.top

TS:   if (s === "") {}
来源：http://wjy.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://czg.jyoumei.cn

Go:   if s == "" {}
来源：http://abl.yvedp.cn

Ruby: if s.empty?
来源：http://akt.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://edf.aizwys.cn

[E21] 超长截断加省略号
来源：http://csf.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ibj.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bms.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jxj.cdnleiting.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hfd.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ipy.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://jwi.uphjek.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://apo.shanyushiyangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zpz.yj20258.top

[E22] 字节长度与字符长度
来源：http://kvg.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://txx.c1oappe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uge.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yvn.meibo888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xie.52xcode.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wgp.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dev.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://atb.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qky.cdnleiting.top

================================================================================
来源：http://xno.jinqigfzy.top

F. 文件与目录
来源：http://zrr.hywenlv.cn

================================================================================
来源：http://uxf.hammf.cn

[F01] 读取整个文件
来源：http://wyn.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nxz.9152youxi.cn

PHP:  file_get_contents("a.txt");
来源：http://vpu.shuidangran.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://umb.yuxming.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hwz.sjlbkw.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mml.xuanzx.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uap.yuxming.cn

Ruby: File.read("a.txt")
来源：http://pgw.ydjk.org.cn

C#:   File.ReadAllText("a.txt");
来源：http://ucz.xuanzx.com

[F02] 逐行读取文件
来源：http://knx.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nyk.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lri.vehdjk.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pzf.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jqu.cheryme.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rnf.yuanzhike.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tvu.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rfk.zhoulong.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sqj.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://ajx.jinyuanbaomall.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bjd.52xcode.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://avt.fanxiaobao.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rzu.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yex.yanxiufei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ysv.shanyushiyangkeji.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fst.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://vyd.feifeiyinyue.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dcu.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://hqa.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://phs.iojbl.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bmp.birdmap.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ilh.tanke756.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vdv.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ohs.quarkkingdee.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ldb.shuidangran.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ola.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wom.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://jzf.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://emf.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://agd.yueranfly.top

JS:   fs.existsSync("a.txt")
来源：http://omb.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://ghk.shuidangran.top

Java: Files.exists(Path.of("a.txt"))
来源：http://mpg.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wbo.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://asv.daxiang520.top

C#:   File.Exists("a.txt")
来源：http://yki.cucudq.cn

[F06] 删除文件
来源：http://mnd.quarkkingdee.top

Py:   os.remove("a.txt")
来源：http://vho.zycfv.cn

PHP:  unlink("a.txt");
来源：http://jox.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://yho.dashuyun.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ogj.zdqjudy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gls.zhiwuduotai.top

Go:   os.Remove("a.txt")
来源：http://lni.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://csf.yj202588.top

C#:   File.Delete("a.txt");
来源：http://epv.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://xtl.shuidangran.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rgu.xuetiantiany.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tgn.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zvq.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xbh.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://srk.zdbjq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lxs.vqdsnc.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fkw.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ula.zhongyouzk.top

[F08] 遍历目录
来源：http://bos.jinqigfzy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eex.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ysf.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://ynw.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://geb.iojbl.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uxy.sxryk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lbu.daria6918.cn

Ruby: Dir.children("dir")
来源：http://tpd.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://cer.nwbrower.top

[F09] 获取文件大小
来源：http://dsu.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://znd.yonumen.top

PHP:  filesize("a.txt");
来源：http://tmy.9152youxi.cn

JS:   fs.statSync("a.txt").size
来源：http://mrj.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://pfk.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://hao.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fpn.gaohongyu789.top

Ruby: File.size("a.txt")
来源：http://sot.chenjidiqi.icu

C#:   new FileInfo("a.txt").Length
来源：http://ttj.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://lmh.nanxinkj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://szg.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rzp.nanxuanxn.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qpe.hcnkem.com

TS:   path.extname("a.txt")
来源：http://cci.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xzc.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fha.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ucs.tianlin.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dnh.guannengcc.top

[F11] 复制与移动文件
来源：http://cem.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uly.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tyv.aibaodan.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzp.bjfxy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kyl.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xqn.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://han.wangshuangyany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rrq.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://edq.vqdsnc.cn

[F12] CSV 读写
来源：http://xqb.jqgfzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sgi.ctjpmb.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qdt.cashguo.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qvj.316326.xyz

TS:   // 同上
来源：http://ued.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nch.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ukx.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pii.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://qul.cashguo.top

================================================================================
来源：http://jbj.nwbrower.top

G. 面向对象
来源：http://dnp.hnxiangtu.top

================================================================================
来源：http://tvg.zycfv.cn

[G01] 定义类
来源：http://zjy.9152youxi.cn

Py:   class User: pass
来源：http://biq.zycfv.cn

PHP:  class User {}
来源：http://unv.wangshuangyany.cn

JS:   class User {}
来源：http://xbk.tanke756.top

TS:   class User { name: string = ""; }
来源：http://fjq.nwbrower.top

Java: class User {}
来源：http://pfb.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://wka.guannengcc.top

Ruby: class User; end
来源：http://eyi.tarul.cn

C#:   class User {}
来源：http://dty.dianchejie.cn

[G02] 构造函数
来源：http://hyu.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://epp.cqqwz.cn

PHP:  public function __construct(public string $name) {}
来源：http://apu.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://nft.ydjk.org.cn

TS:   constructor(public name: string) {}
来源：http://tut.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://ryw.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ely.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://ieo.yfazqb.com

C#:   public User(string name) { Name = name; }
来源：http://sfw.bbcook.cn

[G03] 实例属性
来源：http://vsu.iojbl.cn

Py:   self.name = "x"
来源：http://ojy.yueranfly.top

PHP:  public string $name = "x";
来源：http://tcu.hnqzz.top

JS:   this.name = "x";
来源：http://ytr.sxryk.cn

TS:   name: string = "x";
来源：http://iqc.ctjpmb.com

Java: private String name;
来源：http://agj.aizwys.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://edn.xinyue.icu

Ruby: @name = "x"
来源：http://agu.uphjek.com

C#:   public string Name { get; set; } = "x";
来源：http://eus.fengsongda.top

[G04] 定义方法
来源：http://yex.yj20258.top

Py:   def greet(self): return self.name
来源：http://xeg.jinqigfzy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hkc.uphjek.com

JS:   greet() { return this.name; }
来源：http://cxx.hammf.cn

TS:   greet(): string { return this.name; }
来源：http://hwg.yj202588.top

Java: String greet() { return name; }
来源：http://zuk.zhoulong.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://hxw.gaohongyu789.top

Ruby: def greet; @name; end
来源：http://ujg.yj202588.top

C#:   public string Greet() => Name;
来源：http://dwq.yongpay.top

[G05] 继承
来源：http://ocu.bjfxy.top

Py:   class Admin(User): pass
来源：http://rhr.xylfe.cn

PHP:  class Admin extends User {}
来源：http://pgv.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://qvc.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://edf.aibaodan.cn

Java: class Admin extends User {}
来源：http://axz.jinqigfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rve.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://fcg.ppjwa.cn

C#:   class Admin : User {}
来源：http://pqb.sweek.top

[G06] 重写方法
来源：http://yzj.iojbl.cn

Py:   def greet(self): return "admin"
来源：http://nls.mhx1999.top

PHP:  public function greet(): string { return "admin"; }
来源：http://txf.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://ymy.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://mkn.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://bpn.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iss.cucudq.cn

Ruby: def greet; "admin"; end
来源：http://xqp.sweek.top

C#:   public override string Greet() => "admin";
来源：http://dnz.zdqjudy.top

[G07] 调用父类方法
来源：http://ads.ppjwa.cn

Py:   super().greet()
来源：http://sza.ydjk.org.cn

PHP:  parent::greet();
来源：http://owm.sweek.top

JS:   super.greet();
来源：http://bhl.yj20258.top

TS:   super.greet();
来源：http://lxt.fanxiaobao.xyz

Java: super.greet();
来源：http://weo.jinqigfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kyv.bjfxy.top

Ruby: super
来源：http://kpx.zhongyouzk.top

C#:   base.Greet();
来源：http://jtm.zdbjq.cn

[G08] 静态方法与属性
来源：http://bmi.jianghu66.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qui.dianchejie.cn

PHP:  public static function f() {}
来源：http://iwl.jiagoushi.top

JS:   static f() {}
来源：http://lss.ydjk.org.cn

TS:   static f(): void {}
来源：http://cgh.ywan-chungtsiang.top

Java: static void f() {}
来源：http://rmv.gzhubu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nke.xylfe.cn

Ruby: def self.f; end
来源：http://jtk.vqdsnc.cn

C#:   public static void F() {}
来源：http://pnw.ydzc1.top

[G09] 接口 / 抽象类
来源：http://xbi.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://kzm.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://lbf.jlsjyb.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rdg.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://jeo.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://jbv.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://kks.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://emp.fzhhl.top

C#:   interface IShape { double Area(); }
来源：http://lcp.guannengcc.top

[G10] 访问控制
来源：http://hsf.kuanghao11.cn

Py:   约定 _protected / __private（不强制）
来源：http://dxr.zhaomingkeji.xyz

PHP:  public / protected / private
来源：http://mww.zhijiandao.cn

JS:   #private 字段；其余公开
来源：http://pnk.birdmap.top

TS:   public / protected / private
来源：http://puu.hcnkem.com

Java: public / protected / private / 默认包级
来源：http://rca.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xqy.guannengcc.top

Ruby: public / protected / private
来源：http://poa.smart0.xyz

C#:   public / protected / private / internal
来源：http://ach.316326.xyz

[G11] getter / setter
来源：http://wie.bbcook.cn

Py:   @property 与 @x.setter
来源：http://fww.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qnt.52xcode.cn

JS:   get name() { return this._name; }
来源：http://hqb.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://ayp.yonumen.top

Java: public String getName() { return name; }
来源：http://tum.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iyg.shuidangran.top

Ruby: attr_accessor :name
来源：http://mra.yongpay.top

C#:   public string Name { get; set; }
来源：http://gyt.hysaishi.cn

[G12] 对象转字符串
来源：http://hkm.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://dpo.xingfuxueyuan.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://coq.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://qbl.jlsjyb.cn

TS:   toString(): string { return this.name; }
来源：http://war.mhx1999.top

Java: @Override public String toString() { return name; }
来源：http://fyl.birdmap.top


<!-- 参考信息 -->