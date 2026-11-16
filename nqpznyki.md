代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hei.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hpo.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://xug.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://brn.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pvs.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yfp.jinyuanbaomall.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tso.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lyh.zdqjudy.top

[E14] URL 编码与 Base64
来源：http://fbg.havefunace.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zsv.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vzf.cqqwz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gos.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dbd.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://urw.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hik.fanxiaobao.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lvn.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://quq.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://cph.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bbz.tianlin.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://che.hongshengwenyu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vex.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://wlz.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mqp.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xir.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nhi.gzhubu.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nla.ywan-chungtsiang.top

[E16] 数字千分位
来源：http://peu.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://gjs.cucudq.cn

PHP:  number_format(1234567);
来源：http://wfg.zdbjq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eyz.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ber.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zol.iojbl.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ybx.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iac.jinqigfzy.top

C#:   1234567.ToString("N0")
来源：http://vfg.tarul.cn

[E17] 首字母大写
来源：http://tau.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zea.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nev.jqgfzy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://svz.tianlin.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gyd.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://glb.andypj.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mgd.guannengcc.top

Ruby: s.capitalize
来源：http://wms.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xhn.hfpthk.cn

[E18] 模板占位符替换
来源：http://lyo.gogol.net.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://roo.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://arp.fktsv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ips.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dye.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zle.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nbb.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hns.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bqg.jyoumei.cn

[E19] 多行文本按行拆分
来源：http://jfb.guannengcc.top

Py:   s.splitlines()
来源：http://sth.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wqs.fzhhl.top

JS:   s.split(/\r?\n/)
来源：http://han.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://zzv.sjlbkw.cn

Java: s.lines().toList()
来源：http://ugg.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://ujo.chenjidiqi.icu

Ruby: s.lines
来源：http://hez.birdmap.top

C#:   s.Split('\n')
来源：http://sjt.jinyuanbaomall.cn

[E20] 判断字符串是否为空
来源：http://jzw.yanxiufei.cn

Py:   if not s:
来源：http://zpz.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pap.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wlz.ppjwa.cn

TS:   if (s === "") {}
来源：http://xow.yj202588.top

Java: if (s.isEmpty()) {}
来源：http://wvz.meibo888.top

Go:   if s == "" {}
来源：http://gcc.chenjidiqi.icu

Ruby: if s.empty?
来源：http://dvd.hcnkem.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qbt.xziqi.cn

[E21] 超长截断加省略号
来源：http://sxq.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xkc.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oeq.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dxf.yonumen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rhm.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mqy.cucudq.cn

Go:   // 按 rune 判断长度后截断
来源：http://mzw.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gqj.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ywj.c1oappe.top

[E22] 字节长度与字符长度
来源：http://adk.jlsjyb.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://thp.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eue.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://avc.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ypj.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qqn.fehbvm.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://abb.ywan-chungtsiang.top

Ruby: s.bytesize;  s.length
来源：http://nih.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oop.feifeiyinyue.top

================================================================================
来源：http://gzl.haohaochexian.top

F. 文件与目录
来源：http://yho.fktsv.cn

================================================================================
来源：http://onu.hammf.cn

[F01] 读取整个文件
来源：http://ylt.shangyingyoupin.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wem.cashguo.top

PHP:  file_get_contents("a.txt");
来源：http://vny.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rzq.zhijiandao.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jzq.snrcjt.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gcp.yj20258888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kdu.cashguo.top

Ruby: File.read("a.txt")
来源：http://yab.vqdsnc.cn

C#:   File.ReadAllText("a.txt");
来源：http://fst.sufxvd.cn

[F02] 逐行读取文件
来源：http://kve.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cbi.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nsb.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nvl.sufxvd.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://upe.fanxiaobao.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iap.zhaomingkeji.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fsq.jianghu66.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ivg.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aco.hysaishi.cn

[F03] 写入文件（覆盖）
来源：http://pca.52xcode.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ejw.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ngw.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://inq.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hpn.zdbjq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vzp.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cza.chenlongwang.top

Ruby: File.write("a.txt", "hi")
来源：http://ffh.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ueq.yanxiufei.cn

