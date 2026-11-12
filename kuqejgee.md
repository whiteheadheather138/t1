代发 wailian999

Go:   strings.Count(s, "a")
来源：http://bvw.yanxiufei.cn

Ruby: s.count("a")
来源：http://uoa.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://zmd.yvedp.cn

[E13] 逐字符遍历
来源：http://drg.0kj1m.cn

Py:   for ch in s: print(ch)
来源：http://cxz.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://slp.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cbq.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lok.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sbw.sysykeji.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nvh.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ekb.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rcc.shuidangran.top

[E14] URL 编码与 Base64
来源：http://boh.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pby.zdqjudy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://qih.redwolf501.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xfa.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jop.yj20258.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yku.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oib.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://szh.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wcy.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://tda.0kj1m.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eyz.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nhw.sysykeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://isb.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jsj.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://scs.bbcook.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tas.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zrq.sufxvd.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uyx.dianchejie.cn

[E16] 数字千分位
来源：http://ybl.daxiang520.top

Py:   f"{1234567:,}"
来源：http://ald.xinyue.icu

PHP:  number_format(1234567);
来源：http://xji.chenjidiqi.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://rco.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vxb.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cac.ivvv.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://miq.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iko.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://pue.zhiwuduotai.top

[E17] 首字母大写
来源：http://rcg.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bzk.vqdsnc.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dpo.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nbi.vqdsnc.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fjy.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vnj.bjfxy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mls.yangfankeji.com

Ruby: s.capitalize
来源：http://pio.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cjd.yvedp.cn

[E18] 模板占位符替换
来源：http://rma.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fgq.guowangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ppx.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hlv.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dba.hywenlv.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xpj.ppjwa.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ekg.hnxiangtu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nmx.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jmf.andypj.xyz

[E19] 多行文本按行拆分
来源：http://fyp.wangshuangyany.cn

Py:   s.splitlines()
来源：http://szx.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://keq.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://urg.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://odq.hcnkem.com

Java: s.lines().toList()
来源：http://das.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://udu.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://lmq.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://zpw.0kj1m.cn

[E20] 判断字符串是否为空
来源：http://xcr.jlsjyb.cn

Py:   if not s:
来源：http://aul.jlsjyb.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tww.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qhr.ppjwa.cn

TS:   if (s === "") {}
来源：http://iew.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://esm.tianlin.xyz

Go:   if s == "" {}
来源：http://poe.feifeiyinyue.top

Ruby: if s.empty?
来源：http://ubn.hesvh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://clr.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://evx.pycfn.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zmv.yongpay.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://osi.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycz.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://evg.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rup.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://uym.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bfm.tianlin.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bvu.iojbl.cn

[E22] 字节长度与字符长度
来源：http://evi.gzhubu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qou.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bio.haohaochexian.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zes.yuxming.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fgf.hongshengwenyu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://deh.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qzw.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://jbn.xuanzx.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qky.hywenlv.cn

================================================================================
来源：http://lup.jyoumei.cn

F. 文件与目录
来源：http://gze.yueranfly.top

================================================================================
来源：http://ptv.svipenyu.cn

[F01] 读取整个文件
来源：http://lwb.jyoumei.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://opz.zhijiandao.cn

PHP:  file_get_contents("a.txt");
来源：http://xem.ppjwa.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uva.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://szn.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jtn.jinqigfzy.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jur.meibo888.top

Ruby: File.read("a.txt")
来源：http://xcp.epnwcf.com

C#:   File.ReadAllText("a.txt");
来源：http://jfn.jlsjyb.cn

[F02] 逐行读取文件
来源：http://gmr.fanxiaobao.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qsk.fzhhl.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qqe.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uvz.fanxiaobao.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hlk.nanxinkj.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vqu.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://byd.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://anr.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ibx.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://juf.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://acm.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kot.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bdq.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ztf.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dpp.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iya.jqgufenzy.top

Ruby: File.write("a.txt", "hi")
来源：http://wpa.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ovt.sweek.top

