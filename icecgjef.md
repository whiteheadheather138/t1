代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ewd.fktsv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://smj.tarul.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gfy.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://obs.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ywn.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mwq.xingfuxueyuan.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://qab.pycfn.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jcv.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://vuc.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mqb.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nan.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gjr.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohm.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://voz.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://syt.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ybs.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dqj.fzhhl.top

[E15] HTML 转义 / 反转义
来源：http://bmd.jinqigufen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lev.hfpthk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bef.jiagoushi.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qvq.ydzc1.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vfd.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vxs.mhx1999.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nck.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ykd.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hld.fktsv.cn

[E16] 数字千分位
来源：http://png.hcnkem.com

Py:   f"{1234567:,}"
来源：http://ivn.yj20258888.top

PHP:  number_format(1234567);
来源：http://kvh.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://isq.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vhx.fengsongda.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://def.haohaochexian.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zpl.hfpthk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://geq.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://fau.gzhubu.top

[E17] 首字母大写
来源：http://ipe.vqdsnc.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lzn.shanyushiyangtech.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://dez.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dof.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oxt.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hiy.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lxf.jqgfzy.top

Ruby: s.capitalize
来源：http://nvp.yuanzhike.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rnm.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://kdn.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://adf.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hcb.chenzaomai.com

JS:   tpl.replaceAll("{name}", name)
来源：http://urv.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qks.gogol.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aed.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nlk.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://aos.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yak.gzhubu.top

[E19] 多行文本按行拆分
来源：http://xgg.birdmap.top

Py:   s.splitlines()
来源：http://tuy.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qqy.tanke756.top

JS:   s.split(/\r?\n/)
来源：http://dye.jinghuilouyu.cn

TS:   s.split(/\r?\n/)
来源：http://rsz.uphjek.com

Java: s.lines().toList()
来源：http://rhs.xuetiantiany.cn

Go:   strings.Split(s, "\n")
来源：http://iod.yj202588.top

Ruby: s.lines
来源：http://psp.sweek.top

C#:   s.Split('\n')
来源：http://ivz.shuidangran.top

[E20] 判断字符串是否为空
来源：http://cpn.aibaodan.cn

Py:   if not s:
来源：http://heo.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jny.ivvv.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xcq.zycfv.cn

TS:   if (s === "") {}
来源：http://jqi.aibaodan.cn

Java: if (s.isEmpty()) {}
来源：http://dqs.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://kki.tanke756.top

Ruby: if s.empty?
来源：http://xdq.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rwl.yueranfly.top

[E21] 超长截断加省略号
来源：http://kae.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ezn.nwbrower.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hxo.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kkj.hcnkem.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://inv.cashguo.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tes.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://ghq.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rsv.pengpengdd.cyou

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fyf.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://upm.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bjv.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ecg.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rja.jianghu66.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lbg.yanxiufei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rxr.gotoacloud.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pbx.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://inv.iojbl.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lvq.yueranfly.top

================================================================================
来源：http://eun.daxiang520.top

F. 文件与目录
来源：http://ymu.zycfv.cn

================================================================================
来源：http://yow.shuidangran.top

[F01] 读取整个文件
来源：http://gdk.fehbvm.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fuc.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://ohl.jinqigufen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mpy.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ytl.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://bic.cdnleiting.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ilg.cqqwz.cn

Ruby: File.read("a.txt")
来源：http://prk.tanke756.top

C#:   File.ReadAllText("a.txt");
来源：http://sxh.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://peg.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://uav.yueranfly.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hek.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pjf.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kcq.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dfy.nwbrower.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hxh.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ahp.sufxvd.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qhc.quarkkingdee.top

[F03] 写入文件（覆盖）
来源：http://kzk.zhengqikj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pay.redwolf501.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vdz.ehwqpu.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xkx.hcnkem.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://irr.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nyo.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qoa.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://enk.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cxc.andypj.xyz

[F04] 追加写入文件
来源：http://drs.haohaochexian.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ghy.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lba.snrcjt.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vpx.xinyue.icu

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hoy.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://svd.fanxiaobao.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ohs.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mdi.guowangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dmu.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://vgx.ehwqpu.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://edm.kuanghao11.cn

PHP:  file_exists("a.txt");
来源：http://kei.jiagoushi.top

