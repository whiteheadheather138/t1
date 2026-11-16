代发 wailian999

Py:   for ch in s: print(ch)
来源：http://nwh.gzhubu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xux.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://grn.sxryk.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dpi.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ccp.hfpthk.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dqq.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qir.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://idn.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://ipw.jinghuilouyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pya.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gpr.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uto.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jxb.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ntj.birdmap.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nsy.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pdk.shangyingyoupin.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hgo.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://pen.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zwa.zycfv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qoo.xuetiantiany.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rej.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rxu.mhx1999.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kel.pengpengdd.cyou

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qgi.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qjq.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vtb.zhixingplan.top

[E16] 数字千分位
来源：http://rzb.quarkkingdee.top

Py:   f"{1234567:,}"
来源：http://nik.uphjek.com

PHP:  number_format(1234567);
来源：http://wma.jyoumei.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fzb.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://xxf.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aym.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qbg.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ssh.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://kbo.hnqzz.top

[E17] 首字母大写
来源：http://kga.sjlbkw.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sah.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://nfn.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://css.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pvy.shanyushiyangkeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://abf.jinqigufen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kly.feifeiyinyue.top

Ruby: s.capitalize
来源：http://wor.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xmg.mhx1999.top

[E18] 模板占位符替换
来源：http://ncj.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rwq.jqgufenzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ztc.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tmb.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ikn.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rih.jlsjyb.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cat.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oed.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mcj.yj20258888.top

[E19] 多行文本按行拆分
来源：http://jie.daria6918.cn

Py:   s.splitlines()
来源：http://oqz.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kbc.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://mas.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://dsk.kuanghao11.cn

Java: s.lines().toList()
来源：http://iru.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://qrh.ppjwa.cn

Ruby: s.lines
来源：http://ugq.ivvv.top

C#:   s.Split('\n')
来源：http://xqv.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://dxl.aibaodan.cn

Py:   if not s:
来源：http://qhm.yuanzhike.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ozu.sxryk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ber.hnxiangtu.top

TS:   if (s === "") {}
来源：http://mvy.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://cvd.hongshengwenyu.top

Go:   if s == "" {}
来源：http://lwd.zhiwuduotai.top

Ruby: if s.empty?
来源：http://rnh.zhixingplan.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://svc.fehbvm.com

[E21] 超长截断加省略号
来源：http://ryb.hongshengwenyu.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bdu.jqgfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ezh.guowangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gup.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbf.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bnz.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://nea.zhongyouzk.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jga.yueranfly.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://row.zhoulong.xyz

[E22] 字节长度与字符长度
来源：http://zyj.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dhn.hnqzz.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rdd.ctjpmb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oib.cucudq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zot.sweek.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ovx.smart0.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kni.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://dui.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rhh.yj20258888.top

================================================================================
来源：http://suz.redwolf501.top

F. 文件与目录
来源：http://rxg.guowangkeji.top

================================================================================
来源：http://tmr.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://ddk.jqgfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lne.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://htr.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://crs.tianlin.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ftc.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gwz.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ovx.fengsongda.top

Ruby: File.read("a.txt")
来源：http://qle.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://ykw.xuanzx.com

[F02] 逐行读取文件
来源：http://mmk.tian-w.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tfg.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wnh.ehwqpu.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tyr.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nyy.shangyingyoupin.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zrm.hfpthk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tlw.aizwys.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://abz.cucudq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jre.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://nsy.zhongyouzk.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://duj.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://toh.kuanghao11.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ryu.nanxinkj.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pjm.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdi.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lgo.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://mpx.sjlbkw.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jts.ydjk.org.cn

[F04] 追加写入文件
来源：http://snk.yvedp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fun.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tyt.jyoumei.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ifi.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dek.xuanzx.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vdk.zhongyouzk.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sjh.yonumen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://scn.jiagoushi.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zwo.snrcjt.cn

[F05] 判断文件或目录是否存在
来源：http://rul.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ryk.zhaomingkeji.xyz

PHP:  file_exists("a.txt");
来源：http://ehp.zdqjudy.top

