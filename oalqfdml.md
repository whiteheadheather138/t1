代发 wailian999

Ruby: s.reverse
来源：http://ntm.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://pzk.wangdashe.top

[E12] 统计某字符出现次数
来源：http://jrl.tanke756.top

Py:   s.count("a")
来源：http://emv.52xcode.cn

PHP:  substr_count($s, "a");
来源：http://exy.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://add.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://nom.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://syf.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://xym.jlsjyb.cn

Ruby: s.count("a")
来源：http://qfc.zdbjq.cn

C#:   s.Count(c => c == 'a')
来源：http://mht.jiagoushi.top

[E13] 逐字符遍历
来源：http://xvf.hywenlv.cn

Py:   for ch in s: print(ch)
来源：http://zxi.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://saz.tanke756.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hjd.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://zrn.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://eej.aibaodan.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pik.yj202588.top

Ruby: s.each_char { |ch| puts ch }
来源：http://joo.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cut.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://wqv.pycfn.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://koj.cheryme.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zqo.xuanzx.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://suu.jinghuilouyu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://luz.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://swv.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eva.chenjidiqi.icu

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kvm.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nvx.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://yjc.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xcd.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wqg.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qfg.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://hai.jyoumei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tpf.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://inq.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kse.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vmu.quarkkingdee.top

[E16] 数字千分位
来源：http://evs.xinyue.icu

Py:   f"{1234567:,}"
来源：http://yed.yangfankeji.com

PHP:  number_format(1234567);
来源：http://rnn.tanke756.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mzl.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ekj.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://adf.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xwm.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://atb.zhoulong.xyz

C#:   1234567.ToString("N0")
来源：http://eod.yanxiufei.cn

[E17] 首字母大写
来源：http://ppx.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dmd.cqqwz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bay.hysaishi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewz.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyq.tarul.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kmr.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ajz.hysaishi.cn

Ruby: s.capitalize
来源：http://wat.ehwqpu.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zko.cashguo.top

[E18] 模板占位符替换
来源：http://lvb.sweek.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kay.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bna.jianghu66.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wom.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://euf.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://snw.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vrl.yvedp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jea.jianghu66.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pou.yj20258888.top

[E19] 多行文本按行拆分
来源：http://dwr.aibaodan.cn

Py:   s.splitlines()
来源：http://yft.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://abu.yangfankeji.com

JS:   s.split(/\r?\n/)
来源：http://pia.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://mdm.pengpengdd.cyou

Java: s.lines().toList()
来源：http://rfc.sufxvd.cn

Go:   strings.Split(s, "\n")
来源：http://adr.hfpthk.cn

Ruby: s.lines
来源：http://ytm.0kj1m.cn

C#:   s.Split('\n')
来源：http://oia.zhaomingkeji.xyz

[E20] 判断字符串是否为空
来源：http://dzo.nanxinkj.top

Py:   if not s:
来源：http://vfz.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fgk.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fbp.guowangkeji.top

TS:   if (s === "") {}
来源：http://mvz.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://ybo.jiagoushi.top

Go:   if s == "" {}
来源：http://ean.dianchejie.cn

Ruby: if s.empty?
来源：http://yop.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jbi.meibo888.top

[E21] 超长截断加省略号
来源：http://mqb.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vow.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yos.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wce.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nmc.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://idb.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://bac.tianlin.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lrh.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gmo.shanyushiyangtech.top

[E22] 字节长度与字符长度
来源：http://rod.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vho.wangdashe.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ith.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nma.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://itq.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hxt.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ido.fanxiaobao.xyz

Ruby: s.bytesize;  s.length
来源：http://ofg.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bzb.jiagoushi.top

================================================================================
来源：http://jwu.zhijiandao.cn

F. 文件与目录
来源：http://dok.zhijiandao.cn

================================================================================
来源：http://uxn.c1oappe.top

[F01] 读取整个文件
来源：http://ygm.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://msd.hfpthk.cn

PHP:  file_get_contents("a.txt");
来源：http://rcy.snrcjt.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nqv.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bsx.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wse.hnxiangtu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rcz.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://pyw.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://wfq.yj202588.top

