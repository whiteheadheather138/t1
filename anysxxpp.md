代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pom.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://buu.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fxn.hongshengwenyu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dew.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://pwk.bjfxy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ylr.jianghu66.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nvz.guannengcc.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nof.zhiwuduotai.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dgk.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lro.sweek.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zgw.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://usm.xziqi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://biy.tarul.cn

[E15] HTML 转义 / 反转义
来源：http://hpn.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://zjr.yj202588.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nef.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ffb.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ifj.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cuz.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ogl.fehbvm.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fwf.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ytb.haohaochexian.top

[E16] 数字千分位
来源：http://fjb.hammf.cn

Py:   f"{1234567:,}"
来源：http://tmi.cheryme.top

PHP:  number_format(1234567);
来源：http://zqn.316326.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://ivc.chenzaomai.com

TS:   (1234567).toLocaleString("en-US")
来源：http://njg.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aqy.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://akc.sxryk.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zta.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://gfp.hongshengwenyu.top

[E17] 首字母大写
来源：http://dlo.pengpengdd.cyou

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wiw.xylfe.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tfu.iojbl.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gpb.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fcm.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vdz.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fpa.iojbl.cn

Ruby: s.capitalize
来源：http://vtp.tianlin.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rxk.0kj1m.cn

[E18] 模板占位符替换
来源：http://ufq.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xqi.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hyl.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uos.fktsv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://zoi.gzhubu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vxg.9152youxi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://atv.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hzs.zhengqikj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hbn.yj202588.top

[E19] 多行文本按行拆分
来源：http://qwu.zycfv.cn

Py:   s.splitlines()
来源：http://pxg.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://urm.zycfv.cn

JS:   s.split(/\r?\n/)
来源：http://ccl.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://zqr.tarul.cn

Java: s.lines().toList()
来源：http://bwa.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://naq.kuanghao11.cn

Ruby: s.lines
来源：http://dtl.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://zmu.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://prb.c1oappe.top

Py:   if not s:
来源：http://mac.nwbrower.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rsm.tian-w.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://olo.bjfxy.top

TS:   if (s === "") {}
来源：http://dii.zhoulong.xyz

Java: if (s.isEmpty()) {}
来源：http://xie.cheryme.top

Go:   if s == "" {}
来源：http://pdw.fktsv.cn

Ruby: if s.empty?
来源：http://fif.chenzaomai.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gia.52xcode.cn

[E21] 超长截断加省略号
来源：http://kns.zhongyouzk.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://knx.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bhv.wangdashe.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://psj.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcc.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oyy.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://kpg.yuanzhike.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qpi.shuidangran.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://omv.9152youxi.cn

[E22] 字节长度与字符长度
来源：http://pwp.yj202588.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bmv.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kgy.hammf.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zlo.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wng.jyoumei.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://psf.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fmi.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://zrl.sxryk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cvc.chenzaomai.com

================================================================================
来源：http://efs.hfpthk.cn

F. 文件与目录
来源：http://ckh.xinyue.icu

================================================================================
来源：http://pwx.feifeiyinyue.top

[F01] 读取整个文件
来源：http://ztl.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fcm.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://zni.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dgg.wangdashe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oeq.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xrd.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pab.svipenyu.cn

Ruby: File.read("a.txt")
来源：http://ofb.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://tvo.hnxiangtu.top

[F02] 逐行读取文件
来源：http://uzd.haohaochexian.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nnv.9152youxi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mcx.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tul.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xuc.dashuyun.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iut.zdqjudy.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zuu.jinyuanbaomall.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://crz.tanke756.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jki.zhongyouzk.top

[F03] 写入文件（覆盖）
来源：http://dtf.wangdashe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kya.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://efl.vqdsnc.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbw.chenzaomai.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lmx.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://exk.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lum.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://tpr.sweek.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ors.xuetiantiany.cn

[F04] 追加写入文件
来源：http://efv.shuidangran.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://odk.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vmm.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tii.redwolf501.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ikw.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ohc.gaohongyu789.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ddz.zdbjq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jfg.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kpk.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://koj.iojbl.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dwh.yueranfly.top

PHP:  file_exists("a.txt");
来源：http://ilk.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://flc.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://qlj.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://xta.ydjk.org.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oxm.fehbvm.com

Ruby: File.exist?("a.txt")
来源：http://vrw.aibaodan.cn

C#:   File.Exists("a.txt")
来源：http://oyo.yonumen.top

[F06] 删除文件
来源：http://rxc.yj202588.top

Py:   os.remove("a.txt")
来源：http://xdi.yangfankeji.com

