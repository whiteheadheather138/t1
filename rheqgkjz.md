代发 wailian999

PHP:  substr_count($s, "a");
来源：http://jjb.chenzaomai.com

JS:   s.split("a").length - 1
来源：http://yzx.gzhubu.top

TS:   s.split("a").length - 1
来源：http://xxi.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gzm.tianlin.xyz

Go:   strings.Count(s, "a")
来源：http://rps.aizwys.cn

Ruby: s.count("a")
来源：http://isw.bbcook.cn

C#:   s.Count(c => c == 'a')
来源：http://kon.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://mxw.havefunace.top

Py:   for ch in s: print(ch)
来源：http://yyx.dashuyun.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dse.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://avn.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ibc.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vak.nanxuanxn.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ssg.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://hlj.guannengcc.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bnw.c1oappe.top

[E14] URL 编码与 Base64
来源：http://lwi.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sst.jinyuanbaomall.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bvu.hysaishi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qlh.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xgj.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://awn.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://akp.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xzj.xingfuxueyuan.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zvh.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://vlc.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xlr.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nfi.52xcode.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tqf.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pny.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ika.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tjt.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uro.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://imy.fanxiaobao.xyz

[E16] 数字千分位
来源：http://boa.yvedp.cn

Py:   f"{1234567:,}"
来源：http://tpj.yongpay.top

PHP:  number_format(1234567);
来源：http://zle.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vqi.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lty.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ier.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zws.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bsl.tanke756.top

C#:   1234567.ToString("N0")
来源：http://hjp.hnqzz.top

[E17] 首字母大写
来源：http://gdj.fzhhl.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rgq.svipenyu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dwn.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pfq.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://axp.cucudq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vlb.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rcr.andypj.xyz

Ruby: s.capitalize
来源：http://zlz.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cyh.fzhhl.top

[E18] 模板占位符替换
来源：http://qpf.feifeiyinyue.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vcw.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mfx.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fav.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://psw.chenzaomai.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ozu.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ics.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gem.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vjj.tian-w.cn

[E19] 多行文本按行拆分
来源：http://cki.nwbrower.top

Py:   s.splitlines()
来源：http://fiw.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fmf.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://awr.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://vbm.wangshuangyany.cn

Java: s.lines().toList()
来源：http://ldu.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://exq.tianlin.xyz

Ruby: s.lines
来源：http://tmm.nanxuanxn.top

C#:   s.Split('\n')
来源：http://qlp.yfazqb.com

[E20] 判断字符串是否为空
来源：http://jgi.xingfuxueyuan.xyz

Py:   if not s:
来源：http://fic.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cek.zhiwuduotai.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xeb.c1oappe.top

TS:   if (s === "") {}
来源：http://nfk.zhaomingkeji.xyz

Java: if (s.isEmpty()) {}
来源：http://fem.xziqi.cn

Go:   if s == "" {}
来源：http://zyl.tian-w.cn

Ruby: if s.empty?
来源：http://rlw.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://aec.daria6918.cn

[E21] 超长截断加省略号
来源：http://xhs.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ykp.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://exq.zdbjq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdc.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fdo.fktsv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pcy.tarul.cn

Go:   // 按 rune 判断长度后截断
来源：http://ene.xingfuxueyuan.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eal.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xea.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://mwc.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fuy.sysykeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzy.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vle.vehdjk.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eow.jinqigufen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lzu.havefunace.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jxp.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://kus.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://okt.fzhhl.top

================================================================================
来源：http://dnw.jinyuanbaomall.cn

F. 文件与目录
来源：http://iwe.xingfuxueyuan.xyz

================================================================================
来源：http://dqf.zhoulong.xyz

[F01] 读取整个文件
来源：http://deh.quarkkingdee.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vmw.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://qwp.zhongyouzk.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ydi.tarul.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vlt.ydjk.org.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pnf.daria6918.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqq.epnwcf.com

Ruby: File.read("a.txt")
来源：http://ies.zhixingplan.top

C#:   File.ReadAllText("a.txt");
来源：http://jmd.nanxinkj.top

[F02] 逐行读取文件
来源：http://hbp.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ueh.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dzt.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xmi.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ykj.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wcm.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://nso.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tse.yuanzhike.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wbg.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://rvm.316326.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lii.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fvd.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cfb.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zcs.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pbd.yj20258888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xgy.vqdsnc.cn

