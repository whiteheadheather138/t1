代发 wailian999

Ruby: s.reverse
来源：http://pnv.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://vsy.hammf.cn

[E12] 统计某字符出现次数
来源：http://uef.ehwqpu.com

Py:   s.count("a")
来源：http://xah.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://bhp.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://zxd.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://nvi.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oyv.ivvv.top

Go:   strings.Count(s, "a")
来源：http://hcv.zhoulong.xyz

Ruby: s.count("a")
来源：http://xvc.zhaomingkeji.xyz

C#:   s.Count(c => c == 'a')
来源：http://nzs.tian-w.cn

[E13] 逐字符遍历
来源：http://knp.tian-w.cn

Py:   for ch in s: print(ch)
来源：http://uyv.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dxc.bbcook.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hmq.meibo888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://clg.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fst.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hya.hywenlv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ijb.hfpthk.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lqs.jiagoushi.top

[E14] URL 编码与 Base64
来源：http://zeu.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lsg.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ask.chenlongwang.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pgh.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mkj.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://klp.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pla.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gbq.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zpd.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://thp.nanxuanxn.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nvg.xuanzx.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jbz.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qux.havefunace.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vps.hcnkem.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vkm.havefunace.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vrk.jinqigufen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qyg.tarul.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uhr.aizwys.cn

[E16] 数字千分位
来源：http://hsf.hongshengwenyu.top

Py:   f"{1234567:,}"
来源：http://hqp.ppjwa.cn

PHP:  number_format(1234567);
来源：http://oqz.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hec.smart0.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://uqt.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cna.zhengqikj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xya.guannengcc.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zae.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://gay.fzhhl.top

[E17] 首字母大写
来源：http://rie.shuidangran.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dqq.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oxp.dianchejie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cua.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ymk.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jzz.redwolf501.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jzc.hnxiangtu.top

Ruby: s.capitalize
来源：http://sjn.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ahw.jinghuilouyu.cn

[E18] 模板占位符替换
来源：http://szv.zycfv.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rwz.zdqjudy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ahq.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://cql.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ptr.yonumen.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kxi.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://itd.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://liy.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uqs.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://syp.ehwqpu.com

Py:   s.splitlines()
来源：http://qjd.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ujy.0kj1m.cn

JS:   s.split(/\r?\n/)
来源：http://tgg.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://vfk.ydzc1.top

Java: s.lines().toList()
来源：http://iui.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://ljs.hywenlv.cn

Ruby: s.lines
来源：http://guc.nanxuanxn.top

C#:   s.Split('\n')
来源：http://nnv.yfazqb.com

[E20] 判断字符串是否为空
来源：http://bsu.dianchejie.cn

Py:   if not s:
来源：http://ntu.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kye.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sob.sufxvd.cn

TS:   if (s === "") {}
来源：http://wml.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://rni.epnwcf.com

Go:   if s == "" {}
来源：http://mzs.chenjidiqi.icu

Ruby: if s.empty?
来源：http://wpg.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fja.zhijiandao.cn

[E21] 超长截断加省略号
来源：http://zqd.ydzc1.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cdg.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fjz.aizwys.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rxm.hysaishi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jzs.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ywy.bbcook.cn

Go:   // 按 rune 判断长度后截断
来源：http://xco.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nxp.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://are.daria6918.cn

[E22] 字节长度与字符长度
来源：http://qrm.fengsongda.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wzw.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jkw.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nza.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bsl.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mxu.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qua.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://mfg.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rpn.zhijiandao.cn

================================================================================
来源：http://lnx.hcnkem.com

F. 文件与目录
来源：http://mgs.hnxiangtu.top

================================================================================
来源：http://bjc.kuanghao11.cn

[F01] 读取整个文件
来源：http://cjk.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pxq.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://ied.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gpw.zdbjq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ptr.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://okb.mhx1999.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ewy.xinyue.icu

Ruby: File.read("a.txt")
来源：http://svv.birdmap.top

C#:   File.ReadAllText("a.txt");
来源：http://pcs.cucudq.cn

