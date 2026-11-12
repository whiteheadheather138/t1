代发 wailian999

[E14] URL 编码与 Base64
来源：http://uyd.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kld.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vgs.dianchejie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hig.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gdq.bjfxy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gre.daxiang520.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jmt.fengsongda.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ysd.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://azl.ivvv.top

[E15] HTML 转义 / 反转义
来源：http://ptb.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vsp.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dwc.zhiwuduotai.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gbo.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dmt.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://waj.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ten.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ncy.svipenyu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qxu.gaohongyu789.top

[E16] 数字千分位
来源：http://heu.hcnkem.com

Py:   f"{1234567:,}"
来源：http://vmp.hywenlv.cn

PHP:  number_format(1234567);
来源：http://due.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://xdg.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nat.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xnq.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wnk.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rig.hnqzz.top

C#:   1234567.ToString("N0")
来源：http://uud.zdbjq.cn

[E17] 首字母大写
来源：http://ldk.yueranfly.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mpb.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ciy.sjlbkw.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eyz.kuanghao11.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bib.vqdsnc.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nzh.shuidangran.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qkx.cashguo.top

Ruby: s.capitalize
来源：http://ukq.yj20258.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zdw.redwolf501.top

[E18] 模板占位符替换
来源：http://tss.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://csw.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hmk.iojbl.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://urp.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pxu.nanxuanxn.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xyb.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gda.xingfuxueyuan.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://drt.0kj1m.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bia.shzxlz.cn

[E19] 多行文本按行拆分
来源：http://abg.gogol.net.cn

Py:   s.splitlines()
来源：http://sbf.c1oappe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oxm.yj20258.top

JS:   s.split(/\r?\n/)
来源：http://ocx.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://ydn.cheryme.top

Java: s.lines().toList()
来源：http://hqv.daria6918.cn

Go:   strings.Split(s, "\n")
来源：http://twr.guowangkeji.top

Ruby: s.lines
来源：http://eeg.c1oappe.top

C#:   s.Split('\n')
来源：http://mxb.xinyue.icu

[E20] 判断字符串是否为空
来源：http://spv.jqgfzy.top

Py:   if not s:
来源：http://gpo.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://txk.bjfxy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://got.zhongyouzk.top

TS:   if (s === "") {}
来源：http://yaq.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://sno.yanxiufei.cn

Go:   if s == "" {}
来源：http://zoo.shuidangran.top

Ruby: if s.empty?
来源：http://cue.9152youxi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hab.xziqi.cn

[E21] 超长截断加省略号
来源：http://xaa.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tad.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jpm.gaohongyu789.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hyr.daxiang520.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jlh.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zom.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://qwd.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rdy.fanxiaobao.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ibp.bbcook.cn

[E22] 字节长度与字符长度
来源：http://szs.zhongyouzk.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cws.xinyue.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qnt.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tih.pycfn.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://udd.fehbvm.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jfz.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mtg.cdnleiting.top

Ruby: s.bytesize;  s.length
来源：http://zfy.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yxe.birdmap.top

================================================================================
来源：http://dtv.aizwys.cn

F. 文件与目录
来源：http://yzt.nanxuanxn.top

================================================================================
来源：http://dbo.52xcode.cn

[F01] 读取整个文件
来源：http://dvb.xziqi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ovc.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://gmw.yfazqb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gid.fktsv.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gdn.yvedp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hze.zhengqikj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fcj.vehdjk.com

Ruby: File.read("a.txt")
来源：http://kcx.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://mli.shanyushiyangkeji.top

[F02] 逐行读取文件
来源：http://flx.yanxiufei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dpi.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gew.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skg.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ddw.zhoulong.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fju.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bst.xziqi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oka.zhaomingkeji.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sgi.yj20258888.top

[F03] 写入文件（覆盖）
来源：http://pwb.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hah.c1oappe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://onw.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eun.yfazqb.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwy.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://npi.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://chu.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://dzp.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aax.hnqzz.top

[F04] 追加写入文件
来源：http://qbk.sysykeji.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cog.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xef.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oly.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nfe.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dqm.epnwcf.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oyb.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vie.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pab.zhixingplan.top

[F05] 判断文件或目录是否存在
来源：http://zom.havefunace.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://muy.shanyushiyangtech.top

PHP:  file_exists("a.txt");
来源：http://agc.316326.xyz

