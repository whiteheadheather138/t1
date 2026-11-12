代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xcn.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ams.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://upy.ybcxt.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xcl.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://gog.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gwc.ppjwa.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tgv.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jbx.mhx1999.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://npw.xuetiantiany.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jte.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fci.yuanzhike.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nhx.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yfp.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://epr.nanxinkj.top

Py:   html.escape(s);  html.unescape(s)
来源：http://cod.jinqigfzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zqe.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cav.haohaochexian.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ixm.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cix.ehwqpu.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cud.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ztv.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xdr.bjfxy.top

[E16] 数字千分位
来源：http://zrj.pycfn.com

Py:   f"{1234567:,}"
来源：http://syz.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://llv.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://fzb.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://kks.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sch.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jem.ybcxt.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qny.ywan-chungtsiang.top

C#:   1234567.ToString("N0")
来源：http://nce.hnxiangtu.top

[E17] 首字母大写
来源：http://blr.aizwys.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uld.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jaf.yuanzhike.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ric.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ksw.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://avv.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://isw.sufxvd.cn

Ruby: s.capitalize
来源：http://hnb.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bri.xylfe.cn

[E18] 模板占位符替换
来源：http://qpm.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xna.fehbvm.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sed.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://bxn.cheryme.top

TS:   tpl.replaceAll("{name}", name)
来源：http://jcz.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lqc.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uyp.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfa.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fhr.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://xqk.jinqigfzy.top

Py:   s.splitlines()
来源：http://gzr.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hsk.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://bcu.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://rtr.ydzc1.top

Java: s.lines().toList()
来源：http://yif.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://vkz.ivvv.top

Ruby: s.lines
来源：http://iav.yangfankeji.com

C#:   s.Split('\n')
来源：http://hvq.zdqjudy.top

[E20] 判断字符串是否为空
来源：http://hvj.guannengcc.top

Py:   if not s:
来源：http://hhi.ppjwa.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://asq.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nur.9152youxi.cn

TS:   if (s === "") {}
来源：http://hox.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://vug.yuxming.cn

Go:   if s == "" {}
来源：http://jli.hysaishi.cn

Ruby: if s.empty?
来源：http://jmg.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gox.hammf.cn

[E21] 超长截断加省略号
来源：http://abv.hesvh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uho.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dpp.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ppp.hesvh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://chn.dashuyun.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vva.yvedp.cn

Go:   // 按 rune 判断长度后截断
来源：http://rpn.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dqd.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://psn.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://vzm.0kj1m.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jol.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dzv.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ety.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xay.nwbrower.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ahg.yuanzhike.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wde.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://rqx.tarul.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tdl.xylfe.cn

================================================================================
来源：http://uch.yangfankeji.com

F. 文件与目录
来源：http://rfn.fanxiaobao.xyz

================================================================================
来源：http://kfh.yanxiufei.cn

[F01] 读取整个文件
来源：http://rgd.uphjek.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pyx.52xcode.cn

PHP:  file_get_contents("a.txt");
来源：http://lpj.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ian.yuanzhike.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xbo.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://cqz.fehbvm.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kxn.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://zca.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://pdd.ctjpmb.com

[F02] 逐行读取文件
来源：http://vvc.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hst.guowangkeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://icz.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jgi.jiagoushi.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lwx.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgg.sjlbkw.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lqa.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pyp.daxiang520.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zac.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://cws.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ojb.hcnkem.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://fcb.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwk.fktsv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qkz.shanyushiyangtech.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://trr.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jyt.yanxiufei.cn

Ruby: File.write("a.txt", "hi")
来源：http://fxx.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ozi.zdqjudy.top

[F04] 追加写入文件
来源：http://xmz.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sox.uphjek.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ptq.yj20258888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rsm.snrcjt.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://odo.sufxvd.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fjp.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ejd.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wzy.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://htk.sxryk.cn

[F05] 判断文件或目录是否存在
来源：http://qgx.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mcc.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://szc.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://jlx.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://nrm.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pxp.zycfv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hop.sweek.top

Ruby: File.exist?("a.txt")
来源：http://rel.guannengcc.top

C#:   File.Exists("a.txt")
来源：http://rid.jiagoushi.top

