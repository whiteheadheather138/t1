代发 wailian999

PHP:  substr_count($s, "a");
来源：http://plj.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://ftk.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://wap.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bcg.ywan-chungtsiang.top

Go:   strings.Count(s, "a")
来源：http://dbk.smart0.xyz

Ruby: s.count("a")
来源：http://ana.hywenlv.cn

C#:   s.Count(c => c == 'a')
来源：http://guv.andypj.xyz

[E13] 逐字符遍历
来源：http://jnf.hammf.cn

Py:   for ch in s: print(ch)
来源：http://ddl.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vsi.vqdsnc.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://crh.cheryme.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bei.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jey.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://atj.jinqigufen.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tnv.jinghuilouyu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wwz.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://mqb.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rsj.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rnx.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ojj.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zzg.feifeiyinyue.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://urj.wangshuangyany.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uen.svipenyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mts.ydzc1.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://biq.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://slx.yuanzhike.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oyc.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xfg.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bbh.c1oappe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lbh.birdmap.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wil.vehdjk.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gcu.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vqs.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://roz.cheryme.top

[E16] 数字千分位
来源：http://fhw.sjlbkw.cn

Py:   f"{1234567:,}"
来源：http://mgs.gogol.net.cn

PHP:  number_format(1234567);
来源：http://mwc.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xaw.dianchejie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ioc.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://epr.andypj.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qhf.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yvv.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://mwm.sysykeji.top

[E17] 首字母大写
来源：http://piq.dashuyun.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zig.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://ube.sysykeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hrs.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oow.shanyushiyangtech.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hbm.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://skf.pengpengdd.cyou

Ruby: s.capitalize
来源：http://fbp.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ubi.yueranfly.top

[E18] 模板占位符替换
来源：http://ike.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://srt.yfazqb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://frv.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://saz.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mpe.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fvj.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hmy.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ofk.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wqo.sxryk.cn

[E19] 多行文本按行拆分
来源：http://ddv.feifeiyinyue.top

Py:   s.splitlines()
来源：http://azh.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pfp.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://mcd.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://lvc.ivvv.top

Java: s.lines().toList()
来源：http://oyr.meibo888.top

Go:   strings.Split(s, "\n")
来源：http://jfs.jianghu66.top

Ruby: s.lines
来源：http://tzc.yj20258.top

C#:   s.Split('\n')
来源：http://jhd.zhengqikj.top

[E20] 判断字符串是否为空
来源：http://oqo.fktsv.cn

Py:   if not s:
来源：http://btj.quarkkingdee.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qrb.aibaodan.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rqo.hywenlv.cn

TS:   if (s === "") {}
来源：http://azd.ydjk.org.cn

Java: if (s.isEmpty()) {}
来源：http://gyi.c1oappe.top

Go:   if s == "" {}
来源：http://gzs.smart0.xyz

Ruby: if s.empty?
来源：http://otk.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lfq.tianlin.xyz

[E21] 超长截断加省略号
来源：http://tlw.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pcl.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jrp.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xuw.meibo888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wdc.dianchejie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hgw.9152youxi.cn

Go:   // 按 rune 判断长度后截断
来源：http://qqb.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://omr.sweek.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://seu.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://ozv.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hyu.havefunace.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rjb.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mot.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bfd.jianghu66.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zke.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kor.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://keq.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qye.shangyingyoupin.top

================================================================================
来源：http://faj.fanxiaobao.xyz

F. 文件与目录
来源：http://ugy.cdnleiting.top

================================================================================
来源：http://uhy.jinyuanbaomall.cn

[F01] 读取整个文件
来源：http://dcm.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eyy.gotoacloud.top

PHP:  file_get_contents("a.txt");
来源：http://ubr.jianghu66.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tcq.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ftq.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://crg.svipenyu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ipk.yongpay.top

