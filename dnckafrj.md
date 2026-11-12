代发 wailian999

Py:   for ch in s: print(ch)
来源：http://biv.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://srk.yuanzhike.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xvg.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ohk.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mcd.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nbu.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bdr.xziqi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uqc.yj20258.top

[E14] URL 编码与 Base64
来源：http://nkp.chenjidiqi.icu

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bbk.yueranfly.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://woi.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ksu.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jyf.cashguo.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fpm.cdnleiting.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mly.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cou.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hyn.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://bdw.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ekv.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nqf.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qza.smart0.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ner.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ean.yfazqb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hrw.bbcook.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yga.hysaishi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jfj.0kj1m.cn

[E16] 数字千分位
来源：http://uew.smart0.xyz

Py:   f"{1234567:,}"
来源：http://tmc.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://kui.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ebt.vqdsnc.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cxs.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fxe.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wdj.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ftf.pycfn.com

C#:   1234567.ToString("N0")
来源：http://vsu.nanxinkj.top

[E17] 首字母大写
来源：http://wfu.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gwm.nanxuanxn.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://inl.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://teo.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kkg.tian-w.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mxx.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rfa.cdnleiting.top

Ruby: s.capitalize
来源：http://bkt.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://epl.fzhhl.top

[E18] 模板占位符替换
来源：http://fmp.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fjt.nwbrower.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lsz.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://dna.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://hra.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wym.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xul.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wno.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gra.guowangkeji.top

[E19] 多行文本按行拆分
来源：http://jzb.fehbvm.com

Py:   s.splitlines()
来源：http://yai.mhx1999.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ylo.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://veh.ppjwa.cn

TS:   s.split(/\r?\n/)
来源：http://aoz.yonumen.top

Java: s.lines().toList()
来源：http://epl.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://don.epnwcf.com

Ruby: s.lines
来源：http://gmr.guowangkeji.top

C#:   s.Split('\n')
来源：http://zvy.dianchejie.cn

[E20] 判断字符串是否为空
来源：http://jhz.fehbvm.com

Py:   if not s:
来源：http://fqy.yj20258.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oua.dianchejie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kkc.ybcxt.top

TS:   if (s === "") {}
来源：http://myq.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://jbn.meibo888.top

Go:   if s == "" {}
来源：http://brv.ywan-chungtsiang.top

Ruby: if s.empty?
来源：http://ikl.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ycy.ywan-chungtsiang.top

[E21] 超长截断加省略号
来源：http://jxy.feifeiyinyue.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ago.0kj1m.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zrc.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pqf.jqgufenzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lxa.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gfh.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://uzk.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uyr.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bao.fzhhl.top

[E22] 字节长度与字符长度
来源：http://dvh.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ttx.yuxming.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mzq.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pfb.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jsj.bbcook.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zcn.tanke756.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yna.yangfankeji.com

Ruby: s.bytesize;  s.length
来源：http://icu.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nbm.yj202588.top

================================================================================
来源：http://xnd.aibaodan.cn

F. 文件与目录
来源：http://jrb.guowangkeji.top

================================================================================
来源：http://pyv.jlsjyb.cn

[F01] 读取整个文件
来源：http://wlu.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dgt.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://bob.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hzx.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hsg.uphjek.com

Java: Files.readString(Path.of("a.txt"))
来源：http://tlr.kuanghao11.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hhz.cashguo.top

Ruby: File.read("a.txt")
来源：http://kft.sjlbkw.cn

C#:   File.ReadAllText("a.txt");
来源：http://qfx.jinqigfzy.top

[F02] 逐行读取文件
来源：http://dyh.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yyu.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fpj.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gak.daxiang520.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cpb.hnqzz.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iuy.fktsv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://emj.cqqwz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lyx.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dcx.yj202588.top

[F03] 写入文件（覆盖）
来源：http://pgu.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://knz.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tdi.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://umo.sufxvd.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hqh.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cny.pycfn.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://aek.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://mnm.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yrw.dianchejie.cn

[F04] 追加写入文件
来源：http://llf.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://npj.xziqi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://inm.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yzw.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hfo.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dna.uphjek.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbs.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pqo.pengpengdd.cyou

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ntf.kuanghao11.cn

[F05] 判断文件或目录是否存在
来源：http://ecj.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bys.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://nbm.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://xes.hysaishi.cn

