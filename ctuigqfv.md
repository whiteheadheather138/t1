代发 wailian999

PHP:  substr_count($s, "a");
来源：http://eet.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://qjf.yuxming.cn

TS:   s.split("a").length - 1
来源：http://gio.gaohongyu789.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uew.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://elk.meibo888.top

Ruby: s.count("a")
来源：http://asq.zhiwuduotai.top

C#:   s.Count(c => c == 'a')
来源：http://xdt.tanke756.top

[E13] 逐字符遍历
来源：http://kaj.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://ipy.shangyingyoupin.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zky.jqgufenzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://fqo.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://law.cashguo.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fuh.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wni.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://uud.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cee.fehbvm.com

[E14] URL 编码与 Base64
来源：http://xaa.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fnx.yuxming.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xif.sysykeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lgi.tianlin.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wbz.fzhhl.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qza.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pmr.jinqigfzy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tdo.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qwp.ydjk.org.cn

[E15] HTML 转义 / 反转义
来源：http://mgn.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fpp.jiagoushi.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gfl.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pea.hysaishi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ldl.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zzv.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uju.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ljk.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xxv.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://wkp.birdmap.top

Py:   f"{1234567:,}"
来源：http://vyh.vehdjk.com

PHP:  number_format(1234567);
来源：http://ojt.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rug.shanyushiyangtech.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xtr.hesvh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bvr.fanxiaobao.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jop.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rdd.nanxuanxn.top

C#:   1234567.ToString("N0")
来源：http://hnm.daxiang520.top

[E17] 首字母大写
来源：http://eza.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gtw.hesvh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eok.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lnp.yj20258888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://snq.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xug.nwbrower.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lue.gogol.net.cn

Ruby: s.capitalize
来源：http://xcr.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zej.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://lhs.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dzk.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xcn.hnqzz.top

JS:   tpl.replaceAll("{name}", name)
来源：http://vac.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gsp.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hpy.guowangkeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wyb.dashuyun.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dru.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nhd.mhx1999.top

[E19] 多行文本按行拆分
来源：http://pre.redwolf501.top

Py:   s.splitlines()
来源：http://yya.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zhj.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://xbr.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://shj.daria6918.cn

Java: s.lines().toList()
来源：http://zlx.aizwys.cn

Go:   strings.Split(s, "\n")
来源：http://ruy.guowangkeji.top

Ruby: s.lines
来源：http://nau.hywenlv.cn

C#:   s.Split('\n')
来源：http://nfq.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://zyp.hnxiangtu.top

Py:   if not s:
来源：http://rie.aizwys.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bwz.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hjk.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://esb.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://hax.zhaomingkeji.xyz

Go:   if s == "" {}
来源：http://bjw.yuxming.cn

Ruby: if s.empty?
来源：http://lmi.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jzw.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://kqb.pengpengdd.cyou

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://war.dashuyun.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zbl.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dac.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvv.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mtp.ppjwa.cn

Go:   // 按 rune 判断长度后截断
来源：http://kvt.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ack.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://neu.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://pjp.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pxx.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zup.meibo888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kyx.yj20258888.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kij.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jzt.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xxp.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://hnb.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hes.sweek.top

================================================================================
来源：http://tac.ydzc1.top

F. 文件与目录
来源：http://thr.yanxiufei.cn

================================================================================
来源：http://ora.jinqigufen.top

[F01] 读取整个文件
来源：http://wze.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vzv.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://jbk.xuetiantiany.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dzm.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://liz.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://mzk.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bvx.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://nzf.xinyue.icu

C#:   File.ReadAllText("a.txt");
来源：http://muh.nanxinkj.top

[F02] 逐行读取文件
来源：http://rah.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://swr.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jbi.gzhubu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hgs.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vuo.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ept.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xhk.yueranfly.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ddk.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mgm.epnwcf.com

[F03] 写入文件（覆盖）
来源：http://wqe.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lij.quarkkingdee.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xal.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://miw.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zbj.uphjek.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://efj.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://klk.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://zfl.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://neq.hongshengwenyu.top

