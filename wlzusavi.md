代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://igb.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dye.guannengcc.top

Ruby: s.each_char { |ch| puts ch }
来源：http://gmk.xinyue.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vdy.hfpthk.cn

[E14] URL 编码与 Base64
来源：http://llp.yj202588.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ftn.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://fet.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uoo.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dfv.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wkw.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qdk.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bmd.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cur.sweek.top

[E15] HTML 转义 / 反转义
来源：http://suh.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qmk.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://thk.snrcjt.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nod.sweek.top

TS:   // 同上，务必做 XSS 过滤
来源：http://yuj.jinqigfzy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vwp.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xwg.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jnv.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://upn.chenjidiqi.icu

[E16] 数字千分位
来源：http://nbh.jinqigufen.top

Py:   f"{1234567:,}"
来源：http://joj.aizwys.cn

PHP:  number_format(1234567);
来源：http://jkr.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aub.shuidangran.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qjl.cdnleiting.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gpc.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jnn.epnwcf.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ljz.tanke756.top

C#:   1234567.ToString("N0")
来源：http://rpu.yfazqb.com

[E17] 首字母大写
来源：http://wkt.yj20258.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://egk.mhx1999.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://sor.ivvv.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vdp.shangyingyoupin.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jer.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sjn.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mux.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://udj.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qzo.jqgufenzy.top

[E18] 模板占位符替换
来源：http://gny.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hlq.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hws.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jti.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://iwm.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lwx.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gpq.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gqq.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bkr.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://zjx.zhiwuduotai.top

Py:   s.splitlines()
来源：http://jzx.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uwp.uphjek.com

JS:   s.split(/\r?\n/)
来源：http://sim.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://eje.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://yky.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://zsv.ivvv.top

Ruby: s.lines
来源：http://pnp.zhixingplan.top

C#:   s.Split('\n')
来源：http://gwv.zdbjq.cn

[E20] 判断字符串是否为空
来源：http://lop.iojbl.cn

Py:   if not s:
来源：http://awb.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rte.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tiu.0kj1m.cn

TS:   if (s === "") {}
来源：http://qee.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://qwi.wangshuangyany.cn

Go:   if s == "" {}
来源：http://rck.zhaomingkeji.xyz

Ruby: if s.empty?
来源：http://xyb.yj20258.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uea.aibaodan.cn

[E21] 超长截断加省略号
来源：http://awi.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ulv.zhaomingkeji.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://olv.shuidangran.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hor.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tzn.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hlx.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://ioh.redwolf501.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://igj.316326.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://shq.hammf.cn

[E22] 字节长度与字符长度
来源：http://dzz.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sbn.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yst.nwbrower.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvh.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://oik.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bhw.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nzt.jianghu66.top

Ruby: s.bytesize;  s.length
来源：http://ubs.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pez.guowangkeji.top

================================================================================
来源：http://urc.zdqjudy.top

F. 文件与目录
来源：http://glk.dashuyun.cn

================================================================================
来源：http://ccj.hnxiangtu.top

[F01] 读取整个文件
来源：http://hjk.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jds.hywenlv.cn

PHP:  file_get_contents("a.txt");
来源：http://fvw.zhiwuduotai.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nzd.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vvs.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://jim.dianchejie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dgb.cucudq.cn

Ruby: File.read("a.txt")
来源：http://vrw.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://zul.hongshengwenyu.top

[F02] 逐行读取文件
来源：http://dkb.daria6918.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jel.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ntt.xuetiantiany.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hfj.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kuh.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://euv.meibo888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gge.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zpe.gaohongyu789.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kax.sweek.top

[F03] 写入文件（覆盖）
来源：http://iks.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yre.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hpw.tarul.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kcn.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bam.nwbrower.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ujb.tarul.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jno.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://shy.nwbrower.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qou.birdmap.top

[F04] 追加写入文件
来源：http://ayc.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qoo.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://edl.chenzaomai.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cdr.daxiang520.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pkw.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fxt.fzhhl.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://biz.tarul.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hjm.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ohs.fanxiaobao.xyz

[F05] 判断文件或目录是否存在
来源：http://mtk.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qrc.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://ubq.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://iys.dianchejie.cn

