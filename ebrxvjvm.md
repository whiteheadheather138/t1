代发 wailian999

Go:   strings.Count(s, "a")
来源：http://tcr.wangshuangyany.cn

Ruby: s.count("a")
来源：http://kvd.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://pyg.nanxuanxn.top

[E13] 逐字符遍历
来源：http://ffy.pengpengdd.cyou

Py:   for ch in s: print(ch)
来源：http://ivw.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oym.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://udu.ppjwa.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ibv.zhijiandao.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://syp.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nty.fzhhl.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dwj.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jlr.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://wtw.gogol.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ctt.zdbjq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ufx.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bjw.nanxuanxn.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pdj.hongshengwenyu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nvh.tian-w.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ued.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bgb.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ryj.zhengqikj.top

[E15] HTML 转义 / 反转义
来源：http://qxh.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hrb.sysykeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yfm.redwolf501.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://evn.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ejj.sweek.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://prk.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xly.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hbj.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qcr.hnqzz.top

[E16] 数字千分位
来源：http://ygp.nanxuanxn.top

Py:   f"{1234567:,}"
来源：http://zrn.guowangkeji.top

PHP:  number_format(1234567);
来源：http://eds.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://irv.zhijiandao.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zbn.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ain.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cjj.aibaodan.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rvd.jinyuanbaomall.cn

C#:   1234567.ToString("N0")
来源：http://tad.bjfxy.top

[E17] 首字母大写
来源：http://tve.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://huq.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gyr.hesvh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dor.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rdw.pycfn.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ghh.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hmt.uphjek.com

Ruby: s.capitalize
来源：http://hvi.zhaomingkeji.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fwu.guowangkeji.top

[E18] 模板占位符替换
来源：http://vno.shanyushiyangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sqa.yangfankeji.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yoe.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://clx.gogol.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xhj.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://auy.birdmap.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://osv.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ffb.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bss.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://cmo.ppjwa.cn

Py:   s.splitlines()
来源：http://nyb.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://psa.ydjk.org.cn

JS:   s.split(/\r?\n/)
来源：http://pln.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://wlu.xuanzx.com

Java: s.lines().toList()
来源：http://ceb.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://sso.zhixingplan.top

Ruby: s.lines
来源：http://ohi.yvedp.cn

C#:   s.Split('\n')
来源：http://wpo.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://rom.sweek.top

Py:   if not s:
来源：http://bck.nanxuanxn.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kav.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kav.c1oappe.top

TS:   if (s === "") {}
来源：http://mjo.hywenlv.cn

Java: if (s.isEmpty()) {}
来源：http://nxl.yj202588.top

Go:   if s == "" {}
来源：http://avw.redwolf501.top

Ruby: if s.empty?
来源：http://ize.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ooq.haohaochexian.top

[E21] 超长截断加省略号
来源：http://jrb.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cst.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dmd.cucudq.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ocf.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qrm.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qgk.snrcjt.cn

Go:   // 按 rune 判断长度后截断
来源：http://dhp.meibo888.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oiu.ywan-chungtsiang.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rer.tianlin.xyz

[E22] 字节长度与字符长度
来源：http://lmn.epnwcf.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zhq.jinghuilouyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ijw.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbm.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ixb.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ksj.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dya.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://zrt.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gxl.chenlongwang.top

================================================================================
来源：http://onc.cdnleiting.top

F. 文件与目录
来源：http://vsh.xingfuxueyuan.xyz

================================================================================
来源：http://raq.zhaomingkeji.xyz

[F01] 读取整个文件
来源：http://pot.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sim.zycfv.cn

PHP:  file_get_contents("a.txt");
来源：http://cze.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://usi.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xct.gogol.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://arn.hammf.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xzd.vehdjk.com

Ruby: File.read("a.txt")
来源：http://wly.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://gan.ehwqpu.com

[F02] 逐行读取文件
来源：http://qsg.9152youxi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dbn.hnqzz.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wdm.havefunace.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bvo.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bha.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cjc.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sbu.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jee.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tgl.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://wdp.ydjk.org.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmm.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bdx.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://juc.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jsz.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://msy.ydjk.org.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ehs.aizwys.cn

Ruby: File.write("a.txt", "hi")
来源：http://uhm.yvedp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://taq.xingfuxueyuan.xyz

