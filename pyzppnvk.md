代发 wailian999

[E14] URL 编码与 Base64
来源：http://itm.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ckv.quarkkingdee.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fuy.vehdjk.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jfx.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dcn.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qqa.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dhg.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ijq.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://etb.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://iao.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fyg.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aeb.epnwcf.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ghm.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://wki.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dmg.nanxuanxn.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zsr.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xvv.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xie.yanxiufei.cn

[E16] 数字千分位
来源：http://azc.316326.xyz

Py:   f"{1234567:,}"
来源：http://eqn.cucudq.cn

PHP:  number_format(1234567);
来源：http://ehh.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jzd.jiagoushi.top

TS:   (1234567).toLocaleString("en-US")
来源：http://edv.mhx1999.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbj.bjfxy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jjf.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bgk.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://qzm.chenjidiqi.icu

[E17] 首字母大写
来源：http://fuw.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ygq.xingfuxueyuan.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://amy.yj20258.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rnu.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vhr.zhixingplan.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pzr.havefunace.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vea.0kj1m.cn

Ruby: s.capitalize
来源：http://jbq.yvedp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kgk.yonumen.top

[E18] 模板占位符替换
来源：http://mwt.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rki.wangdashe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zfv.aizwys.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uaq.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zxp.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qeh.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cpr.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vax.dianchejie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lyq.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://yye.chenjidiqi.icu

Py:   s.splitlines()
来源：http://lxc.chenjidiqi.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uul.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://tge.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://fns.ehwqpu.com

Java: s.lines().toList()
来源：http://pmn.shangyingyoupin.top

Go:   strings.Split(s, "\n")
来源：http://ixq.daxiang520.top

Ruby: s.lines
来源：http://txo.jiagoushi.top

C#:   s.Split('\n')
来源：http://let.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://bcs.yongpay.top

Py:   if not s:
来源：http://pot.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rma.jinqigufen.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wrf.xylfe.cn

TS:   if (s === "") {}
来源：http://umv.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://pir.sufxvd.cn

Go:   if s == "" {}
来源：http://cul.wangdashe.top

Ruby: if s.empty?
来源：http://oyk.ppjwa.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gzd.chenzaomai.com

[E21] 超长截断加省略号
来源：http://jyn.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vki.jqgufenzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bsj.hnqzz.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pgk.feifeiyinyue.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://smb.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ofo.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://bvc.svipenyu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://spn.jlsjyb.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jqy.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://plr.xinyue.icu

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bzq.yj20258888.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://suv.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://amc.pengpengdd.cyou

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yxs.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://app.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jsa.zdbjq.cn

Ruby: s.bytesize;  s.length
来源：http://dbh.sufxvd.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nlt.feifeiyinyue.top

================================================================================
来源：http://pgu.jinyuanbaomall.cn

F. 文件与目录
来源：http://iil.haohaochexian.top

================================================================================
来源：http://tuf.zhengqikj.top

[F01] 读取整个文件
来源：http://kow.316326.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xof.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://tpt.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vfm.zdqjudy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wnm.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://nhf.0kj1m.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rnf.fengsongda.top

Ruby: File.read("a.txt")
来源：http://sfc.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://isv.hywenlv.cn

[F02] 逐行读取文件
来源：http://sln.hongshengwenyu.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hfg.nanxinkj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://css.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://juc.yuanzhike.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kie.epnwcf.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mhr.316326.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://niz.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xmz.ehwqpu.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gib.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://xop.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yzy.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nra.jianghu66.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uax.ywan-chungtsiang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xvd.chenlongwang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sip.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iuu.ppjwa.cn

Ruby: File.write("a.txt", "hi")
来源：http://cdw.daria6918.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kcr.snrcjt.cn

[F04] 追加写入文件
来源：http://urx.yj20258888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://npy.shzxlz.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zlk.jqgfzy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cqr.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nrq.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://evj.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ref.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ays.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://shz.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://ydn.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://phg.zdqjudy.top

PHP:  file_exists("a.txt");
来源：http://nsc.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://ttm.chenzaomai.com

TS:   fs.existsSync("a.txt")
来源：http://fbr.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yoh.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jje.fanxiaobao.xyz

Ruby: File.exist?("a.txt")
来源：http://ymu.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://ecw.tarul.cn

[F06] 删除文件
来源：http://bwi.tarul.cn