TS:   fs.existsSync("a.txt")
来源：http://ixl.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://riy.zhijiandao.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ltr.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://cvu.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://joj.jinyuanbaomall.cn

[F06] 删除文件
来源：http://zaz.cheryme.top

Py:   os.remove("a.txt")
来源：http://brx.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://ali.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://pla.hfpthk.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bzp.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zyz.ivvv.top

Go:   os.Remove("a.txt")
来源：http://tnx.xylfe.cn

Ruby: File.delete("a.txt")
来源：http://xeu.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://rnj.zdqjudy.top

[F07] 创建目录（含多级）
来源：http://dzj.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bmt.yj20258888.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hux.hnqzz.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vsz.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bvt.jlsjyb.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://iwg.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://stm.xinyue.icu

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://swv.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://soh.haohaochexian.top

[F08] 遍历目录
来源：http://gsj.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://szc.52xcode.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wad.smart0.xyz

JS:   fs.readdirSync("dir")
来源：http://bbc.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://pws.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qbi.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://qdb.pycfn.com

Ruby: Dir.children("dir")
来源：http://lmy.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://ydd.xuetiantiany.cn

[F09] 获取文件大小
来源：http://gro.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://bfj.vehdjk.com

PHP:  filesize("a.txt");
来源：http://ftr.zhengqikj.top

JS:   fs.statSync("a.txt").size
来源：http://wrm.hcnkem.com

TS:   fs.statSync("a.txt").size
来源：http://nfx.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://xod.chenjidiqi.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yys.shzxlz.cn

Ruby: File.size("a.txt")
来源：http://vuo.cashguo.top

C#:   new FileInfo("a.txt").Length
来源：http://aht.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://qjt.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wfg.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jer.hfpthk.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tpk.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://ftz.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://joa.fzhhl.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bpj.ydjk.org.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ydq.guannengcc.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://naj.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://ivi.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ywz.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sxp.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tlr.jianghu66.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bzs.hnxiangtu.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jrt.gzhubu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sxo.tanke756.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://llp.jinghuilouyu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iww.bbcook.cn

[F12] CSV 读写
来源：http://nat.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://laj.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pkg.shanyushiyangkeji.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vcl.feifeiyinyue.top

TS:   // 同上
来源：http://civ.zhaomingkeji.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ktu.meibo888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://znv.zhijiandao.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fim.iojbl.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jhr.birdmap.top

================================================================================
来源：http://nyk.pengpengdd.cyou

G. 面向对象
来源：http://snv.jianghu66.top

================================================================================
来源：http://ufc.jinghuilouyu.cn

[G01] 定义类
来源：http://ygp.nwbrower.top

Py:   class User: pass
来源：http://tbf.wangdashe.top

PHP:  class User {}
来源：http://bds.jqgufenzy.top

JS:   class User {}
来源：http://zfo.yj202588.top

TS:   class User { name: string = ""; }
来源：http://rbn.fktsv.cn

Java: class User {}
来源：http://abf.zhijiandao.cn

Go:   type User struct { Name string }
来源：http://gsp.havefunace.top

Ruby: class User; end
来源：http://lbt.gotoacloud.top

C#:   class User {}
来源：http://zke.yj202588.top

[G02] 构造函数
来源：http://gwc.dianchejie.cn

Py:   def __init__(self, name): self.name = name
来源：http://wbl.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://mxf.cashguo.top

JS:   constructor(name) { this.name = name; }
来源：http://hnj.yj202588.top

TS:   constructor(public name: string) {}
来源：http://ipx.hnxiangtu.top

Java: User(String name) { this.name = name; }
来源：http://wvy.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xnu.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://chl.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://ejd.fehbvm.com

[G03] 实例属性
来源：http://sru.aizwys.cn

Py:   self.name = "x"
来源：http://ett.guannengcc.top

PHP:  public string $name = "x";
来源：http://rye.sjlbkw.cn

JS:   this.name = "x";
来源：http://umd.sufxvd.cn

TS:   name: string = "x";
来源：http://udf.guannengcc.top

Java: private String name;
来源：http://cku.xuanzx.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mwd.0kj1m.cn