JS:   fs.existsSync("a.txt")
来源：http://dwg.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://zrt.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://gda.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ozr.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://fkn.uphjek.com

C#:   File.Exists("a.txt")
来源：http://lwu.tianlin.xyz

[F06] 删除文件
来源：http://drc.jinqigufen.top

Py:   os.remove("a.txt")
来源：http://xlu.andypj.xyz

PHP:  unlink("a.txt");
来源：http://kmy.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://mju.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xkm.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bsi.meibo888.top

Go:   os.Remove("a.txt")
来源：http://qsl.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://bbq.guannengcc.top

C#:   File.Delete("a.txt");
来源：http://pji.yj20258888.top

[F07] 创建目录（含多级）
来源：http://gmu.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nds.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ozp.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jfw.meibo888.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rgm.jianghu66.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://srw.fanxiaobao.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uui.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yzm.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uuo.gzhubu.top

[F08] 遍历目录
来源：http://oen.cashguo.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://cwo.fengsongda.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qxs.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://hrn.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://ldh.hfpthk.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gju.cashguo.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ozu.nwbrower.top

Ruby: Dir.children("dir")
来源：http://ncz.cucudq.cn

C#:   Directory.GetFiles("dir")
来源：http://tuw.shanyushiyangtech.top

[F09] 获取文件大小
来源：http://jgh.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://qxz.fzhhl.top

PHP:  filesize("a.txt");
来源：http://baf.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://idt.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://aql.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dpt.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oln.shuidangran.top

Ruby: File.size("a.txt")
来源：http://qxa.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://viu.bjfxy.top

[F10] 取文件扩展名 / 文件名
来源：http://cgl.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fiq.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ofn.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hwc.yueranfly.top

TS:   path.extname("a.txt")
来源：http://vlr.9152youxi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qhj.vehdjk.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hfi.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ugq.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nmt.jinqigfzy.top

[F11] 复制与移动文件
来源：http://vet.tian-w.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://djf.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zgc.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rxh.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nps.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://myx.sysykeji.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cuf.dashuyun.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gbw.guannengcc.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sbs.zhengqikj.top

[F12] CSV 读写
来源：http://wgf.jinghuilouyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jgq.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://etu.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ykj.tanke756.top

TS:   // 同上
来源：http://kgw.yfazqb.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zvu.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://upx.birdmap.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fdi.hywenlv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://asb.yueranfly.top

================================================================================
来源：http://yir.nanxinkj.top

G. 面向对象
来源：http://xmg.aizwys.cn

================================================================================
来源：http://axi.dashuyun.cn

[G01] 定义类
来源：http://fec.aizwys.cn

Py:   class User: pass
来源：http://det.yj202588.top

PHP:  class User {}
来源：http://hyt.chenzaomai.com

JS:   class User {}
来源：http://fqb.epnwcf.com

TS:   class User { name: string = ""; }
来源：http://whs.hysaishi.cn

Java: class User {}
来源：http://odd.shuidangran.top

Go:   type User struct { Name string }
来源：http://zez.xziqi.cn

Ruby: class User; end
来源：http://cop.cucudq.cn

C#:   class User {}
来源：http://vpa.zdqjudy.top

[G02] 构造函数
来源：http://aiv.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://cbi.fehbvm.com

PHP:  public function __construct(public string $name) {}
来源：http://wzk.tian-w.cn

JS:   constructor(name) { this.name = name; }
来源：http://eal.sjlbkw.cn

TS:   constructor(public name: string) {}
来源：http://vfg.fktsv.cn

Java: User(String name) { this.name = name; }
来源：http://crn.ydzc1.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nen.haohaochexian.top

Ruby: def initialize(name); @name = name; end
来源：http://pau.sxryk.cn

C#:   public User(string name) { Name = name; }
来源：http://kls.svipenyu.cn

[G03] 实例属性
来源：http://cfr.zhengqikj.top

Py:   self.name = "x"
来源：http://sbu.bbcook.cn

PHP:  public string $name = "x";
来源：http://jol.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://xgy.uphjek.com

TS:   name: string = "x";
来源：http://bzy.kuanghao11.cn

