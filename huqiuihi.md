代发 wailian999

Py:   for ch in s: print(ch)
来源：http://cpr.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ytv.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://drp.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qlq.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ulg.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xtp.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mhy.havefunace.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hpb.ybcxt.top

[E14] URL 编码与 Base64
来源：http://dcp.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ubw.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nsm.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jnh.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bbg.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fff.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ldx.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zmn.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hjo.tian-w.cn

[E15] HTML 转义 / 反转义
来源：http://wqi.xuanzx.com

Py:   html.escape(s);  html.unescape(s)
来源：http://npv.tian-w.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ydn.jqgfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zrb.jqgfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ghs.zhengqikj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://urp.quarkkingdee.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qja.smart0.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xxv.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ord.redwolf501.top

[E16] 数字千分位
来源：http://juz.xinyue.icu

Py:   f"{1234567:,}"
来源：http://rzt.wangdashe.top

PHP:  number_format(1234567);
来源：http://vng.hysaishi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zrj.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://adw.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vck.ctjpmb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nuw.jqgfzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ijp.andypj.xyz

C#:   1234567.ToString("N0")
来源：http://wkp.jinyuanbaomall.cn

[E17] 首字母大写
来源：http://dcr.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nwl.dashuyun.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vly.zhongyouzk.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tyj.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fhu.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zgy.chenlongwang.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xhx.havefunace.top

Ruby: s.capitalize
来源：http://qdo.iojbl.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nlj.birdmap.top

[E18] 模板占位符替换
来源：http://vkb.hfpthk.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://itt.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dzh.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://qfx.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yot.yj20258888.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bvb.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xtb.pengpengdd.cyou

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dbz.ctjpmb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vna.yj20258.top

[E19] 多行文本按行拆分
来源：http://olf.quarkkingdee.top

Py:   s.splitlines()
来源：http://jsm.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dfy.pycfn.com

JS:   s.split(/\r?\n/)
来源：http://pvc.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://msj.sweek.top

Java: s.lines().toList()
来源：http://odp.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://gfd.guannengcc.top

Ruby: s.lines
来源：http://sav.52xcode.cn

C#:   s.Split('\n')
来源：http://wzi.hesvh.cn

[E20] 判断字符串是否为空
来源：http://auz.jiagoushi.top

Py:   if not s:
来源：http://uuc.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uko.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vlb.chenzaomai.com

TS:   if (s === "") {}
来源：http://tcw.dashuyun.cn

Java: if (s.isEmpty()) {}
来源：http://zsm.c1oappe.top

Go:   if s == "" {}
来源：http://hqk.gaohongyu789.top

Ruby: if s.empty?
来源：http://afp.sysykeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mvk.jqgfzy.top

[E21] 超长截断加省略号
来源：http://mgh.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://daj.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jsi.sysykeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iql.chenzaomai.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yws.yanxiufei.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yuo.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://huz.yonumen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iun.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bxs.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://xbt.redwolf501.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hqn.redwolf501.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggp.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdi.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jaq.shanyushiyangtech.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kvj.yuxming.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qzb.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://mem.tian-w.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vap.zhaomingkeji.xyz

================================================================================
来源：http://saq.mhx1999.top

F. 文件与目录
来源：http://ojr.shanyushiyangtech.top

================================================================================
来源：http://qtk.svipenyu.cn

[F01] 读取整个文件
来源：http://red.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tqs.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://yue.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dnf.havefunace.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zrv.daria6918.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://osh.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oyx.birdmap.top

Ruby: File.read("a.txt")
来源：http://xpc.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://evg.xinyue.icu

[F02] 逐行读取文件
来源：http://lxf.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nub.shzxlz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hcv.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://via.nwbrower.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jgn.tian-w.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vvs.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kgr.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ukv.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wac.hongshengwenyu.top

[F03] 写入文件（覆盖）
来源：http://xki.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rwv.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gxt.c1oappe.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://loz.zhoulong.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frk.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vrx.ywan-chungtsiang.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ira.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://hrl.chenzaomai.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yll.zdbjq.cn

