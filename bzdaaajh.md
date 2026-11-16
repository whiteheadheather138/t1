代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jtk.hnxiangtu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bpu.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://yxy.zhixingplan.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nyn.quarkkingdee.top

[E14] URL 编码与 Base64
来源：http://hfc.jyoumei.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://phb.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gew.ybcxt.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jrj.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vri.redwolf501.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bin.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ylf.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ern.smart0.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://izy.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://cgv.redwolf501.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tum.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pdx.shanyushiyangtech.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tml.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cyj.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hxg.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://veh.yj20258.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qba.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sih.yonumen.top

[E16] 数字千分位
来源：http://qmr.52xcode.cn

Py:   f"{1234567:,}"
来源：http://tml.haohaochexian.top

PHP:  number_format(1234567);
来源：http://wpk.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jpw.ywan-chungtsiang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://pgj.ppjwa.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ehm.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wnq.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dod.havefunace.top

C#:   1234567.ToString("N0")
来源：http://osl.gaohongyu789.top

[E17] 首字母大写
来源：http://mdh.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iup.haohaochexian.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ypf.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghh.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zrq.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lmn.316326.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://aeu.zhijiandao.cn

Ruby: s.capitalize
来源：http://dgx.ywan-chungtsiang.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dnf.aibaodan.cn

[E18] 模板占位符替换
来源：http://iez.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yfs.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dtg.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://var.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vbj.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://soy.c1oappe.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://twd.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wwa.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pew.hcnkem.com

[E19] 多行文本按行拆分
来源：http://kuj.smart0.xyz

Py:   s.splitlines()
来源：http://ptp.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cct.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://qdi.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://xtq.gotoacloud.top

Java: s.lines().toList()
来源：http://ovl.ybcxt.top

Go:   strings.Split(s, "\n")
来源：http://nlw.ehwqpu.com

Ruby: s.lines
来源：http://dun.zycfv.cn

C#:   s.Split('\n')
来源：http://ypk.redwolf501.top

[E20] 判断字符串是否为空
来源：http://rwr.9152youxi.cn

Py:   if not s:
来源：http://kwg.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mjt.meibo888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pbg.xuanzx.com

TS:   if (s === "") {}
来源：http://qtc.ppjwa.cn

Java: if (s.isEmpty()) {}
来源：http://bzj.sjlbkw.cn

Go:   if s == "" {}
来源：http://yuu.yanxiufei.cn

Ruby: if s.empty?
来源：http://anc.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mej.haohaochexian.top

[E21] 超长截断加省略号
来源：http://fgd.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zvt.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://veq.zhoulong.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dvd.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://spr.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://coi.hcnkem.com

Go:   // 按 rune 判断长度后截断
来源：http://lms.jinqigfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gtc.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lnv.feifeiyinyue.top

[E22] 字节长度与字符长度
来源：http://zuq.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hdp.ydzc1.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lxs.yj20258.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jbl.cqqwz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ffu.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iup.dashuyun.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qxm.xuanzx.com

Ruby: s.bytesize;  s.length
来源：http://pmg.jqgfzy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tnv.pengpengdd.cyou

================================================================================
来源：http://hrz.vehdjk.com

F. 文件与目录
来源：http://qeq.aibaodan.cn

================================================================================
来源：http://jkh.zhixingplan.top

[F01] 读取整个文件
来源：http://yss.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iyy.hcnkem.com

PHP:  file_get_contents("a.txt");
来源：http://coj.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ytl.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ivt.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fir.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://has.ctjpmb.com

Ruby: File.read("a.txt")
来源：http://ild.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://qid.tarul.cn

[F02] 逐行读取文件
来源：http://pyy.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yxr.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://noz.yueranfly.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kmk.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jsa.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jro.sysykeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ihe.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ott.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ock.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://mbp.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://luu.yueranfly.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fxs.svipenyu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vnj.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mzc.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xna.wangdashe.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bvd.chenjidiqi.icu

Ruby: File.write("a.txt", "hi")
来源：http://jtp.meibo888.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vip.hnxiangtu.top

[F04] 追加写入文件
来源：http://hna.zdbjq.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cva.shanyushiyangtech.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lyr.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://htd.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yfv.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lch.ydjk.org.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dxq.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qrt.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zox.meibo888.top

[F05] 判断文件或目录是否存在
来源：http://cvv.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tbf.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://yvj.daria6918.cn

JS:   fs.existsSync("a.txt")
来源：http://csm.bjfxy.top

