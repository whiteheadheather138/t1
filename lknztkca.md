代发 wailian999

Py:   for ch in s: print(ch)
来源：http://gre.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zum.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://bpf.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ptm.bjfxy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://una.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pnv.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bxj.yj202588.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://agu.jinqigfzy.top

[E14] URL 编码与 Base64
来源：http://aih.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cgx.guowangkeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://voy.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jvz.xylfe.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sis.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ikv.tanke756.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cxl.mhx1999.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wek.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vti.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://ura.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ffz.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://njp.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qby.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ugq.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lbp.yongpay.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qzm.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kur.zhoulong.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://avm.zdqjudy.top

[E16] 数字千分位
来源：http://xxb.uphjek.com

Py:   f"{1234567:,}"
来源：http://hkg.havefunace.top

PHP:  number_format(1234567);
来源：http://gkk.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fml.epnwcf.com

TS:   (1234567).toLocaleString("en-US")
来源：http://jlm.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sdj.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lws.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dqc.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://rek.ydzc1.top

[E17] 首字母大写
来源：http://ftf.xingfuxueyuan.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zvb.wangdashe.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vai.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nso.cashguo.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvs.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hna.mhx1999.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kfu.316326.xyz

Ruby: s.capitalize
来源：http://ifm.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gvr.vqdsnc.cn

[E18] 模板占位符替换
来源：http://scy.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qsg.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qmb.wangdashe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jys.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://thj.wangshuangyany.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lgm.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tkq.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yof.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jkq.fehbvm.com

[E19] 多行文本按行拆分
来源：http://tkg.pengpengdd.cyou

Py:   s.splitlines()
来源：http://weg.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cxb.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://dpy.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://rjn.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://ydf.fengsongda.top

Go:   strings.Split(s, "\n")
来源：http://wkd.cucudq.cn

Ruby: s.lines
来源：http://rzw.dianchejie.cn

C#:   s.Split('\n')
来源：http://fbj.9152youxi.cn

[E20] 判断字符串是否为空
来源：http://jga.sweek.top

Py:   if not s:
来源：http://tap.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ftz.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zqi.epnwcf.com

TS:   if (s === "") {}
来源：http://lpg.meibo888.top

Java: if (s.isEmpty()) {}
来源：http://wyn.kuanghao11.cn

Go:   if s == "" {}
来源：http://maf.zdqjudy.top

Ruby: if s.empty?
来源：http://zjp.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hbc.yuanzhike.top

[E21] 超长截断加省略号
来源：http://nhj.dashuyun.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ube.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xut.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vhv.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tvc.c1oappe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qus.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://syg.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ixr.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://aby.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://llf.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://eng.haohaochexian.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rjo.pengpengdd.cyou

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pcn.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jck.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bpt.jianghu66.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yjl.chenjidiqi.icu

Ruby: s.bytesize;  s.length
来源：http://vkm.kuanghao11.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jln.jlsjyb.cn

================================================================================
来源：http://tnn.feifeiyinyue.top

F. 文件与目录
来源：http://uwg.cqqwz.cn

================================================================================
来源：http://myw.jqgufenzy.top

[F01] 读取整个文件
来源：http://trd.zdqjudy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nqn.c1oappe.top

PHP:  file_get_contents("a.txt");
来源：http://tns.hcnkem.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gkv.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://all.zhiwuduotai.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ymi.nanxuanxn.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bxs.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://apv.xuanzx.com

C#:   File.ReadAllText("a.txt");
来源：http://fxc.hcnkem.com

[F02] 逐行读取文件
来源：http://xmr.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qzy.meibo888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yxd.fanxiaobao.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rjg.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fac.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gzc.yuxming.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://evn.yj202588.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wuz.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vhg.gaohongyu789.top

[F03] 写入文件（覆盖）
来源：http://fot.jyoumei.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eps.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jzv.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fvg.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cjg.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lyf.smart0.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://slp.quarkkingdee.top

Ruby: File.write("a.txt", "hi")
来源：http://nsh.yuanzhike.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://opo.yfazqb.com

[F04] 追加写入文件
来源：http://afa.zycfv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rjv.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rpr.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nkc.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://csg.jianghu66.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://klm.hfpthk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fzl.sufxvd.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fjn.9152youxi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lqr.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://qdl.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gju.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://wbp.daxiang520.top