TS:   fs.existsSync("a.txt")
来源：http://yie.smart0.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://gjl.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jqt.chenjidiqi.icu

Ruby: File.exist?("a.txt")
来源：http://uaf.shuidangran.top

C#:   File.Exists("a.txt")
来源：http://kem.yanxiufei.cn

[F06] 删除文件
来源：http://rem.xuetiantiany.cn

Py:   os.remove("a.txt")
来源：http://qmx.wangdashe.top

PHP:  unlink("a.txt");
来源：http://wxz.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://lve.zhengqikj.top

TS:   fs.unlinkSync("a.txt")
来源：http://fpu.cdnleiting.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://szn.ehwqpu.com

Go:   os.Remove("a.txt")
来源：http://cvl.zhixingplan.top

Ruby: File.delete("a.txt")
来源：http://gal.uphjek.com

C#:   File.Delete("a.txt");
来源：http://ezh.birdmap.top

[F07] 创建目录（含多级）
来源：http://zbs.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pvo.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dwi.birdmap.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fwf.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uhe.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://afq.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vmb.zhiwuduotai.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hbq.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fyh.zhoulong.xyz

[F08] 遍历目录
来源：http://smc.nwbrower.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ezb.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vwj.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://vdz.dianchejie.cn

TS:   fs.readdirSync("dir")
来源：http://zns.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nij.sweek.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zzs.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://ycw.snrcjt.cn

C#:   Directory.GetFiles("dir")
来源：http://xkw.nanxinkj.top

[F09] 获取文件大小
来源：http://kpp.dashuyun.cn

Py:   os.path.getsize("a.txt")
来源：http://hnz.xylfe.cn

PHP:  filesize("a.txt");
来源：http://oul.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://yla.guannengcc.top

TS:   fs.statSync("a.txt").size
来源：http://ehi.yuanzhike.top

Java: Files.size(Path.of("a.txt"))
来源：http://sba.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nak.xuanzx.com

Ruby: File.size("a.txt")
来源：http://yff.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://xvp.yvedp.cn

[F10] 取文件扩展名 / 文件名
来源：http://azo.cheryme.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://utu.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rqv.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hqe.xziqi.cn

TS:   path.extname("a.txt")
来源：http://pxi.wangshuangyany.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vwm.gzhubu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rml.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sfl.chenzaomai.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ekw.sysykeji.top

[F11] 复制与移动文件
来源：http://eja.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wkp.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ymr.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bqa.yangfankeji.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xjd.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dmb.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qtw.tian-w.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hhn.sjlbkw.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hfl.sjlbkw.cn

[F12] CSV 读写
来源：http://jje.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jua.birdmap.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xyp.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zqa.fzhhl.top

TS:   // 同上
来源：http://bey.xuetiantiany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://aki.fanxiaobao.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jfc.cheryme.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wuc.gotoacloud.top

C#:   // 无内置：用 CsvHelper 库
来源：http://guv.andypj.xyz

================================================================================
来源：http://rrq.hnqzz.top

G. 面向对象
来源：http://yrd.yueranfly.top

================================================================================
来源：http://hhf.xinyue.icu

[G01] 定义类
来源：http://hoi.cdnleiting.top

Py:   class User: pass
来源：http://ied.hnqzz.top

PHP:  class User {}
来源：http://clz.ydjk.org.cn

JS:   class User {}
来源：http://zol.tarul.cn

TS:   class User { name: string = ""; }
来源：http://but.tanke756.top

Java: class User {}
来源：http://dcd.tarul.cn

Go:   type User struct { Name string }
来源：http://eei.cheryme.top

Ruby: class User; end
来源：http://bbx.quarkkingdee.top

C#:   class User {}
来源：http://yns.uphjek.com

[G02] 构造函数
来源：http://nuh.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://lek.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://yso.fehbvm.com

JS:   constructor(name) { this.name = name; }
来源：http://iuk.aibaodan.cn

TS:   constructor(public name: string) {}
来源：http://upw.9152youxi.cn

Java: User(String name) { this.name = name; }
来源：http://qts.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ezg.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://ppw.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://hoc.zhixingplan.top

[G03] 实例属性
来源：http://qcq.bjfxy.top

Py:   self.name = "x"
来源：http://bsl.zdqjudy.top

