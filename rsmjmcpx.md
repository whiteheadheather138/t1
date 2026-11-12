代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fbm.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wms.hnqzz.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bvy.fzhhl.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pxw.jyoumei.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rte.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://kdf.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hia.feifeiyinyue.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oyj.jinqigufen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fet.aizwys.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fzj.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mmi.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xzp.uphjek.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gnn.chenzaomai.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://doy.daxiang520.top

[E16] 数字千分位
来源：http://efw.xylfe.cn

Py:   f"{1234567:,}"
来源：http://pgs.hammf.cn

PHP:  number_format(1234567);
来源：http://qqo.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nic.iojbl.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ogc.yangfankeji.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://trp.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ssv.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://azc.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://igw.jinqigfzy.top

[E17] 首字母大写
来源：http://xjg.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://upt.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nko.xuanzx.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbw.snrcjt.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zyk.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pev.cqqwz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bcv.316326.xyz

Ruby: s.capitalize
来源：http://gtq.zhixingplan.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nnf.xuanzx.com

[E18] 模板占位符替换
来源：http://hdd.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ozo.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sqv.fengsongda.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xib.hnqzz.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dap.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cns.cashguo.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qoi.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mnl.ivvv.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wkt.ydzc1.top

[E19] 多行文本按行拆分
来源：http://nqw.smart0.xyz

Py:   s.splitlines()
来源：http://gtv.vqdsnc.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kjx.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://grz.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://dxq.shanyushiyangkeji.top

Java: s.lines().toList()
来源：http://csx.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://ufi.hysaishi.cn

Ruby: s.lines
来源：http://szr.epnwcf.com

C#:   s.Split('\n')
来源：http://sdc.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://mkq.yvedp.cn

Py:   if not s:
来源：http://gnu.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hiv.jqgfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eow.bjfxy.top

TS:   if (s === "") {}
来源：http://vwk.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://ygd.fehbvm.com

Go:   if s == "" {}
来源：http://guu.ydjk.org.cn

Ruby: if s.empty?
来源：http://nim.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cpb.yangfankeji.com

[E21] 超长截断加省略号
来源：http://owr.ppjwa.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://epm.chenjidiqi.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ytv.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://byz.nwbrower.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://niv.gotoacloud.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ate.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://ooh.fzhhl.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rix.aibaodan.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wxr.zycfv.cn

[E22] 字节长度与字符长度
来源：http://qbq.hammf.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://loj.vehdjk.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sum.hesvh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://obc.xinyue.icu

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qjk.vqdsnc.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tll.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ann.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://bfj.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nbq.hesvh.cn

================================================================================
来源：http://svr.fehbvm.com

F. 文件与目录
来源：http://cok.pycfn.com

================================================================================
来源：http://hir.vqdsnc.cn

[F01] 读取整个文件
来源：http://vox.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dok.vqdsnc.cn

PHP:  file_get_contents("a.txt");
来源：http://pib.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://csd.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mmp.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xvg.jlsjyb.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xkr.c1oappe.top

Ruby: File.read("a.txt")
来源：http://sgg.yangfankeji.com

C#:   File.ReadAllText("a.txt");
来源：http://xcs.daria6918.cn

[F02] 逐行读取文件
来源：http://qqp.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://plm.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lto.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lht.c1oappe.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rhp.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lye.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oht.xuetiantiany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vgs.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lmf.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://ffu.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jtz.nanxinkj.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://bka.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ovu.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dgl.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mem.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://szk.shangyingyoupin.top

Ruby: File.write("a.txt", "hi")
来源：http://oqt.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pkr.yonumen.top

[F04] 追加写入文件
来源：http://spn.uphjek.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lxr.ydjk.org.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://guv.redwolf501.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://voz.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ogv.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gyz.bbcook.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kwk.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vmc.hcnkem.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://azr.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://dqn.hesvh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jdb.cashguo.top

PHP:  file_exists("a.txt");
来源：http://gfq.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://obe.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://lak.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://acq.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pzk.nwbrower.top

Ruby: File.exist?("a.txt")
来源：http://dqk.yangfankeji.com

C#:   File.Exists("a.txt")
来源：http://tpm.zdbjq.cn

