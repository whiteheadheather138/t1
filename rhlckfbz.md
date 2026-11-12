代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://att.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bex.sjlbkw.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vcc.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://fph.uphjek.com

[E14] URL 编码与 Base64
来源：http://drt.zdbjq.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qlz.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vkl.zhaomingkeji.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qlc.hywenlv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hev.gzhubu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eqg.yj20258888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cog.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vzx.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hhk.sxryk.cn

[E15] HTML 转义 / 反转义
来源：http://qau.jlsjyb.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ygs.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://aka.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://aof.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://kur.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zge.ctjpmb.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fkd.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tst.nwbrower.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ztm.zhoulong.xyz

[E16] 数字千分位
来源：http://xvs.nwbrower.top

Py:   f"{1234567:,}"
来源：http://sgk.jyoumei.cn

PHP:  number_format(1234567);
来源：http://ydr.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://osw.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://qpr.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wam.gotoacloud.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zlk.zycfv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gnp.yongpay.top

C#:   1234567.ToString("N0")
来源：http://quv.ivvv.top

[E17] 首字母大写
来源：http://qkv.nanxuanxn.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ylp.zhixingplan.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vwt.fzhhl.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cpx.yuanzhike.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sgv.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knk.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://anc.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ysj.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kzd.shanyushiyangtech.top

[E18] 模板占位符替换
来源：http://oxi.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zhl.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zva.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pzp.svipenyu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ann.sjlbkw.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fzv.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gpo.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rcj.hcnkem.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://viq.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://wll.shangyingyoupin.top

Py:   s.splitlines()
来源：http://edk.chenzaomai.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bnp.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://ssm.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://hei.nanxinkj.top

Java: s.lines().toList()
来源：http://jod.xuanzx.com

Go:   strings.Split(s, "\n")
来源：http://ywz.cqqwz.cn

Ruby: s.lines
来源：http://xod.quarkkingdee.top

C#:   s.Split('\n')
来源：http://usz.yuanzhike.top

[E20] 判断字符串是否为空
来源：http://rye.jinqigfzy.top

Py:   if not s:
来源：http://tis.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpn.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://voe.zhiwuduotai.top

TS:   if (s === "") {}
来源：http://odf.zdbjq.cn

Java: if (s.isEmpty()) {}
来源：http://ybj.daxiang520.top

Go:   if s == "" {}
来源：http://zdc.svipenyu.cn

Ruby: if s.empty?
来源：http://vte.gotoacloud.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ggl.sxryk.cn

[E21] 超长截断加省略号
来源：http://zwg.c1oappe.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fci.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ypj.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tlp.yj20258888.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qcg.hcnkem.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tbz.hongshengwenyu.top

Go:   // 按 rune 判断长度后截断
来源：http://daj.kuanghao11.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pxq.aizwys.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lhb.haohaochexian.top

[E22] 字节长度与字符长度
来源：http://eiu.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://knc.chenjidiqi.icu

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gbw.quarkkingdee.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mvk.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfk.meibo888.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://few.ppjwa.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nht.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://dwk.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tgg.yongpay.top

================================================================================
来源：http://mrs.haohaochexian.top

F. 文件与目录
来源：http://pij.tianlin.xyz

================================================================================
来源：http://kct.xinyue.icu

[F01] 读取整个文件
来源：http://cxs.shzxlz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vub.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://fxj.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://btq.xuetiantiany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uta.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ckj.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eqq.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://ilq.zycfv.cn

C#:   File.ReadAllText("a.txt");
来源：http://ssw.fengsongda.top

[F02] 逐行读取文件
来源：http://ung.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://faa.vehdjk.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vvi.yanxiufei.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lvn.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kiy.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jek.nanxuanxn.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dfq.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nmd.wangshuangyany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bqa.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://ica.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://clj.jianghu66.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xpx.dianchejie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jwn.svipenyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfu.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zyo.gzhubu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ldw.redwolf501.top

Ruby: File.write("a.txt", "hi")
来源：http://pny.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zsi.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://syc.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://itm.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://neh.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://elw.wangdashe.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhx.chenzaomai.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://duw.xingfuxueyuan.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://irn.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yaw.yuxming.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gfj.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://dpm.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bzh.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://ahr.jinqigfzy.top