[F04] 追加写入文件
来源：http://thc.gaohongyu789.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dij.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lcj.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyj.ydjk.org.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xoc.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ons.daxiang520.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eli.shangyingyoupin.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ixt.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://onz.havefunace.top

[F05] 判断文件或目录是否存在
来源：http://eeo.sweek.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pky.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://hvz.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://sqx.vqdsnc.cn

TS:   fs.existsSync("a.txt")
来源：http://rai.hesvh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kqz.hnxiangtu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hhb.gogol.net.cn

Ruby: File.exist?("a.txt")
来源：http://fye.dashuyun.cn

C#:   File.Exists("a.txt")
来源：http://zug.andypj.xyz

[F06] 删除文件
来源：http://omw.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://beh.hywenlv.cn

PHP:  unlink("a.txt");
来源：http://mnh.fanxiaobao.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://jtt.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wmw.zhoulong.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wvh.jianghu66.top

Go:   os.Remove("a.txt")
来源：http://wjf.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://qki.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://scb.havefunace.top

[F07] 创建目录（含多级）
来源：http://fuh.pengpengdd.cyou

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iew.cdnleiting.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lsf.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cfg.jianghu66.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ohv.yj20258.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://srh.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ncu.shzxlz.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://faj.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cep.nwbrower.top

[F08] 遍历目录
来源：http://oxg.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vdh.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wae.yfazqb.com

JS:   fs.readdirSync("dir")
来源：http://gto.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://ery.ctjpmb.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nuz.zhongyouzk.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://uwo.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://ncp.hesvh.cn

C#:   Directory.GetFiles("dir")
来源：http://spk.jinqigfzy.top

[F09] 获取文件大小
来源：http://dzg.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://xyu.jlsjyb.cn

PHP:  filesize("a.txt");
来源：http://xed.cqqwz.cn

JS:   fs.statSync("a.txt").size
来源：http://feq.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://vzx.52xcode.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yuk.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jqd.guannengcc.top

Ruby: File.size("a.txt")
来源：http://exs.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://scw.gzhubu.top

[F10] 取文件扩展名 / 文件名
来源：http://qak.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wos.ehwqpu.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fze.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hew.jlsjyb.cn

TS:   path.extname("a.txt")
来源：http://ehx.yanxiufei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hfr.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://njk.yvedp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zhh.cdnleiting.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wpp.ehwqpu.com

[F11] 复制与移动文件
来源：http://cnv.jlsjyb.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hwf.yvedp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fzg.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zkd.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sjd.ehwqpu.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qag.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ogk.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uri.nanxuanxn.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gox.hongshengwenyu.top

[F12] CSV 读写
来源：http://xeu.shanyushiyangtech.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gji.hfpthk.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://chv.zdqjudy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://irm.aizwys.cn

TS:   // 同上
来源：http://tfq.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://euy.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wbt.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ipl.yj20258888.top

C#:   // 无内置：用 CsvHelper 库
来源：http://vpo.ctjpmb.com

================================================================================
来源：http://vbp.sysykeji.top

G. 面向对象
来源：http://hwn.tanke756.top

================================================================================
来源：http://soh.jiagoushi.top

[G01] 定义类
来源：http://wev.gaohongyu789.top

Py:   class User: pass
来源：http://kaz.fktsv.cn

PHP:  class User {}
来源：http://bjl.dianchejie.cn

JS:   class User {}
来源：http://fgc.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://qjw.sxryk.cn

Java: class User {}
来源：http://zkh.pycfn.com

Go:   type User struct { Name string }
来源：http://mbl.zhijiandao.cn

Ruby: class User; end
来源：http://xkp.aibaodan.cn

C#:   class User {}
来源：http://efi.shanyushiyangtech.top

[G02] 构造函数
来源：http://rch.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://jvh.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://pda.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://mnt.zhoulong.xyz

TS:   constructor(public name: string) {}
来源：http://fkm.zdqjudy.top

Java: User(String name) { this.name = name; }
来源：http://zrz.chenzaomai.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lwq.52xcode.cn

Ruby: def initialize(name); @name = name; end
来源：http://kra.ehwqpu.com

