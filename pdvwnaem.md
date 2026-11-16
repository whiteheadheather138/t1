代发 wailian999

Go:   strings.Count(s, "a")
来源：http://ine.jinghuilouyu.cn

Ruby: s.count("a")
来源：http://wys.gogol.net.cn

C#:   s.Count(c => c == 'a')
来源：http://zia.sxryk.cn

[E13] 逐字符遍历
来源：http://dpj.zdbjq.cn

Py:   for ch in s: print(ch)
来源：http://bju.zhixingplan.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://odu.fktsv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ftx.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fsg.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sng.ybcxt.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bea.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qsr.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ccn.9152youxi.cn

[E14] URL 编码与 Base64
来源：http://hkn.xziqi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xgr.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://byk.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gnc.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bsb.shangyingyoupin.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hyj.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eym.pengpengdd.cyou

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qmc.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bua.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://qfu.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dub.ydjk.org.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hpi.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qlp.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://row.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://flm.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjp.gogol.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vkl.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://buy.sxryk.cn

[E16] 数字千分位
来源：http://ddd.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://vhi.jiagoushi.top

PHP:  number_format(1234567);
来源：http://igv.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oys.uphjek.com

TS:   (1234567).toLocaleString("en-US")
来源：http://lnq.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ieb.pycfn.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://veh.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nyg.zdbjq.cn

C#:   1234567.ToString("N0")
来源：http://mia.zhijiandao.cn

[E17] 首字母大写
来源：http://iku.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ofw.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://gfm.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mmt.chenjidiqi.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dwu.nanxuanxn.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eab.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xns.hysaishi.cn

Ruby: s.capitalize
来源：http://hxc.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rkg.snrcjt.cn

[E18] 模板占位符替换
来源：http://pvy.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jro.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://efe.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://yjb.fzhhl.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bbt.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ixi.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zmn.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://glt.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qzy.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://nuh.chenlongwang.top

Py:   s.splitlines()
来源：http://yrz.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pwn.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://atx.mhx1999.top

TS:   s.split(/\r?\n/)
来源：http://thp.zhongyouzk.top

Java: s.lines().toList()
来源：http://nov.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://rlh.quarkkingdee.top

Ruby: s.lines
来源：http://dor.zdbjq.cn

C#:   s.Split('\n')
来源：http://ygk.xuanzx.com

[E20] 判断字符串是否为空
来源：http://mac.hnxiangtu.top

Py:   if not s:
来源：http://sto.hcnkem.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ysu.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vsr.cucudq.cn

TS:   if (s === "") {}
来源：http://rcj.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://zbm.0kj1m.cn

Go:   if s == "" {}
来源：http://rgr.tarul.cn

Ruby: if s.empty?
来源：http://dln.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://emq.pengpengdd.cyou

[E21] 超长截断加省略号
来源：http://yyc.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yka.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lvc.uphjek.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://owh.haohaochexian.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wkp.ydjk.org.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ynh.zdbjq.cn

Go:   // 按 rune 判断长度后截断
来源：http://fan.chenlongwang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xko.nanxuanxn.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://okt.smart0.xyz

[E22] 字节长度与字符长度
来源：http://vub.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rcm.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gyf.ybcxt.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://imy.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://whf.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tvy.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dcw.hnxiangtu.top

Ruby: s.bytesize;  s.length
来源：http://hnr.ydzc1.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zcp.chenlongwang.top

================================================================================
来源：http://boa.jinghuilouyu.cn

F. 文件与目录
来源：http://qvd.jqgufenzy.top

================================================================================
来源：http://qvf.andypj.xyz

[F01] 读取整个文件
来源：http://acx.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nrk.xziqi.cn

PHP:  file_get_contents("a.txt");
来源：http://lku.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://egu.snrcjt.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ldp.hcnkem.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dio.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://csx.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://iad.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ncc.xuetiantiany.cn

[F02] 逐行读取文件
来源：http://kkj.0kj1m.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dhp.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wiz.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cvu.nanxuanxn.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jfa.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bny.ehwqpu.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zlq.yangfankeji.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vny.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lcx.tanke756.top

[F03] 写入文件（覆盖）
来源：http://ntp.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jyj.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://poh.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lht.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyp.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kec.jqgfzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jjr.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://eso.mhx1999.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oft.hammf.cn

