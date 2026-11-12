代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tfy.jinyuanbaomall.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jtw.hesvh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tks.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wqr.fzhhl.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fju.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://hpw.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oxj.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wzp.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://llm.zhijiandao.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rlq.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cka.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rxu.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ibc.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hwc.uphjek.com

[E16] 数字千分位
来源：http://xvr.smart0.xyz

Py:   f"{1234567:,}"
来源：http://gqo.yueranfly.top

PHP:  number_format(1234567);
来源：http://rjw.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ikx.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gnw.jyoumei.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://djz.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iiw.c1oappe.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://brc.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://xku.sxryk.cn

[E17] 首字母大写
来源：http://sck.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sho.guannengcc.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vmp.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmz.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qkv.mhx1999.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jpp.yuanzhike.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://liz.yj20258888.top

Ruby: s.capitalize
来源：http://ddr.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ybn.gaohongyu789.top

[E18] 模板占位符替换
来源：http://hja.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nef.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pha.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kys.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ane.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nsn.kuanghao11.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sjy.bbcook.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yaq.9152youxi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zfl.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://mnq.yvedp.cn

Py:   s.splitlines()
来源：http://lyh.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://axk.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://mmi.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://xct.uphjek.com

Java: s.lines().toList()
来源：http://ocz.yanxiufei.cn

Go:   strings.Split(s, "\n")
来源：http://tbo.gzhubu.top

Ruby: s.lines
来源：http://myf.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://rst.mhx1999.top

[E20] 判断字符串是否为空
来源：http://jxs.sysykeji.top

Py:   if not s:
来源：http://ywt.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cgu.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://exi.pycfn.com

TS:   if (s === "") {}
来源：http://bfy.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://ujy.iojbl.cn

Go:   if s == "" {}
来源：http://gud.jinqigufen.top

Ruby: if s.empty?
来源：http://wgb.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://crr.gotoacloud.top

[E21] 超长截断加省略号
来源：http://htb.zhaomingkeji.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://udj.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://amj.haohaochexian.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lpu.yangfankeji.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jut.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ivx.pycfn.com

Go:   // 按 rune 判断长度后截断
来源：http://ukf.yanxiufei.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bvk.mhx1999.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rom.guannengcc.top

[E22] 字节长度与字符长度
来源：http://mtg.vqdsnc.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dmu.ehwqpu.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://thw.hysaishi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gvj.shuidangran.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zai.ivvv.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uyh.guannengcc.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fec.tian-w.cn

Ruby: s.bytesize;  s.length
来源：http://ntu.xziqi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://aup.yj20258888.top

================================================================================
来源：http://qbq.xinyue.icu

F. 文件与目录
来源：http://uuz.nanxinkj.top

================================================================================
来源：http://wiy.shangyingyoupin.top

[F01] 读取整个文件
来源：http://gry.jlsjyb.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dwe.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://zxh.hongshengwenyu.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uzv.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tvu.jlsjyb.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jju.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rba.haohaochexian.top

Ruby: File.read("a.txt")
来源：http://jni.gzhubu.top

C#:   File.ReadAllText("a.txt");
来源：http://lio.nwbrower.top

[F02] 逐行读取文件
来源：http://hcd.zhijiandao.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nzx.xylfe.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aju.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kno.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dvf.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fpt.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wzt.guowangkeji.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fzv.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ous.kuanghao11.cn

[F03] 写入文件（覆盖）
来源：http://lab.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hnm.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://eql.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://apj.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iiq.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rty.gotoacloud.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hjt.shzxlz.cn

Ruby: File.write("a.txt", "hi")
来源：http://vzc.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://amt.yj20258.top

[F04] 追加写入文件
来源：http://odu.zhiwuduotai.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oqm.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cos.tarul.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hcj.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wfg.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://iiv.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wxc.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dan.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wxg.hnxiangtu.top

[F05] 判断文件或目录是否存在
来源：http://fbp.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://axl.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://pwx.meibo888.top

JS:   fs.existsSync("a.txt")
来源：http://ulf.pycfn.com

TS:   fs.existsSync("a.txt")
来源：http://frh.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tup.yanxiufei.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zqm.316326.xyz

Ruby: File.exist?("a.txt")
来源：http://hzi.sjlbkw.cn

C#:   File.Exists("a.txt")
来源：http://dhd.nanxuanxn.top

[F06] 删除文件
来源：http://ppn.aizwys.cn

Py:   os.remove("a.txt")
来源：http://biy.hysaishi.cn

