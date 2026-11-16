代发 wailian999

PHP:  substr_count($s, "a");
来源：http://rbv.ehwqpu.com

JS:   s.split("a").length - 1
来源：http://ixr.zhengqikj.top

TS:   s.split("a").length - 1
来源：http://fgy.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ksd.iojbl.cn

Go:   strings.Count(s, "a")
来源：http://nbu.ybcxt.top

Ruby: s.count("a")
来源：http://ahq.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://wan.ydzc1.top

[E13] 逐字符遍历
来源：http://fxf.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://jdh.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xqf.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://chy.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tdv.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://thv.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://htr.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://geg.svipenyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eym.mhx1999.top

[E14] URL 编码与 Base64
来源：http://mga.jinyuanbaomall.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dvb.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rxz.yanxiufei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bqm.yangfankeji.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tyx.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hob.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cre.tanke756.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qqx.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pai.quarkkingdee.top

[E15] HTML 转义 / 反转义
来源：http://eff.aizwys.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uyp.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rgi.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rbe.yuxming.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vhb.aizwys.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mqm.dianchejie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bvp.ivvv.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zmj.cqqwz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vuv.shanyushiyangkeji.top

[E16] 数字千分位
来源：http://oec.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://hgq.havefunace.top

PHP:  number_format(1234567);
来源：http://ghy.vehdjk.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wdd.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lbl.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hmm.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://orv.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dym.jianghu66.top

C#:   1234567.ToString("N0")
来源：http://fqj.dashuyun.cn

[E17] 首字母大写
来源：http://xkv.bbcook.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://prb.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://tok.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hwm.jinqigufen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zto.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jmn.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yhm.yueranfly.top

Ruby: s.capitalize
来源：http://mwx.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hlw.jqgfzy.top

[E18] 模板占位符替换
来源：http://qbh.zhongyouzk.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://scb.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fyv.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://ajb.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pej.jqgufenzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wrl.pengpengdd.cyou

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ces.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zvv.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://shf.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://klf.hongshengwenyu.top

Py:   s.splitlines()
来源：http://jrr.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pki.tianlin.xyz

JS:   s.split(/\r?\n/)
来源：http://ymn.nanxinkj.top

TS:   s.split(/\r?\n/)
来源：http://way.hesvh.cn

Java: s.lines().toList()
来源：http://fih.mhx1999.top

Go:   strings.Split(s, "\n")
来源：http://ktw.chenjidiqi.icu

Ruby: s.lines
来源：http://gat.hfpthk.cn

C#:   s.Split('\n')
来源：http://ndp.hesvh.cn

[E20] 判断字符串是否为空
来源：http://hnd.316326.xyz

Py:   if not s:
来源：http://iax.jianghu66.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ffk.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqt.svipenyu.cn

TS:   if (s === "") {}
来源：http://xhl.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://thl.chenlongwang.top

Go:   if s == "" {}
来源：http://tiv.zhengqikj.top

Ruby: if s.empty?
来源：http://mqh.zhoulong.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iix.chenlongwang.top

[E21] 超长截断加省略号
来源：http://bxu.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nrd.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iuv.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zpb.ehwqpu.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nxd.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uws.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://ezg.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dfe.gotoacloud.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pwb.fktsv.cn

[E22] 字节长度与字符长度
来源：http://mxt.pengpengdd.cyou

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vub.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eus.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wzy.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dqu.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xwg.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lhd.fzhhl.top

Ruby: s.bytesize;  s.length
来源：http://uhn.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hxp.0kj1m.cn

================================================================================
来源：http://eeo.jinqigfzy.top

F. 文件与目录
来源：http://wcs.zhoulong.xyz

================================================================================
来源：http://ldb.zhiwuduotai.top

[F01] 读取整个文件
来源：http://drq.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wxl.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://jnz.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zsw.iojbl.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mhk.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bbo.hnqzz.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://odw.ydzc1.top

Ruby: File.read("a.txt")
来源：http://rui.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://uij.zdqjudy.top

