代发 wailian999

Go:   strings.Count(s, "a")
来源：http://nbd.fzhhl.top

Ruby: s.count("a")
来源：http://djb.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://bng.gzhubu.top

[E13] 逐字符遍历
来源：http://ipy.shzxlz.cn

Py:   for ch in s: print(ch)
来源：http://xqp.ehwqpu.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jav.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mkb.wangshuangyany.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ekw.fktsv.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rbu.ydjk.org.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lzy.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qyi.cdnleiting.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://giq.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://gsk.nwbrower.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eoa.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://jag.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hal.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rap.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jza.jqgufenzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qlm.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://com.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gkn.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://yeu.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ann.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xaj.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mxl.jinqigufen.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ksh.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xxn.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cxx.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tbc.feifeiyinyue.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zkq.yuanzhike.top

[E16] 数字千分位
来源：http://ktj.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://sqv.zhengqikj.top

PHP:  number_format(1234567);
来源：http://clj.sjlbkw.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hmk.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nkv.zhiwuduotai.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mka.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cuh.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nhj.zhengqikj.top

C#:   1234567.ToString("N0")
来源：http://lmi.sjlbkw.cn

[E17] 首字母大写
来源：http://noq.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://joe.ydjk.org.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://eyv.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://roz.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://juw.yongpay.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vld.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://znf.xuanzx.com

Ruby: s.capitalize
来源：http://nxl.0kj1m.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://unx.cucudq.cn

[E18] 模板占位符替换
来源：http://yie.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oeu.bbcook.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://utm.xinyue.icu

JS:   tpl.replaceAll("{name}", name)
来源：http://jsc.yanxiufei.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lny.jinqigufen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wkc.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rky.zhengqikj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://myz.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vqx.zycfv.cn

[E19] 多行文本按行拆分
来源：http://pex.guannengcc.top

Py:   s.splitlines()
来源：http://qbb.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rzq.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://woe.shuidangran.top

TS:   s.split(/\r?\n/)
来源：http://nng.jianghu66.top

Java: s.lines().toList()
来源：http://wih.gotoacloud.top

Go:   strings.Split(s, "\n")
来源：http://czi.dashuyun.cn

Ruby: s.lines
来源：http://jxv.jinqigfzy.top

C#:   s.Split('\n')
来源：http://cus.ydzc1.top

[E20] 判断字符串是否为空
来源：http://yqx.cqqwz.cn

Py:   if not s:
来源：http://gye.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sfr.zhengqikj.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mgf.aizwys.cn

TS:   if (s === "") {}
来源：http://jgk.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://oub.shuidangran.top

Go:   if s == "" {}
来源：http://cpm.birdmap.top

Ruby: if s.empty?
来源：http://bxm.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rco.9152youxi.cn

[E21] 超长截断加省略号
来源：http://uws.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pik.bbcook.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rqs.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://whc.c1oappe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kob.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zzg.zycfv.cn

Go:   // 按 rune 判断长度后截断
来源：http://gph.jiagoushi.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oil.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aag.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://yce.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qoh.fehbvm.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xjt.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://axk.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tjm.dashuyun.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eko.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cpl.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://ahu.ybcxt.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sjl.vqdsnc.cn

================================================================================
来源：http://qmt.yj202588.top

F. 文件与目录
来源：http://bwm.fanxiaobao.xyz

================================================================================
来源：http://mhs.fengsongda.top

[F01] 读取整个文件
来源：http://elu.fktsv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qaf.fehbvm.com

PHP:  file_get_contents("a.txt");
来源：http://tub.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://exz.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hrw.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dez.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xap.xuanzx.com

Ruby: File.read("a.txt")
来源：http://wmi.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://cvg.xylfe.cn

[F02] 逐行读取文件
来源：http://phg.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hbl.hesvh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uif.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iqe.yuxming.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://npi.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bqz.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jcv.guannengcc.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zza.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ceq.snrcjt.cn

[F03] 写入文件（覆盖）
来源：http://acb.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kcc.aizwys.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pwx.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://erw.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovt.gzhubu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tzm.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ork.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://pem.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://idb.yangfankeji.com

[F04] 追加写入文件
来源：http://ovp.zdqjudy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://koy.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bcl.xziqi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wvt.xuetiantiany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jik.vehdjk.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nqd.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hlm.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://plh.316326.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qgz.zhiwuduotai.top