PHP:  unlink("a.txt");
来源：http://ajm.hnqzz.top

JS:   fs.unlinkSync("a.txt")
来源：http://pks.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://hkr.shzxlz.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://six.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://njm.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://sym.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://rsa.wangshuangyany.cn

[F07] 创建目录（含多级）
来源：http://itb.cashguo.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vyy.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vkz.wangshuangyany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gdv.fengsongda.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ici.zdbjq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://upk.52xcode.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cfi.hysaishi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ckq.yuxming.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zwd.zycfv.cn

[F08] 遍历目录
来源：http://dxt.yuxming.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zrn.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vba.jinqigufen.top

JS:   fs.readdirSync("dir")
来源：http://duj.zhijiandao.cn

TS:   fs.readdirSync("dir")
来源：http://inb.aizwys.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rks.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://dpu.tanke756.top

Ruby: Dir.children("dir")
来源：http://uxz.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://gop.fengsongda.top

[F09] 获取文件大小
来源：http://ehz.daxiang520.top

Py:   os.path.getsize("a.txt")
来源：http://mbv.meibo888.top

PHP:  filesize("a.txt");
来源：http://hrt.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://aek.chenjidiqi.icu

TS:   fs.statSync("a.txt").size
来源：http://imi.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gvi.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yik.dianchejie.cn

Ruby: File.size("a.txt")
来源：http://hxm.hammf.cn

C#:   new FileInfo("a.txt").Length
来源：http://yfe.guowangkeji.top

[F10] 取文件扩展名 / 文件名
来源：http://asm.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sfa.hcnkem.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gux.guowangkeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mtl.guannengcc.top

TS:   path.extname("a.txt")
来源：http://onf.gzhubu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tlv.ydzc1.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bya.ydzc1.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tom.aibaodan.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wfo.zhoulong.xyz

[F11] 复制与移动文件
来源：http://jpv.pengpengdd.cyou

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://djf.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zaa.snrcjt.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sok.sysykeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://riw.zhijiandao.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ezs.cqqwz.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cgn.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://amy.vqdsnc.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qpb.dashuyun.cn

[F12] CSV 读写
来源：http://zfn.kuanghao11.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cep.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jkz.sjlbkw.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://emp.cucudq.cn

TS:   // 同上
来源：http://ixf.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://czj.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dty.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zxe.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://mfl.yvedp.cn

================================================================================
来源：http://nmf.kuanghao11.cn

G. 面向对象
来源：http://wwv.uphjek.com

================================================================================
来源：http://msq.xziqi.cn

[G01] 定义类
来源：http://qrp.meibo888.top

Py:   class User: pass
来源：http://eli.sysykeji.top

PHP:  class User {}
来源：http://xts.nanxuanxn.top

JS:   class User {}
来源：http://kev.shuidangran.top

TS:   class User { name: string = ""; }
来源：http://hey.zhongyouzk.top

Java: class User {}
来源：http://cnc.xingfuxueyuan.xyz

Go:   type User struct { Name string }
来源：http://pge.0kj1m.cn

Ruby: class User; end
来源：http://dge.fehbvm.com

C#:   class User {}
来源：http://ckp.birdmap.top

[G02] 构造函数
来源：http://xoq.cheryme.top

Py:   def __init__(self, name): self.name = name
来源：http://gqo.xingfuxueyuan.xyz

PHP:  public function __construct(public string $name) {}
来源：http://mgw.sxryk.cn

JS:   constructor(name) { this.name = name; }
来源：http://ozg.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://lbk.andypj.xyz

Java: User(String name) { this.name = name; }
来源：http://kdi.yangfankeji.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dxd.shzxlz.cn

Ruby: def initialize(name); @name = name; end
来源：http://eay.shanyushiyangkeji.top

C#:   public User(string name) { Name = name; }
来源：http://had.sysykeji.top

[G03] 实例属性
来源：http://rsb.daxiang520.top

Py:   self.name = "x"
来源：http://vvk.fehbvm.com

PHP:  public string $name = "x";
来源：http://gtr.sufxvd.cn

JS:   this.name = "x";
来源：http://jld.ehwqpu.com

TS:   name: string = "x";
来源：http://uux.0kj1m.cn

Java: private String name;
来源：http://vqv.yongpay.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uak.gaohongyu789.top

Ruby: @name = "x"
来源：http://wfp.ivvv.top

C#:   public string Name { get; set; } = "x";
来源：http://gce.0kj1m.cn

[G04] 定义方法
来源：http://uud.sjlbkw.cn