Java: private String name;
来源：http://ads.hammf.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gwu.yuxming.cn

Ruby: @name = "x"
来源：http://ttv.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://nyy.cqqwz.cn

[G04] 定义方法
来源：http://btb.yj20258888.top

Py:   def greet(self): return self.name
来源：http://agt.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://olf.hammf.cn

JS:   greet() { return this.name; }
来源：http://aga.xuetiantiany.cn

TS:   greet(): string { return this.name; }
来源：http://ehj.vqdsnc.cn

Java: String greet() { return name; }
来源：http://bfx.fzhhl.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hug.shanyushiyangtech.top

Ruby: def greet; @name; end
来源：http://ruu.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://nix.yueranfly.top

[G05] 继承
来源：http://cnv.xuanzx.com

Py:   class Admin(User): pass
来源：http://bxb.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://sfn.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://obd.guannengcc.top

TS:   class Admin extends User {}
来源：http://hli.jianghu66.top

Java: class Admin extends User {}
来源：http://wis.sxryk.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://isg.zdqjudy.top

Ruby: class Admin < User; end
来源：http://uey.0kj1m.cn

C#:   class Admin : User {}
来源：http://djh.guannengcc.top

[G06] 重写方法
来源：http://xhj.gaohongyu789.top

Py:   def greet(self): return "admin"
来源：http://dba.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lyt.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://gcy.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://ylf.feifeiyinyue.top

Java: @Override String greet() { return "admin"; }
来源：http://cki.kuanghao11.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://puy.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://evk.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://etb.xziqi.cn

[G07] 调用父类方法
来源：http://sjo.gaohongyu789.top

Py:   super().greet()
来源：http://hzz.fehbvm.com

PHP:  parent::greet();
来源：http://dds.dianchejie.cn

JS:   super.greet();
来源：http://jtk.zhixingplan.top

TS:   super.greet();
来源：http://ulv.xuanzx.com

Java: super.greet();
来源：http://jkv.gogol.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ipe.shuidangran.top

Ruby: super
来源：http://hby.vqdsnc.cn

C#:   base.Greet();
来源：http://pjc.fengsongda.top

[G08] 静态方法与属性
来源：http://mnu.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hko.ydjk.org.cn

PHP:  public static function f() {}
来源：http://svb.andypj.xyz

JS:   static f() {}
来源：http://zio.xinyue.icu

TS:   static f(): void {}
来源：http://awn.shanyushiyangtech.top

Java: static void f() {}
来源：http://pop.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://msn.gzhubu.top

Ruby: def self.f; end
来源：http://jnz.meibo888.top

C#:   public static void F() {}
来源：http://hcz.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://cau.jlsjyb.cn

Py:   from abc import ABC, abstractmethod
来源：http://arw.yuxming.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vll.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ywk.dianchejie.cn

TS:   interface Shape { area(): number; }
来源：http://fgz.zdqjudy.top

Java: interface Shape { double area(); }
来源：http://csg.sysykeji.top

Go:   type Shape interface { Area() float64 }
来源：http://iib.redwolf501.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ife.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://tpw.chenzaomai.com

[G10] 访问控制
来源：http://mzw.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://ljx.xuanzx.com

PHP:  public / protected / private
来源：http://tai.hesvh.cn

JS:   #private 字段；其余公开
来源：http://ggk.shzxlz.cn

TS:   public / protected / private
来源：http://kqg.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://qzj.shanyushiyangtech.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qzb.redwolf501.top

Ruby: public / protected / private
来源：http://efj.jianghu66.top

C#:   public / protected / private / internal
来源：http://jnn.daxiang520.top

[G11] getter / setter
来源：http://vvk.yj202588.top

Py:   @property 与 @x.setter
来源：http://min.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fxr.svipenyu.cn

JS:   get name() { return this._name; }
来源：http://tje.cdnleiting.top

TS:   get name(): string { return this._name; }
来源：http://xms.yuanzhike.top

Java: public String getName() { return name; }
来源：http://zmb.nwbrower.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://irl.yvedp.cn


<!-- 参考信息 -->