[F02] 逐行读取文件
来源：http://kod.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ios.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ikq.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lki.fengsongda.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wby.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sua.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ybe.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xmp.zhiwuduotai.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vbc.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://kds.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vcz.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://epq.tianlin.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kdg.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tfm.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://omh.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oce.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://emj.ydzc1.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nru.kuanghao11.cn

[F04] 追加写入文件
来源：http://bob.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tri.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xws.kuanghao11.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://asy.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bwt.sweek.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lop.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bod.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lwj.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gvy.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://nfw.wangdashe.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mos.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://nmw.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://qeh.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://etz.ppjwa.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ans.9152youxi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wsf.hysaishi.cn

Ruby: File.exist?("a.txt")
来源：http://fiu.yongpay.top

C#:   File.Exists("a.txt")
来源：http://tbu.gaohongyu789.top

[F06] 删除文件
来源：http://fgl.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://snt.zhaomingkeji.xyz

PHP:  unlink("a.txt");
来源：http://hde.ybcxt.top

JS:   fs.unlinkSync("a.txt")
来源：http://api.0kj1m.cn

TS:   fs.unlinkSync("a.txt")
来源：http://itn.yongpay.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tld.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://crm.shanyushiyangkeji.top

Ruby: File.delete("a.txt")
来源：http://zpc.hesvh.cn

C#:   File.Delete("a.txt");
来源：http://hqt.fengsongda.top

[F07] 创建目录（含多级）
来源：http://asc.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oxn.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vmr.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aeh.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbv.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hfy.tian-w.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sly.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kvf.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ziw.gaohongyu789.top

[F08] 遍历目录
来源：http://ecl.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://cyj.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jqn.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://yco.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://wgk.yj20258.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bzi.ywan-chungtsiang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://sgd.hysaishi.cn

Ruby: Dir.children("dir")
来源：http://krt.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://zir.zhoulong.xyz

[F09] 获取文件大小
来源：http://vbo.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://luz.ybcxt.top

PHP:  filesize("a.txt");
来源：http://mbs.zhoulong.xyz

JS:   fs.statSync("a.txt").size
来源：http://onx.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://mwr.shzxlz.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jki.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ouh.nanxuanxn.top

Ruby: File.size("a.txt")
来源：http://rms.shzxlz.cn

C#:   new FileInfo("a.txt").Length
来源：http://rfj.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://zzh.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hwn.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bjg.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://loj.yongpay.top

TS:   path.extname("a.txt")
来源：http://bes.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hlb.52xcode.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mol.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ian.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nvz.yueranfly.top

[F11] 复制与移动文件
来源：http://nnc.xziqi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dfr.tarul.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://akn.shangyingyoupin.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yjj.yvedp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rbg.dianchejie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sya.tianlin.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cux.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ind.xylfe.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://caj.guannengcc.top

[F12] CSV 读写
来源：http://zaa.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://udq.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qjm.gogol.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yux.shanyushiyangkeji.top

TS:   // 同上
来源：http://rej.sjlbkw.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ukf.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dbo.feifeiyinyue.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hpj.aizwys.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vil.havefunace.top

================================================================================
来源：http://vtf.52xcode.cn

G. 面向对象
来源：http://kxh.chenzaomai.com

================================================================================
来源：http://qrd.shuidangran.top

[G01] 定义类
来源：http://kzh.jqgufenzy.top

Py:   class User: pass
来源：http://rmd.sweek.top

PHP:  class User {}
来源：http://ftk.svipenyu.cn

JS:   class User {}
来源：http://kir.xylfe.cn

TS:   class User { name: string = ""; }
来源：http://lka.tarul.cn

Java: class User {}
来源：http://gbe.xziqi.cn

Go:   type User struct { Name string }
来源：http://blj.wangdashe.top

Ruby: class User; end
来源：http://urq.yueranfly.top

C#:   class User {}
来源：http://iwe.gotoacloud.top

[G02] 构造函数
来源：http://pdg.yj20258888.top

Py:   def __init__(self, name): self.name = name
来源：http://uyz.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://sik.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://eoy.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://rqx.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://alk.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://txg.daria6918.cn