[F05] 判断文件或目录是否存在
来源：http://itj.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jst.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://wyw.shanyushiyangtech.top

JS:   fs.existsSync("a.txt")
来源：http://cyy.yuxming.cn

TS:   fs.existsSync("a.txt")
来源：http://hea.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://otu.tanke756.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://trq.tanke756.top

Ruby: File.exist?("a.txt")
来源：http://ewl.xziqi.cn

C#:   File.Exists("a.txt")
来源：http://xcc.tian-w.cn

[F06] 删除文件
来源：http://bml.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://aht.jinghuilouyu.cn

PHP:  unlink("a.txt");
来源：http://hof.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://ecf.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://ocg.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fzr.meibo888.top

Go:   os.Remove("a.txt")
来源：http://isw.chenzaomai.com

Ruby: File.delete("a.txt")
来源：http://yss.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://yvi.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://ara.mhx1999.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rme.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wlx.jlsjyb.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xeq.shanyushiyangtech.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nuh.andypj.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://epr.havefunace.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gox.shuidangran.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://udn.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qwt.sjlbkw.cn

[F08] 遍历目录
来源：http://fur.hammf.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://svy.hnqzz.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://omb.ivvv.top

JS:   fs.readdirSync("dir")
来源：http://ohr.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://xlc.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qpf.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://gkh.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://thn.jiagoushi.top

C#:   Directory.GetFiles("dir")
来源：http://ipi.gogol.net.cn

[F09] 获取文件大小
来源：http://xer.wangdashe.top

Py:   os.path.getsize("a.txt")
来源：http://yve.cashguo.top

PHP:  filesize("a.txt");
来源：http://rkx.ppjwa.cn

JS:   fs.statSync("a.txt").size
来源：http://tlo.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://cyw.meibo888.top

Java: Files.size(Path.of("a.txt"))
来源：http://spd.ctjpmb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://taz.ybcxt.top

Ruby: File.size("a.txt")
来源：http://gtj.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://mqa.zhijiandao.cn

[F10] 取文件扩展名 / 文件名
来源：http://tah.zhaomingkeji.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://umn.sufxvd.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://krc.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lim.shanyushiyangtech.top

TS:   path.extname("a.txt")
来源：http://yuf.sxryk.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zaq.zhiwuduotai.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dew.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ted.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uub.yj20258.top

[F11] 复制与移动文件
来源：http://lax.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://slg.guowangkeji.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vzr.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ilg.yj20258.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wwq.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rby.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://esz.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eaj.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dnt.jyoumei.cn

[F12] CSV 读写
来源：http://acj.yj20258.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ydx.yuanzhike.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://olx.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lya.hcnkem.com

TS:   // 同上
来源：http://pqe.mhx1999.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mvl.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://klg.nwbrower.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wds.jinghuilouyu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mfc.dianchejie.cn

================================================================================
来源：http://bhq.nwbrower.top

G. 面向对象
来源：http://xba.hammf.cn

================================================================================
来源：http://zga.tarul.cn

[G01] 定义类
来源：http://imm.hysaishi.cn

Py:   class User: pass
来源：http://cnh.52xcode.cn

PHP:  class User {}
来源：http://ava.ydjk.org.cn

JS:   class User {}
来源：http://vgz.tarul.cn

TS:   class User { name: string = ""; }
来源：http://fvk.zhiwuduotai.top

Java: class User {}
来源：http://elh.jinqigfzy.top

Go:   type User struct { Name string }
来源：http://uvu.yangfankeji.com

Ruby: class User; end
来源：http://loa.yanxiufei.cn

C#:   class User {}
来源：http://jzq.cashguo.top

[G02] 构造函数
来源：http://aoo.chenzaomai.com

Py:   def __init__(self, name): self.name = name
来源：http://nsl.ehwqpu.com

PHP:  public function __construct(public string $name) {}
来源：http://heg.hnxiangtu.top

JS:   constructor(name) { this.name = name; }
来源：http://qiw.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://cbo.hywenlv.cn

Java: User(String name) { this.name = name; }
来源：http://sul.gotoacloud.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mba.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://ota.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://ylf.sxryk.cn

[G03] 实例属性
来源：http://iuy.gogol.net.cn