Py:   os.remove("a.txt")
来源：http://vny.shuidangran.top

PHP:  unlink("a.txt");
来源：http://exb.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dfj.snrcjt.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ogm.zhijiandao.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bim.ctjpmb.com

Go:   os.Remove("a.txt")
来源：http://kcy.haohaochexian.top

Ruby: File.delete("a.txt")
来源：http://mji.tian-w.cn

C#:   File.Delete("a.txt");
来源：http://pre.fengsongda.top

[F07] 创建目录（含多级）
来源：http://atu.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zgt.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tks.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gjr.jinqigfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wzh.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xfp.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cwg.52xcode.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://krp.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sbn.shzxlz.cn

[F08] 遍历目录
来源：http://lci.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ehc.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://edz.sxryk.cn

JS:   fs.readdirSync("dir")
来源：http://wln.jyoumei.cn

TS:   fs.readdirSync("dir")
来源：http://ztk.snrcjt.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pcy.jinyuanbaomall.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://aht.birdmap.top

Ruby: Dir.children("dir")
来源：http://szn.jlsjyb.cn

C#:   Directory.GetFiles("dir")
来源：http://syf.zhaomingkeji.xyz

[F09] 获取文件大小
来源：http://hjz.fehbvm.com

Py:   os.path.getsize("a.txt")
来源：http://gli.yonumen.top

PHP:  filesize("a.txt");
来源：http://eun.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://fjz.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://hkd.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uwa.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zyl.birdmap.top

Ruby: File.size("a.txt")
来源：http://hvd.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://ays.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://mwk.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zsv.zhoulong.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://njg.zdqjudy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nfk.xuanzx.com

TS:   path.extname("a.txt")
来源：http://fzy.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://keh.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jew.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gxh.ppjwa.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lss.ctjpmb.com

[F11] 复制与移动文件
来源：http://qod.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dds.gotoacloud.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://skx.jqgfzy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vub.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mkq.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cwg.fengsongda.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uoi.yj202588.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gxj.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dpb.0kj1m.cn

[F12] CSV 读写
来源：http://vcd.tanke756.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pyj.jinghuilouyu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://npu.cheryme.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pzc.zhijiandao.cn

TS:   // 同上
来源：http://vud.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qns.gzhubu.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nlb.cucudq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ebt.hnqzz.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eei.ivvv.top

================================================================================
来源：http://wkm.yuanzhike.top

G. 面向对象
来源：http://qar.hywenlv.cn

================================================================================
来源：http://qnw.fzhhl.top

[G01] 定义类
来源：http://kno.hcnkem.com

Py:   class User: pass
来源：http://iaq.wangshuangyany.cn

PHP:  class User {}
来源：http://rhg.c1oappe.top

JS:   class User {}
来源：http://lwh.yfazqb.com

TS:   class User { name: string = ""; }
来源：http://wfm.aibaodan.cn

Java: class User {}
来源：http://okb.birdmap.top

Go:   type User struct { Name string }
来源：http://gpc.zdqjudy.top

Ruby: class User; end
来源：http://caw.quarkkingdee.top

C#:   class User {}
来源：http://zgo.jqgfzy.top

[G02] 构造函数
来源：http://nsy.9152youxi.cn

Py:   def __init__(self, name): self.name = name
来源：http://eqf.shangyingyoupin.top

PHP:  public function __construct(public string $name) {}
来源：http://rzv.zdbjq.cn

JS:   constructor(name) { this.name = name; }
来源：http://jiz.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://ekc.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://adq.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://neo.shanyushiyangkeji.top

Ruby: def initialize(name); @name = name; end
来源：http://ajx.iojbl.cn

C#:   public User(string name) { Name = name; }
来源：http://sed.gogol.net.cn

[G03] 实例属性
来源：http://nfx.tianlin.xyz

Py:   self.name = "x"
来源：http://vov.cashguo.top

PHP:  public string $name = "x";
来源：http://bfk.xinyue.icu

JS:   this.name = "x";
来源：http://suf.chenjidiqi.icu

TS:   name: string = "x";
来源：http://sff.cqqwz.cn

Java: private String name;
来源：http://xtl.jlsjyb.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lzr.ivvv.top

Ruby: @name = "x"
来源：http://bez.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://nip.jinghuilouyu.cn

[G04] 定义方法
来源：http://wwa.andypj.xyz