Ruby: File.write("a.txt", "hi")
来源：http://qem.fengsongda.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dek.tanke756.top

[F04] 追加写入文件
来源：http://qjc.jiagoushi.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://iei.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kke.guannengcc.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gsx.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yqg.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vts.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://msj.ppjwa.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ldn.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rxf.tianlin.xyz

[F05] 判断文件或目录是否存在
来源：http://ecx.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zha.nanxuanxn.top

PHP:  file_exists("a.txt");
来源：http://jjm.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://shu.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://pmc.fehbvm.com

Java: Files.exists(Path.of("a.txt"))
来源：http://fui.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lwm.hongshengwenyu.top

Ruby: File.exist?("a.txt")
来源：http://tax.jiagoushi.top

C#:   File.Exists("a.txt")
来源：http://xsa.52xcode.cn

[F06] 删除文件
来源：http://brs.dashuyun.cn

Py:   os.remove("a.txt")
来源：http://hue.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://igs.hongshengwenyu.top

JS:   fs.unlinkSync("a.txt")
来源：http://tar.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://vwo.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://liv.shangyingyoupin.top

Go:   os.Remove("a.txt")
来源：http://pkc.yj202588.top

Ruby: File.delete("a.txt")
来源：http://uek.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://tvi.birdmap.top

[F07] 创建目录（含多级）
来源：http://mnu.uphjek.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://klb.jianghu66.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sjk.xingfuxueyuan.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jtb.bjfxy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ihr.nwbrower.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ouv.ydzc1.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dln.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://csl.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://adj.jlsjyb.cn

[F08] 遍历目录
来源：http://kej.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kgx.gaohongyu789.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gjh.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://zft.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://zdf.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://olv.birdmap.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://keh.xziqi.cn

Ruby: Dir.children("dir")
来源：http://tjo.zhengqikj.top

C#:   Directory.GetFiles("dir")
来源：http://yhd.wangshuangyany.cn

[F09] 获取文件大小
来源：http://afn.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://nhm.tian-w.cn

PHP:  filesize("a.txt");
来源：http://wno.shzxlz.cn

JS:   fs.statSync("a.txt").size
来源：http://ose.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://cii.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://pob.yonumen.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fhg.guannengcc.top

Ruby: File.size("a.txt")
来源：http://bpm.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://hzn.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://ixb.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ebp.xingfuxueyuan.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vui.ctjpmb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hqq.yanxiufei.cn

TS:   path.extname("a.txt")
来源：http://mce.xziqi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vvy.c1oappe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bjq.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bio.daxiang520.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ebh.xylfe.cn

[F11] 复制与移动文件
来源：http://cjg.sweek.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fgv.ydzc1.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xll.ehwqpu.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fqh.quarkkingdee.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tfi.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ybe.jyoumei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://olp.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eqe.gogol.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kpt.ydjk.org.cn

[F12] CSV 读写
来源：http://fen.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nln.dashuyun.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xkd.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blv.mhx1999.top

TS:   // 同上
来源：http://zjy.cheryme.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cyw.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wbt.tarul.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tek.sysykeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tbf.chenjidiqi.icu

================================================================================
来源：http://bvn.52xcode.cn

G. 面向对象
来源：http://zsk.fengsongda.top

================================================================================
来源：http://wyx.redwolf501.top

[G01] 定义类
来源：http://mdn.ctjpmb.com

Py:   class User: pass
来源：http://tep.redwolf501.top

PHP:  class User {}
来源：http://wmc.zhixingplan.top

JS:   class User {}
来源：http://nyn.c1oappe.top

TS:   class User { name: string = ""; }
来源：http://ztf.fengsongda.top

Java: class User {}
来源：http://cas.sxryk.cn

Go:   type User struct { Name string }
来源：http://mtc.hcnkem.com

Ruby: class User; end
来源：http://wco.vqdsnc.cn

C#:   class User {}
来源：http://dsm.zhongyouzk.top

[G02] 构造函数
来源：http://tui.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://vfl.shzxlz.cn

PHP:  public function __construct(public string $name) {}
来源：http://jzc.zdqjudy.top