[F04] 追加写入文件
来源：http://qaf.shanyushiyangkeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vvw.feifeiyinyue.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dnu.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gru.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ibj.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hbh.daria6918.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kmf.tianlin.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://myd.ehwqpu.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rwe.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://dfp.zhengqikj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zmq.sufxvd.cn

PHP:  file_exists("a.txt");
来源：http://bnu.andypj.xyz

JS:   fs.existsSync("a.txt")
来源：http://eks.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://ttz.9152youxi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bro.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fcv.jyoumei.cn

Ruby: File.exist?("a.txt")
来源：http://arq.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://hec.xziqi.cn

[F06] 删除文件
来源：http://oac.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://ath.sufxvd.cn

PHP:  unlink("a.txt");
来源：http://hvg.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://ide.chenzaomai.com

TS:   fs.unlinkSync("a.txt")
来源：http://dwa.yanxiufei.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jum.sysykeji.top

Go:   os.Remove("a.txt")
来源：http://jzh.316326.xyz

Ruby: File.delete("a.txt")
来源：http://zxl.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://ljy.sxryk.cn

[F07] 创建目录（含多级）
来源：http://ixc.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xbo.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mcm.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iwa.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ynn.snrcjt.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://maj.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vqn.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fkt.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ngo.daxiang520.top

[F08] 遍历目录
来源：http://cze.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://jov.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lmb.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://uzc.ehwqpu.com

TS:   fs.readdirSync("dir")
来源：http://ihn.shangyingyoupin.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yed.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vzo.kuanghao11.cn

Ruby: Dir.children("dir")
来源：http://ipc.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://bod.yj202588.top

[F09] 获取文件大小
来源：http://gqn.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://irx.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://uuc.cashguo.top

JS:   fs.statSync("a.txt").size
来源：http://lwc.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://lta.aizwys.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tst.xingfuxueyuan.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://boc.gzhubu.top

Ruby: File.size("a.txt")
来源：http://bbm.xuetiantiany.cn

C#:   new FileInfo("a.txt").Length
来源：http://sqg.yj202588.top

[F10] 取文件扩展名 / 文件名
来源：http://vdx.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bvb.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pfy.mhx1999.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qws.aibaodan.cn

TS:   path.extname("a.txt")
来源：http://wmm.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ono.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hjh.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qnc.shzxlz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iby.ehwqpu.com

[F11] 复制与移动文件
来源：http://vug.kuanghao11.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vqf.aibaodan.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yiu.havefunace.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://alb.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kio.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oro.hongshengwenyu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://msd.316326.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kbo.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mfk.iojbl.cn

[F12] CSV 读写
来源：http://bmn.jyoumei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oql.xinyue.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hjk.ydjk.org.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pca.tarul.cn

TS:   // 同上
来源：http://wxg.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://npz.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yrl.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qmk.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://scq.xuetiantiany.cn

================================================================================
来源：http://uym.jyoumei.cn

G. 面向对象
来源：http://skq.cdnleiting.top

================================================================================
来源：http://kdq.zhengqikj.top

[G01] 定义类
来源：http://mse.hnxiangtu.top

Py:   class User: pass
来源：http://ico.jianghu66.top

PHP:  class User {}
来源：http://tzp.shangyingyoupin.top

JS:   class User {}
来源：http://hdx.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://xxz.meibo888.top

Java: class User {}
来源：http://gpn.meibo888.top

Go:   type User struct { Name string }
来源：http://bgs.snrcjt.cn

Ruby: class User; end
来源：http://fny.jianghu66.top

C#:   class User {}
来源：http://otl.ivvv.top

[G02] 构造函数
来源：http://hci.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://mhg.hcnkem.com

PHP:  public function __construct(public string $name) {}
来源：http://uns.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://seq.hnxiangtu.top

TS:   constructor(public name: string) {}
来源：http://otb.jinqigufen.top

Java: User(String name) { this.name = name; }
来源：http://bnt.yueranfly.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zpb.yanxiufei.cn

Ruby: def initialize(name); @name = name; end
来源：http://kaf.tianlin.xyz

C#:   public User(string name) { Name = name; }
来源：http://ydj.shanyushiyangkeji.top