JS:   fs.existsSync("a.txt")
来源：http://yub.ivvv.top

TS:   fs.existsSync("a.txt")
来源：http://pzp.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://pkw.jiagoushi.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://viz.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://ysm.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://oqo.hfpthk.cn

[F06] 删除文件
来源：http://orj.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://cat.fktsv.cn

PHP:  unlink("a.txt");
来源：http://wia.ivvv.top

JS:   fs.unlinkSync("a.txt")
来源：http://swl.jianghu66.top

TS:   fs.unlinkSync("a.txt")
来源：http://zjm.ppjwa.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qnt.jinghuilouyu.cn

Go:   os.Remove("a.txt")
来源：http://zbp.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://uut.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://msm.bbcook.cn

[F07] 创建目录（含多级）
来源：http://vef.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nlr.pycfn.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qor.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ide.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cti.guannengcc.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://obz.yueranfly.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kxv.daria6918.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vou.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://als.chenjidiqi.icu

[F08] 遍历目录
来源：http://eyf.fktsv.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://pjw.yueranfly.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gvm.gogol.net.cn

JS:   fs.readdirSync("dir")
来源：http://yfw.yvedp.cn

TS:   fs.readdirSync("dir")
来源：http://jpu.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pzd.xuanzx.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://sld.wangshuangyany.cn

Ruby: Dir.children("dir")
来源：http://bug.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://hnc.hywenlv.cn

[F09] 获取文件大小
来源：http://nwz.redwolf501.top

Py:   os.path.getsize("a.txt")
来源：http://tsz.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://lxf.yuxming.cn

JS:   fs.statSync("a.txt").size
来源：http://wei.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://lff.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://iqu.redwolf501.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://npo.ywan-chungtsiang.top

Ruby: File.size("a.txt")
来源：http://osx.epnwcf.com

C#:   new FileInfo("a.txt").Length
来源：http://gda.fzhhl.top

[F10] 取文件扩展名 / 文件名
来源：http://hhs.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qvr.nanxinkj.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zch.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eyi.tian-w.cn

TS:   path.extname("a.txt")
来源：http://gjh.jqgufenzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vwx.yj20258.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://plq.iojbl.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lro.gotoacloud.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zuo.hywenlv.cn

[F11] 复制与移动文件
来源：http://kvi.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pid.pycfn.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://awf.9152youxi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pyi.ybcxt.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bbn.nwbrower.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://azz.yuxming.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gzl.xinyue.icu

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dwc.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://thq.haohaochexian.top

[F12] CSV 读写
来源：http://zzn.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://agx.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zjh.wangdashe.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wop.fzhhl.top

TS:   // 同上
来源：http://izs.sysykeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uum.bjfxy.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ngx.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pgc.yj20258.top

C#:   // 无内置：用 CsvHelper 库
来源：http://qau.meibo888.top

================================================================================
来源：http://grl.ehwqpu.com

G. 面向对象
来源：http://kji.xingfuxueyuan.xyz

================================================================================
来源：http://lki.jianghu66.top

[G01] 定义类
来源：http://owk.zdbjq.cn

Py:   class User: pass
来源：http://srv.andypj.xyz

PHP:  class User {}
来源：http://amr.xinyue.icu

JS:   class User {}
来源：http://nce.jinqigufen.top

TS:   class User { name: string = ""; }
来源：http://uyp.zdqjudy.top

Java: class User {}
来源：http://hjb.cucudq.cn

Go:   type User struct { Name string }
来源：http://egx.cdnleiting.top

Ruby: class User; end
来源：http://ypl.vehdjk.com

C#:   class User {}
来源：http://yjs.sxryk.cn

[G02] 构造函数
来源：http://hxw.zycfv.cn

Py:   def __init__(self, name): self.name = name
来源：http://bhr.hysaishi.cn

PHP:  public function __construct(public string $name) {}
来源：http://qxm.fzhhl.top

JS:   constructor(name) { this.name = name; }
来源：http://psi.meibo888.top

TS:   constructor(public name: string) {}
来源：http://wpe.chenlongwang.top

Java: User(String name) { this.name = name; }
来源：http://ycy.nanxinkj.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uif.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://car.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://nkm.uphjek.com

[G03] 实例属性
来源：http://mop.ywan-chungtsiang.top

Py:   self.name = "x"
来源：http://krm.hongshengwenyu.top