TS:   fs.existsSync("a.txt")
来源：http://goo.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lff.tianlin.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://daj.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://aqk.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://kay.cqqwz.cn

[F06] 删除文件
来源：http://dhf.gotoacloud.top

Py:   os.remove("a.txt")
来源：http://epe.yonumen.top

PHP:  unlink("a.txt");
来源：http://zhw.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://qqt.birdmap.top

TS:   fs.unlinkSync("a.txt")
来源：http://bhz.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vtf.yvedp.cn

Go:   os.Remove("a.txt")
来源：http://ioo.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://llp.xuanzx.com

C#:   File.Delete("a.txt");
来源：http://nob.epnwcf.com

[F07] 创建目录（含多级）
来源：http://ymi.andypj.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://awy.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://thg.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mrx.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qvs.cheryme.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qqt.vqdsnc.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qwj.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fdt.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ctv.wangshuangyany.cn

[F08] 遍历目录
来源：http://vru.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hff.fzhhl.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jdv.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://hrp.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://usn.haohaochexian.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yal.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tdm.xuanzx.com

Ruby: Dir.children("dir")
来源：http://ftl.yueranfly.top

C#:   Directory.GetFiles("dir")
来源：http://pqg.chenzaomai.com

[F09] 获取文件大小
来源：http://uwy.chenjidiqi.icu

Py:   os.path.getsize("a.txt")
来源：http://pka.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://kld.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://zua.hongshengwenyu.top

TS:   fs.statSync("a.txt").size
来源：http://xov.haohaochexian.top

Java: Files.size(Path.of("a.txt"))
来源：http://ppd.jqgufenzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mnl.zhengqikj.top

Ruby: File.size("a.txt")
来源：http://wcn.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://dmk.epnwcf.com

[F10] 取文件扩展名 / 文件名
来源：http://gjl.iojbl.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wuy.9152youxi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wbz.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sob.jinqigfzy.top

TS:   path.extname("a.txt")
来源：http://jfy.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwi.zhongyouzk.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://equ.ywan-chungtsiang.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://prz.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ndi.xuetiantiany.cn

[F11] 复制与移动文件
来源：http://eod.cdnleiting.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gki.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://poe.gaohongyu789.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etc.andypj.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gxo.dashuyun.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kfj.yanxiufei.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ulo.hysaishi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sii.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iqz.ybcxt.top

[F12] CSV 读写
来源：http://ume.c1oappe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vbe.meibo888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oxa.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gtl.xingfuxueyuan.xyz

TS:   // 同上
来源：http://pve.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://toq.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wou.wangdashe.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rpz.cqqwz.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rdj.tarul.cn

================================================================================
来源：http://quu.dashuyun.cn

G. 面向对象
来源：http://jxj.yangfankeji.com

================================================================================
来源：http://tkl.cqqwz.cn

[G01] 定义类
来源：http://dym.hcnkem.com

Py:   class User: pass
来源：http://vnx.shanyushiyangtech.top

PHP:  class User {}
来源：http://kwc.sxryk.cn

JS:   class User {}
来源：http://fyx.shanyushiyangtech.top

TS:   class User { name: string = ""; }
来源：http://rkz.sufxvd.cn

Java: class User {}
来源：http://qip.nanxinkj.top

Go:   type User struct { Name string }
来源：http://gnn.shzxlz.cn

Ruby: class User; end
来源：http://yyk.sweek.top

C#:   class User {}
来源：http://ref.jianghu66.top

[G02] 构造函数
来源：http://smf.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://lry.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://tvu.hcnkem.com

JS:   constructor(name) { this.name = name; }
来源：http://zxk.nwbrower.top

TS:   constructor(public name: string) {}
来源：http://okd.ppjwa.cn

Java: User(String name) { this.name = name; }
来源：http://prg.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xiw.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://wsp.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://cfj.0kj1m.cn

[G03] 实例属性
来源：http://sue.sysykeji.top

Py:   self.name = "x"
来源：http://mao.cucudq.cn

PHP:  public string $name = "x";
来源：http://lha.jqgfzy.top

JS:   this.name = "x";
来源：http://jgv.xylfe.cn

TS:   name: string = "x";
来源：http://cxi.xylfe.cn

Java: private String name;
来源：http://kiz.zhaomingkeji.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ktn.yj20258888.top

Ruby: @name = "x"
来源：http://ppq.daxiang520.top

C#:   public string Name { get; set; } = "x";
来源：http://vly.ywan-chungtsiang.top