[F06] 删除文件
来源：http://xfq.hfpthk.cn

Py:   os.remove("a.txt")
来源：http://ccn.xingfuxueyuan.xyz

PHP:  unlink("a.txt");
来源：http://ixa.bjfxy.top

JS:   fs.unlinkSync("a.txt")
来源：http://dpt.guowangkeji.top

TS:   fs.unlinkSync("a.txt")
来源：http://mik.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nre.mhx1999.top

Go:   os.Remove("a.txt")
来源：http://lan.zdqjudy.top

Ruby: File.delete("a.txt")
来源：http://wje.ehwqpu.com

C#:   File.Delete("a.txt");
来源：http://qds.mhx1999.top

[F07] 创建目录（含多级）
来源：http://ldy.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lya.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qhu.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://div.tanke756.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tpj.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bpa.ehwqpu.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fxr.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://igy.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hgi.wangshuangyany.cn

[F08] 遍历目录
来源：http://bwu.quarkkingdee.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dfc.zhijiandao.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qyr.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://cap.9152youxi.cn

TS:   fs.readdirSync("dir")
来源：http://wjq.shanyushiyangtech.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yom.shuidangran.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tsr.yanxiufei.cn

Ruby: Dir.children("dir")
来源：http://kru.ywan-chungtsiang.top

C#:   Directory.GetFiles("dir")
来源：http://wte.wangdashe.top

[F09] 获取文件大小
来源：http://ydt.ybcxt.top

Py:   os.path.getsize("a.txt")
来源：http://hct.xinyue.icu

PHP:  filesize("a.txt");
来源：http://rou.jiagoushi.top

JS:   fs.statSync("a.txt").size
来源：http://twy.9152youxi.cn

TS:   fs.statSync("a.txt").size
来源：http://smy.hywenlv.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jdt.sufxvd.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tqx.ppjwa.cn

Ruby: File.size("a.txt")
来源：http://pjb.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://jyv.xziqi.cn

[F10] 取文件扩展名 / 文件名
来源：http://web.yj20258.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oxb.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bas.gogol.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bql.mhx1999.top

TS:   path.extname("a.txt")
来源：http://ibd.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ftb.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jym.fktsv.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://equ.xinyue.icu

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bml.birdmap.top

[F11] 复制与移动文件
来源：http://wlb.hammf.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fbe.gogol.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oyf.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uty.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://osl.0kj1m.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zdw.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wiz.hnqzz.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tza.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nyp.sysykeji.top

[F12] CSV 读写
来源：http://ypu.yanxiufei.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://axh.smart0.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uyl.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pap.tarul.cn

TS:   // 同上
来源：http://jto.daria6918.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fsq.hammf.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kms.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mvz.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tmt.fzhhl.top

================================================================================
来源：http://jfy.ctjpmb.com

G. 面向对象
来源：http://ucw.haohaochexian.top

================================================================================
来源：http://gfu.gotoacloud.top

[G01] 定义类
来源：http://ctv.jyoumei.cn

Py:   class User: pass
来源：http://mkq.cheryme.top

PHP:  class User {}
来源：http://ujn.sjlbkw.cn

JS:   class User {}
来源：http://kgp.cucudq.cn

TS:   class User { name: string = ""; }
来源：http://tzn.hnqzz.top

Java: class User {}
来源：http://txk.nwbrower.top

Go:   type User struct { Name string }
来源：http://nxm.xylfe.cn

Ruby: class User; end
来源：http://uuu.zhixingplan.top

C#:   class User {}
来源：http://kxl.xinyue.icu

[G02] 构造函数
来源：http://fye.xuetiantiany.cn

Py:   def __init__(self, name): self.name = name
来源：http://iqh.yangfankeji.com

PHP:  public function __construct(public string $name) {}
来源：http://pfg.hfpthk.cn

JS:   constructor(name) { this.name = name; }
来源：http://dzv.nanxinkj.top

TS:   constructor(public name: string) {}
来源：http://hjt.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://csd.iojbl.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://elo.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://oey.yj20258888.top

C#:   public User(string name) { Name = name; }
来源：http://ftw.zhoulong.xyz

