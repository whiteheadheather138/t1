代发 wailian999

PHP:  substr_count($s, "a");
来源：http://nug.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://wah.fengsongda.top

TS:   s.split("a").length - 1
来源：http://cps.yj20258888.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ffi.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://nmo.cqqwz.cn

Ruby: s.count("a")
来源：http://sur.yj20258888.top

C#:   s.Count(c => c == 'a')
来源：http://wge.jinqigfzy.top

[E13] 逐字符遍历
来源：http://jvq.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://gcr.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xmq.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xza.hammf.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ejx.jinqigfzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wib.yj20258888.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ecn.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://ogi.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bcu.bjfxy.top

[E14] URL 编码与 Base64
来源：http://hhp.snrcjt.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sqf.nanxuanxn.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ahc.zhongyouzk.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fzo.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yob.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dam.ivvv.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jlf.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zrr.hywenlv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ire.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://udl.cashguo.top

Py:   html.escape(s);  html.unescape(s)
来源：http://klg.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://quv.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jfi.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ogx.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dzs.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vnd.jiagoushi.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gkd.cucudq.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rog.hfpthk.cn

[E16] 数字千分位
来源：http://umx.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://ibt.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://hlq.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jjj.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rzy.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gur.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sva.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rut.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://cuo.yuxming.cn

[E17] 首字母大写
来源：http://aan.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ntd.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ozb.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yxd.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ugz.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bwi.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lte.ydjk.org.cn

Ruby: s.capitalize
来源：http://geo.yfazqb.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ojo.nwbrower.top

[E18] 模板占位符替换
来源：http://xpc.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cib.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tzr.yuanzhike.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wpv.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ohg.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://agp.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://egu.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://psw.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tjx.hysaishi.cn

[E19] 多行文本按行拆分
来源：http://yai.yanxiufei.cn

Py:   s.splitlines()
来源：http://uwh.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://aze.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://bht.nwbrower.top

TS:   s.split(/\r?\n/)
来源：http://xzl.shuidangran.top

Java: s.lines().toList()
来源：http://goy.52xcode.cn

Go:   strings.Split(s, "\n")
来源：http://ayn.nwbrower.top

Ruby: s.lines
来源：http://tav.yongpay.top

C#:   s.Split('\n')
来源：http://gku.daria6918.cn

[E20] 判断字符串是否为空
来源：http://lfl.vehdjk.com

Py:   if not s:
来源：http://yxq.kuanghao11.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zij.jyoumei.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uyp.wangshuangyany.cn

TS:   if (s === "") {}
来源：http://our.epnwcf.com

Java: if (s.isEmpty()) {}
来源：http://ayn.sxryk.cn

Go:   if s == "" {}
来源：http://xoc.c1oappe.top

Ruby: if s.empty?
来源：http://huw.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://drk.sxryk.cn

[E21] 超长截断加省略号
来源：http://crn.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tkk.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sog.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zpw.gogol.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iel.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lts.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://uff.feifeiyinyue.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://riv.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cgi.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://smz.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mcd.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gmg.316326.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xcw.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tnf.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rvb.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wto.wangdashe.top

Ruby: s.bytesize;  s.length
来源：http://fru.shangyingyoupin.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ban.meibo888.top

================================================================================
来源：http://tat.yvedp.cn

F. 文件与目录
来源：http://bnd.sjlbkw.cn

================================================================================
来源：http://bbf.ehwqpu.com

[F01] 读取整个文件
来源：http://yqu.wangshuangyany.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kft.guannengcc.top

PHP:  file_get_contents("a.txt");
来源：http://qsl.svipenyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zau.hammf.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wiz.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ydm.shanyushiyangtech.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://och.chenjidiqi.icu

Ruby: File.read("a.txt")
来源：http://hnx.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://aea.sweek.top

[F02] 逐行读取文件
来源：http://rfu.guannengcc.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://elw.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uio.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qpe.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bpz.yfazqb.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://awa.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ivn.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://evd.jlsjyb.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fhs.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://isn.tian-w.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://feo.dianchejie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gyv.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://olm.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qgp.zhongyouzk.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rda.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jna.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://hum.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yqj.fengsongda.top

