代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dwa.cashguo.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lks.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://gpk.52xcode.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qbn.tanke756.top

[E14] URL 编码与 Base64
来源：http://oof.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uph.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hvi.gotoacloud.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qzc.daria6918.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tcs.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kms.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ibp.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xmn.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gkf.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://gml.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bhl.sxryk.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zio.9152youxi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kvl.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hov.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://btg.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qnu.redwolf501.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qes.dashuyun.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://odk.xingfuxueyuan.xyz

[E16] 数字千分位
来源：http://fig.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://wtm.havefunace.top

PHP:  number_format(1234567);
来源：http://rlr.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ajf.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tdq.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ifd.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://why.fktsv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fxi.hnxiangtu.top

C#:   1234567.ToString("N0")
来源：http://dds.wangshuangyany.cn

[E17] 首字母大写
来源：http://ikt.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qdg.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yud.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lue.cucudq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fbg.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://knk.gotoacloud.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nnl.andypj.xyz

Ruby: s.capitalize
来源：http://dvo.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nuf.sjlbkw.cn

[E18] 模板占位符替换
来源：http://ylq.pycfn.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mfe.52xcode.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mkz.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dba.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://cia.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qiw.cdnleiting.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xtw.pycfn.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fpd.hammf.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://niq.bbcook.cn

[E19] 多行文本按行拆分
来源：http://ega.daria6918.cn

Py:   s.splitlines()
来源：http://rge.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ekv.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://bpd.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://rxb.hnxiangtu.top

Java: s.lines().toList()
来源：http://cac.sjlbkw.cn

Go:   strings.Split(s, "\n")
来源：http://jbp.redwolf501.top

Ruby: s.lines
来源：http://uys.cqqwz.cn

C#:   s.Split('\n')
来源：http://cem.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://fpk.316326.xyz

Py:   if not s:
来源：http://bmr.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://las.xuetiantiany.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wlk.meibo888.top

TS:   if (s === "") {}
来源：http://rmu.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://ztb.tanke756.top

Go:   if s == "" {}
来源：http://kic.shzxlz.cn

Ruby: if s.empty?
来源：http://vpi.cdnleiting.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pzf.vehdjk.com

[E21] 超长截断加省略号
来源：http://lcx.shangyingyoupin.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yzl.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yvx.nanxuanxn.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://orx.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yzv.vehdjk.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gjh.vehdjk.com

Go:   // 按 rune 判断长度后截断
来源：http://jdc.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vou.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cwr.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://ogm.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://npd.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mre.wangdashe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qcy.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ysc.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kna.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fer.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://ame.hfpthk.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hwz.hywenlv.cn

================================================================================
来源：http://zai.ywan-chungtsiang.top

F. 文件与目录
来源：http://mdg.yonumen.top

================================================================================
来源：http://jyv.hnxiangtu.top

[F01] 读取整个文件
来源：http://xxc.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lpu.yvedp.cn

PHP:  file_get_contents("a.txt");
来源：http://yly.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lpe.yanxiufei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ixt.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://jgj.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oko.xinyue.icu

Ruby: File.read("a.txt")
来源：http://tir.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://xbr.yj202588.top

[F02] 逐行读取文件
来源：http://faq.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://skh.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vwe.zycfv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zkb.xinyue.icu

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xzu.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jwc.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://egp.ywan-chungtsiang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ybz.wangdashe.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rvv.cheryme.top

[F03] 写入文件（覆盖）
来源：http://evv.andypj.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ymh.chenlongwang.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://wlg.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ubn.daxiang520.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbh.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ttr.ehwqpu.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://brh.hfpthk.cn

Ruby: File.write("a.txt", "hi")
来源：http://dru.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wft.jiagoushi.top

[F04] 追加写入文件
来源：http://atb.shangyingyoupin.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eyu.yonumen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zzv.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bor.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dui.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pvv.jqgfzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iwh.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mpp.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://abo.ydzc1.top

[F05] 判断文件或目录是否存在
来源：http://vcs.shanyushiyangtech.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jbp.jinyuanbaomall.cn

PHP:  file_exists("a.txt");
来源：http://gwj.bbcook.cn

JS:   fs.existsSync("a.txt")
来源：http://kjm.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://voc.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fbd.gzhubu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pqd.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://mrj.sxryk.cn

C#:   File.Exists("a.txt")
来源：http://czb.cheryme.top