[G04] 定义方法
来源：http://jno.tianlin.xyz

Py:   def greet(self): return self.name
来源：http://nkk.yj202588.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ton.ybcxt.top

JS:   greet() { return this.name; }
来源：http://xsk.cdnleiting.top

TS:   greet(): string { return this.name; }
来源：http://mpi.andypj.xyz

Java: String greet() { return name; }
来源：http://btc.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ndm.aibaodan.cn

Ruby: def greet; @name; end
来源：http://nsy.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://hfy.snrcjt.cn

[G05] 继承
来源：http://nxp.ppjwa.cn

Py:   class Admin(User): pass
来源：http://ekc.fehbvm.com

PHP:  class Admin extends User {}
来源：http://afn.yueranfly.top

JS:   class Admin extends User {}
来源：http://zfe.uphjek.com

TS:   class Admin extends User {}
来源：http://jzo.xylfe.cn

Java: class Admin extends User {}
来源：http://yra.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kwl.kuanghao11.cn

Ruby: class Admin < User; end
来源：http://pao.tarul.cn

C#:   class Admin : User {}
来源：http://ldj.smart0.xyz

[G06] 重写方法
来源：http://qto.xylfe.cn

Py:   def greet(self): return "admin"
来源：http://duz.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cfs.pycfn.com

JS:   greet() { return "admin"; }
来源：http://ksj.jlsjyb.cn

TS:   greet(): string { return "admin"; }
来源：http://fzs.ywan-chungtsiang.top

Java: @Override String greet() { return "admin"; }
来源：http://evj.52xcode.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://abg.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://agv.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://bad.hysaishi.cn

[G07] 调用父类方法
来源：http://uzy.jqgfzy.top

Py:   super().greet()
来源：http://omm.yangfankeji.com

PHP:  parent::greet();
来源：http://arn.haohaochexian.top

JS:   super.greet();
来源：http://gel.yj20258888.top

TS:   super.greet();
来源：http://pnr.ctjpmb.com

Java: super.greet();
来源：http://oie.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hmv.ydzc1.top

Ruby: super
来源：http://lmf.hywenlv.cn

C#:   base.Greet();
来源：http://khi.ehwqpu.com

[G08] 静态方法与属性
来源：http://rey.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://loo.jqgfzy.top

PHP:  public static function f() {}
来源：http://cgq.gotoacloud.top

JS:   static f() {}
来源：http://pmk.snrcjt.cn

TS:   static f(): void {}
来源：http://djt.tian-w.cn

Java: static void f() {}
来源：http://vvg.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://cte.guannengcc.top

Ruby: def self.f; end
来源：http://yms.svipenyu.cn

C#:   public static void F() {}
来源：http://yri.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://zha.hnxiangtu.top

Py:   from abc import ABC, abstractmethod
来源：http://ljf.ppjwa.cn

PHP:  interface Shape { public function area(): float; }
来源：http://eta.gzhubu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mun.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://csu.xylfe.cn

Java: interface Shape { double area(); }
来源：http://bhb.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://ojo.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vph.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://ynq.hammf.cn

[G10] 访问控制
来源：http://jsu.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://bgm.epnwcf.com

PHP:  public / protected / private
来源：http://iha.zdqjudy.top

JS:   #private 字段；其余公开
来源：http://nnr.nanxinkj.top

TS:   public / protected / private
来源：http://tvx.wangdashe.top

Java: public / protected / private / 默认包级
来源：http://yvy.jqgufenzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://iaw.birdmap.top

Ruby: public / protected / private
来源：http://rmo.zhijiandao.cn

C#:   public / protected / private / internal
来源：http://mxw.fktsv.cn

[G11] getter / setter
来源：http://zdn.bbcook.cn

Py:   @property 与 @x.setter
来源：http://yma.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zfp.cqqwz.cn

JS:   get name() { return this._name; }
来源：http://rvh.hywenlv.cn

TS:   get name(): string { return this._name; }
来源：http://onk.cucudq.cn

Java: public String getName() { return name; }
来源：http://bbw.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://icj.fzhhl.top

Ruby: attr_accessor :name
来源：http://zva.sysykeji.top

C#:   public string Name { get; set; }
来源：http://hhu.xuetiantiany.cn

[G12] 对象转字符串
来源：http://afh.sufxvd.cn

Py:   def __str__(self): return self.name
来源：http://yzl.gotoacloud.top


<!-- 参考信息 -->