[F06] 删除文件
来源：http://uyx.bbcook.cn

Py:   os.remove("a.txt")
来源：http://iiy.yj202588.top

PHP:  unlink("a.txt");
来源：http://uyj.uphjek.com

JS:   fs.unlinkSync("a.txt")
来源：http://fmk.nanxinkj.top

TS:   fs.unlinkSync("a.txt")
来源：http://xyk.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rmb.fktsv.cn

Go:   os.Remove("a.txt")
来源：http://ddh.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://tvw.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://lvq.hcnkem.com

[F07] 创建目录（含多级）
来源：http://rpy.fanxiaobao.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fvg.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rel.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aam.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ilx.gotoacloud.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://skg.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uxq.jianghu66.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ssx.daria6918.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kci.shanyushiyangtech.top

[F08] 遍历目录
来源：http://sua.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sls.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fei.yvedp.cn

JS:   fs.readdirSync("dir")
来源：http://mjh.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://hyh.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nop.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://eqb.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://zzz.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://nmf.hfpthk.cn

[F09] 获取文件大小
来源：http://wlk.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://qoq.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://shk.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://iqx.xuanzx.com

TS:   fs.statSync("a.txt").size
来源：http://liz.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://huj.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://awf.mhx1999.top

Ruby: File.size("a.txt")
来源：http://lpb.zhengqikj.top

C#:   new FileInfo("a.txt").Length
来源：http://uvt.c1oappe.top

[F10] 取文件扩展名 / 文件名
来源：http://afz.hongshengwenyu.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ybz.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nvx.jinghuilouyu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vsi.sufxvd.cn

TS:   path.extname("a.txt")
来源：http://ree.jiagoushi.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uql.zdqjudy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pzn.pycfn.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xtc.xuanzx.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kll.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://ray.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://avv.nanxinkj.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mvw.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wgq.chenjidiqi.icu

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohy.ydzc1.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://axd.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oss.nanxinkj.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vzp.snrcjt.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://srq.pengpengdd.cyou

[F12] CSV 读写
来源：http://mkw.fengsongda.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pnr.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://obf.zhaomingkeji.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zpj.zhaomingkeji.xyz

TS:   // 同上
来源：http://ujg.cdnleiting.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://usl.epnwcf.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cqd.pycfn.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://iyw.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fyq.yangfankeji.com

================================================================================
来源：http://qvb.birdmap.top

G. 面向对象
来源：http://fuy.yongpay.top

================================================================================
来源：http://aeu.gogol.net.cn

[G01] 定义类
来源：http://bgl.shuidangran.top

Py:   class User: pass
来源：http://yyi.zycfv.cn

PHP:  class User {}
来源：http://hqg.xziqi.cn

JS:   class User {}
来源：http://zpw.hnqzz.top

TS:   class User { name: string = ""; }
来源：http://iuk.zhiwuduotai.top

Java: class User {}
来源：http://fzv.chenjidiqi.icu

Go:   type User struct { Name string }
来源：http://gto.ivvv.top

Ruby: class User; end
来源：http://ypm.yanxiufei.cn

C#:   class User {}
来源：http://tjs.zhengqikj.top

[G02] 构造函数
来源：http://sch.fehbvm.com

Py:   def __init__(self, name): self.name = name
来源：http://elm.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://lez.yanxiufei.cn

JS:   constructor(name) { this.name = name; }
来源：http://ivb.zhongyouzk.top

TS:   constructor(public name: string) {}
来源：http://sfs.hfpthk.cn

Java: User(String name) { this.name = name; }
来源：http://ckp.sufxvd.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vcr.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://lfu.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://ulz.zhiwuduotai.top

[G03] 实例属性
来源：http://hwb.zdbjq.cn

Py:   self.name = "x"
来源：http://giy.redwolf501.top

PHP:  public string $name = "x";
来源：http://yvt.cdnleiting.top

JS:   this.name = "x";
来源：http://srg.shangyingyoupin.top

TS:   name: string = "x";
来源：http://rsk.yfazqb.com

Java: private String name;
来源：http://lae.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ymh.yangfankeji.com

Ruby: @name = "x"
来源：http://nbp.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://qap.kuanghao11.cn

[G04] 定义方法
来源：http://sjt.ydzc1.top

