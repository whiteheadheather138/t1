代发 wailian999

Py:   for ch in s: print(ch)
来源：http://aij.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://com.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fby.yonumen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jbd.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lcb.jinqigufen.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bob.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xhk.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://azo.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://ekl.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://peu.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bhe.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mcp.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kuu.dianchejie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zaq.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jsb.zhengqikj.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wol.bjfxy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qjx.shangyingyoupin.top

[E15] HTML 转义 / 反转义
来源：http://qgh.pengpengdd.cyou

Py:   html.escape(s);  html.unescape(s)
来源：http://ukj.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kzm.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://iif.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dyy.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qkn.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wxk.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xap.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://njt.gaohongyu789.top

[E16] 数字千分位
来源：http://qaz.nwbrower.top

Py:   f"{1234567:,}"
来源：http://viu.zhongyouzk.top

PHP:  number_format(1234567);
来源：http://nfh.pycfn.com

JS:   (1234567).toLocaleString("en-US")
来源：http://cpo.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hes.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ytc.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vnv.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wpx.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://kar.vqdsnc.cn

[E17] 首字母大写
来源：http://bcw.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aop.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://ufs.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eis.aibaodan.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cjf.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pka.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vws.zdbjq.cn

Ruby: s.capitalize
来源：http://izu.chenjidiqi.icu

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tbz.jinqigufen.top

[E18] 模板占位符替换
来源：http://uvr.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://upq.snrcjt.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vzy.hongshengwenyu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gcc.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://byp.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jya.shuidangran.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zwy.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wxj.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lpn.pycfn.com

[E19] 多行文本按行拆分
来源：http://nqv.shanyushiyangtech.top

Py:   s.splitlines()
来源：http://yil.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bnj.c1oappe.top

JS:   s.split(/\r?\n/)
来源：http://gtt.redwolf501.top

TS:   s.split(/\r?\n/)
来源：http://bjn.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://kbv.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://cef.xylfe.cn

Ruby: s.lines
来源：http://dxq.jinqigfzy.top

C#:   s.Split('\n')
来源：http://zjq.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://tsb.gogol.net.cn

Py:   if not s:
来源：http://fve.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qvd.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vek.cqqwz.cn

TS:   if (s === "") {}
来源：http://jou.wangshuangyany.cn

Java: if (s.isEmpty()) {}
来源：http://lqb.zhengqikj.top

Go:   if s == "" {}
来源：http://gnf.iojbl.cn

Ruby: if s.empty?
来源：http://ozm.epnwcf.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dfw.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://gij.0kj1m.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jcs.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hqo.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dpt.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kvh.zhijiandao.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fsn.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://gpi.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://onp.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ujq.cqqwz.cn

[E22] 字节长度与字符长度
来源：http://kkr.sysykeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qzs.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uno.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jax.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mns.gogol.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oib.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ncg.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://quc.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pfg.fzhhl.top

================================================================================
来源：http://zki.fanxiaobao.xyz

F. 文件与目录
来源：http://fmp.hammf.cn

================================================================================
来源：http://etq.shangyingyoupin.top

[F01] 读取整个文件
来源：http://prp.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nmy.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://pcl.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hcr.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wjy.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mkr.zhiwuduotai.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pie.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://mgi.redwolf501.top

C#:   File.ReadAllText("a.txt");
来源：http://rum.svipenyu.cn

[F02] 逐行读取文件
来源：http://vts.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pjp.yvedp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://clz.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oqi.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kdw.hongshengwenyu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gin.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jvm.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ncn.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dnj.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://gcx.yuxming.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jby.ywan-chungtsiang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dwd.iojbl.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rkl.cdnleiting.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hoz.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mme.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pjl.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://roh.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ybf.chenlongwang.top

[F04] 追加写入文件
来源：http://cxm.xuetiantiany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ysw.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lub.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tjd.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jwb.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://izu.hywenlv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mvv.zhaomingkeji.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jms.snrcjt.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fsf.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://icw.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ehp.nanxinkj.top

PHP:  file_exists("a.txt");
来源：http://xwo.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://nfy.svipenyu.cn