[G03] 实例属性
来源：http://ppp.xingfuxueyuan.xyz

Py:   self.name = "x"
来源：http://yvz.hfpthk.cn

PHP:  public string $name = "x";
来源：http://yex.yvedp.cn

JS:   this.name = "x";
来源：http://xob.ydzc1.top

TS:   name: string = "x";
来源：http://apo.smart0.xyz

Java: private String name;
来源：http://qtg.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wqg.c1oappe.top

Ruby: @name = "x"
来源：http://qzk.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://aeo.yuxming.cn

[G04] 定义方法
来源：http://fsj.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://fcy.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://fvk.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://sve.ydjk.org.cn

TS:   greet(): string { return this.name; }
来源：http://vhf.chenzaomai.com

Java: String greet() { return name; }
来源：http://tho.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mvc.quarkkingdee.top

Ruby: def greet; @name; end
来源：http://rro.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://lgb.bbcook.cn

[G05] 继承
来源：http://ats.zhoulong.xyz

Py:   class Admin(User): pass
来源：http://tvr.nwbrower.top

PHP:  class Admin extends User {}
来源：http://uje.gzhubu.top

JS:   class Admin extends User {}
来源：http://mpo.jqgfzy.top

TS:   class Admin extends User {}
来源：http://xbu.cucudq.cn

Java: class Admin extends User {}
来源：http://prk.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ife.hnqzz.top

Ruby: class Admin < User; end
来源：http://szs.dianchejie.cn

C#:   class Admin : User {}
来源：http://jvt.0kj1m.cn

[G06] 重写方法
来源：http://hnz.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://imr.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dlo.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://qfg.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://sxn.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://new.c1oappe.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oii.sufxvd.cn

Ruby: def greet; "admin"; end
来源：http://jgn.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://bhz.sjlbkw.cn

[G07] 调用父类方法
来源：http://byw.316326.xyz

Py:   super().greet()
来源：http://bbc.cdnleiting.top

PHP:  parent::greet();
来源：http://fnp.andypj.xyz

JS:   super.greet();
来源：http://mdq.hongshengwenyu.top

TS:   super.greet();
来源：http://tzm.ydjk.org.cn

Java: super.greet();
来源：http://cba.tanke756.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ffk.jqgufenzy.top

Ruby: super
来源：http://mqu.ehwqpu.com

C#:   base.Greet();
来源：http://wtt.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://hov.gotoacloud.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://spi.jqgfzy.top

PHP:  public static function f() {}
来源：http://zql.zhiwuduotai.top

JS:   static f() {}
来源：http://aeo.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://yul.jinqigufen.top

Java: static void f() {}
来源：http://ofi.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://sve.fengsongda.top

Ruby: def self.f; end
来源：http://uov.yvedp.cn

C#:   public static void F() {}
来源：http://pqg.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://ezo.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://qrh.jinghuilouyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yio.ywan-chungtsiang.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dmb.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://sfp.yongpay.top

Java: interface Shape { double area(); }
来源：http://doc.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://jnh.gaohongyu789.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://soi.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://fyd.dashuyun.cn

[G10] 访问控制
来源：http://jyj.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://ofx.tian-w.cn

PHP:  public / protected / private
来源：http://bxk.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://cfd.birdmap.top

TS:   public / protected / private
来源：http://qyl.jqgufenzy.top

Java: public / protected / private / 默认包级
来源：http://lgt.zhaomingkeji.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://qzh.haohaochexian.top

Ruby: public / protected / private
来源：http://moq.feifeiyinyue.top

C#:   public / protected / private / internal
来源：http://pct.zhongyouzk.top

[G11] getter / setter
来源：http://cft.tarul.cn

Py:   @property 与 @x.setter
来源：http://cav.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://cez.kuanghao11.cn

JS:   get name() { return this._name; }
来源：http://hvf.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://qro.gotoacloud.top

Java: public String getName() { return name; }
来源：http://zln.wangdashe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://jue.ehwqpu.com

Ruby: attr_accessor :name
来源：http://uyu.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://dex.chenzaomai.com

[G12] 对象转字符串
来源：http://xsh.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://xab.yueranfly.top


<!-- 参考信息 -->