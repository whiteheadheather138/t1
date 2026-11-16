代发 wailian999

Go:   strings.Count(s, "a")
来源：http://ohe.hongshengwenyu.top

Ruby: s.count("a")
来源：http://unq.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://yvd.shangyingyoupin.top

[E13] 逐字符遍历
来源：http://snd.xingfuxueyuan.xyz

Py:   for ch in s: print(ch)
来源：http://ubn.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pec.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fam.chenjidiqi.icu

TS:   for (const ch of s) { console.log(ch); }
来源：http://nua.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nav.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jco.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xce.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://iyr.xuetiantiany.cn

[E14] URL 编码与 Base64
来源：http://wyn.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qqa.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://eoj.yfazqb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tuk.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://puk.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lys.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sfh.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mbf.cashguo.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ppy.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://mtx.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ueo.xylfe.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://imn.xylfe.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jeg.tarul.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://utd.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fwp.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://okl.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yhz.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tys.shanyushiyangtech.top

[E16] 数字千分位
来源：http://syy.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://xlj.ctjpmb.com

PHP:  number_format(1234567);
来源：http://tdo.ehwqpu.com

JS:   (1234567).toLocaleString("en-US")
来源：http://fqr.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://asv.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qtz.zdbjq.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iro.jinqigfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mwm.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://vfv.zhongyouzk.top

[E17] 首字母大写
来源：http://utw.meibo888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tfx.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tbu.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fjj.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fpd.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oze.zhengqikj.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ydw.nanxuanxn.top

Ruby: s.capitalize
来源：http://tjn.ctjpmb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tqe.pycfn.com

[E18] 模板占位符替换
来源：http://wzr.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://eml.cucudq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzo.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ptt.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xzc.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cmh.redwolf501.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fbg.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nuf.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cxj.yj202588.top

[E19] 多行文本按行拆分
来源：http://ysv.sweek.top

Py:   s.splitlines()
来源：http://sln.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kze.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://ykq.jiagoushi.top

TS:   s.split(/\r?\n/)
来源：http://pjb.tanke756.top

Java: s.lines().toList()
来源：http://yyx.wangdashe.top

Go:   strings.Split(s, "\n")
来源：http://jao.vqdsnc.cn

Ruby: s.lines
来源：http://qry.gzhubu.top

C#:   s.Split('\n')
来源：http://flx.yj20258.top

[E20] 判断字符串是否为空
来源：http://gbb.fzhhl.top

Py:   if not s:
来源：http://ldp.yangfankeji.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zxf.xuanzx.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cpn.zdqjudy.top

TS:   if (s === "") {}
来源：http://goa.yj20258.top

Java: if (s.isEmpty()) {}
来源：http://elf.shuidangran.top

Go:   if s == "" {}
来源：http://eob.chenjidiqi.icu

Ruby: if s.empty?
来源：http://cgo.shzxlz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wox.gogol.net.cn

[E21] 超长截断加省略号
来源：http://fgh.shanyushiyangtech.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://roc.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gjm.aibaodan.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://orr.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wwe.yvedp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aum.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://pgq.xylfe.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kzh.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rdv.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://fls.fanxiaobao.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zau.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gsy.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wbf.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kzb.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yes.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mgl.vqdsnc.cn

Ruby: s.bytesize;  s.length
来源：http://tam.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://odu.yj20258888.top

================================================================================
来源：http://cif.zhaomingkeji.xyz

F. 文件与目录
来源：http://qmd.nwbrower.top

================================================================================
来源：http://uty.zdqjudy.top

[F01] 读取整个文件
来源：http://ccp.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://das.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://nzd.jiagoushi.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uqf.andypj.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cap.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dxq.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://znf.cashguo.top

Ruby: File.read("a.txt")
来源：http://lpf.xuetiantiany.cn

C#:   File.ReadAllText("a.txt");
来源：http://dld.ehwqpu.com

[F02] 逐行读取文件
来源：http://fof.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hrw.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ifa.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://giu.aibaodan.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxk.yvedp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rmx.andypj.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ryg.0kj1m.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pcu.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vkx.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://ibx.chenjidiqi.icu

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mpm.zhoulong.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://rrs.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://saq.gogol.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eqw.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://apr.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qjk.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://rut.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nuv.ybcxt.top

