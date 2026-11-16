代发 wailian999

PHP:  substr_count($s, "a");
来源：http://thv.c1oappe.top

JS:   s.split("a").length - 1
来源：http://kva.sxryk.cn

TS:   s.split("a").length - 1
来源：http://oje.jyoumei.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ylo.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://bmw.sufxvd.cn

Ruby: s.count("a")
来源：http://jey.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://xgb.daria6918.cn

[E13] 逐字符遍历
来源：http://yvh.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://fgy.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ais.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hxp.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lgs.haohaochexian.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dax.yvedp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jqn.shanyushiyangtech.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gom.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ilr.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://sxo.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aoi.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qwm.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mjx.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wdj.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fal.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rvr.shanyushiyangtech.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lrt.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hid.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://qcq.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://qev.yueranfly.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nyb.zhengqikj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://apu.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://tsw.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ozk.xinyue.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vtl.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gvj.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xqb.fzhhl.top

[E16] 数字千分位
来源：http://tqe.yfazqb.com

Py:   f"{1234567:,}"
来源：http://pqm.yuanzhike.top

PHP:  number_format(1234567);
来源：http://tph.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://hlw.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://mpz.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://usd.ydjk.org.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yhz.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cob.nwbrower.top

C#:   1234567.ToString("N0")
来源：http://fkh.xziqi.cn

[E17] 首字母大写
来源：http://nbb.gogol.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mom.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sfa.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lmi.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nki.gogol.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cdn.xziqi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tsp.52xcode.cn

Ruby: s.capitalize
来源：http://mkm.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rvn.cqqwz.cn

[E18] 模板占位符替换
来源：http://mhz.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sjq.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tvm.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tzn.kuanghao11.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://eed.dianchejie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://frq.sxryk.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sil.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://msa.ppjwa.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wxm.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://nlx.tarul.cn

Py:   s.splitlines()
来源：http://gfi.hnxiangtu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tps.hysaishi.cn

JS:   s.split(/\r?\n/)
来源：http://agy.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://jrw.hongshengwenyu.top

Java: s.lines().toList()
来源：http://wkq.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://imc.xingfuxueyuan.xyz

Ruby: s.lines
来源：http://kyc.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://tip.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://bxq.aizwys.cn

Py:   if not s:
来源：http://xpd.haohaochexian.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ljd.bbcook.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qmi.shuidangran.top

TS:   if (s === "") {}
来源：http://ztp.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://qel.tian-w.cn

Go:   if s == "" {}
来源：http://mig.hywenlv.cn

Ruby: if s.empty?
来源：http://pki.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gqd.yongpay.top

[E21] 超长截断加省略号
来源：http://crl.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gsj.52xcode.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hod.cqqwz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cya.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ire.kuanghao11.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tgg.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://dpd.sysykeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aaw.jqgufenzy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nej.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://son.aibaodan.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qfg.316326.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fph.sjlbkw.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xch.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jaz.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qdc.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gge.dianchejie.cn

Ruby: s.bytesize;  s.length
来源：http://lgc.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lai.jqgfzy.top

================================================================================
来源：http://tog.chenlongwang.top

F. 文件与目录
来源：http://mvd.9152youxi.cn

================================================================================
来源：http://qkf.shuidangran.top

[F01] 读取整个文件
来源：http://dxe.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tti.cucudq.cn

PHP:  file_get_contents("a.txt");
来源：http://lzx.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aif.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://plr.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ame.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cvo.yonumen.top

Ruby: File.read("a.txt")
来源：http://klb.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://hph.wangshuangyany.cn

[F02] 逐行读取文件
来源：http://rxq.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zle.haohaochexian.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lfc.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xcb.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wfe.feifeiyinyue.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dad.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qyy.chenzaomai.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://woi.shangyingyoupin.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ddx.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://uxz.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qml.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xlm.ctjpmb.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjq.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kgn.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lok.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yjp.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://zoj.ehwqpu.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dqo.jlsjyb.cn