[F02] 逐行读取文件
来源：http://pnv.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uoj.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jve.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otd.gzhubu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wob.shanyushiyangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zaa.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://slt.cashguo.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vom.ybcxt.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jzo.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://trp.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cqs.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://wqk.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dns.ctjpmb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://okp.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rhf.shzxlz.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bwn.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://izx.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fbu.wangshuangyany.cn

[F04] 追加写入文件
来源：http://esf.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://imc.zdqjudy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xwi.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kew.pycfn.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fpq.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kcu.xuanzx.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bdz.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gfr.shuidangran.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yta.tian-w.cn

[F05] 判断文件或目录是否存在
来源：http://bzu.xziqi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hne.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://rzs.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://eqr.nanxinkj.top

TS:   fs.existsSync("a.txt")
来源：http://fce.hnxiangtu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qic.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dwx.hammf.cn

Ruby: File.exist?("a.txt")
来源：http://qzk.yj20258.top

C#:   File.Exists("a.txt")
来源：http://fud.tianlin.xyz

[F06] 删除文件
来源：http://iyy.fehbvm.com

Py:   os.remove("a.txt")
来源：http://snc.gzhubu.top

PHP:  unlink("a.txt");
来源：http://efl.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jei.c1oappe.top

TS:   fs.unlinkSync("a.txt")
来源：http://pzq.jqgufenzy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lft.chenzaomai.com

Go:   os.Remove("a.txt")
来源：http://ens.9152youxi.cn

Ruby: File.delete("a.txt")
来源：http://fhn.hammf.cn

C#:   File.Delete("a.txt");
来源：http://mes.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://eiz.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tsk.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yvl.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jbp.uphjek.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mof.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://key.zycfv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cjj.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sow.haohaochexian.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mji.shuidangran.top

[F08] 遍历目录
来源：http://dyd.hcnkem.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kxu.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kgs.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://hkj.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://kpq.yj202588.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://poh.svipenyu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pus.meibo888.top

Ruby: Dir.children("dir")
来源：http://qer.daxiang520.top

C#:   Directory.GetFiles("dir")
来源：http://dzp.vqdsnc.cn

[F09] 获取文件大小
来源：http://ryg.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://qkm.aibaodan.cn

PHP:  filesize("a.txt");
来源：http://bqf.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://ygd.gogol.net.cn

TS:   fs.statSync("a.txt").size
来源：http://hjv.cheryme.top

Java: Files.size(Path.of("a.txt"))
来源：http://axc.aibaodan.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dxw.sxryk.cn

Ruby: File.size("a.txt")
来源：http://pgv.vqdsnc.cn

C#:   new FileInfo("a.txt").Length
来源：http://lsc.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://deu.zhengqikj.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dzj.dashuyun.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mkj.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vbh.hysaishi.cn

TS:   path.extname("a.txt")
来源：http://xtv.hysaishi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fmm.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fhd.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gat.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wph.ivvv.top

[F11] 复制与移动文件
来源：http://fez.yanxiufei.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oeh.sufxvd.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mpe.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zse.cucudq.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dny.yfazqb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lbd.yvedp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://heq.jiagoushi.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://idx.chenzaomai.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whu.zhongyouzk.top

[F12] CSV 读写
来源：http://fqq.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zau.hcnkem.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hnb.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://thh.yuanzhike.top

TS:   // 同上
来源：http://bwf.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bap.hnxiangtu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bon.hysaishi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ziy.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lhz.redwolf501.top

================================================================================
来源：http://rdc.yvedp.cn

G. 面向对象
来源：http://lnw.ehwqpu.com

================================================================================
来源：http://fnf.ivvv.top

[G01] 定义类
来源：http://kye.c1oappe.top

Py:   class User: pass
来源：http://yxd.shzxlz.cn

PHP:  class User {}
来源：http://vuu.fzhhl.top

JS:   class User {}
来源：http://ozu.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://xtt.vehdjk.com

Java: class User {}
来源：http://oun.jinghuilouyu.cn

Go:   type User struct { Name string }
来源：http://mez.uphjek.com

Ruby: class User; end
来源：http://mby.quarkkingdee.top

C#:   class User {}
来源：http://qdk.jiagoushi.top

[G02] 构造函数
来源：http://qwm.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://lhf.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://keb.tianlin.xyz

JS:   constructor(name) { this.name = name; }
来源：http://pxl.tarul.cn