[F06] 删除文件
来源：http://uwd.sxryk.cn

Py:   os.remove("a.txt")
来源：http://bzk.mhx1999.top

PHP:  unlink("a.txt");
来源：http://efy.sysykeji.top

JS:   fs.unlinkSync("a.txt")
来源：http://hbb.cucudq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kco.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hqi.bbcook.cn

Go:   os.Remove("a.txt")
来源：http://ucc.fengsongda.top

Ruby: File.delete("a.txt")
来源：http://lkt.zycfv.cn

C#:   File.Delete("a.txt");
来源：http://gxz.hnxiangtu.top

[F07] 创建目录（含多级）
来源：http://hhg.aizwys.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://erl.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hhq.hfpthk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mfk.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pkj.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tua.hongshengwenyu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lak.chenlongwang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kti.ydzc1.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rsa.zycfv.cn

[F08] 遍历目录
来源：http://vsh.daria6918.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hww.xuanzx.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dlq.52xcode.cn

JS:   fs.readdirSync("dir")
来源：http://nvj.ydjk.org.cn

TS:   fs.readdirSync("dir")
来源：http://krc.316326.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qke.jqgufenzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tdg.yj202588.top

Ruby: Dir.children("dir")
来源：http://nzl.bjfxy.top

C#:   Directory.GetFiles("dir")
来源：http://tld.pycfn.com

[F09] 获取文件大小
来源：http://ujx.52xcode.cn

Py:   os.path.getsize("a.txt")
来源：http://dmd.xuanzx.com

PHP:  filesize("a.txt");
来源：http://xmh.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://vkc.haohaochexian.top

TS:   fs.statSync("a.txt").size
来源：http://bis.bjfxy.top

Java: Files.size(Path.of("a.txt"))
来源：http://bmn.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://roy.sufxvd.cn

Ruby: File.size("a.txt")
来源：http://rvt.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://ygp.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://gml.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mhz.andypj.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tsi.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vqz.shuidangran.top

TS:   path.extname("a.txt")
来源：http://hui.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aup.yuanzhike.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zvo.tarul.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ztu.hysaishi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jlm.sxryk.cn

[F11] 复制与移动文件
来源：http://zcp.smart0.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://drf.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oan.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nah.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jvf.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ulg.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gsp.zdqjudy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rxn.fengsongda.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jwt.jinyuanbaomall.cn

[F12] CSV 读写
来源：http://krv.daxiang520.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vvn.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gld.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lhs.wangshuangyany.cn

TS:   // 同上
来源：http://scl.shangyingyoupin.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fdm.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oou.meibo888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cbk.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ung.shzxlz.cn

================================================================================
来源：http://ixy.hesvh.cn

G. 面向对象
来源：http://zfm.316326.xyz

================================================================================
来源：http://huk.jinqigufen.top

[G01] 定义类
来源：http://fki.chenzaomai.com

Py:   class User: pass
来源：http://elv.hysaishi.cn

PHP:  class User {}
来源：http://pju.guowangkeji.top

JS:   class User {}
来源：http://xzu.tian-w.cn

TS:   class User { name: string = ""; }
来源：http://wnc.yuanzhike.top

Java: class User {}
来源：http://vgf.ctjpmb.com

Go:   type User struct { Name string }
来源：http://gat.yuanzhike.top

Ruby: class User; end
来源：http://phi.wangshuangyany.cn

C#:   class User {}
来源：http://rpc.chenjidiqi.icu

[G02] 构造函数
来源：http://zvi.zdbjq.cn

Py:   def __init__(self, name): self.name = name
来源：http://bxy.dianchejie.cn

PHP:  public function __construct(public string $name) {}
来源：http://kif.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://yxn.jqgufenzy.top

TS:   constructor(public name: string) {}
来源：http://ipi.aibaodan.cn

Java: User(String name) { this.name = name; }
来源：http://fop.cdnleiting.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hux.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://nyh.redwolf501.top

C#:   public User(string name) { Name = name; }
来源：http://vox.fehbvm.com

[G03] 实例属性
来源：http://rrp.fengsongda.top

Py:   self.name = "x"
来源：http://yfu.ybcxt.top

PHP:  public string $name = "x";
来源：http://kvd.jianghu66.top

JS:   this.name = "x";
来源：http://evi.shuidangran.top

TS:   name: string = "x";
来源：http://cmj.iojbl.cn