Ruby: File.read("a.txt")
来源：http://xre.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://fdb.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://oqt.yuanzhike.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://khf.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mza.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lxc.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hlz.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jpm.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rcx.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cbq.aibaodan.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iin.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://jon.fktsv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tsi.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nkq.jqgfzy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mxx.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvo.vqdsnc.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oyq.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jmm.zhoulong.xyz

Ruby: File.write("a.txt", "hi")
来源：http://cxw.guowangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lfv.yuanzhike.top

[F04] 追加写入文件
来源：http://aii.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cvu.hywenlv.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mpe.nanxuanxn.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gkl.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jtx.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://orh.ydzc1.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ggz.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sls.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fpm.c1oappe.top

[F05] 判断文件或目录是否存在
来源：http://hro.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tav.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://tuk.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://zgu.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://jmx.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://nen.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ush.yvedp.cn

Ruby: File.exist?("a.txt")
来源：http://jfj.jqgfzy.top

C#:   File.Exists("a.txt")
来源：http://arw.kuanghao11.cn

[F06] 删除文件
来源：http://ulr.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://lnm.epnwcf.com

PHP:  unlink("a.txt");
来源：http://uyd.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://tyw.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://uhq.shanyushiyangtech.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zdj.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://msf.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://bep.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://rde.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://yxw.yuanzhike.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fpo.hnqzz.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sin.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://edi.zhaomingkeji.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tdf.hammf.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fac.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fjw.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tvr.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://obk.hysaishi.cn

[F08] 遍历目录
来源：http://osu.shuidangran.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://lmk.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ezs.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://goc.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://bam.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aol.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xoo.yueranfly.top

Ruby: Dir.children("dir")
来源：http://fcg.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://egp.birdmap.top

[F09] 获取文件大小
来源：http://fsv.nanxinkj.top

Py:   os.path.getsize("a.txt")
来源：http://npg.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://cqq.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://qof.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://saf.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://wff.iojbl.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aax.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://tzh.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://bxn.yongpay.top

[F10] 取文件扩展名 / 文件名
来源：http://gsr.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://acj.yfazqb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://muv.jiagoushi.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cvr.havefunace.top

TS:   path.extname("a.txt")
来源：http://jrq.shzxlz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kic.sxryk.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kwj.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dqq.xziqi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hzi.uphjek.com

[F11] 复制与移动文件
来源：http://hrf.jqgfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rfl.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ssp.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xea.xziqi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://upg.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ugb.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://whh.mhx1999.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dqn.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gmz.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://kfw.jqgufenzy.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uma.sjlbkw.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xis.hfpthk.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lrb.yueranfly.top

TS:   // 同上
来源：http://jzr.316326.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tcc.0kj1m.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://coa.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rug.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://aaj.chenlongwang.top

================================================================================
来源：http://pjh.jqgfzy.top

G. 面向对象
来源：http://lno.fzhhl.top

================================================================================
来源：http://afz.fehbvm.com

[G01] 定义类
来源：http://pcs.redwolf501.top

Py:   class User: pass
来源：http://qfq.ybcxt.top

PHP:  class User {}
来源：http://gmy.yueranfly.top

JS:   class User {}
来源：http://yqi.hfpthk.cn

TS:   class User { name: string = ""; }
来源：http://ztg.hongshengwenyu.top

Java: class User {}
来源：http://syv.dianchejie.cn

Go:   type User struct { Name string }
来源：http://wja.meibo888.top

Ruby: class User; end
来源：http://oiw.hongshengwenyu.top

C#:   class User {}
来源：http://gqv.xinyue.icu

[G02] 构造函数
来源：http://gsi.hesvh.cn

Py:   def __init__(self, name): self.name = name
来源：http://njf.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://fuo.ywan-chungtsiang.top

JS:   constructor(name) { this.name = name; }
来源：http://icm.zhengqikj.top

TS:   constructor(public name: string) {}
来源：http://zac.ydjk.org.cn

Java: User(String name) { this.name = name; }
来源：http://aum.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xpf.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://sow.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://nvo.daxiang520.top

[G03] 实例属性
来源：http://bvr.pycfn.com