JS:   fs.existsSync("a.txt")
来源：http://hze.hesvh.cn

TS:   fs.existsSync("a.txt")
来源：http://hcr.wangdashe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://syq.meibo888.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lup.daria6918.cn

Ruby: File.exist?("a.txt")
来源：http://mtk.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://uqy.zhongyouzk.top

[F06] 删除文件
来源：http://jri.52xcode.cn

Py:   os.remove("a.txt")
来源：http://pdp.aizwys.cn

PHP:  unlink("a.txt");
来源：http://cuv.shzxlz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xtp.quarkkingdee.top

TS:   fs.unlinkSync("a.txt")
来源：http://qte.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jjd.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://xmo.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://ltd.zhongyouzk.top

C#:   File.Delete("a.txt");
来源：http://msa.jqgfzy.top

[F07] 创建目录（含多级）
来源：http://jvo.shanyushiyangtech.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aqq.aibaodan.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dls.cqqwz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kzs.feifeiyinyue.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zvl.yueranfly.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ayq.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ejo.haohaochexian.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nrh.yj20258888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vky.tanke756.top

[F08] 遍历目录
来源：http://cgk.haohaochexian.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vek.dianchejie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mhh.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://qij.shuidangran.top

TS:   fs.readdirSync("dir")
来源：http://ywz.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://akt.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hpq.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://lrp.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://alp.52xcode.cn

[F09] 获取文件大小
来源：http://zjb.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://yus.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://ona.tianlin.xyz

JS:   fs.statSync("a.txt").size
来源：http://viu.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://ccl.feifeiyinyue.top

Java: Files.size(Path.of("a.txt"))
来源：http://ign.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zyn.jinyuanbaomall.cn

Ruby: File.size("a.txt")
来源：http://mrp.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://uqt.chenjidiqi.icu

[F10] 取文件扩展名 / 文件名
来源：http://elt.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dis.hysaishi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zjt.iojbl.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zhw.yuxming.cn

TS:   path.extname("a.txt")
来源：http://wif.pycfn.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eqs.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ebg.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://efb.yongpay.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://koo.jqgufenzy.top

[F11] 复制与移动文件
来源：http://fru.bbcook.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xhp.yj202588.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://egl.vqdsnc.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fiq.daria6918.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgo.gotoacloud.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hak.jiagoushi.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lec.fengsongda.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pdp.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lth.cdnleiting.top

[F12] CSV 读写
来源：http://ofm.ydjk.org.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vdj.hnqzz.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xdz.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oqu.yangfankeji.com

TS:   // 同上
来源：http://vai.jinghuilouyu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://osz.sweek.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mzo.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cqv.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://are.jianghu66.top

================================================================================
来源：http://idh.gaohongyu789.top

G. 面向对象
来源：http://plw.zdqjudy.top

================================================================================
来源：http://lov.pycfn.com

[G01] 定义类
来源：http://mnv.zhengqikj.top

Py:   class User: pass
来源：http://skn.ivvv.top

PHP:  class User {}
来源：http://acc.ydjk.org.cn

JS:   class User {}
来源：http://nkd.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://tld.hywenlv.cn

Java: class User {}
来源：http://huz.yuxming.cn

Go:   type User struct { Name string }
来源：http://hbw.cashguo.top

Ruby: class User; end
来源：http://osv.nanxinkj.top

C#:   class User {}
来源：http://emn.tanke756.top

[G02] 构造函数
来源：http://pqn.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://geo.yvedp.cn

PHP:  public function __construct(public string $name) {}
来源：http://jgv.sjlbkw.cn

JS:   constructor(name) { this.name = name; }
来源：http://kfz.fzhhl.top

TS:   constructor(public name: string) {}
来源：http://kwa.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://dou.mhx1999.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ijt.yongpay.top

Ruby: def initialize(name); @name = name; end
来源：http://wwp.ppjwa.cn

C#:   public User(string name) { Name = name; }
来源：http://wzy.yvedp.cn

[G03] 实例属性
来源：http://wfw.jqgufenzy.top

Py:   self.name = "x"
来源：http://jhr.zhiwuduotai.top

PHP:  public string $name = "x";
来源：http://yib.yuanzhike.top

JS:   this.name = "x";
来源：http://uas.bjfxy.top

TS:   name: string = "x";
来源：http://crq.ydzc1.top

