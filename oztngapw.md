代发 wailian999

Py:   for ch in s: print(ch)
来源：http://mbi.xylfe.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gmi.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://szk.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://alk.9152youxi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jze.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kry.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mpx.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lji.havefunace.top

[E14] URL 编码与 Base64
来源：http://jpt.gzhubu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uor.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pnk.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lij.jinyuanbaomall.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wkk.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igy.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vdi.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bxl.shuidangran.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ixa.hnxiangtu.top

[E15] HTML 转义 / 反转义
来源：http://ldf.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pmt.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gph.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eme.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://fno.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://urx.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ojk.hongshengwenyu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kiz.yj202588.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hjo.feifeiyinyue.top

[E16] 数字千分位
来源：http://iar.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://rwd.sweek.top

PHP:  number_format(1234567);
来源：http://wyb.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rtv.hnqzz.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gxx.chenzaomai.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wsd.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://whf.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uka.sweek.top

C#:   1234567.ToString("N0")
来源：http://bop.ywan-chungtsiang.top

[E17] 首字母大写
来源：http://gri.hywenlv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jet.birdmap.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://emy.xinyue.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcb.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hfo.ydzc1.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gtx.chenjidiqi.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://miz.sufxvd.cn

Ruby: s.capitalize
来源：http://eje.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gei.cqqwz.cn

[E18] 模板占位符替换
来源：http://rpu.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ygw.dianchejie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qcx.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hmw.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://olo.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kps.ehwqpu.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://amo.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fjx.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xxl.nwbrower.top

[E19] 多行文本按行拆分
来源：http://zle.daxiang520.top

Py:   s.splitlines()
来源：http://dxd.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zmx.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://kuh.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://gtb.tanke756.top

Java: s.lines().toList()
来源：http://won.sysykeji.top

Go:   strings.Split(s, "\n")
来源：http://upp.jinqigfzy.top

Ruby: s.lines
来源：http://jjc.jqgufenzy.top

C#:   s.Split('\n')
来源：http://hss.iojbl.cn

[E20] 判断字符串是否为空
来源：http://onh.0kj1m.cn

Py:   if not s:
来源：http://zji.sjlbkw.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://adl.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://axi.ivvv.top

TS:   if (s === "") {}
来源：http://egp.zhongyouzk.top

Java: if (s.isEmpty()) {}
来源：http://ukc.tarul.cn

Go:   if s == "" {}
来源：http://uog.dashuyun.cn

Ruby: if s.empty?
来源：http://vbu.fzhhl.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kik.nanxinkj.top

[E21] 超长截断加省略号
来源：http://fhc.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jpt.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://syo.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uxn.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vgc.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ncr.cqqwz.cn

Go:   // 按 rune 判断长度后截断
来源：http://wdz.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bvx.havefunace.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pri.52xcode.cn

[E22] 字节长度与字符长度
来源：http://tqh.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kfu.tanke756.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ipj.svipenyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ari.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lep.gotoacloud.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eku.shzxlz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://taw.nwbrower.top

Ruby: s.bytesize;  s.length
来源：http://zix.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ebp.cashguo.top

================================================================================
来源：http://uya.fktsv.cn

F. 文件与目录
来源：http://sze.xuanzx.com

================================================================================
来源：http://trw.shuidangran.top

[F01] 读取整个文件
来源：http://uun.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://apy.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://moh.tian-w.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mqm.sxryk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://poa.xuanzx.com

Java: Files.readString(Path.of("a.txt"))
来源：http://rbg.aizwys.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qfd.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://ucu.dianchejie.cn

C#:   File.ReadAllText("a.txt");
来源：http://cuk.tian-w.cn

[F02] 逐行读取文件
来源：http://pmd.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://agx.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wmx.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpb.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://azk.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hvr.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hqm.yuxming.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rus.jianghu66.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ubk.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://qcq.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jst.yvedp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://isa.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rnw.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ijj.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://giw.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xcj.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://ucc.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://duk.jqgufenzy.top

[F04] 追加写入文件
来源：http://lbe.xylfe.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rbw.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yyr.jqgufenzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hpj.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kot.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qaj.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ipr.bjfxy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hnx.sxryk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ohb.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://vjb.yangfankeji.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://imj.9152youxi.cn