PHP:  unlink("a.txt");
来源：http://hhw.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://rrj.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://cza.nanxuanxn.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mwn.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://ekm.ywan-chungtsiang.top

Ruby: File.delete("a.txt")
来源：http://kxw.gogol.net.cn

C#:   File.Delete("a.txt");
来源：http://ujk.tanke756.top

[F07] 创建目录（含多级）
来源：http://qhw.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xkm.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bpc.dashuyun.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://myo.xylfe.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://brb.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qlc.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aan.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ndq.52xcode.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pso.yanxiufei.cn

[F08] 遍历目录
来源：http://wba.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://ajx.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://khm.andypj.xyz

JS:   fs.readdirSync("dir")
来源：http://uqz.52xcode.cn

TS:   fs.readdirSync("dir")
来源：http://tuc.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oge.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mhb.316326.xyz

Ruby: Dir.children("dir")
来源：http://fow.yvedp.cn

C#:   Directory.GetFiles("dir")
来源：http://poa.nwbrower.top

[F09] 获取文件大小
来源：http://nsf.ydzc1.top

Py:   os.path.getsize("a.txt")
来源：http://hcn.svipenyu.cn

PHP:  filesize("a.txt");
来源：http://lgz.zhaomingkeji.xyz

JS:   fs.statSync("a.txt").size
来源：http://ssx.yueranfly.top

TS:   fs.statSync("a.txt").size
来源：http://fqw.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://fwi.0kj1m.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sdy.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://lcz.xingfuxueyuan.xyz

C#:   new FileInfo("a.txt").Length
来源：http://zau.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://tzy.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ftb.jlsjyb.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ktf.ehwqpu.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gfa.guannengcc.top

TS:   path.extname("a.txt")
来源：http://wrj.hywenlv.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pvc.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://srb.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wko.birdmap.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cmx.c1oappe.top

[F11] 复制与移动文件
来源：http://syv.shuidangran.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xha.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wae.bbcook.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://riy.xuetiantiany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mxe.wangdashe.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zwe.kuanghao11.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://azd.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ody.sysykeji.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://whx.bbcook.cn

[F12] CSV 读写
来源：http://mkk.zhongyouzk.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://udq.chenjidiqi.icu

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tjs.zhijiandao.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://suz.zhijiandao.cn

TS:   // 同上
来源：http://pae.zycfv.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uzr.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://weq.xylfe.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oet.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://weg.smart0.xyz

================================================================================
来源：http://tns.ydjk.org.cn

G. 面向对象
来源：http://jvr.52xcode.cn

================================================================================
来源：http://afz.yj20258.top

[G01] 定义类
来源：http://dap.aibaodan.cn

Py:   class User: pass
来源：http://cmy.yj202588.top

PHP:  class User {}
来源：http://mdz.hammf.cn

JS:   class User {}
来源：http://ppd.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://smr.ehwqpu.com

Java: class User {}
来源：http://pzm.ybcxt.top

Go:   type User struct { Name string }
来源：http://gih.gzhubu.top

Ruby: class User; end
来源：http://whf.epnwcf.com

C#:   class User {}
来源：http://pju.jiagoushi.top

[G02] 构造函数
来源：http://ycw.ywan-chungtsiang.top

Py:   def __init__(self, name): self.name = name
来源：http://hdu.52xcode.cn

PHP:  public function __construct(public string $name) {}
来源：http://zgz.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://lzr.sysykeji.top

TS:   constructor(public name: string) {}
来源：http://qjc.ywan-chungtsiang.top

Java: User(String name) { this.name = name; }
来源：http://gem.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uio.zycfv.cn

Ruby: def initialize(name); @name = name; end
来源：http://ogd.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://chi.yuanzhike.top

[G03] 实例属性
来源：http://kxt.daxiang520.top

Py:   self.name = "x"
来源：http://ftx.daxiang520.top

PHP:  public string $name = "x";
来源：http://rqi.xingfuxueyuan.xyz

JS:   this.name = "x";
来源：http://eay.redwolf501.top

TS:   name: string = "x";
来源：http://vje.ctjpmb.com

Java: private String name;
来源：http://dyb.pengpengdd.cyou

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ogt.gogol.net.cn

Ruby: @name = "x"
来源：http://lal.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://ppu.yvedp.cn

[G04] 定义方法
来源：http://dxm.zycfv.cn

Py:   def greet(self): return self.name
来源：http://tiu.c1oappe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lhs.cashguo.top

JS:   greet() { return this.name; }
来源：http://zxz.gzhubu.top