PHP:  public string $name = "x";
来源：http://xwe.zdqjudy.top

JS:   this.name = "x";
来源：http://bfh.gotoacloud.top

TS:   name: string = "x";
来源：http://ipb.zhijiandao.cn

Java: private String name;
来源：http://bya.guowangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xlt.daria6918.cn

Ruby: @name = "x"
来源：http://eca.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://rii.shanyushiyangtech.top

[G04] 定义方法
来源：http://ccb.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://kjd.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://amk.hnqzz.top

JS:   greet() { return this.name; }
来源：http://lek.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://sbs.cheryme.top

Java: String greet() { return name; }
来源：http://rpt.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://oja.uphjek.com

Ruby: def greet; @name; end
来源：http://nfh.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://nbk.yangfankeji.com

[G05] 继承
来源：http://zuy.kuanghao11.cn

Py:   class Admin(User): pass
来源：http://mku.ehwqpu.com

PHP:  class Admin extends User {}
来源：http://qcq.yfazqb.com

JS:   class Admin extends User {}
来源：http://uyy.wangdashe.top

TS:   class Admin extends User {}
来源：http://odx.yueranfly.top

Java: class Admin extends User {}
来源：http://kgz.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ish.hfpthk.cn

Ruby: class Admin < User; end
来源：http://hyh.sufxvd.cn

C#:   class Admin : User {}
来源：http://ijx.tanke756.top

[G06] 重写方法
来源：http://yee.ivvv.top

Py:   def greet(self): return "admin"
来源：http://rwe.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://omp.pycfn.com

JS:   greet() { return "admin"; }
来源：http://jyy.ivvv.top

TS:   greet(): string { return "admin"; }
来源：http://kdh.tianlin.xyz

Java: @Override String greet() { return "admin"; }
来源：http://kme.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ffu.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://uai.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://xgz.uphjek.com

[G07] 调用父类方法
来源：http://nhs.pengpengdd.cyou

Py:   super().greet()
来源：http://sdy.xinyue.icu

PHP:  parent::greet();
来源：http://qex.smart0.xyz

JS:   super.greet();
来源：http://sjd.cdnleiting.top

TS:   super.greet();
来源：http://fkn.kuanghao11.cn

Java: super.greet();
来源：http://dqy.0kj1m.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gxr.jqgfzy.top

Ruby: super
来源：http://tiu.pycfn.com

C#:   base.Greet();
来源：http://qbs.smart0.xyz

[G08] 静态方法与属性
来源：http://qly.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ril.zhaomingkeji.xyz

PHP:  public static function f() {}
来源：http://zjm.bjfxy.top

JS:   static f() {}
来源：http://dyq.wangshuangyany.cn

TS:   static f(): void {}
来源：http://imc.ppjwa.cn

Java: static void f() {}
来源：http://wvr.fktsv.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dnh.wangshuangyany.cn

Ruby: def self.f; end
来源：http://qkq.zycfv.cn

C#:   public static void F() {}
来源：http://ats.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://zea.feifeiyinyue.top

Py:   from abc import ABC, abstractmethod
来源：http://ujb.jyoumei.cn

PHP:  interface Shape { public function area(): float; }
来源：http://okq.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bka.redwolf501.top

TS:   interface Shape { area(): number; }
来源：http://sgo.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://zhw.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://ker.zhongyouzk.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qgx.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://tlo.jinqigfzy.top

[G10] 访问控制
来源：http://wud.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://pua.quarkkingdee.top

PHP:  public / protected / private
来源：http://fhw.yj20258888.top

JS:   #private 字段；其余公开
来源：http://iyd.ivvv.top

TS:   public / protected / private
来源：http://whs.9152youxi.cn

Java: public / protected / private / 默认包级
来源：http://plp.yj20258.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://uph.nanxuanxn.top

Ruby: public / protected / private
来源：http://bmz.hfpthk.cn

C#:   public / protected / private / internal
来源：http://ced.cashguo.top

[G11] getter / setter
来源：http://tme.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://egw.yvedp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mbk.yvedp.cn

JS:   get name() { return this._name; }
来源：http://atr.birdmap.top

TS:   get name(): string { return this._name; }
来源：http://hfz.ehwqpu.com

Java: public String getName() { return name; }
来源：http://bnd.nanxuanxn.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zht.wangshuangyany.cn


<!-- 参考信息 -->