[F02] 逐行读取文件
来源：http://pfu.c1oappe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sks.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ovf.snrcjt.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jdx.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sxk.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xox.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ref.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zhf.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://civ.fengsongda.top

[F03] 写入文件（覆盖）
来源：http://uio.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zaq.tanke756.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://pxt.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://krq.yj202588.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://suc.52xcode.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wml.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lzu.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://svb.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oys.svipenyu.cn

[F04] 追加写入文件
来源：http://vmw.nanxinkj.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vnz.yanxiufei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rjy.tanke756.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hyg.nanxuanxn.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fin.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://opv.shanyushiyangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ree.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mva.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lmz.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://haa.ydzc1.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gjh.tarul.cn

PHP:  file_exists("a.txt");
来源：http://kwt.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://ybq.jyoumei.cn

TS:   fs.existsSync("a.txt")
来源：http://vsa.vqdsnc.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wlo.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jyv.iojbl.cn

Ruby: File.exist?("a.txt")
来源：http://cuc.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://asr.pengpengdd.cyou

[F06] 删除文件
来源：http://lfv.yuxming.cn

Py:   os.remove("a.txt")
来源：http://oey.fehbvm.com

PHP:  unlink("a.txt");
来源：http://orh.zhongyouzk.top

JS:   fs.unlinkSync("a.txt")
来源：http://cki.zhaomingkeji.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://pjn.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ccx.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://iez.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://agj.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://ekn.yongpay.top

[F07] 创建目录（含多级）
来源：http://nzo.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://crj.iojbl.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gzx.bjfxy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lvt.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zds.redwolf501.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tqs.yuanzhike.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lxx.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nzr.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ums.yj20258.top

[F08] 遍历目录
来源：http://jey.meibo888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tek.quarkkingdee.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ddi.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://ypd.hnqzz.top

TS:   fs.readdirSync("dir")
来源：http://btu.zhijiandao.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lyo.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://qwz.316326.xyz

Ruby: Dir.children("dir")
来源：http://cti.yongpay.top

C#:   Directory.GetFiles("dir")
来源：http://utt.cdnleiting.top

[F09] 获取文件大小
来源：http://sln.nwbrower.top

Py:   os.path.getsize("a.txt")
来源：http://qer.yuanzhike.top

PHP:  filesize("a.txt");
来源：http://kvf.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://buc.jinghuilouyu.cn

TS:   fs.statSync("a.txt").size
来源：http://mwb.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://gog.cqqwz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kvy.mhx1999.top

Ruby: File.size("a.txt")
来源：http://ndn.ivvv.top

C#:   new FileInfo("a.txt").Length
来源：http://nro.jyoumei.cn

[F10] 取文件扩展名 / 文件名
来源：http://lkx.smart0.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://byw.xuetiantiany.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://abr.yvedp.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://onn.nanxinkj.top

TS:   path.extname("a.txt")
来源：http://rpi.zdbjq.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wcj.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hqm.sweek.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xxq.smart0.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cjt.bbcook.cn

[F11] 复制与移动文件
来源：http://ydr.nanxinkj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rkk.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://abh.fanxiaobao.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ard.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://whu.cheryme.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ocy.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ksm.hfpthk.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tbw.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://stq.gogol.net.cn

[F12] CSV 读写
来源：http://baf.chenlongwang.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yga.hywenlv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mcy.epnwcf.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://asd.nanxuanxn.top

TS:   // 同上
来源：http://zuq.jyoumei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dty.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mxp.chenzaomai.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kgs.pycfn.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lme.bbcook.cn

================================================================================
来源：http://ruv.vehdjk.com

G. 面向对象
来源：http://gan.c1oappe.top

================================================================================
来源：http://xml.yvedp.cn

[G01] 定义类
来源：http://crj.epnwcf.com

Py:   class User: pass
来源：http://kkz.xziqi.cn

PHP:  class User {}
来源：http://igc.tanke756.top

JS:   class User {}
来源：http://nie.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://xpn.smart0.xyz

Java: class User {}
来源：http://wrf.ybcxt.top

Go:   type User struct { Name string }
来源：http://adg.fengsongda.top

Ruby: class User; end
来源：http://gdu.tanke756.top