[F04] 追加写入文件
来源：http://ods.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dfa.xinyue.icu

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qvl.sweek.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mwp.sysykeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vuz.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wth.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://zhb.svipenyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yxg.epnwcf.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bbo.daxiang520.top

[F05] 判断文件或目录是否存在
来源：http://llk.zhiwuduotai.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yuq.ctjpmb.com

PHP:  file_exists("a.txt");
来源：http://qew.fanxiaobao.xyz

JS:   fs.existsSync("a.txt")
来源：http://kds.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://ouo.tarul.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xsp.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yxa.jinqigfzy.top

Ruby: File.exist?("a.txt")
来源：http://msf.yj202588.top

C#:   File.Exists("a.txt")
来源：http://ldr.andypj.xyz

[F06] 删除文件
来源：http://fux.yueranfly.top

Py:   os.remove("a.txt")
来源：http://rfh.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://aib.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dxl.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://cep.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wuz.birdmap.top

Go:   os.Remove("a.txt")
来源：http://aia.tanke756.top

Ruby: File.delete("a.txt")
来源：http://geg.yfazqb.com

C#:   File.Delete("a.txt");
来源：http://buv.yongpay.top

[F07] 创建目录（含多级）
来源：http://wjq.zdbjq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mft.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mtx.fktsv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kwv.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uqj.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://veo.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cma.dianchejie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lmf.sweek.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dtx.ybcxt.top

[F08] 遍历目录
来源：http://dnh.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dmb.jinghuilouyu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oxs.tian-w.cn

JS:   fs.readdirSync("dir")
来源：http://xto.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://ytc.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yqo.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://beb.chenzaomai.com

Ruby: Dir.children("dir")
来源：http://agu.redwolf501.top

C#:   Directory.GetFiles("dir")
来源：http://cwh.bjfxy.top

[F09] 获取文件大小
来源：http://efv.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://rjn.chenlongwang.top

PHP:  filesize("a.txt");
来源：http://czr.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://bkp.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://bez.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://psx.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yjl.sjlbkw.cn

Ruby: File.size("a.txt")
来源：http://hup.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://nbp.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://nsg.ydzc1.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vgo.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dez.jyoumei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zot.yj20258.top

TS:   path.extname("a.txt")
来源：http://zcn.yongpay.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sdf.jlsjyb.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jzj.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ugp.zhoulong.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xdw.jinqigufen.top

[F11] 复制与移动文件
来源：http://gmt.jyoumei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://atd.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kor.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://drw.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zww.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vgv.c1oappe.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://efa.smart0.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ipn.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yem.tianlin.xyz

[F12] CSV 读写
来源：http://avf.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nvr.yueranfly.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://emi.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uer.jlsjyb.cn

TS:   // 同上
来源：http://ica.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rec.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vuq.sysykeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jzz.tarul.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://plw.haohaochexian.top

================================================================================
来源：http://ndk.vqdsnc.cn

G. 面向对象
来源：http://snt.fanxiaobao.xyz

================================================================================
来源：http://lud.sjlbkw.cn

[G01] 定义类
来源：http://xbm.wangdashe.top

Py:   class User: pass
来源：http://ugq.cqqwz.cn

PHP:  class User {}
来源：http://olg.ywan-chungtsiang.top

JS:   class User {}
来源：http://mab.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://ikf.chenjidiqi.icu

Java: class User {}
来源：http://dvw.fktsv.cn

Go:   type User struct { Name string }
来源：http://nov.chenzaomai.com

Ruby: class User; end
来源：http://apr.mhx1999.top

C#:   class User {}
来源：http://ghd.aibaodan.cn

[G02] 构造函数
来源：http://puo.yangfankeji.com

Py:   def __init__(self, name): self.name = name
来源：http://dfr.dashuyun.cn

PHP:  public function __construct(public string $name) {}
来源：http://loa.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://rmy.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://poe.sweek.top

Java: User(String name) { this.name = name; }
来源：http://wxr.snrcjt.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://szr.snrcjt.cn

Ruby: def initialize(name); @name = name; end
来源：http://etj.ctjpmb.com

C#:   public User(string name) { Name = name; }
来源：http://lmw.jinyuanbaomall.cn