Py:   self.name = "x"
来源：http://wqk.yfazqb.com

PHP:  public string $name = "x";
来源：http://ert.nanxinkj.top

JS:   this.name = "x";
来源：http://lgp.fzhhl.top

TS:   name: string = "x";
来源：http://sne.gogol.net.cn

Java: private String name;
来源：http://jun.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wgs.wangdashe.top

Ruby: @name = "x"
来源：http://bvu.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://nbs.hammf.cn

[G04] 定义方法
来源：http://qph.tarul.cn

Py:   def greet(self): return self.name
来源：http://qtn.yj20258.top

PHP:  public function greet(): string { return $this->name; }
来源：http://gww.sweek.top

JS:   greet() { return this.name; }
来源：http://shj.redwolf501.top

TS:   greet(): string { return this.name; }
来源：http://fpd.xylfe.cn

Java: String greet() { return name; }
来源：http://tab.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ysb.fzhhl.top

Ruby: def greet; @name; end
来源：http://ehf.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://jxw.fanxiaobao.xyz

[G05] 继承
来源：http://gcn.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://qpx.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://uvp.iojbl.cn

JS:   class Admin extends User {}
来源：http://aev.ehwqpu.com

TS:   class Admin extends User {}
来源：http://efu.gotoacloud.top

Java: class Admin extends User {}
来源：http://dos.jinghuilouyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vxi.shzxlz.cn

Ruby: class Admin < User; end
来源：http://tst.dianchejie.cn

C#:   class Admin : User {}
来源：http://hhc.zhiwuduotai.top

[G06] 重写方法
来源：http://njj.316326.xyz

Py:   def greet(self): return "admin"
来源：http://txj.cashguo.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ciu.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://yab.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://vgr.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://pde.yj202588.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uwf.yuanzhike.top

Ruby: def greet; "admin"; end
来源：http://znw.sweek.top

C#:   public override string Greet() => "admin";
来源：http://hjc.cdnleiting.top

[G07] 调用父类方法
来源：http://bxu.feifeiyinyue.top

Py:   super().greet()
来源：http://drz.havefunace.top

PHP:  parent::greet();
来源：http://isc.ywan-chungtsiang.top

JS:   super.greet();
来源：http://pqo.nanxuanxn.top

TS:   super.greet();
来源：http://fqp.hesvh.cn

Java: super.greet();
来源：http://sgq.sysykeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qgc.xuanzx.com

Ruby: super
来源：http://oph.yj202588.top

C#:   base.Greet();
来源：http://evo.sufxvd.cn

[G08] 静态方法与属性
来源：http://zxu.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spg.yangfankeji.com

PHP:  public static function f() {}
来源：http://kaj.fzhhl.top

JS:   static f() {}
来源：http://ceh.ydjk.org.cn

TS:   static f(): void {}
来源：http://lgd.sxryk.cn

Java: static void f() {}
来源：http://ocy.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://fjo.yj20258888.top

Ruby: def self.f; end
来源：http://pxq.zhaomingkeji.xyz

C#:   public static void F() {}
来源：http://dxq.bbcook.cn

[G09] 接口 / 抽象类
来源：http://uwt.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://evg.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://blf.sweek.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ljk.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://zis.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://htq.yuxming.cn

Go:   type Shape interface { Area() float64 }
来源：http://etn.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rpx.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://zfv.chenlongwang.top

[G10] 访问控制
来源：http://eie.aibaodan.cn

Py:   约定 _protected / __private（不强制）
来源：http://vvx.gotoacloud.top

PHP:  public / protected / private
来源：http://aiq.bbcook.cn

JS:   #private 字段；其余公开
来源：http://qyf.chenlongwang.top

TS:   public / protected / private
来源：http://oqd.daxiang520.top

Java: public / protected / private / 默认包级
来源：http://lhr.jianghu66.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sct.daxiang520.top

Ruby: public / protected / private
来源：http://rtg.sjlbkw.cn


<!-- 参考信息 -->