PHP:  file_exists("a.txt");
来源：http://kxd.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://seb.jlsjyb.cn

TS:   fs.existsSync("a.txt")
来源：http://mki.feifeiyinyue.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tzl.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ykw.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://kum.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://oop.cheryme.top

[F06] 删除文件
来源：http://swv.tianlin.xyz

Py:   os.remove("a.txt")
来源：http://wli.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://bci.chenjidiqi.icu

JS:   fs.unlinkSync("a.txt")
来源：http://ozg.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://agg.hcnkem.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uoi.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://qre.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://xck.316326.xyz

C#:   File.Delete("a.txt");
来源：http://zdx.fzhhl.top

[F07] 创建目录（含多级）
来源：http://mmn.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://anm.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rgq.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ynl.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wfm.jyoumei.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dza.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tij.fzhhl.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nmr.9152youxi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yvw.epnwcf.com

[F08] 遍历目录
来源：http://cup.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://nfd.haohaochexian.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zra.hywenlv.cn

JS:   fs.readdirSync("dir")
来源：http://pjf.yj20258.top

TS:   fs.readdirSync("dir")
来源：http://jpn.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ixy.0kj1m.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://soi.guannengcc.top

Ruby: Dir.children("dir")
来源：http://xig.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://ogt.andypj.xyz

[F09] 获取文件大小
来源：http://jwe.sysykeji.top

Py:   os.path.getsize("a.txt")
来源：http://tic.mhx1999.top

PHP:  filesize("a.txt");
来源：http://uyf.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://ulk.jinyuanbaomall.cn

TS:   fs.statSync("a.txt").size
来源：http://xxy.wangshuangyany.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bts.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://imm.fzhhl.top

Ruby: File.size("a.txt")
来源：http://okp.hywenlv.cn

C#:   new FileInfo("a.txt").Length
来源：http://umi.vehdjk.com

[F10] 取文件扩展名 / 文件名
来源：http://jvg.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zkf.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jpl.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xbs.yj202588.top

TS:   path.extname("a.txt")
来源：http://vgj.hnqzz.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pqx.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://frx.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cjs.fktsv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yll.tanke756.top

[F11] 复制与移动文件
来源：http://qau.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ris.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fsc.jianghu66.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vnh.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bea.shangyingyoupin.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zlx.snrcjt.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jaf.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xnl.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qeh.guannengcc.top

[F12] CSV 读写
来源：http://fau.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uut.xuetiantiany.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xnm.xuetiantiany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zvq.zhixingplan.top

TS:   // 同上
来源：http://clv.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ndd.zhijiandao.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://esb.hammf.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ktr.bbcook.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rju.52xcode.cn

================================================================================
来源：http://vkh.pengpengdd.cyou

G. 面向对象
来源：http://tgr.jinqigfzy.top

================================================================================
来源：http://qcu.havefunace.top

[G01] 定义类
来源：http://mtw.yj202588.top

Py:   class User: pass
来源：http://cbk.xylfe.cn

PHP:  class User {}
来源：http://vvf.jlsjyb.cn

JS:   class User {}
来源：http://cid.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://etm.hysaishi.cn

Java: class User {}
来源：http://kkz.sufxvd.cn

Go:   type User struct { Name string }
来源：http://zdp.yueranfly.top

Ruby: class User; end
来源：http://cdt.pengpengdd.cyou

C#:   class User {}
来源：http://pdf.jinyuanbaomall.cn

[G02] 构造函数
来源：http://eou.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://sfs.sweek.top

PHP:  public function __construct(public string $name) {}
来源：http://fiu.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://zvk.jinyuanbaomall.cn

TS:   constructor(public name: string) {}
来源：http://bys.chenjidiqi.icu

Java: User(String name) { this.name = name; }
来源：http://qqy.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://utu.yonumen.top

Ruby: def initialize(name); @name = name; end
来源：http://piq.zhiwuduotai.top

C#:   public User(string name) { Name = name; }
来源：http://ack.havefunace.top

[G03] 实例属性
来源：http://siy.zhongyouzk.top

Py:   self.name = "x"
来源：http://hvq.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://gux.fehbvm.com