JS:   fs.existsSync("a.txt")
来源：http://ecx.gogol.net.cn

TS:   fs.existsSync("a.txt")
来源：http://ucj.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://idz.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ecl.yongpay.top

Ruby: File.exist?("a.txt")
来源：http://vjs.haohaochexian.top

C#:   File.Exists("a.txt")
来源：http://lwa.gogol.net.cn

[F06] 删除文件
来源：http://ojr.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://axx.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://ivx.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://oah.yueranfly.top

TS:   fs.unlinkSync("a.txt")
来源：http://ruk.mhx1999.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nxg.9152youxi.cn

Go:   os.Remove("a.txt")
来源：http://vza.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://aih.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://mwt.ctjpmb.com

[F07] 创建目录（含多级）
来源：http://ryu.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uqo.cashguo.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dat.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zet.ydzc1.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://irf.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kgq.cucudq.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ldd.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lsp.bjfxy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kdc.yueranfly.top

[F08] 遍历目录
来源：http://ivc.fengsongda.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tsa.hcnkem.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dmk.fzhhl.top

JS:   fs.readdirSync("dir")
来源：http://eee.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://qeq.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://igm.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hbx.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://oua.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://wxu.vehdjk.com

[F09] 获取文件大小
来源：http://vxi.9152youxi.cn

Py:   os.path.getsize("a.txt")
来源：http://ntl.nanxuanxn.top

PHP:  filesize("a.txt");
来源：http://lri.shuidangran.top

JS:   fs.statSync("a.txt").size
来源：http://yet.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://bji.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://mpd.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qna.cashguo.top

Ruby: File.size("a.txt")
来源：http://jnc.ydzc1.top

C#:   new FileInfo("a.txt").Length
来源：http://ztp.andypj.xyz

[F10] 取文件扩展名 / 文件名
来源：http://fad.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://olm.svipenyu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xzj.daria6918.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rdy.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://tea.yj20258888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xjw.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gfv.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jvm.zhaomingkeji.xyz

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eur.mhx1999.top

[F11] 复制与移动文件
来源：http://rml.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://scs.cheryme.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xpa.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qnr.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xqw.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gij.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vtu.yj20258888.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rml.fktsv.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kzz.sweek.top

[F12] CSV 读写
来源：http://met.jinyuanbaomall.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qtd.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bsb.kuanghao11.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ihe.shzxlz.cn

TS:   // 同上
来源：http://owx.cqqwz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zky.nanxinkj.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qjl.hongshengwenyu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mtb.zhixingplan.top

C#:   // 无内置：用 CsvHelper 库
来源：http://wvg.yuanzhike.top

================================================================================
来源：http://ekc.gogol.net.cn

G. 面向对象
来源：http://bns.hnxiangtu.top

================================================================================
来源：http://nuc.fanxiaobao.xyz

[G01] 定义类
来源：http://psm.gogol.net.cn

Py:   class User: pass
来源：http://xfp.snrcjt.cn

PHP:  class User {}
来源：http://ljh.zhoulong.xyz

JS:   class User {}
来源：http://xme.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://bje.vqdsnc.cn

Java: class User {}
来源：http://mvo.sweek.top

Go:   type User struct { Name string }
来源：http://tbv.yangfankeji.com

Ruby: class User; end
来源：http://zjn.guowangkeji.top

C#:   class User {}
来源：http://ndp.yj20258888.top

[G02] 构造函数
来源：http://ise.tanke756.top

Py:   def __init__(self, name): self.name = name
来源：http://ryz.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://ggd.snrcjt.cn

JS:   constructor(name) { this.name = name; }
来源：http://xxl.tanke756.top

TS:   constructor(public name: string) {}
来源：http://fru.vehdjk.com

Java: User(String name) { this.name = name; }
来源：http://uvq.smart0.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://kwe.bjfxy.top

Ruby: def initialize(name); @name = name; end
来源：http://vey.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://bbu.feifeiyinyue.top

[G03] 实例属性
来源：http://tha.zdbjq.cn

Py:   self.name = "x"
来源：http://xte.pycfn.com

PHP:  public string $name = "x";
来源：http://pde.zhoulong.xyz

JS:   this.name = "x";
来源：http://jlb.dashuyun.cn

TS:   name: string = "x";
来源：http://jbx.zdqjudy.top