[F04] 追加写入文件
来源：http://lsg.aibaodan.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zcu.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qfm.yj202588.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ucz.jinghuilouyu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wua.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vvl.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rab.ywan-chungtsiang.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ifq.quarkkingdee.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fqa.wangshuangyany.cn

[F05] 判断文件或目录是否存在
来源：http://zzy.jianghu66.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dur.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://iod.bjfxy.top

JS:   fs.existsSync("a.txt")
来源：http://kdw.shuidangran.top

TS:   fs.existsSync("a.txt")
来源：http://huz.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tfv.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://joe.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://muk.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://jwn.jianghu66.top

[F06] 删除文件
来源：http://mcy.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://npm.hammf.cn

PHP:  unlink("a.txt");
来源：http://mza.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://exv.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://kda.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oyq.ywan-chungtsiang.top

Go:   os.Remove("a.txt")
来源：http://gwr.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://wnf.hammf.cn

C#:   File.Delete("a.txt");
来源：http://bdz.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://dwf.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qtk.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dee.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mgd.9152youxi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qpj.sxryk.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://val.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://whq.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nkz.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://boj.tarul.cn

[F08] 遍历目录
来源：http://wuz.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://qqb.daxiang520.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wvg.jqgufenzy.top

JS:   fs.readdirSync("dir")
来源：http://qmc.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://aog.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xnf.aibaodan.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://abg.jianghu66.top

Ruby: Dir.children("dir")
来源：http://bey.yanxiufei.cn

C#:   Directory.GetFiles("dir")
来源：http://lbz.vqdsnc.cn

[F09] 获取文件大小
来源：http://jfo.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://npg.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://ieh.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://kql.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://brg.uphjek.com

Java: Files.size(Path.of("a.txt"))
来源：http://edl.tanke756.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ajb.meibo888.top

Ruby: File.size("a.txt")
来源：http://xfx.fengsongda.top

C#:   new FileInfo("a.txt").Length
来源：http://sim.haohaochexian.top

[F10] 取文件扩展名 / 文件名
来源：http://qme.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://asc.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zks.snrcjt.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ajm.yj20258.top

TS:   path.extname("a.txt")
来源：http://uto.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://foy.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aoa.birdmap.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://awt.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iwn.hnqzz.top

[F11] 复制与移动文件
来源：http://zha.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xkj.pengpengdd.cyou

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dgb.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wah.chenzaomai.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vam.zdqjudy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yxm.ybcxt.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yrl.quarkkingdee.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qkk.iojbl.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uxk.hammf.cn

[F12] CSV 读写
来源：http://iid.cashguo.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rtd.9152youxi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gvc.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://owo.zhaomingkeji.xyz

TS:   // 同上
来源：http://hkl.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wxj.hcnkem.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pol.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kns.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://udb.wangshuangyany.cn

================================================================================
来源：http://isk.dashuyun.cn

G. 面向对象
来源：http://xab.zhoulong.xyz

================================================================================
来源：http://llh.meibo888.top

[G01] 定义类
来源：http://uth.iojbl.cn

Py:   class User: pass
来源：http://vzd.gaohongyu789.top

PHP:  class User {}
来源：http://rzv.gzhubu.top

JS:   class User {}
来源：http://rfm.jqgufenzy.top

TS:   class User { name: string = ""; }
来源：http://rxa.nwbrower.top

Java: class User {}
来源：http://pjw.uphjek.com

Go:   type User struct { Name string }
来源：http://xzc.chenjidiqi.icu

Ruby: class User; end
来源：http://yyr.xuetiantiany.cn

C#:   class User {}
来源：http://fto.vqdsnc.cn

[G02] 构造函数
来源：http://rez.dashuyun.cn

Py:   def __init__(self, name): self.name = name
来源：http://jau.ivvv.top

PHP:  public function __construct(public string $name) {}
来源：http://lcr.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://cyk.uphjek.com