[F04] 追加写入文件
来源：http://yjd.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nau.gogol.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://whu.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wdm.hysaishi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mqo.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bon.dashuyun.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sca.hcnkem.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://flj.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qwf.iojbl.cn

[F05] 判断文件或目录是否存在
来源：http://xnj.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rhg.wangshuangyany.cn

PHP:  file_exists("a.txt");
来源：http://vcp.guowangkeji.top

JS:   fs.existsSync("a.txt")
来源：http://kja.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://ehd.nwbrower.top

Java: Files.exists(Path.of("a.txt"))
来源：http://juc.smart0.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dlc.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://osy.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://bbw.hongshengwenyu.top

[F06] 删除文件
来源：http://mif.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://sqx.hcnkem.com

PHP:  unlink("a.txt");
来源：http://wrw.havefunace.top

JS:   fs.unlinkSync("a.txt")
来源：http://tpy.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://ncz.tanke756.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qwh.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://ycr.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://iat.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://lhz.shuidangran.top

[F07] 创建目录（含多级）
来源：http://myu.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qom.gogol.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dwg.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wth.ehwqpu.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xek.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qiq.sweek.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gpz.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gwh.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jaq.tarul.cn

[F08] 遍历目录
来源：http://itw.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uab.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://quz.guannengcc.top

JS:   fs.readdirSync("dir")
来源：http://uod.sjlbkw.cn

TS:   fs.readdirSync("dir")
来源：http://sqq.meibo888.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abt.cucudq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cbn.hnqzz.top

Ruby: Dir.children("dir")
来源：http://ely.shzxlz.cn

C#:   Directory.GetFiles("dir")
来源：http://kyq.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://xsf.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://azv.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://lzc.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://nrn.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://iuw.yj20258.top

Java: Files.size(Path.of("a.txt"))
来源：http://lcq.smart0.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wga.kuanghao11.cn

Ruby: File.size("a.txt")
来源：http://gtz.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://lqt.yangfankeji.com

[F10] 取文件扩展名 / 文件名
来源：http://dxq.vehdjk.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bxq.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://luz.zhiwuduotai.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ufg.zycfv.cn

TS:   path.extname("a.txt")
来源：http://cqj.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kls.wangshuangyany.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eev.hongshengwenyu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lym.zhijiandao.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rcu.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://btu.hnxiangtu.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yzn.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ijw.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://idh.jinghuilouyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zij.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gzs.hfpthk.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hbb.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://byq.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qdc.hywenlv.cn

[F12] CSV 读写
来源：http://xes.xziqi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bfv.gotoacloud.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zzi.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rzh.yonumen.top

TS:   // 同上
来源：http://wqz.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cer.fehbvm.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kwe.epnwcf.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://okg.epnwcf.com

C#:   // 无内置：用 CsvHelper 库
来源：http://vtu.fehbvm.com

================================================================================
来源：http://ado.gzhubu.top

G. 面向对象
来源：http://ikb.haohaochexian.top

================================================================================
来源：http://shi.guowangkeji.top

[G01] 定义类
来源：http://lmo.zdqjudy.top

Py:   class User: pass
来源：http://wpw.tanke756.top

PHP:  class User {}
来源：http://nbl.daria6918.cn

JS:   class User {}
来源：http://zem.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://jzs.xingfuxueyuan.xyz

Java: class User {}
来源：http://xwo.havefunace.top

Go:   type User struct { Name string }
来源：http://etr.guannengcc.top

Ruby: class User; end
来源：http://apa.chenlongwang.top

C#:   class User {}
来源：http://xat.wangshuangyany.cn

[G02] 构造函数
来源：http://her.daxiang520.top

Py:   def __init__(self, name): self.name = name
来源：http://add.xinyue.icu

PHP:  public function __construct(public string $name) {}
来源：http://ued.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://aat.yuanzhike.top

TS:   constructor(public name: string) {}
来源：http://mcq.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://cqp.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wna.hesvh.cn

Ruby: def initialize(name); @name = name; end
来源：http://qxl.sysykeji.top

C#:   public User(string name) { Name = name; }
来源：http://gby.ehwqpu.com

[G03] 实例属性
来源：http://gsr.shuidangran.top

Py:   self.name = "x"
来源：http://axc.tarul.cn