[F04] 追加写入文件
来源：http://yex.ctjpmb.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://myu.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tjy.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://piw.sjlbkw.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yuu.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lkc.yueranfly.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jwc.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bso.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yis.haohaochexian.top

[F05] 判断文件或目录是否存在
来源：http://sgy.jinyuanbaomall.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ylg.ydjk.org.cn

PHP:  file_exists("a.txt");
来源：http://cba.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://vjh.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://qnc.jyoumei.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zzw.fzhhl.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pdm.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://ffi.kuanghao11.cn

C#:   File.Exists("a.txt")
来源：http://aov.mhx1999.top

[F06] 删除文件
来源：http://scb.ppjwa.cn

Py:   os.remove("a.txt")
来源：http://fxh.zhengqikj.top

PHP:  unlink("a.txt");
来源：http://xub.shanyushiyangkeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hcy.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://nvl.guowangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vxn.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://evq.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://nmr.kuanghao11.cn

C#:   File.Delete("a.txt");
来源：http://klw.tian-w.cn

[F07] 创建目录（含多级）
来源：http://zwh.dashuyun.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tyl.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qxy.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xhw.yvedp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uvn.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jdc.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zqc.yfazqb.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ufc.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nfo.meibo888.top

[F08] 遍历目录
来源：http://nfs.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://srr.yj20258888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ixk.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://bdo.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://pyh.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://otn.yongpay.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://afs.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://syc.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://jgk.jyoumei.cn

[F09] 获取文件大小
来源：http://sqv.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://wiv.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://pju.hysaishi.cn

JS:   fs.statSync("a.txt").size
来源：http://uoq.yongpay.top

TS:   fs.statSync("a.txt").size
来源：http://kyn.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sku.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wcq.andypj.xyz

Ruby: File.size("a.txt")
来源：http://ccp.yonumen.top

C#:   new FileInfo("a.txt").Length
来源：http://vgu.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://kob.fzhhl.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ztn.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hli.cashguo.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vsi.hfpthk.cn

TS:   path.extname("a.txt")
来源：http://uew.xuetiantiany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vyo.0kj1m.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hvx.wangshuangyany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vyg.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hna.cashguo.top

[F11] 复制与移动文件
来源：http://aus.birdmap.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xor.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ahx.chenlongwang.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ier.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://unw.bjfxy.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mdq.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hpl.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wde.jianghu66.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ich.cheryme.top

[F12] CSV 读写
来源：http://zxa.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cgs.gzhubu.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kkl.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pra.daxiang520.top

TS:   // 同上
来源：http://lta.9152youxi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fdd.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://auy.ehwqpu.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bit.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://kzi.feifeiyinyue.top

================================================================================
来源：http://wff.yonumen.top

G. 面向对象
来源：http://vrg.wangdashe.top

================================================================================
来源：http://hau.xinyue.icu

[G01] 定义类
来源：http://hes.ivvv.top

Py:   class User: pass
来源：http://pbw.cqqwz.cn

PHP:  class User {}
来源：http://anz.guannengcc.top

JS:   class User {}
来源：http://zie.zhengqikj.top

TS:   class User { name: string = ""; }
来源：http://fxw.andypj.xyz

Java: class User {}
来源：http://nwl.yueranfly.top

Go:   type User struct { Name string }
来源：http://iwj.chenzaomai.com

Ruby: class User; end
来源：http://cje.pengpengdd.cyou

C#:   class User {}
来源：http://ndh.cashguo.top

[G02] 构造函数
来源：http://qjt.wangshuangyany.cn

Py:   def __init__(self, name): self.name = name
来源：http://ets.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://xfa.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://rgw.shangyingyoupin.top

TS:   constructor(public name: string) {}
来源：http://xsa.zhiwuduotai.top

Java: User(String name) { this.name = name; }
来源：http://jao.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sta.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://pfl.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://pah.fzhhl.top

[G03] 实例属性
来源：http://oxw.jinqigufen.top

Py:   self.name = "x"
来源：http://dsh.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://wrk.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://zuf.hfpthk.cn

TS:   name: string = "x";
来源：http://sdd.zhoulong.xyz