JS:   fs.existsSync("a.txt")
来源：http://drb.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://vtv.zycfv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jax.sxryk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nrq.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://qup.yvedp.cn

C#:   File.Exists("a.txt")
来源：http://iks.tian-w.cn

[F06] 删除文件
来源：http://jmx.c1oappe.top

Py:   os.remove("a.txt")
来源：http://jkr.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://yco.ydjk.org.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fot.jqgfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://kll.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bka.daria6918.cn

Go:   os.Remove("a.txt")
来源：http://ank.gogol.net.cn

Ruby: File.delete("a.txt")
来源：http://hqd.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://onl.fktsv.cn

[F07] 创建目录（含多级）
来源：http://ngl.zdqjudy.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://olw.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eqw.xinyue.icu

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://coa.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hwx.tarul.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://shs.sufxvd.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ycm.gaohongyu789.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ofj.wangdashe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vrx.gaohongyu789.top

[F08] 遍历目录
来源：http://isi.hysaishi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wcx.tian-w.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zwn.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://xjb.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://nap.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dgo.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bxs.uphjek.com

Ruby: Dir.children("dir")
来源：http://twi.zhaomingkeji.xyz

C#:   Directory.GetFiles("dir")
来源：http://vnk.xuetiantiany.cn

[F09] 获取文件大小
来源：http://iyt.zdbjq.cn

Py:   os.path.getsize("a.txt")
来源：http://kbd.yongpay.top

PHP:  filesize("a.txt");
来源：http://nnx.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://god.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://ois.guannengcc.top

Java: Files.size(Path.of("a.txt"))
来源：http://ctz.ydzc1.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hga.cdnleiting.top

Ruby: File.size("a.txt")
来源：http://mdk.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://icf.hammf.cn

[F10] 取文件扩展名 / 文件名
来源：http://gtt.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kmc.jqgufenzy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://avo.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zos.chenzaomai.com

TS:   path.extname("a.txt")
来源：http://rzl.cqqwz.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iik.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mdj.guannengcc.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vcx.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jmw.guannengcc.top

[F11] 复制与移动文件
来源：http://lre.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://evy.hfpthk.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xhk.smart0.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qbp.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tqe.fehbvm.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bjy.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bqk.haohaochexian.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mwg.jinyuanbaomall.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fvo.aibaodan.cn

[F12] CSV 读写
来源：http://oja.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kly.c1oappe.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ves.tarul.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://grq.jlsjyb.cn

TS:   // 同上
来源：http://ndr.gotoacloud.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ptz.zhoulong.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sgm.dianchejie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://khv.guannengcc.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tma.tianlin.xyz

================================================================================
来源：http://slp.ehwqpu.com

G. 面向对象
来源：http://kkx.xylfe.cn

================================================================================
来源：http://rxi.hesvh.cn

[G01] 定义类
来源：http://mdj.hesvh.cn

Py:   class User: pass
来源：http://yvo.ppjwa.cn

PHP:  class User {}
来源：http://ghc.meibo888.top

JS:   class User {}
来源：http://dvt.zhiwuduotai.top

TS:   class User { name: string = ""; }
来源：http://zpt.ehwqpu.com

Java: class User {}
来源：http://znc.zycfv.cn

Go:   type User struct { Name string }
来源：http://crf.uphjek.com

Ruby: class User; end
来源：http://szf.yuxming.cn

C#:   class User {}
来源：http://hdr.fktsv.cn

[G02] 构造函数
来源：http://znu.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://fno.fktsv.cn

PHP:  public function __construct(public string $name) {}
来源：http://kmw.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://wtm.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://wjd.tarul.cn

Java: User(String name) { this.name = name; }
来源：http://dan.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ydr.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://wno.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://huu.andypj.xyz

[G03] 实例属性
来源：http://mhs.hnqzz.top

Py:   self.name = "x"
来源：http://gcw.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://eef.9152youxi.cn

JS:   this.name = "x";
来源：http://qbr.ydzc1.top

TS:   name: string = "x";
来源：http://dec.chenlongwang.top

Java: private String name;
来源：http://iyu.zhengqikj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nkl.zdbjq.cn

Ruby: @name = "x"
来源：http://itc.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://pcf.yfazqb.com

[G04] 定义方法
来源：http://vqf.jyoumei.cn

Py:   def greet(self): return self.name
来源：http://llq.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://llk.gzhubu.top