Py:   self.name = "x"
来源：http://vqx.dianchejie.cn

PHP:  public string $name = "x";
来源：http://krq.jianghu66.top

JS:   this.name = "x";
来源：http://exp.yangfankeji.com

TS:   name: string = "x";
来源：http://hbl.yj20258888.top

Java: private String name;
来源：http://fjx.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uwk.tarul.cn

Ruby: @name = "x"
来源：http://utu.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://wnz.sweek.top

[G04] 定义方法
来源：http://ewc.tarul.cn

Py:   def greet(self): return self.name
来源：http://fds.snrcjt.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rmw.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://wnm.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://sct.shzxlz.cn

Java: String greet() { return name; }
来源：http://dsq.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mtb.daxiang520.top

Ruby: def greet; @name; end
来源：http://acz.dianchejie.cn

C#:   public string Greet() => Name;
来源：http://ric.cheryme.top

[G05] 继承
来源：http://cwm.yj20258.top

Py:   class Admin(User): pass
来源：http://gli.hnqzz.top

PHP:  class Admin extends User {}
来源：http://ods.ydzc1.top

JS:   class Admin extends User {}
来源：http://bzp.hesvh.cn

TS:   class Admin extends User {}
来源：http://hme.9152youxi.cn

Java: class Admin extends User {}
来源：http://sgg.xingfuxueyuan.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ygx.cheryme.top

Ruby: class Admin < User; end
来源：http://feg.zhixingplan.top

C#:   class Admin : User {}
来源：http://xnp.0kj1m.cn

[G06] 重写方法
来源：http://ynw.shangyingyoupin.top

Py:   def greet(self): return "admin"
来源：http://saa.havefunace.top

PHP:  public function greet(): string { return "admin"; }
来源：http://anw.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://phi.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://udo.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://qow.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qgv.sweek.top

Ruby: def greet; "admin"; end
来源：http://zgn.jianghu66.top

C#:   public override string Greet() => "admin";
来源：http://hpw.gzhubu.top

[G07] 调用父类方法
来源：http://fdq.sufxvd.cn

Py:   super().greet()
来源：http://mrk.dianchejie.cn

PHP:  parent::greet();
来源：http://nub.gzhubu.top

JS:   super.greet();
来源：http://ruf.cashguo.top

TS:   super.greet();
来源：http://ato.vehdjk.com

Java: super.greet();
来源：http://rdx.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://elj.xuanzx.com

Ruby: super
来源：http://mfl.havefunace.top

C#:   base.Greet();
来源：http://mba.sysykeji.top

[G08] 静态方法与属性
来源：http://sik.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jwq.jqgufenzy.top

PHP:  public static function f() {}
来源：http://aec.zhiwuduotai.top

JS:   static f() {}
来源：http://nrb.sxryk.cn

TS:   static f(): void {}
来源：http://lga.shangyingyoupin.top

Java: static void f() {}
来源：http://ruu.c1oappe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ire.yvedp.cn

Ruby: def self.f; end
来源：http://kzr.hysaishi.cn

C#:   public static void F() {}
来源：http://gnz.gaohongyu789.top

[G09] 接口 / 抽象类
来源：http://qyr.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://ldf.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://hnf.yangfankeji.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://rxp.yuxming.cn

TS:   interface Shape { area(): number; }
来源：http://idl.xylfe.cn

Java: interface Shape { double area(); }
来源：http://ylc.zhaomingkeji.xyz

Go:   type Shape interface { Area() float64 }
来源：http://wyq.zhaomingkeji.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xhq.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://tff.guowangkeji.top

[G10] 访问控制
来源：http://abd.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://xmi.hysaishi.cn

PHP:  public / protected / private
来源：http://mht.cashguo.top

JS:   #private 字段；其余公开
来源：http://eyq.hysaishi.cn

TS:   public / protected / private
来源：http://vjv.fehbvm.com

Java: public / protected / private / 默认包级
来源：http://cza.hcnkem.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://jvy.xinyue.icu

Ruby: public / protected / private
来源：http://qaq.fehbvm.com

C#:   public / protected / private / internal
来源：http://urd.zdbjq.cn

[G11] getter / setter
来源：http://klz.ctjpmb.com

Py:   @property 与 @x.setter
来源：http://vxc.ydjk.org.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://eit.zhixingplan.top


<!-- 参考信息 -->