JS:   constructor(name) { this.name = name; }
来源：http://vac.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://dqe.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://ghb.zhoulong.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ede.svipenyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://qux.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://zlv.0kj1m.cn

[G03] 实例属性
来源：http://clq.zhiwuduotai.top

Py:   self.name = "x"
来源：http://wwl.daxiang520.top

PHP:  public string $name = "x";
来源：http://cav.ybcxt.top

JS:   this.name = "x";
来源：http://mbs.zhijiandao.cn

TS:   name: string = "x";
来源：http://ohe.snrcjt.cn

Java: private String name;
来源：http://tru.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lcr.zhixingplan.top

Ruby: @name = "x"
来源：http://gwd.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://sfj.havefunace.top

[G04] 定义方法
来源：http://qlr.yfazqb.com

Py:   def greet(self): return self.name
来源：http://aan.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lpk.haohaochexian.top

JS:   greet() { return this.name; }
来源：http://asl.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://jpz.xuanzx.com

Java: String greet() { return name; }
来源：http://moy.yj20258.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ifg.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://ace.yuanzhike.top

C#:   public string Greet() => Name;
来源：http://pkm.havefunace.top

[G05] 继承
来源：http://quj.meibo888.top

Py:   class Admin(User): pass
来源：http://fnb.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://mft.ivvv.top

JS:   class Admin extends User {}
来源：http://tur.smart0.xyz

TS:   class Admin extends User {}
来源：http://jbr.yj20258.top

Java: class Admin extends User {}
来源：http://mtz.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kzh.yj20258888.top

Ruby: class Admin < User; end
来源：http://fux.sweek.top

C#:   class Admin : User {}
来源：http://hbw.shanyushiyangkeji.top

[G06] 重写方法
来源：http://cad.52xcode.cn

Py:   def greet(self): return "admin"
来源：http://ohm.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bdi.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://cnp.fengsongda.top

TS:   greet(): string { return "admin"; }
来源：http://xua.snrcjt.cn

Java: @Override String greet() { return "admin"; }
来源：http://oev.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tnr.jlsjyb.cn

Ruby: def greet; "admin"; end
来源：http://htl.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://nhd.gzhubu.top

[G07] 调用父类方法
来源：http://yzo.yj20258888.top

Py:   super().greet()
来源：http://wei.quarkkingdee.top

PHP:  parent::greet();
来源：http://pwy.tanke756.top

JS:   super.greet();
来源：http://wbt.tianlin.xyz

TS:   super.greet();
来源：http://uny.cheryme.top

Java: super.greet();
来源：http://bbx.vehdjk.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ijt.cashguo.top

Ruby: super
来源：http://duc.zhaomingkeji.xyz

C#:   base.Greet();
来源：http://xlr.zhiwuduotai.top

[G08] 静态方法与属性
来源：http://vjl.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ilr.smart0.xyz

PHP:  public static function f() {}
来源：http://jwf.havefunace.top

JS:   static f() {}
来源：http://yje.fktsv.cn

TS:   static f(): void {}
来源：http://val.feifeiyinyue.top

Java: static void f() {}
来源：http://hsc.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vgr.aibaodan.cn

Ruby: def self.f; end
来源：http://cbc.ydzc1.top

C#:   public static void F() {}
来源：http://rxk.tanke756.top

[G09] 接口 / 抽象类
来源：http://efx.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://fcg.hammf.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ltp.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://imx.fanxiaobao.xyz

TS:   interface Shape { area(): number; }
来源：http://lee.ehwqpu.com

Java: interface Shape { double area(); }
来源：http://sjd.quarkkingdee.top

Go:   type Shape interface { Area() float64 }
来源：http://rdf.xziqi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oem.jinqigufen.top

C#:   interface IShape { double Area(); }
来源：http://tbk.fehbvm.com

[G10] 访问控制
来源：http://bte.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://rbe.birdmap.top

PHP:  public / protected / private
来源：http://phs.bjfxy.top

JS:   #private 字段；其余公开
来源：http://tho.yangfankeji.com

TS:   public / protected / private
来源：http://tij.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://urm.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zuc.aibaodan.cn

Ruby: public / protected / private
来源：http://cnq.jinyuanbaomall.cn


<!-- 参考信息 -->