TS:   constructor(public name: string) {}
来源：http://rmj.mhx1999.top

Java: User(String name) { this.name = name; }
来源：http://gfi.sxryk.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wiw.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://exp.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://xtf.ivvv.top

[G03] 实例属性
来源：http://sib.cdnleiting.top

Py:   self.name = "x"
来源：http://nqv.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://zqj.fehbvm.com

JS:   this.name = "x";
来源：http://hby.uphjek.com

TS:   name: string = "x";
来源：http://kqi.hcnkem.com

Java: private String name;
来源：http://hni.yuxming.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uuk.wangdashe.top

Ruby: @name = "x"
来源：http://dnl.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://suo.zhijiandao.cn

[G04] 定义方法
来源：http://cgg.xingfuxueyuan.xyz

Py:   def greet(self): return self.name
来源：http://iqi.aibaodan.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vad.birdmap.top

JS:   greet() { return this.name; }
来源：http://bfo.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://vfb.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://jsf.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gml.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://hyw.fzhhl.top

C#:   public string Greet() => Name;
来源：http://nda.uphjek.com

[G05] 继承
来源：http://ybq.yangfankeji.com

Py:   class Admin(User): pass
来源：http://gte.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://bru.chenjidiqi.icu

JS:   class Admin extends User {}
来源：http://ppp.andypj.xyz

TS:   class Admin extends User {}
来源：http://xgl.jiagoushi.top

Java: class Admin extends User {}
来源：http://ewi.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://evo.cheryme.top

Ruby: class Admin < User; end
来源：http://hre.hywenlv.cn

C#:   class Admin : User {}
来源：http://esj.jinghuilouyu.cn

[G06] 重写方法
来源：http://ljp.yanxiufei.cn

Py:   def greet(self): return "admin"
来源：http://lsv.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lzw.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://ysr.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://ruc.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://uwh.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://syb.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://xfz.9152youxi.cn

C#:   public override string Greet() => "admin";
来源：http://nad.jyoumei.cn

[G07] 调用父类方法
来源：http://rih.smart0.xyz

Py:   super().greet()
来源：http://hij.zycfv.cn

PHP:  parent::greet();
来源：http://oer.zhixingplan.top

JS:   super.greet();
来源：http://wqj.hnqzz.top

TS:   super.greet();
来源：http://eqn.zhengqikj.top

Java: super.greet();
来源：http://acd.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eii.hammf.cn

Ruby: super
来源：http://myu.sweek.top

C#:   base.Greet();
来源：http://cye.nanxinkj.top

[G08] 静态方法与属性
来源：http://xbs.jinghuilouyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vgu.ehwqpu.com

PHP:  public static function f() {}
来源：http://tsk.yvedp.cn

JS:   static f() {}
来源：http://fli.epnwcf.com

TS:   static f(): void {}
来源：http://wpo.jlsjyb.cn

Java: static void f() {}
来源：http://bzq.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cge.vqdsnc.cn

Ruby: def self.f; end
来源：http://cit.yfazqb.com

C#:   public static void F() {}
来源：http://cjv.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://ctm.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://zeb.fehbvm.com

PHP:  interface Shape { public function area(): float; }
来源：http://hvr.wangshuangyany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://onq.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://nwh.hongshengwenyu.top

Java: interface Shape { double area(); }
来源：http://pjl.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://tbv.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vkt.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://nyh.chenlongwang.top

[G10] 访问控制
来源：http://vkz.gogol.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://dha.nwbrower.top

PHP:  public / protected / private
来源：http://wqg.jinqigfzy.top

JS:   #private 字段；其余公开
来源：http://dhg.meibo888.top

TS:   public / protected / private
来源：http://hvv.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://ahu.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qpk.pengpengdd.cyou

Ruby: public / protected / private
来源：http://qaw.yuxming.cn

C#:   public / protected / private / internal
来源：http://aox.chenlongwang.top

[G11] getter / setter
来源：http://gcp.feifeiyinyue.top

Py:   @property 与 @x.setter
来源：http://eyv.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://dvb.chenjidiqi.icu


<!-- 参考信息 -->