C#:   class User {}
来源：http://uqr.dianchejie.cn

[G02] 构造函数
来源：http://yil.yj20258.top

Py:   def __init__(self, name): self.name = name
来源：http://ebt.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://soa.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://kcl.jinqigfzy.top

TS:   constructor(public name: string) {}
来源：http://uqu.dianchejie.cn

Java: User(String name) { this.name = name; }
来源：http://okq.shanyushiyangtech.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ibz.dashuyun.cn

Ruby: def initialize(name); @name = name; end
来源：http://nno.xingfuxueyuan.xyz

C#:   public User(string name) { Name = name; }
来源：http://eap.jinyuanbaomall.cn

[G03] 实例属性
来源：http://gcr.hongshengwenyu.top

Py:   self.name = "x"
来源：http://ulb.feifeiyinyue.top

PHP:  public string $name = "x";
来源：http://ofx.yvedp.cn

JS:   this.name = "x";
来源：http://cxn.sxryk.cn

TS:   name: string = "x";
来源：http://dve.fengsongda.top

Java: private String name;
来源：http://qia.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://trb.yj20258888.top

Ruby: @name = "x"
来源：http://ios.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://gtx.ehwqpu.com

[G04] 定义方法
来源：http://lfl.tarul.cn

Py:   def greet(self): return self.name
来源：http://pbc.yanxiufei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dww.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://lek.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://avi.hfpthk.cn

Java: String greet() { return name; }
来源：http://tce.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qdy.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://huf.sufxvd.cn

C#:   public string Greet() => Name;
来源：http://zdb.yfazqb.com

[G05] 继承
来源：http://mlv.cashguo.top

Py:   class Admin(User): pass
来源：http://rlf.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://eha.gaohongyu789.top

JS:   class Admin extends User {}
来源：http://ssx.shzxlz.cn

TS:   class Admin extends User {}
来源：http://uvm.daria6918.cn

Java: class Admin extends User {}
来源：http://xeu.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ilk.bbcook.cn

Ruby: class Admin < User; end
来源：http://gsj.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://vwk.xuetiantiany.cn

[G06] 重写方法
来源：http://cmr.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://eow.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ftz.ivvv.top

JS:   greet() { return "admin"; }
来源：http://ubg.cqqwz.cn

TS:   greet(): string { return "admin"; }
来源：http://wwh.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://doy.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cgi.meibo888.top

Ruby: def greet; "admin"; end
来源：http://kqv.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://cff.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://ocg.hcnkem.com

Py:   super().greet()
来源：http://mjk.xinyue.icu

PHP:  parent::greet();
来源：http://otb.cashguo.top

JS:   super.greet();
来源：http://iqr.guowangkeji.top

TS:   super.greet();
来源：http://ylp.vehdjk.com

Java: super.greet();
来源：http://ywn.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rko.kuanghao11.cn

Ruby: super
来源：http://uro.wangdashe.top

C#:   base.Greet();
来源：http://vmq.quarkkingdee.top

[G08] 静态方法与属性
来源：http://gzr.ppjwa.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mel.aizwys.cn

PHP:  public static function f() {}
来源：http://zyq.hfpthk.cn

JS:   static f() {}
来源：http://jpo.vqdsnc.cn

TS:   static f(): void {}
来源：http://mph.ybcxt.top

Java: static void f() {}
来源：http://kmm.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://spi.zdqjudy.top

Ruby: def self.f; end
来源：http://cng.ppjwa.cn

C#:   public static void F() {}
来源：http://oaf.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://vrw.zhaomingkeji.xyz

Py:   from abc import ABC, abstractmethod
来源：http://gwu.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://idv.xziqi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://swx.hysaishi.cn

TS:   interface Shape { area(): number; }
来源：http://sez.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://tpp.gaohongyu789.top

Go:   type Shape interface { Area() float64 }
来源：http://phk.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ldl.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://nnc.nwbrower.top

[G10] 访问控制
来源：http://ayz.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://jtx.vqdsnc.cn

PHP:  public / protected / private
来源：http://hpn.andypj.xyz

JS:   #private 字段；其余公开
来源：http://cjj.ehwqpu.com


<!-- 参考信息 -->