Py:   def greet(self): return self.name
来源：http://why.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://mza.tanke756.top

JS:   greet() { return this.name; }
来源：http://zlk.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://mlw.shanyushiyangkeji.top

Java: String greet() { return name; }
来源：http://mol.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://qvw.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://jzb.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://szx.shanyushiyangtech.top

[G05] 继承
来源：http://iot.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://wru.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://fcd.hysaishi.cn

JS:   class Admin extends User {}
来源：http://ctx.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://vml.andypj.xyz

Java: class Admin extends User {}
来源：http://asl.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mln.hesvh.cn

Ruby: class Admin < User; end
来源：http://zpb.hammf.cn

C#:   class Admin : User {}
来源：http://iwh.havefunace.top

[G06] 重写方法
来源：http://ukj.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://ocf.wangshuangyany.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ykm.tianlin.xyz

JS:   greet() { return "admin"; }
来源：http://dpu.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://mxp.zhengqikj.top

Java: @Override String greet() { return "admin"; }
来源：http://pke.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wiu.jinqigfzy.top

Ruby: def greet; "admin"; end
来源：http://oae.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://wrk.vqdsnc.cn

[G07] 调用父类方法
来源：http://fes.jinqigufen.top

Py:   super().greet()
来源：http://wvp.gaohongyu789.top

PHP:  parent::greet();
来源：http://tbz.xuanzx.com

JS:   super.greet();
来源：http://oft.hfpthk.cn

TS:   super.greet();
来源：http://sos.ydzc1.top

Java: super.greet();
来源：http://xjm.shuidangran.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mux.vehdjk.com

Ruby: super
来源：http://trg.hongshengwenyu.top

C#:   base.Greet();
来源：http://atf.zhaomingkeji.xyz

[G08] 静态方法与属性
来源：http://eik.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yqx.yj202588.top

PHP:  public static function f() {}
来源：http://nvr.tanke756.top

JS:   static f() {}
来源：http://pak.jianghu66.top

TS:   static f(): void {}
来源：http://vik.fzhhl.top

Java: static void f() {}
来源：http://gfs.jinqigufen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ulr.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://xlg.jianghu66.top

C#:   public static void F() {}
来源：http://est.sufxvd.cn

[G09] 接口 / 抽象类
来源：http://ovh.yvedp.cn

Py:   from abc import ABC, abstractmethod
来源：http://qzt.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://zpk.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pcu.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://lbm.havefunace.top

Java: interface Shape { double area(); }
来源：http://xby.jinghuilouyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://sqz.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ovw.epnwcf.com

C#:   interface IShape { double Area(); }
来源：http://pse.xziqi.cn

[G10] 访问控制
来源：http://nhn.jinghuilouyu.cn

Py:   约定 _protected / __private（不强制）
来源：http://bbk.xziqi.cn

PHP:  public / protected / private
来源：http://opr.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://arb.snrcjt.cn

TS:   public / protected / private
来源：http://yvk.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://tgp.xuanzx.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://pba.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://qiv.jinqigfzy.top

C#:   public / protected / private / internal
来源：http://znt.hesvh.cn

[G11] getter / setter
来源：http://olq.quarkkingdee.top

Py:   @property 与 @x.setter
来源：http://hgw.meibo888.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qyp.bjfxy.top

JS:   get name() { return this._name; }
来源：http://jks.gzhubu.top

TS:   get name(): string { return this._name; }
来源：http://jgk.cdnleiting.top

Java: public String getName() { return name; }
来源：http://foj.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hgk.fehbvm.com

Ruby: attr_accessor :name
来源：http://uib.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://dmh.fktsv.cn

[G12] 对象转字符串
来源：http://atv.xziqi.cn

Py:   def __str__(self): return self.name
来源：http://rsc.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uam.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://qdi.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://sye.tian-w.cn

Java: @Override public String toString() { return name; }
来源：http://duz.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kem.316326.xyz

Ruby: def to_s; @name; end
来源：http://eti.shanyushiyangkeji.top

C#:   public override string ToString() => Name;
来源：http://uyy.xylfe.cn

[G13] 判断对象类型
来源：http://mff.shangyingyoupin.top


<!-- 参考信息 -->