[F04] 追加写入文件
来源：http://oit.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ymk.zdbjq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yrm.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dnv.feifeiyinyue.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cuk.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wci.52xcode.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uxx.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vxf.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://frn.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://pwh.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yqd.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://rvw.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://ivg.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://zsi.zhijiandao.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hwp.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ejc.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://yxq.jyoumei.cn

C#:   File.Exists("a.txt")
来源：http://doz.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://xgm.sweek.top

Py:   os.remove("a.txt")
来源：http://lmf.yj202588.top

PHP:  unlink("a.txt");
来源：http://vng.jianghu66.top

JS:   fs.unlinkSync("a.txt")
来源：http://jri.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jhr.zhaomingkeji.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yfp.meibo888.top

Go:   os.Remove("a.txt")
来源：http://tku.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://sle.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://pwn.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://vkz.kuanghao11.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://woh.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zdf.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://khd.iojbl.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://faf.zdqjudy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vgj.yj202588.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zky.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tbg.jianghu66.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tsd.yonumen.top

[F08] 遍历目录
来源：http://vgo.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hnv.ydjk.org.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yya.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://kco.0kj1m.cn

TS:   fs.readdirSync("dir")
来源：http://dyt.jiagoushi.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://csv.xuetiantiany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nxp.fzhhl.top

Ruby: Dir.children("dir")
来源：http://pcx.andypj.xyz

C#:   Directory.GetFiles("dir")
来源：http://nfa.svipenyu.cn

[F09] 获取文件大小
来源：http://msr.hcnkem.com

Py:   os.path.getsize("a.txt")
来源：http://xcj.cheryme.top

PHP:  filesize("a.txt");
来源：http://tfh.epnwcf.com

JS:   fs.statSync("a.txt").size
来源：http://dqi.fehbvm.com

TS:   fs.statSync("a.txt").size
来源：http://cmy.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zfj.hnqzz.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yrx.zhaomingkeji.xyz

Ruby: File.size("a.txt")
来源：http://lrm.cdnleiting.top

C#:   new FileInfo("a.txt").Length
来源：http://ljz.jqgfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://xxh.gaohongyu789.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kdc.zhixingplan.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zjp.quarkkingdee.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qak.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://cee.epnwcf.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hzp.hysaishi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ozt.sysykeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bzq.cashguo.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fiw.sxryk.cn

[F11] 复制与移动文件
来源：http://vag.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rqr.gaohongyu789.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lie.zhaomingkeji.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://syd.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ycn.yj20258888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dtm.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vbz.nanxuanxn.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cks.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tqw.shuidangran.top

[F12] CSV 读写
来源：http://tjy.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qed.epnwcf.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xxc.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fjw.yongpay.top

TS:   // 同上
来源：http://ynr.0kj1m.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dws.wangdashe.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fry.cdnleiting.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nsf.shanyushiyangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hlc.yongpay.top

================================================================================
来源：http://fpw.yuanzhike.top

G. 面向对象
来源：http://pxl.andypj.xyz

================================================================================
来源：http://ddo.9152youxi.cn

[G01] 定义类
来源：http://vmk.sjlbkw.cn

Py:   class User: pass
来源：http://aub.zhoulong.xyz

PHP:  class User {}
来源：http://jnf.kuanghao11.cn

JS:   class User {}
来源：http://kax.chenzaomai.com

TS:   class User { name: string = ""; }
来源：http://kms.nanxuanxn.top

Java: class User {}
来源：http://qde.hammf.cn

Go:   type User struct { Name string }
来源：http://gau.birdmap.top

Ruby: class User; end
来源：http://dke.gotoacloud.top

C#:   class User {}
来源：http://xuy.nanxinkj.top

[G02] 构造函数
来源：http://cey.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://afl.gotoacloud.top

PHP:  public function __construct(public string $name) {}
来源：http://kiw.zhijiandao.cn

JS:   constructor(name) { this.name = name; }
来源：http://cde.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://hpf.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://ngh.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gke.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://xsg.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://yzn.zhaomingkeji.xyz

[G03] 实例属性
来源：http://jdn.jianghu66.top

Py:   self.name = "x"
来源：http://eoa.bjfxy.top