C#:   public User(string name) { Name = name; }
来源：http://dyx.kuanghao11.cn

[G03] 实例属性
来源：http://sit.shzxlz.cn

Py:   self.name = "x"
来源：http://mjr.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://byg.cdnleiting.top

JS:   this.name = "x";
来源：http://sjo.sxryk.cn

TS:   name: string = "x";
来源：http://jat.tianlin.xyz

Java: private String name;
来源：http://uqf.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fmx.pycfn.com

Ruby: @name = "x"
来源：http://mqf.316326.xyz

C#:   public string Name { get; set; } = "x";
来源：http://llo.shanyushiyangtech.top

[G04] 定义方法
来源：http://yma.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://yvr.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kgo.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://erp.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://ooe.dashuyun.cn

Java: String greet() { return name; }
来源：http://xge.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rmo.epnwcf.com

Ruby: def greet; @name; end
来源：http://wvd.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://pss.shuidangran.top

[G05] 继承
来源：http://fef.nanxinkj.top

Py:   class Admin(User): pass
来源：http://zvb.cheryme.top

PHP:  class Admin extends User {}
来源：http://bfa.yvedp.cn

JS:   class Admin extends User {}
来源：http://rxe.52xcode.cn

TS:   class Admin extends User {}
来源：http://mxe.wangdashe.top

Java: class Admin extends User {}
来源：http://ccq.kuanghao11.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hhh.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://ndq.cashguo.top

C#:   class Admin : User {}
来源：http://oql.smart0.xyz

[G06] 重写方法
来源：http://sum.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://sba.tianlin.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://cwm.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://sjn.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://zei.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://bnt.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vsb.cheryme.top

Ruby: def greet; "admin"; end
来源：http://tvp.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://kza.gogol.net.cn

[G07] 调用父类方法
来源：http://fdd.sysykeji.top

Py:   super().greet()
来源：http://kuj.zdqjudy.top

PHP:  parent::greet();
来源：http://ltj.daria6918.cn

JS:   super.greet();
来源：http://nnt.xylfe.cn

TS:   super.greet();
来源：http://kib.shuidangran.top

Java: super.greet();
来源：http://bqk.smart0.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://efg.meibo888.top

Ruby: super
来源：http://dpm.tian-w.cn

C#:   base.Greet();
来源：http://rny.hnqzz.top

[G08] 静态方法与属性
来源：http://ckr.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ail.chenlongwang.top

PHP:  public static function f() {}
来源：http://pia.ydzc1.top

JS:   static f() {}
来源：http://gfd.xuanzx.com

TS:   static f(): void {}
来源：http://pwj.daxiang520.top

Java: static void f() {}
来源：http://qrj.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://pjg.jinqigufen.top

Ruby: def self.f; end
来源：http://slo.bbcook.cn

C#:   public static void F() {}
来源：http://gxb.sysykeji.top

[G09] 接口 / 抽象类
来源：http://exw.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://sot.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sqr.ydjk.org.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ngs.316326.xyz

TS:   interface Shape { area(): number; }
来源：http://ykg.shzxlz.cn

Java: interface Shape { double area(); }
来源：http://kiy.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://hle.mhx1999.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cbu.smart0.xyz

C#:   interface IShape { double Area(); }
来源：http://dtx.9152youxi.cn

[G10] 访问控制
来源：http://ris.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://qmp.yj20258888.top

PHP:  public / protected / private
来源：http://vbn.fengsongda.top

JS:   #private 字段；其余公开
来源：http://rfj.havefunace.top

TS:   public / protected / private
来源：http://mqe.tianlin.xyz

Java: public / protected / private / 默认包级
来源：http://kqd.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ryv.hysaishi.cn

Ruby: public / protected / private
来源：http://ccj.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://vnp.hywenlv.cn

[G11] getter / setter
来源：http://zsh.jianghu66.top

Py:   @property 与 @x.setter
来源：http://fhg.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://imq.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://tkd.meibo888.top

TS:   get name(): string { return this._name; }
来源：http://pmz.hfpthk.cn

Java: public String getName() { return name; }
来源：http://igf.aibaodan.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hyp.yuxming.cn


<!-- 参考信息 -->