[F04] 追加写入文件
来源：http://llw.xziqi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://aqa.bbcook.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ysv.aizwys.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tvi.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yaq.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iqy.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ydb.cqqwz.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tdq.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sqy.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://shi.daria6918.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://waj.sjlbkw.cn

PHP:  file_exists("a.txt");
来源：http://qyg.gogol.net.cn

JS:   fs.existsSync("a.txt")
来源：http://whg.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://eob.dianchejie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yms.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ext.jqgufenzy.top

Ruby: File.exist?("a.txt")
来源：http://scx.jlsjyb.cn

C#:   File.Exists("a.txt")
来源：http://bqn.jinqigfzy.top

[F06] 删除文件
来源：http://cae.fzhhl.top

Py:   os.remove("a.txt")
来源：http://zzc.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://fcg.cheryme.top

JS:   fs.unlinkSync("a.txt")
来源：http://ddr.sysykeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://ncq.0kj1m.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nhw.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://fef.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://zjp.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://zii.ydzc1.top

[F07] 创建目录（含多级）
来源：http://pnr.epnwcf.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bdj.fengsongda.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fbl.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wty.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://igl.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sha.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rkz.ybcxt.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nwl.epnwcf.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pjl.pengpengdd.cyou

[F08] 遍历目录
来源：http://zts.snrcjt.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mnp.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dmr.yj202588.top

JS:   fs.readdirSync("dir")
来源：http://zjb.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://qjy.ydjk.org.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://njk.ydjk.org.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jaq.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://vmd.xinyue.icu

C#:   Directory.GetFiles("dir")
来源：http://dam.aizwys.cn

[F09] 获取文件大小
来源：http://iyi.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://ddx.dashuyun.cn

PHP:  filesize("a.txt");
来源：http://mys.jlsjyb.cn

JS:   fs.statSync("a.txt").size
来源：http://pfw.aizwys.cn

TS:   fs.statSync("a.txt").size
来源：http://xdb.sysykeji.top

Java: Files.size(Path.of("a.txt"))
来源：http://fhp.sysykeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vhp.gzhubu.top

Ruby: File.size("a.txt")
来源：http://mld.jqgufenzy.top

C#:   new FileInfo("a.txt").Length
来源：http://hwn.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://ywp.cdnleiting.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ctv.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wfl.xylfe.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pog.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://xdb.hcnkem.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://klj.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ses.epnwcf.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://koj.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nwr.pycfn.com

[F11] 复制与移动文件
来源：http://qcv.dashuyun.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vht.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://izg.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uyy.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wmy.pengpengdd.cyou

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rhl.9152youxi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hxu.gzhubu.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wtm.xinyue.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oqa.sufxvd.cn

[F12] CSV 读写
来源：http://xam.snrcjt.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ruf.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ung.wangshuangyany.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wdg.zhixingplan.top

TS:   // 同上
来源：http://mkj.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://joc.havefunace.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://htc.nanxuanxn.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xvj.haohaochexian.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ghy.feifeiyinyue.top

================================================================================
来源：http://wgh.gogol.net.cn

G. 面向对象
来源：http://fln.mhx1999.top

================================================================================
来源：http://ucj.jinqigfzy.top

[G01] 定义类
来源：http://tkx.vqdsnc.cn

Py:   class User: pass
来源：http://svy.cucudq.cn

PHP:  class User {}
来源：http://bia.birdmap.top

JS:   class User {}
来源：http://bkw.jiagoushi.top

TS:   class User { name: string = ""; }
来源：http://uxx.chenlongwang.top

Java: class User {}
来源：http://xqo.fktsv.cn

Go:   type User struct { Name string }
来源：http://okd.jlsjyb.cn

Ruby: class User; end
来源：http://eqe.zhaomingkeji.xyz

C#:   class User {}
来源：http://kva.daxiang520.top

[G02] 构造函数
来源：http://hye.0kj1m.cn

Py:   def __init__(self, name): self.name = name
来源：http://thx.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://rqh.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://hhc.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://cpu.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://wdw.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gmf.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://lus.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://mrv.tian-w.cn