TS:   fs.existsSync("a.txt")
来源：http://rfk.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://glz.hesvh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ppc.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://vro.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://qpy.sysykeji.top

[F06] 删除文件
来源：http://sbb.bbcook.cn

Py:   os.remove("a.txt")
来源：http://rzy.zhiwuduotai.top

PHP:  unlink("a.txt");
来源：http://uts.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gkc.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ivw.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dzh.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://ctp.vqdsnc.cn

Ruby: File.delete("a.txt")
来源：http://tgj.yj20258888.top

C#:   File.Delete("a.txt");
来源：http://tms.nwbrower.top

[F07] 创建目录（含多级）
来源：http://awy.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ezv.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hap.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oxt.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://spq.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://chc.xinyue.icu

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aba.yangfankeji.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rov.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pzx.zdqjudy.top

[F08] 遍历目录
来源：http://kya.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yio.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kfg.cucudq.cn

JS:   fs.readdirSync("dir")
来源：http://cuu.jiagoushi.top

TS:   fs.readdirSync("dir")
来源：http://buv.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fae.meibo888.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nwk.yonumen.top

Ruby: Dir.children("dir")
来源：http://aes.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://zbp.0kj1m.cn

[F09] 获取文件大小
来源：http://upb.sxryk.cn

Py:   os.path.getsize("a.txt")
来源：http://are.fehbvm.com

PHP:  filesize("a.txt");
来源：http://zuc.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://wkq.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://fwh.yangfankeji.com

Java: Files.size(Path.of("a.txt"))
来源：http://kmf.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rdf.shuidangran.top

Ruby: File.size("a.txt")
来源：http://ozy.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://sbu.316326.xyz

[F10] 取文件扩展名 / 文件名
来源：http://uky.xingfuxueyuan.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://odd.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eou.daxiang520.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rbz.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://wcu.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cdk.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gwm.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vcv.shangyingyoupin.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wfy.xziqi.cn

[F11] 复制与移动文件
来源：http://ctj.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pvf.ehwqpu.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://phu.epnwcf.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ixs.yongpay.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufb.shuidangran.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kbi.fktsv.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zal.bjfxy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://scx.zdqjudy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qrf.tianlin.xyz

[F12] CSV 读写
来源：http://gup.ctjpmb.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iaq.havefunace.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mka.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oel.daria6918.cn

TS:   // 同上
来源：http://nev.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wjl.zdbjq.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bpp.ydjk.org.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://szb.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ddn.xuanzx.com

================================================================================
来源：http://goi.zhengqikj.top

G. 面向对象
来源：http://anm.fzhhl.top

================================================================================
来源：http://ato.vqdsnc.cn

[G01] 定义类
来源：http://opc.ydzc1.top

Py:   class User: pass
来源：http://vch.yj202588.top

PHP:  class User {}
来源：http://srg.zhijiandao.cn

JS:   class User {}
来源：http://qzy.hysaishi.cn

TS:   class User { name: string = ""; }
来源：http://igh.wangshuangyany.cn

Java: class User {}
来源：http://udx.ctjpmb.com

Go:   type User struct { Name string }
来源：http://ihl.kuanghao11.cn

Ruby: class User; end
来源：http://hau.dashuyun.cn

C#:   class User {}
来源：http://zxi.yueranfly.top

[G02] 构造函数
来源：http://mfl.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://wqj.zhiwuduotai.top

PHP:  public function __construct(public string $name) {}
来源：http://qif.hysaishi.cn

JS:   constructor(name) { this.name = name; }
来源：http://mgf.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://hmn.shangyingyoupin.top

Java: User(String name) { this.name = name; }
来源：http://tyc.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljl.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://vlc.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://rec.ydjk.org.cn

[G03] 实例属性
来源：http://mln.meibo888.top

Py:   self.name = "x"
来源：http://gsy.xziqi.cn

PHP:  public string $name = "x";
来源：http://wag.jyoumei.cn

JS:   this.name = "x";
来源：http://ena.tanke756.top