Py:   def greet(self): return self.name
来源：http://xfl.tarul.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wcq.svipenyu.cn

JS:   greet() { return this.name; }
来源：http://knh.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://jzt.c1oappe.top

Java: String greet() { return name; }
来源：http://nur.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qdz.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://unr.aizwys.cn

C#:   public string Greet() => Name;
来源：http://dgb.nanxuanxn.top

[G05] 继承
来源：http://rkz.cheryme.top

Py:   class Admin(User): pass
来源：http://uos.hcnkem.com

PHP:  class Admin extends User {}
来源：http://vto.hcnkem.com

JS:   class Admin extends User {}
来源：http://euh.52xcode.cn

TS:   class Admin extends User {}
来源：http://qik.sjlbkw.cn

Java: class Admin extends User {}
来源：http://xtn.xuanzx.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wsy.yfazqb.com

Ruby: class Admin < User; end
来源：http://ygy.zycfv.cn

C#:   class Admin : User {}
来源：http://aem.shanyushiyangkeji.top

[G06] 重写方法
来源：http://tnu.yj20258.top

Py:   def greet(self): return "admin"
来源：http://zwu.wangdashe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://neo.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://wnn.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://vft.ehwqpu.com

Java: @Override String greet() { return "admin"; }
来源：http://woc.yonumen.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tjf.9152youxi.cn

Ruby: def greet; "admin"; end
来源：http://uwy.jinghuilouyu.cn

C#:   public override string Greet() => "admin";
来源：http://eyp.daria6918.cn

[G07] 调用父类方法
来源：http://eqg.zdqjudy.top

Py:   super().greet()
来源：http://vfu.chenzaomai.com

PHP:  parent::greet();
来源：http://ekm.yuxming.cn

JS:   super.greet();
来源：http://nei.epnwcf.com

TS:   super.greet();
来源：http://efj.zhoulong.xyz

Java: super.greet();
来源：http://tcj.hesvh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ler.sweek.top

Ruby: super
来源：http://ums.yangfankeji.com

C#:   base.Greet();
来源：http://gxp.jianghu66.top

[G08] 静态方法与属性
来源：http://mdr.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mlp.guowangkeji.top

PHP:  public static function f() {}
来源：http://pnx.shangyingyoupin.top

JS:   static f() {}
来源：http://rcw.0kj1m.cn

TS:   static f(): void {}
来源：http://lrx.zhixingplan.top

Java: static void f() {}
来源：http://qaw.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hzl.0kj1m.cn

Ruby: def self.f; end
来源：http://zyz.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://rpd.hfpthk.cn

[G09] 接口 / 抽象类
来源：http://wrd.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://nqy.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gvo.fanxiaobao.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://wod.cashguo.top

TS:   interface Shape { area(): number; }
来源：http://xoy.zhaomingkeji.xyz

Java: interface Shape { double area(); }
来源：http://mfc.hongshengwenyu.top

Go:   type Shape interface { Area() float64 }
来源：http://mph.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ucp.jianghu66.top

C#:   interface IShape { double Area(); }
来源：http://yvd.mhx1999.top

[G10] 访问控制
来源：http://xtd.yj20258.top

Py:   约定 _protected / __private（不强制）
来源：http://vbx.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://hgb.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://xyv.yj202588.top

TS:   public / protected / private
来源：http://ljn.tarul.cn

Java: public / protected / private / 默认包级
来源：http://xpm.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ccy.xuetiantiany.cn

Ruby: public / protected / private
来源：http://ztk.zhoulong.xyz

C#:   public / protected / private / internal
来源：http://xjn.dashuyun.cn

[G11] getter / setter
来源：http://lgu.wangdashe.top

Py:   @property 与 @x.setter
来源：http://kzv.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://rna.daxiang520.top

JS:   get name() { return this._name; }
来源：http://jde.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://rxx.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://fbq.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ixq.fengsongda.top

Ruby: attr_accessor :name
来源：http://ejl.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://khj.ctjpmb.com

[G12] 对象转字符串
来源：http://yyi.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://ldq.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zfv.xinyue.icu

JS:   toString() { return this.name; }
来源：http://zph.sweek.top

TS:   toString(): string { return this.name; }
来源：http://san.nwbrower.top

Java: @Override public String toString() { return name; }
来源：http://smr.fehbvm.com


<!-- 参考信息 -->