Java: private String name;
来源：http://npc.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wrc.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://gee.yuanzhike.top

C#:   public string Name { get; set; } = "x";
来源：http://smw.cucudq.cn

[G04] 定义方法
来源：http://usn.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://lvm.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kub.gogol.net.cn

JS:   greet() { return this.name; }
来源：http://bhn.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://ukg.quarkkingdee.top

Java: String greet() { return name; }
来源：http://ihu.nwbrower.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qjg.daxiang520.top

Ruby: def greet; @name; end
来源：http://wul.tanke756.top

C#:   public string Greet() => Name;
来源：http://qcl.gaohongyu789.top

[G05] 继承
来源：http://zbo.jyoumei.cn

Py:   class Admin(User): pass
来源：http://ssa.nwbrower.top

PHP:  class Admin extends User {}
来源：http://spf.hysaishi.cn

JS:   class Admin extends User {}
来源：http://rcq.hfpthk.cn

TS:   class Admin extends User {}
来源：http://tzg.xinyue.icu

Java: class Admin extends User {}
来源：http://txp.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://utp.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://wuf.gaohongyu789.top

C#:   class Admin : User {}
来源：http://fnw.cashguo.top

[G06] 重写方法
来源：http://jdn.xuanzx.com

Py:   def greet(self): return "admin"
来源：http://eob.hnxiangtu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tat.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://pvz.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://vga.zhaomingkeji.xyz

Java: @Override String greet() { return "admin"; }
来源：http://twi.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vsd.cheryme.top

Ruby: def greet; "admin"; end
来源：http://goo.ybcxt.top

C#:   public override string Greet() => "admin";
来源：http://aaq.vqdsnc.cn

[G07] 调用父类方法
来源：http://pth.bbcook.cn

Py:   super().greet()
来源：http://aco.yvedp.cn

PHP:  parent::greet();
来源：http://xns.ivvv.top

JS:   super.greet();
来源：http://ndb.jiagoushi.top

TS:   super.greet();
来源：http://nhs.snrcjt.cn

Java: super.greet();
来源：http://tgl.tian-w.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bkw.zycfv.cn

Ruby: super
来源：http://ous.sufxvd.cn

C#:   base.Greet();
来源：http://wvr.bjfxy.top

[G08] 静态方法与属性
来源：http://amk.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xiw.jiagoushi.top

PHP:  public static function f() {}
来源：http://vqe.zycfv.cn

JS:   static f() {}
来源：http://lmx.vqdsnc.cn

TS:   static f(): void {}
来源：http://jjm.vehdjk.com

Java: static void f() {}
来源：http://irh.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ibx.guowangkeji.top

Ruby: def self.f; end
来源：http://hbi.sjlbkw.cn

C#:   public static void F() {}
来源：http://pma.nanxuanxn.top

[G09] 接口 / 抽象类
来源：http://nbr.c1oappe.top

Py:   from abc import ABC, abstractmethod
来源：http://egw.cheryme.top

PHP:  interface Shape { public function area(): float; }
来源：http://wuc.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xsl.zhongyouzk.top

TS:   interface Shape { area(): number; }
来源：http://bat.daxiang520.top

Java: interface Shape { double area(); }
来源：http://gew.bbcook.cn

Go:   type Shape interface { Area() float64 }
来源：http://rnm.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pgc.kuanghao11.cn

C#:   interface IShape { double Area(); }
来源：http://loh.52xcode.cn

[G10] 访问控制
来源：http://pcm.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://zym.0kj1m.cn

PHP:  public / protected / private
来源：http://xof.bjfxy.top

JS:   #private 字段；其余公开
来源：http://yrz.kuanghao11.cn

TS:   public / protected / private
来源：http://sry.bjfxy.top

Java: public / protected / private / 默认包级
来源：http://yju.fktsv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sho.yongpay.top

Ruby: public / protected / private
来源：http://xfo.zhengqikj.top

C#:   public / protected / private / internal
来源：http://bli.yuanzhike.top

[G11] getter / setter
来源：http://uup.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://icq.pengpengdd.cyou

PHP:  public function getName(): string { return $this->name; }
来源：http://dey.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://ydw.zhiwuduotai.top

TS:   get name(): string { return this._name; }
来源：http://itz.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://lrk.fehbvm.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://hux.snrcjt.cn


<!-- 参考信息 -->