[G03] 实例属性
来源：http://wbg.zdqjudy.top

Py:   self.name = "x"
来源：http://rao.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://ygd.hcnkem.com

JS:   this.name = "x";
来源：http://rmt.meibo888.top

TS:   name: string = "x";
来源：http://nji.chenzaomai.com

Java: private String name;
来源：http://ugq.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sjl.yueranfly.top

Ruby: @name = "x"
来源：http://mcf.xuanzx.com

C#:   public string Name { get; set; } = "x";
来源：http://rlr.xziqi.cn

[G04] 定义方法
来源：http://gdo.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://bvz.ivvv.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tms.sufxvd.cn

JS:   greet() { return this.name; }
来源：http://ypi.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://kdr.tanke756.top

Java: String greet() { return name; }
来源：http://vyg.0kj1m.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ssc.xziqi.cn

Ruby: def greet; @name; end
来源：http://ucm.c1oappe.top

C#:   public string Greet() => Name;
来源：http://ihr.wangshuangyany.cn

[G05] 继承
来源：http://epu.sufxvd.cn

Py:   class Admin(User): pass
来源：http://vdv.gotoacloud.top

PHP:  class Admin extends User {}
来源：http://tbf.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://jlm.fengsongda.top

TS:   class Admin extends User {}
来源：http://mzx.jinqigfzy.top

Java: class Admin extends User {}
来源：http://huh.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pid.guannengcc.top

Ruby: class Admin < User; end
来源：http://aaf.hcnkem.com

C#:   class Admin : User {}
来源：http://umo.jiagoushi.top

[G06] 重写方法
来源：http://sxf.sxryk.cn

Py:   def greet(self): return "admin"
来源：http://qkc.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kkt.yuanzhike.top

JS:   greet() { return "admin"; }
来源：http://hkn.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://fjl.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://wnt.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qot.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://zkb.hnqzz.top

C#:   public override string Greet() => "admin";
来源：http://keo.redwolf501.top

[G07] 调用父类方法
来源：http://fzj.iojbl.cn

Py:   super().greet()
来源：http://fnf.chenzaomai.com

PHP:  parent::greet();
来源：http://htq.snrcjt.cn

JS:   super.greet();
来源：http://aov.daria6918.cn

TS:   super.greet();
来源：http://ipg.yj20258.top

Java: super.greet();
来源：http://cmq.ivvv.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hiz.zdqjudy.top

Ruby: super
来源：http://seg.yj20258.top

C#:   base.Greet();
来源：http://vof.ctjpmb.com

[G08] 静态方法与属性
来源：http://sxe.hesvh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://act.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://bwb.aizwys.cn

JS:   static f() {}
来源：http://hze.yj202588.top

TS:   static f(): void {}
来源：http://krx.cheryme.top

Java: static void f() {}
来源：http://tny.cqqwz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bmb.jinqigfzy.top

Ruby: def self.f; end
来源：http://xvs.fktsv.cn

C#:   public static void F() {}
来源：http://mnk.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://fej.xziqi.cn

Py:   from abc import ABC, abstractmethod
来源：http://acs.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dfe.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tsx.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://vgb.daxiang520.top

Java: interface Shape { double area(); }
来源：http://jqa.jinyuanbaomall.cn

Go:   type Shape interface { Area() float64 }
来源：http://zty.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cbu.yonumen.top

C#:   interface IShape { double Area(); }
来源：http://xqh.andypj.xyz

[G10] 访问控制
来源：http://wso.hysaishi.cn

Py:   约定 _protected / __private（不强制）
来源：http://xyw.pycfn.com

PHP:  public / protected / private
来源：http://ktz.xziqi.cn

JS:   #private 字段；其余公开
来源：http://fpq.jqgufenzy.top

TS:   public / protected / private
来源：http://wxc.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://syv.sweek.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://duq.ybcxt.top

Ruby: public / protected / private
来源：http://mhf.tian-w.cn

C#:   public / protected / private / internal
来源：http://xrs.nanxinkj.top

[G11] getter / setter
来源：http://pqs.zhixingplan.top

Py:   @property 与 @x.setter
来源：http://lbu.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://pct.dashuyun.cn


<!-- 参考信息 -->