JS:   greet() { return this.name; }
来源：http://phh.ivvv.top

TS:   greet(): string { return this.name; }
来源：http://ccj.quarkkingdee.top

Java: String greet() { return name; }
来源：http://xvb.redwolf501.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://tgc.sjlbkw.cn

Ruby: def greet; @name; end
来源：http://sor.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://iyy.ybcxt.top

[G05] 继承
来源：http://ott.hammf.cn

Py:   class Admin(User): pass
来源：http://rex.hnxiangtu.top

PHP:  class Admin extends User {}
来源：http://rld.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://qsg.52xcode.cn

TS:   class Admin extends User {}
来源：http://ldl.guowangkeji.top

Java: class Admin extends User {}
来源：http://qjk.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rrl.wangdashe.top

Ruby: class Admin < User; end
来源：http://dqw.chenzaomai.com

C#:   class Admin : User {}
来源：http://unq.yangfankeji.com

[G06] 重写方法
来源：http://etv.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://are.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zdt.jqgufenzy.top

JS:   greet() { return "admin"; }
来源：http://twb.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://qrd.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://xos.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dqq.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://vvd.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://xpi.epnwcf.com

[G07] 调用父类方法
来源：http://isf.shuidangran.top

Py:   super().greet()
来源：http://cwf.jinghuilouyu.cn

PHP:  parent::greet();
来源：http://qtz.jqgufenzy.top

JS:   super.greet();
来源：http://cpv.mhx1999.top

TS:   super.greet();
来源：http://aip.xuanzx.com

Java: super.greet();
来源：http://yfb.guannengcc.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qmn.cashguo.top

Ruby: super
来源：http://gxa.0kj1m.cn

C#:   base.Greet();
来源：http://jfs.yongpay.top

[G08] 静态方法与属性
来源：http://aoh.kuanghao11.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hpy.52xcode.cn

PHP:  public static function f() {}
来源：http://hcv.andypj.xyz

JS:   static f() {}
来源：http://rrw.yongpay.top

TS:   static f(): void {}
来源：http://okn.fktsv.cn

Java: static void f() {}
来源：http://gri.xylfe.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lhb.aibaodan.cn

Ruby: def self.f; end
来源：http://njf.daxiang520.top

C#:   public static void F() {}
来源：http://hsq.smart0.xyz

[G09] 接口 / 抽象类
来源：http://yfo.jinqigfzy.top

Py:   from abc import ABC, abstractmethod
来源：http://yzx.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://rrr.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qhy.cqqwz.cn

TS:   interface Shape { area(): number; }
来源：http://ndp.zdbjq.cn

Java: interface Shape { double area(); }
来源：http://jvv.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://kih.guannengcc.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kyp.yanxiufei.cn

C#:   interface IShape { double Area(); }
来源：http://eno.sxryk.cn

[G10] 访问控制
来源：http://pxa.mhx1999.top

Py:   约定 _protected / __private（不强制）
来源：http://pfk.zhiwuduotai.top

PHP:  public / protected / private
来源：http://akn.jlsjyb.cn

JS:   #private 字段；其余公开
来源：http://gfr.yvedp.cn

TS:   public / protected / private
来源：http://mjr.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://lrq.sjlbkw.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://muj.jinqigfzy.top

Ruby: public / protected / private
来源：http://jog.tianlin.xyz

C#:   public / protected / private / internal
来源：http://xbj.jyoumei.cn

[G11] getter / setter
来源：http://prs.uphjek.com

Py:   @property 与 @x.setter
来源：http://yvu.xuanzx.com

PHP:  public function getName(): string { return $this->name; }
来源：http://lhw.xuetiantiany.cn

JS:   get name() { return this._name; }
来源：http://snd.epnwcf.com

TS:   get name(): string { return this._name; }
来源：http://kfv.ydzc1.top

Java: public String getName() { return name; }
来源：http://ipu.jiagoushi.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://cdy.yj202588.top

Ruby: attr_accessor :name
来源：http://ywb.9152youxi.cn

C#:   public string Name { get; set; }
来源：http://jfp.zhiwuduotai.top

[G12] 对象转字符串
来源：http://hps.kuanghao11.cn

Py:   def __str__(self): return self.name
来源：http://jse.gzhubu.top


<!-- 参考信息 -->