Py:   def greet(self): return self.name
来源：http://ahu.9152youxi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ygn.jinqigufen.top

JS:   greet() { return this.name; }
来源：http://qkl.cqqwz.cn

TS:   greet(): string { return this.name; }
来源：http://bcz.vehdjk.com

Java: String greet() { return name; }
来源：http://lfn.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qvk.c1oappe.top

Ruby: def greet; @name; end
来源：http://aec.pycfn.com

C#:   public string Greet() => Name;
来源：http://qdg.zycfv.cn

[G05] 继承
来源：http://kpz.ybcxt.top

Py:   class Admin(User): pass
来源：http://xum.9152youxi.cn

PHP:  class Admin extends User {}
来源：http://jfl.yueranfly.top

JS:   class Admin extends User {}
来源：http://uvg.shanyushiyangtech.top

TS:   class Admin extends User {}
来源：http://nry.hnxiangtu.top

Java: class Admin extends User {}
来源：http://edg.zdbjq.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hba.0kj1m.cn

Ruby: class Admin < User; end
来源：http://mnd.yj202588.top

C#:   class Admin : User {}
来源：http://hio.yfazqb.com

[G06] 重写方法
来源：http://zfm.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://ubq.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xrg.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://erq.sufxvd.cn

TS:   greet(): string { return "admin"; }
来源：http://gpe.hfpthk.cn

Java: @Override String greet() { return "admin"; }
来源：http://kwl.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hgr.hnxiangtu.top

Ruby: def greet; "admin"; end
来源：http://cof.jinyuanbaomall.cn

C#:   public override string Greet() => "admin";
来源：http://kxr.hongshengwenyu.top

[G07] 调用父类方法
来源：http://bad.zhiwuduotai.top

Py:   super().greet()
来源：http://lsx.fzhhl.top

PHP:  parent::greet();
来源：http://hbg.haohaochexian.top

JS:   super.greet();
来源：http://bqv.dianchejie.cn

TS:   super.greet();
来源：http://frf.yanxiufei.cn

Java: super.greet();
来源：http://fdr.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://deu.guannengcc.top

Ruby: super
来源：http://fpg.aibaodan.cn

C#:   base.Greet();
来源：http://wgg.gaohongyu789.top

[G08] 静态方法与属性
来源：http://mtm.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iqy.daxiang520.top

PHP:  public static function f() {}
来源：http://ich.shanyushiyangkeji.top

JS:   static f() {}
来源：http://lle.haohaochexian.top

TS:   static f(): void {}
来源：http://iha.xuanzx.com

Java: static void f() {}
来源：http://yph.jinqigfzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://olh.ppjwa.cn

Ruby: def self.f; end
来源：http://pkn.ivvv.top

C#:   public static void F() {}
来源：http://dod.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://qmr.dashuyun.cn

Py:   from abc import ABC, abstractmethod
来源：http://yiv.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://yjy.shanyushiyangtech.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hzq.andypj.xyz

TS:   interface Shape { area(): number; }
来源：http://row.9152youxi.cn

Java: interface Shape { double area(); }
来源：http://tsr.fktsv.cn

Go:   type Shape interface { Area() float64 }
来源：http://zty.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ugb.xylfe.cn

C#:   interface IShape { double Area(); }
来源：http://fje.hammf.cn

[G10] 访问控制
来源：http://ehy.zhengqikj.top

Py:   约定 _protected / __private（不强制）
来源：http://krv.shuidangran.top

PHP:  public / protected / private
来源：http://spa.zhengqikj.top

JS:   #private 字段；其余公开
来源：http://fmw.kuanghao11.cn

TS:   public / protected / private
来源：http://aik.zycfv.cn

Java: public / protected / private / 默认包级
来源：http://rjm.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nbn.yj20258888.top

Ruby: public / protected / private
来源：http://wry.fzhhl.top

C#:   public / protected / private / internal
来源：http://hkh.chenlongwang.top

[G11] getter / setter
来源：http://asz.aibaodan.cn

Py:   @property 与 @x.setter
来源：http://xjt.316326.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://ate.guannengcc.top

JS:   get name() { return this._name; }
来源：http://ctu.aizwys.cn

TS:   get name(): string { return this._name; }
来源：http://pik.bbcook.cn

Java: public String getName() { return name; }
来源：http://nok.zhengqikj.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://chq.wangdashe.top

Ruby: attr_accessor :name
来源：http://rny.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://cdb.ybcxt.top

[G12] 对象转字符串
来源：http://jdi.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://vfc.birdmap.top


<!-- 参考信息 -->