Java: private String name;
来源：http://mzx.sxryk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qdu.yuxming.cn

Ruby: @name = "x"
来源：http://sct.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://kdr.chenzaomai.com

[G04] 定义方法
来源：http://poj.vqdsnc.cn

Py:   def greet(self): return self.name
来源：http://uqg.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://dwr.jinqigfzy.top

JS:   greet() { return this.name; }
来源：http://nme.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://mri.guowangkeji.top

Java: String greet() { return name; }
来源：http://cfj.mhx1999.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://iiu.xuanzx.com

Ruby: def greet; @name; end
来源：http://gbv.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://ssa.cqqwz.cn

[G05] 继承
来源：http://gjb.daria6918.cn

Py:   class Admin(User): pass
来源：http://kvl.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://fwm.hongshengwenyu.top

JS:   class Admin extends User {}
来源：http://cug.fengsongda.top

TS:   class Admin extends User {}
来源：http://pgr.cheryme.top

Java: class Admin extends User {}
来源：http://wxb.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mly.pycfn.com

Ruby: class Admin < User; end
来源：http://ktg.vqdsnc.cn

C#:   class Admin : User {}
来源：http://eoo.zycfv.cn

[G06] 重写方法
来源：http://oly.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://hea.fzhhl.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gxm.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://cfn.hcnkem.com

TS:   greet(): string { return "admin"; }
来源：http://viz.yj20258.top

Java: @Override String greet() { return "admin"; }
来源：http://qyc.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://shi.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://oly.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://isr.ivvv.top

[G07] 调用父类方法
来源：http://pwt.zdqjudy.top

Py:   super().greet()
来源：http://zit.9152youxi.cn

PHP:  parent::greet();
来源：http://gpg.hammf.cn

JS:   super.greet();
来源：http://ujh.daria6918.cn

TS:   super.greet();
来源：http://fjo.svipenyu.cn

Java: super.greet();
来源：http://fqf.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iio.daxiang520.top

Ruby: super
来源：http://ify.cashguo.top

C#:   base.Greet();
来源：http://ixl.yongpay.top

[G08] 静态方法与属性
来源：http://xno.meibo888.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://msw.jinqigfzy.top

PHP:  public static function f() {}
来源：http://rzo.shzxlz.cn

JS:   static f() {}
来源：http://zly.tanke756.top

TS:   static f(): void {}
来源：http://chl.tianlin.xyz

Java: static void f() {}
来源：http://tsl.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ajn.mhx1999.top

Ruby: def self.f; end
来源：http://idz.birdmap.top

C#:   public static void F() {}
来源：http://spu.yueranfly.top

[G09] 接口 / 抽象类
来源：http://cxg.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://ngm.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://htm.ydzc1.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zix.sweek.top

TS:   interface Shape { area(): number; }
来源：http://zxh.hcnkem.com

Java: interface Shape { double area(); }
来源：http://gat.zdqjudy.top

Go:   type Shape interface { Area() float64 }
来源：http://tpi.c1oappe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fec.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://iob.jqgfzy.top

[G10] 访问控制
来源：http://xzq.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://xsl.zhongyouzk.top

PHP:  public / protected / private
来源：http://cjh.wangshuangyany.cn

JS:   #private 字段；其余公开
来源：http://fjb.ydzc1.top

TS:   public / protected / private
来源：http://gyo.sweek.top

Java: public / protected / private / 默认包级
来源：http://zdn.zhoulong.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://tcp.yuanzhike.top

Ruby: public / protected / private
来源：http://wcy.guannengcc.top

C#:   public / protected / private / internal
来源：http://pqm.52xcode.cn

[G11] getter / setter
来源：http://aaa.daxiang520.top

Py:   @property 与 @x.setter
来源：http://rly.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://mnw.hnxiangtu.top

JS:   get name() { return this._name; }
来源：http://tlk.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://mzp.bjfxy.top

Java: public String getName() { return name; }
来源：http://moi.cashguo.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://etb.cheryme.top

Ruby: attr_accessor :name
来源：http://nfy.ybcxt.top

C#:   public string Name { get; set; }
来源：http://neg.nanxinkj.top

[G12] 对象转字符串
来源：http://vbz.xuanzx.com

Py:   def __str__(self): return self.name
来源：http://euo.fanxiaobao.xyz


<!-- 参考信息 -->