TS:   greet(): string { return this.name; }
来源：http://uoq.birdmap.top

Java: String greet() { return name; }
来源：http://fli.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://kkm.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://blp.yfazqb.com

C#:   public string Greet() => Name;
来源：http://lhm.yangfankeji.com

[G05] 继承
来源：http://ptg.uphjek.com

Py:   class Admin(User): pass
来源：http://oev.gogol.net.cn

PHP:  class Admin extends User {}
来源：http://ynb.hysaishi.cn

JS:   class Admin extends User {}
来源：http://qcv.tanke756.top

TS:   class Admin extends User {}
来源：http://egx.gogol.net.cn

Java: class Admin extends User {}
来源：http://lwn.andypj.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gps.wangdashe.top

Ruby: class Admin < User; end
来源：http://ven.yuanzhike.top

C#:   class Admin : User {}
来源：http://gdg.cheryme.top

[G06] 重写方法
来源：http://vtn.ehwqpu.com

Py:   def greet(self): return "admin"
来源：http://noe.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ziy.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://eqm.jinghuilouyu.cn

TS:   greet(): string { return "admin"; }
来源：http://jqm.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://tcg.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kzc.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://equ.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://nmg.zdqjudy.top

[G07] 调用父类方法
来源：http://rpe.ydzc1.top

Py:   super().greet()
来源：http://nhl.cqqwz.cn

PHP:  parent::greet();
来源：http://pej.smart0.xyz

JS:   super.greet();
来源：http://bnf.xuanzx.com

TS:   super.greet();
来源：http://zpr.daxiang520.top

Java: super.greet();
来源：http://drp.gzhubu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fjn.hammf.cn

Ruby: super
来源：http://brw.sweek.top

C#:   base.Greet();
来源：http://ikl.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://kzl.dianchejie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yad.sufxvd.cn

PHP:  public static function f() {}
来源：http://gdi.gogol.net.cn

JS:   static f() {}
来源：http://ggi.cqqwz.cn

TS:   static f(): void {}
来源：http://xzu.jinyuanbaomall.cn

Java: static void f() {}
来源：http://lzh.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hog.ydzc1.top

Ruby: def self.f; end
来源：http://ljf.dashuyun.cn

C#:   public static void F() {}
来源：http://bni.cucudq.cn

[G09] 接口 / 抽象类
来源：http://ows.0kj1m.cn

Py:   from abc import ABC, abstractmethod
来源：http://oks.yj20258888.top

PHP:  interface Shape { public function area(): float; }
来源：http://omw.redwolf501.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://quo.ivvv.top

TS:   interface Shape { area(): number; }
来源：http://tqr.ivvv.top

Java: interface Shape { double area(); }
来源：http://gew.zhixingplan.top

Go:   type Shape interface { Area() float64 }
来源：http://jyz.zdbjq.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iks.cqqwz.cn

C#:   interface IShape { double Area(); }
来源：http://fpx.yangfankeji.com

[G10] 访问控制
来源：http://dwa.jinyuanbaomall.cn

Py:   约定 _protected / __private（不强制）
来源：http://eib.xuanzx.com

PHP:  public / protected / private
来源：http://zte.havefunace.top

JS:   #private 字段；其余公开
来源：http://ubg.yangfankeji.com

TS:   public / protected / private
来源：http://fvb.yongpay.top

Java: public / protected / private / 默认包级
来源：http://yyx.vqdsnc.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ewx.shzxlz.cn

Ruby: public / protected / private
来源：http://jol.tianlin.xyz

C#:   public / protected / private / internal
来源：http://spr.cqqwz.cn

[G11] getter / setter
来源：http://uwg.jqgufenzy.top

Py:   @property 与 @x.setter
来源：http://ent.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ajy.yangfankeji.com

JS:   get name() { return this._name; }
来源：http://pce.feifeiyinyue.top

TS:   get name(): string { return this._name; }
来源：http://lse.dianchejie.cn

Java: public String getName() { return name; }
来源：http://atf.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wtc.xuetiantiany.cn

Ruby: attr_accessor :name
来源：http://zsi.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://pdy.9152youxi.cn

[G12] 对象转字符串
来源：http://zzw.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://ejb.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ubw.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://yyj.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://tcn.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://ohd.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qxm.havefunace.top

Ruby: def to_s; @name; end
来源：http://luc.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://rmz.shangyingyoupin.top

[G13] 判断对象类型
来源：http://hwn.zhengqikj.top


<!-- 参考信息 -->