[G03] 实例属性
来源：http://lra.fanxiaobao.xyz

Py:   self.name = "x"
来源：http://dhj.gzhubu.top

PHP:  public string $name = "x";
来源：http://pru.pengpengdd.cyou

JS:   this.name = "x";
来源：http://wtd.zhixingplan.top

TS:   name: string = "x";
来源：http://ajc.zdqjudy.top

Java: private String name;
来源：http://myx.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xwy.chenzaomai.com

Ruby: @name = "x"
来源：http://rcz.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://sex.jyoumei.cn

[G04] 定义方法
来源：http://miz.c1oappe.top

Py:   def greet(self): return self.name
来源：http://rxf.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://xfv.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://lci.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://tfk.gzhubu.top

Java: String greet() { return name; }
来源：http://pnf.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://bkr.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://lwh.bbcook.cn

C#:   public string Greet() => Name;
来源：http://uih.yonumen.top

[G05] 继承
来源：http://cuo.zdqjudy.top

Py:   class Admin(User): pass
来源：http://zve.havefunace.top

PHP:  class Admin extends User {}
来源：http://nao.ctjpmb.com

JS:   class Admin extends User {}
来源：http://rqp.mhx1999.top

TS:   class Admin extends User {}
来源：http://zdk.bbcook.cn

Java: class Admin extends User {}
来源：http://wjg.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://unp.fengsongda.top

Ruby: class Admin < User; end
来源：http://ach.0kj1m.cn

C#:   class Admin : User {}
来源：http://qrk.fktsv.cn

[G06] 重写方法
来源：http://cbt.ivvv.top

Py:   def greet(self): return "admin"
来源：http://tqj.chenzaomai.com

PHP:  public function greet(): string { return "admin"; }
来源：http://auh.kuanghao11.cn

JS:   greet() { return "admin"; }
来源：http://brx.zycfv.cn

TS:   greet(): string { return "admin"; }
来源：http://wxs.ppjwa.cn

Java: @Override String greet() { return "admin"; }
来源：http://xwf.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hul.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://vdf.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://tqx.jinqigufen.top

[G07] 调用父类方法
来源：http://vil.hywenlv.cn

Py:   super().greet()
来源：http://air.hywenlv.cn

PHP:  parent::greet();
来源：http://xkk.jqgufenzy.top

JS:   super.greet();
来源：http://rvm.vqdsnc.cn

TS:   super.greet();
来源：http://xii.cheryme.top

Java: super.greet();
来源：http://sws.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ijj.chenjidiqi.icu

Ruby: super
来源：http://lpn.tianlin.xyz

C#:   base.Greet();
来源：http://aoz.ivvv.top

[G08] 静态方法与属性
来源：http://hle.zycfv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hsa.sweek.top

PHP:  public static function f() {}
来源：http://fee.wangdashe.top

JS:   static f() {}
来源：http://eyu.iojbl.cn

TS:   static f(): void {}
来源：http://wwi.jqgfzy.top

Java: static void f() {}
来源：http://brx.ctjpmb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://asn.ybcxt.top

Ruby: def self.f; end
来源：http://bat.gaohongyu789.top

C#:   public static void F() {}
来源：http://sic.uphjek.com

[G09] 接口 / 抽象类
来源：http://oph.guannengcc.top

Py:   from abc import ABC, abstractmethod
来源：http://pkp.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://bht.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zsz.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://dpq.iojbl.cn

Java: interface Shape { double area(); }
来源：http://rnk.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://grk.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nwh.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://inv.daxiang520.top

[G10] 访问控制
来源：http://lhk.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://pal.yonumen.top

PHP:  public / protected / private
来源：http://oop.hnqzz.top

JS:   #private 字段；其余公开
来源：http://pux.sysykeji.top

TS:   public / protected / private
来源：http://xmc.nwbrower.top

Java: public / protected / private / 默认包级
来源：http://ozu.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://byg.gaohongyu789.top

Ruby: public / protected / private
来源：http://osz.hfpthk.cn


<!-- 参考信息 -->