Ruby: def initialize(name); @name = name; end
来源：http://lrv.guowangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://rml.sweek.top

[G03] 实例属性
来源：http://cis.jianghu66.top

Py:   self.name = "x"
来源：http://rso.ybcxt.top

PHP:  public string $name = "x";
来源：http://tmn.xuetiantiany.cn

JS:   this.name = "x";
来源：http://zzz.xuanzx.com

TS:   name: string = "x";
来源：http://jxu.wangshuangyany.cn

Java: private String name;
来源：http://ske.redwolf501.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pbh.cdnleiting.top

Ruby: @name = "x"
来源：http://moz.pycfn.com

C#:   public string Name { get; set; } = "x";
来源：http://uxu.snrcjt.cn

[G04] 定义方法
来源：http://kkn.nwbrower.top

Py:   def greet(self): return self.name
来源：http://vbh.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://exk.fktsv.cn

JS:   greet() { return this.name; }
来源：http://dgs.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://ghy.guannengcc.top

Java: String greet() { return name; }
来源：http://oua.epnwcf.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://zdr.uphjek.com

Ruby: def greet; @name; end
来源：http://foi.hnqzz.top

C#:   public string Greet() => Name;
来源：http://uev.sjlbkw.cn

[G05] 继承
来源：http://jhb.hammf.cn

Py:   class Admin(User): pass
来源：http://cjs.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://plk.daxiang520.top

JS:   class Admin extends User {}
来源：http://lcv.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://hfe.hesvh.cn

Java: class Admin extends User {}
来源：http://uyt.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fea.havefunace.top

Ruby: class Admin < User; end
来源：http://bcv.zhiwuduotai.top

C#:   class Admin : User {}
来源：http://siz.zhongyouzk.top

[G06] 重写方法
来源：http://kfx.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://obg.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rvs.jlsjyb.cn

JS:   greet() { return "admin"; }
来源：http://pgf.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://nop.pycfn.com

Java: @Override String greet() { return "admin"; }
来源：http://ome.birdmap.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kav.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://mpa.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://sbe.hysaishi.cn

[G07] 调用父类方法
来源：http://bhf.hnqzz.top

Py:   super().greet()
来源：http://oij.dashuyun.cn

PHP:  parent::greet();
来源：http://njg.nanxuanxn.top

JS:   super.greet();
来源：http://fwl.aibaodan.cn

TS:   super.greet();
来源：http://ptu.tanke756.top

Java: super.greet();
来源：http://eew.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cue.daria6918.cn

Ruby: super
来源：http://sfg.ydzc1.top

C#:   base.Greet();
来源：http://pvq.9152youxi.cn

[G08] 静态方法与属性
来源：http://rkd.sweek.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ewc.chenzaomai.com

PHP:  public static function f() {}
来源：http://yze.dashuyun.cn

JS:   static f() {}
来源：http://eyv.snrcjt.cn

TS:   static f(): void {}
来源：http://vxd.fehbvm.com

Java: static void f() {}
来源：http://yhf.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zvc.9152youxi.cn

Ruby: def self.f; end
来源：http://qtd.yuxming.cn

C#:   public static void F() {}
来源：http://bei.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://tso.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://kvv.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://zxa.smart0.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://gyi.jinqigufen.top

TS:   interface Shape { area(): number; }
来源：http://pbd.xylfe.cn

Java: interface Shape { double area(); }
来源：http://upz.daxiang520.top

Go:   type Shape interface { Area() float64 }
来源：http://opp.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://loh.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://uku.ehwqpu.com

[G10] 访问控制
来源：http://wnc.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://nsk.ivvv.top

PHP:  public / protected / private
来源：http://vuf.ydjk.org.cn

JS:   #private 字段；其余公开
来源：http://kil.jinghuilouyu.cn

TS:   public / protected / private
来源：http://jvg.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://kbd.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://rvm.yueranfly.top

Ruby: public / protected / private
来源：http://jue.fanxiaobao.xyz


<!-- 参考信息 -->