Java: private String name;
来源：http://ljm.jinghuilouyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hxf.xziqi.cn

Ruby: @name = "x"
来源：http://not.jianghu66.top

C#:   public string Name { get; set; } = "x";
来源：http://zgq.yuanzhike.top

[G04] 定义方法
来源：http://ppj.316326.xyz

Py:   def greet(self): return self.name
来源：http://srv.0kj1m.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ivz.sysykeji.top

JS:   greet() { return this.name; }
来源：http://nhp.yfazqb.com

TS:   greet(): string { return this.name; }
来源：http://sgn.yueranfly.top

Java: String greet() { return name; }
来源：http://zgh.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iqm.jinqigufen.top

Ruby: def greet; @name; end
来源：http://qbl.havefunace.top

C#:   public string Greet() => Name;
来源：http://kiy.jinghuilouyu.cn

[G05] 继承
来源：http://njh.yfazqb.com

Py:   class Admin(User): pass
来源：http://mnz.smart0.xyz

PHP:  class Admin extends User {}
来源：http://sby.dashuyun.cn

JS:   class Admin extends User {}
来源：http://exb.sweek.top

TS:   class Admin extends User {}
来源：http://zei.sufxvd.cn

Java: class Admin extends User {}
来源：http://itw.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://obo.yj202588.top

Ruby: class Admin < User; end
来源：http://fne.jlsjyb.cn

C#:   class Admin : User {}
来源：http://aeq.jinqigfzy.top

[G06] 重写方法
来源：http://upf.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://hqp.zhijiandao.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nxk.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://kyd.316326.xyz

TS:   greet(): string { return "admin"; }
来源：http://jhr.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://opd.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lbg.hongshengwenyu.top

Ruby: def greet; "admin"; end
来源：http://ios.hysaishi.cn

C#:   public override string Greet() => "admin";
来源：http://inh.zhixingplan.top

[G07] 调用父类方法
来源：http://csg.zhoulong.xyz

Py:   super().greet()
来源：http://kum.316326.xyz

PHP:  parent::greet();
来源：http://mhg.hongshengwenyu.top

JS:   super.greet();
来源：http://kxi.redwolf501.top

TS:   super.greet();
来源：http://sfc.sufxvd.cn

Java: super.greet();
来源：http://htd.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xrd.tianlin.xyz

Ruby: super
来源：http://gqc.jinqigfzy.top

C#:   base.Greet();
来源：http://vib.bjfxy.top

[G08] 静态方法与属性
来源：http://zfd.chenzaomai.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qhv.cqqwz.cn

PHP:  public static function f() {}
来源：http://uju.ybcxt.top

JS:   static f() {}
来源：http://rpq.xylfe.cn

TS:   static f(): void {}
来源：http://wtk.jiagoushi.top

Java: static void f() {}
来源：http://hcn.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://dvd.nwbrower.top

Ruby: def self.f; end
来源：http://kfq.jqgufenzy.top

C#:   public static void F() {}
来源：http://gvd.yongpay.top

[G09] 接口 / 抽象类
来源：http://sxp.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://rbl.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://iqt.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://bdi.zhengqikj.top

TS:   interface Shape { area(): number; }
来源：http://wgt.zhijiandao.cn

Java: interface Shape { double area(); }
来源：http://tup.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://ckj.gogol.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lol.andypj.xyz

C#:   interface IShape { double Area(); }
来源：http://vbs.bjfxy.top

[G10] 访问控制
来源：http://fsk.ivvv.top

Py:   约定 _protected / __private（不强制）
来源：http://dnw.epnwcf.com

PHP:  public / protected / private
来源：http://zer.ivvv.top

JS:   #private 字段；其余公开
来源：http://tpq.fktsv.cn

TS:   public / protected / private
来源：http://yxh.sweek.top

Java: public / protected / private / 默认包级
来源：http://spb.yuanzhike.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://seu.andypj.xyz

Ruby: public / protected / private
来源：http://fzx.fehbvm.com


<!-- 参考信息 -->