Java: private String name;
来源：http://uqh.sysykeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://icg.shuidangran.top

Ruby: @name = "x"
来源：http://ipt.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://vsf.jinqigufen.top

[G04] 定义方法
来源：http://guf.shzxlz.cn

Py:   def greet(self): return self.name
来源：http://abt.zdqjudy.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xbs.yj20258888.top

JS:   greet() { return this.name; }
来源：http://udn.pengpengdd.cyou

TS:   greet(): string { return this.name; }
来源：http://dak.9152youxi.cn

Java: String greet() { return name; }
来源：http://jhi.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vmb.yongpay.top

Ruby: def greet; @name; end
来源：http://civ.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://lgt.meibo888.top

[G05] 继承
来源：http://fgi.0kj1m.cn

Py:   class Admin(User): pass
来源：http://nmc.bbcook.cn

PHP:  class Admin extends User {}
来源：http://mph.hysaishi.cn

JS:   class Admin extends User {}
来源：http://fum.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://fnu.epnwcf.com

Java: class Admin extends User {}
来源：http://rwo.aizwys.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hcf.hywenlv.cn

Ruby: class Admin < User; end
来源：http://qwr.hfpthk.cn

C#:   class Admin : User {}
来源：http://dir.yj20258888.top

[G06] 重写方法
来源：http://uzs.0kj1m.cn

Py:   def greet(self): return "admin"
来源：http://lhi.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://yyy.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://pkp.andypj.xyz

TS:   greet(): string { return "admin"; }
来源：http://lai.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://ccn.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://npd.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://txn.fzhhl.top

C#:   public override string Greet() => "admin";
来源：http://ntp.zdqjudy.top

[G07] 调用父类方法
来源：http://mrs.cdnleiting.top

Py:   super().greet()
来源：http://zil.iojbl.cn

PHP:  parent::greet();
来源：http://tip.xinyue.icu

JS:   super.greet();
来源：http://wxu.zhiwuduotai.top

TS:   super.greet();
来源：http://ezx.52xcode.cn

Java: super.greet();
来源：http://btv.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aez.zhengqikj.top

Ruby: super
来源：http://gkx.daxiang520.top

C#:   base.Greet();
来源：http://gzt.sysykeji.top

[G08] 静态方法与属性
来源：http://tlb.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://prx.haohaochexian.top

PHP:  public static function f() {}
来源：http://jnn.zhongyouzk.top

JS:   static f() {}
来源：http://ofp.nanxuanxn.top

TS:   static f(): void {}
来源：http://cii.fanxiaobao.xyz

Java: static void f() {}
来源：http://ems.quarkkingdee.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ivm.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://qvt.fktsv.cn

C#:   public static void F() {}
来源：http://fhv.hnqzz.top

[G09] 接口 / 抽象类
来源：http://dxb.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://ouj.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vhd.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://prf.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://zzo.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://inr.feifeiyinyue.top

Go:   type Shape interface { Area() float64 }
来源：http://zmr.yuxming.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://joc.xingfuxueyuan.xyz

C#:   interface IShape { double Area(); }
来源：http://azs.uphjek.com

[G10] 访问控制
来源：http://azn.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://uvk.hfpthk.cn

PHP:  public / protected / private
来源：http://vjt.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://drt.xuetiantiany.cn

TS:   public / protected / private
来源：http://vde.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://kwm.pycfn.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://yuo.yueranfly.top

Ruby: public / protected / private
来源：http://ngm.daxiang520.top

C#:   public / protected / private / internal
来源：http://blw.gogol.net.cn

[G11] getter / setter
来源：http://oto.xuanzx.com

Py:   @property 与 @x.setter
来源：http://qxt.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dgi.gaohongyu789.top

JS:   get name() { return this._name; }
来源：http://rbe.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://wdb.bjfxy.top

Java: public String getName() { return name; }
来源：http://lpg.9152youxi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xkf.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://rwf.jinghuilouyu.cn

C#:   public string Name { get; set; }
来源：http://ant.yj20258.top

[G12] 对象转字符串
来源：http://xkz.redwolf501.top

Py:   def __str__(self): return self.name
来源：http://vvn.hfpthk.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ihh.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://owi.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://hfi.hcnkem.com

Java: @Override public String toString() { return name; }
来源：http://xdi.yfazqb.com


<!-- 参考信息 -->