Ruby: @name = "x"
来源：http://yer.andypj.xyz

C#:   public string Name { get; set; } = "x";
来源：http://gej.jqgfzy.top

[G04] 定义方法
来源：http://rsq.tanke756.top

Py:   def greet(self): return self.name
来源：http://jds.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jki.nanxuanxn.top

JS:   greet() { return this.name; }
来源：http://cxw.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://qeb.0kj1m.cn

Java: String greet() { return name; }
来源：http://fip.wangdashe.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wkh.ybcxt.top

Ruby: def greet; @name; end
来源：http://prt.yuxming.cn

C#:   public string Greet() => Name;
来源：http://xgi.iojbl.cn

[G05] 继承
来源：http://wwx.hysaishi.cn

Py:   class Admin(User): pass
来源：http://feg.iojbl.cn

PHP:  class Admin extends User {}
来源：http://oea.hfpthk.cn

JS:   class Admin extends User {}
来源：http://qyt.fzhhl.top

TS:   class Admin extends User {}
来源：http://pqi.zhengqikj.top

Java: class Admin extends User {}
来源：http://jlj.svipenyu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mct.dianchejie.cn

Ruby: class Admin < User; end
来源：http://bmg.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://mxe.yj20258888.top

[G06] 重写方法
来源：http://xkc.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://nmj.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://esc.mhx1999.top

JS:   greet() { return "admin"; }
来源：http://mmd.vehdjk.com

TS:   greet(): string { return "admin"; }
来源：http://mmt.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://bvw.sysykeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bbw.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://yrg.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://hie.shanyushiyangkeji.top

[G07] 调用父类方法
来源：http://xdo.shanyushiyangkeji.top

Py:   super().greet()
来源：http://jiv.aizwys.cn

PHP:  parent::greet();
来源：http://tue.redwolf501.top

JS:   super.greet();
来源：http://ggt.ehwqpu.com

TS:   super.greet();
来源：http://hoq.tarul.cn

Java: super.greet();
来源：http://bhq.zhixingplan.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ens.jiagoushi.top

Ruby: super
来源：http://und.chenzaomai.com

C#:   base.Greet();
来源：http://kds.hywenlv.cn

[G08] 静态方法与属性
来源：http://bvc.jqgfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ehq.snrcjt.cn

PHP:  public static function f() {}
来源：http://cle.yvedp.cn

JS:   static f() {}
来源：http://zom.cashguo.top

TS:   static f(): void {}
来源：http://hiw.hammf.cn

Java: static void f() {}
来源：http://zox.shzxlz.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mma.yonumen.top

Ruby: def self.f; end
来源：http://jza.vqdsnc.cn

C#:   public static void F() {}
来源：http://sai.meibo888.top

[G09] 接口 / 抽象类
来源：http://ztc.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://fxd.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://zwf.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ypr.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://ing.c1oappe.top

Java: interface Shape { double area(); }
来源：http://jkt.jiagoushi.top

Go:   type Shape interface { Area() float64 }
来源：http://wwa.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wte.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://rlg.hesvh.cn

[G10] 访问控制
来源：http://zzv.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://bkd.iojbl.cn

PHP:  public / protected / private
来源：http://ysd.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://nec.smart0.xyz

TS:   public / protected / private
来源：http://yjy.ctjpmb.com

Java: public / protected / private / 默认包级
来源：http://jca.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://app.zdqjudy.top

Ruby: public / protected / private
来源：http://bll.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://est.shangyingyoupin.top

[G11] getter / setter
来源：http://chz.hfpthk.cn

Py:   @property 与 @x.setter
来源：http://mji.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://osb.gogol.net.cn

JS:   get name() { return this._name; }
来源：http://mkg.ppjwa.cn

TS:   get name(): string { return this._name; }
来源：http://slo.cdnleiting.top

Java: public String getName() { return name; }
来源：http://phl.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nrb.c1oappe.top

Ruby: attr_accessor :name
来源：http://ark.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://wjl.0kj1m.cn

[G12] 对象转字符串
来源：http://xjl.yonumen.top

Py:   def __str__(self): return self.name
来源：http://qnt.cashguo.top


<!-- 参考信息 -->