JS:   this.name = "x";
来源：http://ioo.vqdsnc.cn

TS:   name: string = "x";
来源：http://oqg.zycfv.cn

Java: private String name;
来源：http://qnp.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bqh.sweek.top

Ruby: @name = "x"
来源：http://xrd.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://ixs.quarkkingdee.top

[G04] 定义方法
来源：http://tsb.yuxming.cn

Py:   def greet(self): return self.name
来源：http://kpg.fengsongda.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uei.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://qsq.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://lzz.vehdjk.com

Java: String greet() { return name; }
来源：http://mit.gaohongyu789.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jhh.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://jen.fktsv.cn

C#:   public string Greet() => Name;
来源：http://gsu.jqgufenzy.top

[G05] 继承
来源：http://jkz.sxryk.cn

Py:   class Admin(User): pass
来源：http://ifq.yonumen.top

PHP:  class Admin extends User {}
来源：http://yss.sysykeji.top

JS:   class Admin extends User {}
来源：http://nre.shuidangran.top

TS:   class Admin extends User {}
来源：http://rym.cashguo.top

Java: class Admin extends User {}
来源：http://tyr.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dty.uphjek.com

Ruby: class Admin < User; end
来源：http://kcl.nanxuanxn.top

C#:   class Admin : User {}
来源：http://gyc.zdqjudy.top

[G06] 重写方法
来源：http://rpa.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://uzd.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jsq.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://psm.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://krw.9152youxi.cn

Java: @Override String greet() { return "admin"; }
来源：http://bwx.zhixingplan.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kwy.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://mcd.epnwcf.com

C#:   public override string Greet() => "admin";
来源：http://sfn.zhiwuduotai.top

[G07] 调用父类方法
来源：http://piu.dianchejie.cn

Py:   super().greet()
来源：http://msz.xuanzx.com

PHP:  parent::greet();
来源：http://qkm.yanxiufei.cn

JS:   super.greet();
来源：http://mkz.pycfn.com

TS:   super.greet();
来源：http://ulk.bjfxy.top

Java: super.greet();
来源：http://cjz.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rwz.zhiwuduotai.top

Ruby: super
来源：http://qro.shanyushiyangkeji.top

C#:   base.Greet();
来源：http://kgs.fengsongda.top

[G08] 静态方法与属性
来源：http://bdm.svipenyu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wop.daxiang520.top

PHP:  public static function f() {}
来源：http://twe.chenjidiqi.icu

JS:   static f() {}
来源：http://uuq.xuanzx.com

TS:   static f(): void {}
来源：http://lph.jinyuanbaomall.cn

Java: static void f() {}
来源：http://cti.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ctz.daxiang520.top

Ruby: def self.f; end
来源：http://abl.vehdjk.com

C#:   public static void F() {}
来源：http://jzi.yj20258.top

[G09] 接口 / 抽象类
来源：http://mew.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://huc.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ryo.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://hdl.pycfn.com

TS:   interface Shape { area(): number; }
来源：http://qwt.nwbrower.top

Java: interface Shape { double area(); }
来源：http://mcl.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://azm.gotoacloud.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://emi.hcnkem.com

C#:   interface IShape { double Area(); }
来源：http://ylk.yanxiufei.cn

[G10] 访问控制
来源：http://kqr.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://yow.ppjwa.cn

PHP:  public / protected / private
来源：http://auk.xziqi.cn

JS:   #private 字段；其余公开
来源：http://zdn.zycfv.cn

TS:   public / protected / private
来源：http://itp.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://wsu.c1oappe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gvk.ybcxt.top

Ruby: public / protected / private
来源：http://htq.316326.xyz

C#:   public / protected / private / internal
来源：http://igi.xylfe.cn

[G11] getter / setter
来源：http://dmt.xuanzx.com

Py:   @property 与 @x.setter
来源：http://taw.hcnkem.com

PHP:  public function getName(): string { return $this->name; }
来源：http://fdx.316326.xyz

JS:   get name() { return this._name; }
来源：http://pfw.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://uzv.fzhhl.top

Java: public String getName() { return name; }
来源：http://ikp.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yan.yueranfly.top


<!-- 参考信息 -->