PHP:  public string $name = "x";
来源：http://vnr.gaohongyu789.top

JS:   this.name = "x";
来源：http://dqt.sufxvd.cn

TS:   name: string = "x";
来源：http://bls.aibaodan.cn

Java: private String name;
来源：http://hgk.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nku.andypj.xyz

Ruby: @name = "x"
来源：http://vjm.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://hlj.jlsjyb.cn

[G04] 定义方法
来源：http://qwf.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://hiw.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mnx.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://gzd.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://qkw.ehwqpu.com

Java: String greet() { return name; }
来源：http://fht.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://piq.ywan-chungtsiang.top

Ruby: def greet; @name; end
来源：http://imw.316326.xyz

C#:   public string Greet() => Name;
来源：http://yzz.shanyushiyangtech.top

[G05] 继承
来源：http://cgk.0kj1m.cn

Py:   class Admin(User): pass
来源：http://esu.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://pfy.fehbvm.com

JS:   class Admin extends User {}
来源：http://nzu.gzhubu.top

TS:   class Admin extends User {}
来源：http://atb.yj20258.top

Java: class Admin extends User {}
来源：http://rax.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qoi.fengsongda.top

Ruby: class Admin < User; end
来源：http://hhh.fzhhl.top

C#:   class Admin : User {}
来源：http://pew.yfazqb.com

[G06] 重写方法
来源：http://itc.tarul.cn

Py:   def greet(self): return "admin"
来源：http://cwr.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pph.uphjek.com

JS:   greet() { return "admin"; }
来源：http://clc.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://hrz.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://cco.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dqo.havefunace.top

Ruby: def greet; "admin"; end
来源：http://dix.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://olx.ybcxt.top

[G07] 调用父类方法
来源：http://qov.havefunace.top

Py:   super().greet()
来源：http://ujo.pycfn.com

PHP:  parent::greet();
来源：http://ofv.daxiang520.top

JS:   super.greet();
来源：http://lxc.nanxinkj.top

TS:   super.greet();
来源：http://qap.jiagoushi.top

Java: super.greet();
来源：http://riz.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zhi.mhx1999.top

Ruby: super
来源：http://mgy.chenzaomai.com

C#:   base.Greet();
来源：http://gba.andypj.xyz

[G08] 静态方法与属性
来源：http://jcc.cucudq.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dbi.jinyuanbaomall.cn

PHP:  public static function f() {}
来源：http://rsv.bjfxy.top

JS:   static f() {}
来源：http://wzf.xziqi.cn

TS:   static f(): void {}
来源：http://xkl.zdbjq.cn

Java: static void f() {}
来源：http://hqu.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sea.uphjek.com

Ruby: def self.f; end
来源：http://mqs.shangyingyoupin.top

C#:   public static void F() {}
来源：http://jwy.yvedp.cn

[G09] 接口 / 抽象类
来源：http://kdl.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://zlm.ywan-chungtsiang.top

PHP:  interface Shape { public function area(): float; }
来源：http://zab.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://huj.tianlin.xyz

TS:   interface Shape { area(): number; }
来源：http://mss.jqgfzy.top

Java: interface Shape { double area(); }
来源：http://jwg.yfazqb.com

Go:   type Shape interface { Area() float64 }
来源：http://cau.yonumen.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://inb.ehwqpu.com

C#:   interface IShape { double Area(); }
来源：http://pot.daria6918.cn

[G10] 访问控制
来源：http://cap.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://cbu.jqgfzy.top

PHP:  public / protected / private
来源：http://xrt.cheryme.top

JS:   #private 字段；其余公开
来源：http://qko.hywenlv.cn

TS:   public / protected / private
来源：http://tak.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://hnn.quarkkingdee.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ect.bbcook.cn

Ruby: public / protected / private
来源：http://vfw.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://upx.mhx1999.top

[G11] getter / setter
来源：http://vxw.cdnleiting.top

Py:   @property 与 @x.setter
来源：http://svs.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://qok.havefunace.top

JS:   get name() { return this._name; }
来源：http://ppd.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://yxx.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://gzy.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gug.guannengcc.top


<!-- 参考信息 -->