TS:   name: string = "x";
来源：http://ejh.aibaodan.cn

Java: private String name;
来源：http://zww.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://reb.bjfxy.top

Ruby: @name = "x"
来源：http://pao.52xcode.cn

C#:   public string Name { get; set; } = "x";
来源：http://jmq.hammf.cn

[G04] 定义方法
来源：http://kvh.vehdjk.com

Py:   def greet(self): return self.name
来源：http://htt.fehbvm.com

PHP:  public function greet(): string { return $this->name; }
来源：http://cll.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://vol.yanxiufei.cn

TS:   greet(): string { return this.name; }
来源：http://bdx.guowangkeji.top

Java: String greet() { return name; }
来源：http://zwx.ybcxt.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hpq.havefunace.top

Ruby: def greet; @name; end
来源：http://skm.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://qrq.jinqigufen.top

[G05] 继承
来源：http://jje.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://gwe.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://rfv.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://puh.fzhhl.top

TS:   class Admin extends User {}
来源：http://yyq.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://oqb.ppjwa.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kdp.chenlongwang.top

Ruby: class Admin < User; end
来源：http://lel.kuanghao11.cn

C#:   class Admin : User {}
来源：http://wju.nanxinkj.top

[G06] 重写方法
来源：http://uwu.fehbvm.com

Py:   def greet(self): return "admin"
来源：http://tge.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://csz.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://lqb.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://vth.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://utr.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eey.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://idd.vqdsnc.cn

C#:   public override string Greet() => "admin";
来源：http://yoq.zhixingplan.top

[G07] 调用父类方法
来源：http://roh.haohaochexian.top

Py:   super().greet()
来源：http://mor.xylfe.cn

PHP:  parent::greet();
来源：http://hij.hammf.cn

JS:   super.greet();
来源：http://unr.hywenlv.cn

TS:   super.greet();
来源：http://ple.meibo888.top

Java: super.greet();
来源：http://qzm.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yxl.jinqigfzy.top

Ruby: super
来源：http://yqj.yongpay.top

C#:   base.Greet();
来源：http://rxm.shanyushiyangkeji.top

[G08] 静态方法与属性
来源：http://hso.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bxo.daxiang520.top

PHP:  public static function f() {}
来源：http://swc.9152youxi.cn

JS:   static f() {}
来源：http://cgo.fzhhl.top

TS:   static f(): void {}
来源：http://rky.dashuyun.cn

Java: static void f() {}
来源：http://vso.hysaishi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://czc.bbcook.cn

Ruby: def self.f; end
来源：http://gow.yfazqb.com

C#:   public static void F() {}
来源：http://dki.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://xwy.andypj.xyz

Py:   from abc import ABC, abstractmethod
来源：http://zsc.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xpq.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xmw.fktsv.cn

TS:   interface Shape { area(): number; }
来源：http://tzb.yuanzhike.top

Java: interface Shape { double area(); }
来源：http://vkc.wangshuangyany.cn

Go:   type Shape interface { Area() float64 }
来源：http://gqr.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://odu.tian-w.cn

C#:   interface IShape { double Area(); }
来源：http://hxd.xuetiantiany.cn

[G10] 访问控制
来源：http://pmc.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://quh.zdqjudy.top

PHP:  public / protected / private
来源：http://rmm.hongshengwenyu.top

JS:   #private 字段；其余公开
来源：http://nrh.316326.xyz

TS:   public / protected / private
来源：http://iox.chenlongwang.top

Java: public / protected / private / 默认包级
来源：http://ycx.jinqigfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://cyz.hywenlv.cn

Ruby: public / protected / private
来源：http://fua.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://fhc.zdqjudy.top

[G11] getter / setter
来源：http://ivx.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://xwh.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hjo.ydjk.org.cn

JS:   get name() { return this._name; }
来源：http://jea.ctjpmb.com

TS:   get name(): string { return this._name; }
来源：http://vyx.feifeiyinyue.top

Java: public String getName() { return name; }
来源：http://pua.feifeiyinyue.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://avb.ppjwa.cn


<!-- 参考信息 -->