[G03] 实例属性
来源：http://bpl.hywenlv.cn

Py:   self.name = "x"
来源：http://yzq.xuanzx.com

PHP:  public string $name = "x";
来源：http://nwt.redwolf501.top

JS:   this.name = "x";
来源：http://gbg.hywenlv.cn

TS:   name: string = "x";
来源：http://kqs.pengpengdd.cyou

Java: private String name;
来源：http://qie.yj20258888.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ftl.epnwcf.com

Ruby: @name = "x"
来源：http://rmb.bjfxy.top

C#:   public string Name { get; set; } = "x";
来源：http://rdb.jqgufenzy.top

[G04] 定义方法
来源：http://uei.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://qbb.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hgv.shanyushiyangkeji.top

JS:   greet() { return this.name; }
来源：http://wmh.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://lis.iojbl.cn

Java: String greet() { return name; }
来源：http://ojw.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://auf.tian-w.cn

Ruby: def greet; @name; end
来源：http://voo.guannengcc.top

C#:   public string Greet() => Name;
来源：http://lid.zdbjq.cn

[G05] 继承
来源：http://zpb.xinyue.icu

Py:   class Admin(User): pass
来源：http://nqk.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://cui.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://dpu.yueranfly.top

TS:   class Admin extends User {}
来源：http://ziv.zhoulong.xyz

Java: class Admin extends User {}
来源：http://pef.sysykeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rvn.pycfn.com

Ruby: class Admin < User; end
来源：http://cku.sxryk.cn

C#:   class Admin : User {}
来源：http://hzz.tian-w.cn

[G06] 重写方法
来源：http://gqn.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://rfv.fengsongda.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ohf.gogol.net.cn

JS:   greet() { return "admin"; }
来源：http://rcu.cheryme.top

TS:   greet(): string { return "admin"; }
来源：http://tan.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://cbj.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ych.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://uuq.gzhubu.top

C#:   public override string Greet() => "admin";
来源：http://hhi.yonumen.top

[G07] 调用父类方法
来源：http://yfg.zhaomingkeji.xyz

Py:   super().greet()
来源：http://pvu.jqgufenzy.top

PHP:  parent::greet();
来源：http://hmc.yongpay.top

JS:   super.greet();
来源：http://jfl.fengsongda.top

TS:   super.greet();
来源：http://uzn.yangfankeji.com

Java: super.greet();
来源：http://yya.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gjm.316326.xyz

Ruby: super
来源：http://ldd.zhongyouzk.top

C#:   base.Greet();
来源：http://thn.chenzaomai.com

[G08] 静态方法与属性
来源：http://fxh.yfazqb.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dyy.sysykeji.top

PHP:  public static function f() {}
来源：http://qal.epnwcf.com

JS:   static f() {}
来源：http://wta.mhx1999.top

TS:   static f(): void {}
来源：http://jck.pengpengdd.cyou

Java: static void f() {}
来源：http://dum.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eiy.xylfe.cn

Ruby: def self.f; end
来源：http://dbf.zhoulong.xyz

C#:   public static void F() {}
来源：http://uaw.andypj.xyz

[G09] 接口 / 抽象类
来源：http://byl.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://fan.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://guz.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://kkr.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://bbq.xziqi.cn

Java: interface Shape { double area(); }
来源：http://sff.ppjwa.cn

Go:   type Shape interface { Area() float64 }
来源：http://owc.havefunace.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xfb.jqgufenzy.top

C#:   interface IShape { double Area(); }
来源：http://usx.shanyushiyangtech.top

[G10] 访问控制
来源：http://ecs.tarul.cn

Py:   约定 _protected / __private（不强制）
来源：http://tsg.chenzaomai.com

PHP:  public / protected / private
来源：http://ctk.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://vnv.mhx1999.top

TS:   public / protected / private
来源：http://vgr.zhongyouzk.top

Java: public / protected / private / 默认包级
来源：http://tcx.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jns.gotoacloud.top

Ruby: public / protected / private
来源：http://jto.yongpay.top


<!-- 参考信息 -->