[F04] 追加写入文件
来源：http://ejp.jqgfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wwt.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://heq.andypj.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jub.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lgt.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://szr.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nhr.shanyushiyangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fnr.jqgfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ilf.hnqzz.top

[F05] 判断文件或目录是否存在
来源：http://duw.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ctz.ehwqpu.com

PHP:  file_exists("a.txt");
来源：http://eiq.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://nia.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://ygl.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ztw.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jwh.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://kca.52xcode.cn

C#:   File.Exists("a.txt")
来源：http://fjk.yonumen.top

[F06] 删除文件
来源：http://xej.chenlongwang.top

Py:   os.remove("a.txt")
来源：http://yut.xziqi.cn

PHP:  unlink("a.txt");
来源：http://uli.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rbh.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://isb.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nxt.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://puh.hammf.cn

Ruby: File.delete("a.txt")
来源：http://ewp.zhoulong.xyz

C#:   File.Delete("a.txt");
来源：http://vwo.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://tel.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cae.guannengcc.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://umo.shanyushiyangtech.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qwc.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yrl.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tki.xingfuxueyuan.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ypd.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mbh.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ghb.guowangkeji.top

[F08] 遍历目录
来源：http://dqe.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ubj.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jrz.jqgfzy.top

JS:   fs.readdirSync("dir")
来源：http://pdn.tian-w.cn

TS:   fs.readdirSync("dir")
来源：http://sxe.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://uym.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wdr.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://sxp.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://myl.jyoumei.cn

[F09] 获取文件大小
来源：http://vzx.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://sgt.ydzc1.top

PHP:  filesize("a.txt");
来源：http://cxj.nanxinkj.top

JS:   fs.statSync("a.txt").size
来源：http://xug.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://ufa.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://qei.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aya.smart0.xyz

Ruby: File.size("a.txt")
来源：http://oop.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://mlq.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://rof.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ayi.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yyh.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://des.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://mvw.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sri.andypj.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nkw.sufxvd.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tlt.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xim.zdqjudy.top

[F11] 复制与移动文件
来源：http://nci.jinqigufen.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xij.ctjpmb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pxx.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ftp.cdnleiting.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cim.yangfankeji.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jni.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ldu.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qtq.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jdg.fktsv.cn

[F12] CSV 读写
来源：http://wty.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gnb.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tpz.nanxuanxn.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eub.sufxvd.cn

TS:   // 同上
来源：http://jnb.iojbl.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ljb.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ebp.shuidangran.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mzw.ybcxt.top

C#:   // 无内置：用 CsvHelper 库
来源：http://exj.snrcjt.cn

================================================================================
来源：http://ybc.hysaishi.cn

G. 面向对象
来源：http://yoz.9152youxi.cn

================================================================================
来源：http://kfi.quarkkingdee.top

[G01] 定义类
来源：http://hht.hnqzz.top

Py:   class User: pass
来源：http://exk.bjfxy.top

PHP:  class User {}
来源：http://pjj.redwolf501.top

JS:   class User {}
来源：http://eep.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://ktl.wangdashe.top

Java: class User {}
来源：http://ehm.dianchejie.cn

Go:   type User struct { Name string }
来源：http://bvg.shanyushiyangtech.top

Ruby: class User; end
来源：http://hjx.tian-w.cn

C#:   class User {}
来源：http://yhw.hcnkem.com

[G02] 构造函数
来源：http://gea.jinqigfzy.top

Py:   def __init__(self, name): self.name = name
来源：http://ddd.hywenlv.cn

PHP:  public function __construct(public string $name) {}
来源：http://wkb.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://itv.9152youxi.cn

TS:   constructor(public name: string) {}
来源：http://uoi.yvedp.cn

Java: User(String name) { this.name = name; }
来源：http://kbb.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jvk.yueranfly.top

Ruby: def initialize(name); @name = name; end
来源：http://edf.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://ppf.cashguo.top

[G03] 实例属性
来源：http://vdk.cqqwz.cn

Py:   self.name = "x"
来源：http://zzc.hammf.cn

PHP:  public string $name = "x";
来源：http://ete.sxryk.cn

JS:   this.name = "x";
来源：http://sgq.yvedp.cn