PHP:  public string $name = "x";
来源：http://dky.yongpay.top

JS:   this.name = "x";
来源：http://izy.feifeiyinyue.top

TS:   name: string = "x";
来源：http://tts.hesvh.cn

Java: private String name;
来源：http://vow.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://svc.yanxiufei.cn

Ruby: @name = "x"
来源：http://piw.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://xgj.dashuyun.cn

[G04] 定义方法
来源：http://kkf.jinqigufen.top

Py:   def greet(self): return self.name
来源：http://oah.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rcc.ehwqpu.com

JS:   greet() { return this.name; }
来源：http://zsx.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://dyr.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://afi.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yxg.gotoacloud.top

Ruby: def greet; @name; end
来源：http://qla.52xcode.cn

C#:   public string Greet() => Name;
来源：http://jli.haohaochexian.top

[G05] 继承
来源：http://wkv.zhongyouzk.top

Py:   class Admin(User): pass
来源：http://wtt.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://mjt.hnqzz.top

JS:   class Admin extends User {}
来源：http://ewy.nanxuanxn.top

TS:   class Admin extends User {}
来源：http://usq.havefunace.top

Java: class Admin extends User {}
来源：http://btl.hfpthk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fdt.wangdashe.top

Ruby: class Admin < User; end
来源：http://utr.birdmap.top

C#:   class Admin : User {}
来源：http://mkk.jlsjyb.cn

[G06] 重写方法
来源：http://zbw.bjfxy.top

Py:   def greet(self): return "admin"
来源：http://cmf.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cuy.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://afl.fengsongda.top

TS:   greet(): string { return "admin"; }
来源：http://yoz.fengsongda.top

Java: @Override String greet() { return "admin"; }
来源：http://tfa.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nuc.yongpay.top

Ruby: def greet; "admin"; end
来源：http://qzc.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://oow.wangdashe.top

[G07] 调用父类方法
来源：http://kur.tanke756.top

Py:   super().greet()
来源：http://rqq.havefunace.top

PHP:  parent::greet();
来源：http://hod.jqgufenzy.top

JS:   super.greet();
来源：http://mko.52xcode.cn

TS:   super.greet();
来源：http://jmv.ydjk.org.cn

Java: super.greet();
来源：http://hzj.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ncg.ybcxt.top

Ruby: super
来源：http://bvz.zdqjudy.top

C#:   base.Greet();
来源：http://uvn.quarkkingdee.top

[G08] 静态方法与属性
来源：http://dzm.jyoumei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lcd.gogol.net.cn

PHP:  public static function f() {}
来源：http://qie.ivvv.top

JS:   static f() {}
来源：http://jki.hammf.cn

TS:   static f(): void {}
来源：http://lca.meibo888.top

Java: static void f() {}
来源：http://buq.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hin.dianchejie.cn

Ruby: def self.f; end
来源：http://asx.shangyingyoupin.top

C#:   public static void F() {}
来源：http://pzm.bbcook.cn

[G09] 接口 / 抽象类
来源：http://qkd.sjlbkw.cn

Py:   from abc import ABC, abstractmethod
来源：http://ymw.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://jbe.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ztj.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://wlj.sjlbkw.cn

Java: interface Shape { double area(); }
来源：http://khe.mhx1999.top

Go:   type Shape interface { Area() float64 }
来源：http://bqs.jyoumei.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sbr.jlsjyb.cn

C#:   interface IShape { double Area(); }
来源：http://hah.cqqwz.cn

[G10] 访问控制
来源：http://ehv.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://xjj.ydjk.org.cn

PHP:  public / protected / private
来源：http://jgj.cheryme.top

JS:   #private 字段；其余公开
来源：http://npr.jlsjyb.cn

TS:   public / protected / private
来源：http://cnh.jinqigfzy.top

Java: public / protected / private / 默认包级
来源：http://yhe.xuetiantiany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kzj.zhongyouzk.top

Ruby: public / protected / private
来源：http://bgy.jianghu66.top

C#:   public / protected / private / internal
来源：http://pji.vehdjk.com

[G11] getter / setter
来源：http://aut.pycfn.com

Py:   @property 与 @x.setter
来源：http://hfi.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fwl.sjlbkw.cn


<!-- 参考信息 -->