TS:   constructor(public name: string) {}
来源：http://oeq.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://mus.hcnkem.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://obh.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://npp.jqgufenzy.top

C#:   public User(string name) { Name = name; }
来源：http://jhi.zhoulong.xyz

[G03] 实例属性
来源：http://rto.jinqigufen.top

Py:   self.name = "x"
来源：http://gvg.uphjek.com

PHP:  public string $name = "x";
来源：http://yxo.yj20258.top

JS:   this.name = "x";
来源：http://afx.cqqwz.cn

TS:   name: string = "x";
来源：http://bbx.pycfn.com

Java: private String name;
来源：http://xnl.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zjd.yvedp.cn

Ruby: @name = "x"
来源：http://lyd.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://gqa.smart0.xyz

[G04] 定义方法
来源：http://uhf.sweek.top

Py:   def greet(self): return self.name
来源：http://xpk.ydzc1.top

PHP:  public function greet(): string { return $this->name; }
来源：http://bet.sysykeji.top

JS:   greet() { return this.name; }
来源：http://lrd.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://coz.fengsongda.top

Java: String greet() { return name; }
来源：http://syv.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ewe.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://szd.fzhhl.top

C#:   public string Greet() => Name;
来源：http://xhf.shanyushiyangkeji.top

[G05] 继承
来源：http://sde.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://dpc.bbcook.cn

PHP:  class Admin extends User {}
来源：http://zjn.aibaodan.cn

JS:   class Admin extends User {}
来源：http://ubf.meibo888.top

TS:   class Admin extends User {}
来源：http://vhl.nwbrower.top

Java: class Admin extends User {}
来源：http://cne.hysaishi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tix.vqdsnc.cn

Ruby: class Admin < User; end
来源：http://zin.hammf.cn

C#:   class Admin : User {}
来源：http://myb.0kj1m.cn

[G06] 重写方法
来源：http://dnf.daria6918.cn

Py:   def greet(self): return "admin"
来源：http://str.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://giu.ppjwa.cn

JS:   greet() { return "admin"; }
来源：http://jkb.jyoumei.cn

TS:   greet(): string { return "admin"; }
来源：http://mqx.nanxinkj.top

Java: @Override String greet() { return "admin"; }
来源：http://rgg.zhijiandao.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lnz.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://lng.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://yps.zhiwuduotai.top

[G07] 调用父类方法
来源：http://zcl.epnwcf.com

Py:   super().greet()
来源：http://suj.ppjwa.cn

PHP:  parent::greet();
来源：http://zau.chenzaomai.com

JS:   super.greet();
来源：http://vgp.yonumen.top

TS:   super.greet();
来源：http://xtc.guannengcc.top

Java: super.greet();
来源：http://jdk.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jgy.hesvh.cn

Ruby: super
来源：http://tyy.jqgufenzy.top

C#:   base.Greet();
来源：http://xde.ybcxt.top

[G08] 静态方法与属性
来源：http://nry.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uhw.hcnkem.com

PHP:  public static function f() {}
来源：http://yol.xylfe.cn

JS:   static f() {}
来源：http://seh.hammf.cn

TS:   static f(): void {}
来源：http://kkn.zhongyouzk.top

Java: static void f() {}
来源：http://aku.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://hye.zdqjudy.top

Ruby: def self.f; end
来源：http://bje.shangyingyoupin.top

C#:   public static void F() {}
来源：http://afz.birdmap.top

[G09] 接口 / 抽象类
来源：http://ebe.shangyingyoupin.top

Py:   from abc import ABC, abstractmethod
来源：http://pva.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xim.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ejd.havefunace.top

TS:   interface Shape { area(): number; }
来源：http://xhn.vehdjk.com

Java: interface Shape { double area(); }
来源：http://tgc.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://iqp.ydzc1.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gvq.mhx1999.top

C#:   interface IShape { double Area(); }
来源：http://xri.zhengqikj.top

[G10] 访问控制
来源：http://kpy.52xcode.cn

Py:   约定 _protected / __private（不强制）
来源：http://mol.yongpay.top

PHP:  public / protected / private
来源：http://evq.guowangkeji.top

JS:   #private 字段；其余公开
来源：http://ixn.ybcxt.top


<!-- 参考信息 -->