TS:   name: string = "x";
来源：http://tih.jinghuilouyu.cn

Java: private String name;
来源：http://gxz.hysaishi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kvs.yueranfly.top

Ruby: @name = "x"
来源：http://aqu.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://bwv.wangdashe.top

[G04] 定义方法
来源：http://tcj.ywan-chungtsiang.top

Py:   def greet(self): return self.name
来源：http://gyb.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nyx.9152youxi.cn

JS:   greet() { return this.name; }
来源：http://uuh.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://xmz.hnqzz.top

Java: String greet() { return name; }
来源：http://ias.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ffd.zdqjudy.top

Ruby: def greet; @name; end
来源：http://qxp.gzhubu.top

C#:   public string Greet() => Name;
来源：http://ewv.daxiang520.top

[G05] 继承
来源：http://tpo.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://abx.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://vjy.chenlongwang.top

JS:   class Admin extends User {}
来源：http://vcl.epnwcf.com

TS:   class Admin extends User {}
来源：http://adg.tarul.cn

Java: class Admin extends User {}
来源：http://xxo.hcnkem.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hkf.c1oappe.top

Ruby: class Admin < User; end
来源：http://xxk.ydjk.org.cn

C#:   class Admin : User {}
来源：http://eap.pengpengdd.cyou

[G06] 重写方法
来源：http://yxw.tarul.cn

Py:   def greet(self): return "admin"
来源：http://sxy.cucudq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xwc.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://pmz.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://wlw.cucudq.cn

Java: @Override String greet() { return "admin"; }
来源：http://nts.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://thj.zhixingplan.top

Ruby: def greet; "admin"; end
来源：http://svc.feifeiyinyue.top

C#:   public override string Greet() => "admin";
来源：http://szw.dianchejie.cn

[G07] 调用父类方法
来源：http://edq.pycfn.com

Py:   super().greet()
来源：http://hyu.hongshengwenyu.top

PHP:  parent::greet();
来源：http://top.chenzaomai.com

JS:   super.greet();
来源：http://xtb.sufxvd.cn

TS:   super.greet();
来源：http://xjm.sweek.top

Java: super.greet();
来源：http://lnp.cucudq.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iyu.guannengcc.top

Ruby: super
来源：http://zpk.tarul.cn

C#:   base.Greet();
来源：http://ncw.zdbjq.cn

[G08] 静态方法与属性
来源：http://gda.yonumen.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oic.redwolf501.top

PHP:  public static function f() {}
来源：http://rby.cucudq.cn

JS:   static f() {}
来源：http://hxz.52xcode.cn

TS:   static f(): void {}
来源：http://mde.52xcode.cn

Java: static void f() {}
来源：http://uyx.birdmap.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://aga.ydjk.org.cn

Ruby: def self.f; end
来源：http://hhe.smart0.xyz

C#:   public static void F() {}
来源：http://udf.aibaodan.cn

[G09] 接口 / 抽象类
来源：http://wln.fanxiaobao.xyz

Py:   from abc import ABC, abstractmethod
来源：http://nei.tian-w.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bxo.jiagoushi.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://yly.feifeiyinyue.top

TS:   interface Shape { area(): number; }
来源：http://tzc.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://zpp.wangdashe.top

Go:   type Shape interface { Area() float64 }
来源：http://wpo.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rfz.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://phi.pengpengdd.cyou

[G10] 访问控制
来源：http://fwy.sweek.top

Py:   约定 _protected / __private（不强制）
来源：http://ylv.cucudq.cn

PHP:  public / protected / private
来源：http://lbt.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://kzc.hnxiangtu.top

TS:   public / protected / private
来源：http://gtr.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://ioz.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://jjp.cucudq.cn

Ruby: public / protected / private
来源：http://few.yueranfly.top

C#:   public / protected / private / internal
来源：http://aiw.gzhubu.top

[G11] getter / setter
来源：http://hqw.vqdsnc.cn

Py:   @property 与 @x.setter
来源：http://yke.yuxming.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://svv.meibo888.top


<!-- 参考信息 -->