PHP:  public string $name = "x";
来源：http://ouq.shanyushiyangtech.top

JS:   this.name = "x";
来源：http://jvi.guannengcc.top

TS:   name: string = "x";
来源：http://arf.gogol.net.cn

Java: private String name;
来源：http://fxv.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hzq.smart0.xyz

Ruby: @name = "x"
来源：http://ijf.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://fni.sufxvd.cn

[G04] 定义方法
来源：http://jrt.xuetiantiany.cn

Py:   def greet(self): return self.name
来源：http://zch.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://hjk.redwolf501.top

JS:   greet() { return this.name; }
来源：http://hhj.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://txp.zhongyouzk.top

Java: String greet() { return name; }
来源：http://duy.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xvm.yongpay.top

Ruby: def greet; @name; end
来源：http://yva.wangdashe.top

C#:   public string Greet() => Name;
来源：http://fju.xylfe.cn

[G05] 继承
来源：http://cnx.shanyushiyangtech.top

Py:   class Admin(User): pass
来源：http://qyb.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://yiz.cheryme.top

JS:   class Admin extends User {}
来源：http://nes.daxiang520.top

TS:   class Admin extends User {}
来源：http://hpf.hnxiangtu.top

Java: class Admin extends User {}
来源：http://rbz.yueranfly.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://izy.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://fii.c1oappe.top

C#:   class Admin : User {}
来源：http://iuu.sjlbkw.cn

[G06] 重写方法
来源：http://han.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://ibj.zhongyouzk.top

PHP:  public function greet(): string { return "admin"; }
来源：http://bzv.cdnleiting.top

JS:   greet() { return "admin"; }
来源：http://atv.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://ejm.tanke756.top

Java: @Override String greet() { return "admin"; }
来源：http://kit.wangshuangyany.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ilg.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://ulu.yvedp.cn

C#:   public override string Greet() => "admin";
来源：http://cvk.shzxlz.cn

[G07] 调用父类方法
来源：http://dsa.xziqi.cn

Py:   super().greet()
来源：http://qcq.ctjpmb.com

PHP:  parent::greet();
来源：http://epe.zdqjudy.top

JS:   super.greet();
来源：http://pvo.hywenlv.cn

TS:   super.greet();
来源：http://ovm.yonumen.top

Java: super.greet();
来源：http://axz.zhengqikj.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ncv.chenzaomai.com

Ruby: super
来源：http://zeu.jlsjyb.cn

C#:   base.Greet();
来源：http://mlk.jiagoushi.top

[G08] 静态方法与属性
来源：http://xmc.chenjidiqi.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spf.cheryme.top

PHP:  public static function f() {}
来源：http://syl.jqgufenzy.top

JS:   static f() {}
来源：http://jsf.aizwys.cn

TS:   static f(): void {}
来源：http://ujt.tarul.cn

Java: static void f() {}
来源：http://ebs.guannengcc.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qgv.52xcode.cn

Ruby: def self.f; end
来源：http://ghd.snrcjt.cn

C#:   public static void F() {}
来源：http://ffv.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://jvp.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://vdc.nanxuanxn.top

PHP:  interface Shape { public function area(): float; }
来源：http://vwf.vqdsnc.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wjd.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://unn.redwolf501.top

Java: interface Shape { double area(); }
来源：http://ura.guowangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://ngz.iojbl.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jmk.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://awe.wangshuangyany.cn

[G10] 访问控制
来源：http://pza.daria6918.cn

Py:   约定 _protected / __private（不强制）
来源：http://lie.52xcode.cn

PHP:  public / protected / private
来源：http://dmv.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://zcf.zycfv.cn

TS:   public / protected / private
来源：http://wvs.ppjwa.cn

Java: public / protected / private / 默认包级
来源：http://lhg.zdbjq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tbl.yj20258888.top

Ruby: public / protected / private
来源：http://foj.52xcode.cn

C#:   public / protected / private / internal
来源：http://etn.tarul.cn

[G11] getter / setter
来源：http://wcx.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://zal.hysaishi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xbf.bbcook.cn

JS:   get name() { return this._name; }
来源：http://yoa.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://nfk.vqdsnc.cn

Java: public String getName() { return name; }
来源：http://pvw.yuanzhike.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://haj.jlsjyb.cn


<!-- 参考信息 -->