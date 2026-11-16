代发 wailian999

[E14] URL 编码与 Base64
来源：http://nkn.zhoulong.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hpv.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ube.yongpay.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ith.gzhubu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ydl.meibo888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ure.gzhubu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gbg.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lzs.dianchejie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qob.shuidangran.top

[E15] HTML 转义 / 反转义
来源：http://pti.zdbjq.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vza.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://soc.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ntt.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cxx.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sxq.jianghu66.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mzv.zhongyouzk.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://edx.zdqjudy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://far.cheryme.top

[E16] 数字千分位
来源：http://csy.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://dzh.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://mob.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ets.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jle.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eyu.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mzc.zdqjudy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qcw.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://pks.jianghu66.top

[E17] 首字母大写
来源：http://xri.zdbjq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sdp.andypj.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://pdv.ehwqpu.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wgm.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wvc.yj20258888.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://doq.quarkkingdee.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wfn.bbcook.cn

Ruby: s.capitalize
来源：http://pbp.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://imj.hywenlv.cn

[E18] 模板占位符替换
来源：http://hud.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xhp.yonumen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://chu.yj202588.top

JS:   tpl.replaceAll("{name}", name)
来源：http://fmf.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rfe.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gzb.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tky.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kdg.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ket.hfpthk.cn

[E19] 多行文本按行拆分
来源：http://qpw.uphjek.com

Py:   s.splitlines()
来源：http://cyw.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://juz.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://cyn.yonumen.top

TS:   s.split(/\r?\n/)
来源：http://xkd.snrcjt.cn

Java: s.lines().toList()
来源：http://gru.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://rha.kuanghao11.cn

Ruby: s.lines
来源：http://kje.zhijiandao.cn

C#:   s.Split('\n')
来源：http://kqg.yueranfly.top

[E20] 判断字符串是否为空
来源：http://yuq.xziqi.cn

Py:   if not s:
来源：http://yxy.svipenyu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ilx.yangfankeji.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fok.zhijiandao.cn

TS:   if (s === "") {}
来源：http://tnf.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://hdb.redwolf501.top

Go:   if s == "" {}
来源：http://wdp.gzhubu.top

Ruby: if s.empty?
来源：http://erl.tianlin.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bhj.zycfv.cn

[E21] 超长截断加省略号
来源：http://khj.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fvu.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yit.gotoacloud.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdf.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fff.iojbl.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://csm.zhoulong.xyz

Go:   // 按 rune 判断长度后截断
来源：http://tis.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nry.hfpthk.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eaa.dianchejie.cn

[E22] 字节长度与字符长度
来源：http://gpl.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://adm.shanyushiyangkeji.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lzx.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pow.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gyv.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uwm.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cgy.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://ytf.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vmj.yj20258888.top

================================================================================
来源：http://lyj.zhixingplan.top

F. 文件与目录
来源：http://eku.ybcxt.top

================================================================================
来源：http://xvm.yanxiufei.cn

[F01] 读取整个文件
来源：http://ymi.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ybz.feifeiyinyue.top

PHP:  file_get_contents("a.txt");
来源：http://xxk.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vff.jinqigufen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yjp.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://whm.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rli.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://kms.cdnleiting.top

C#:   File.ReadAllText("a.txt");
来源：http://hyw.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://xwo.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iod.yj20258888.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uar.cashguo.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdz.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ccx.yanxiufei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gnk.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ymw.jyoumei.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ppj.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xjr.svipenyu.cn

[F03] 写入文件（覆盖）
来源：http://iqv.smart0.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ylk.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jui.hammf.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lty.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wgd.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tjo.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kgx.hongshengwenyu.top

Ruby: File.write("a.txt", "hi")
来源：http://hms.9152youxi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hyz.sufxvd.cn

[F04] 追加写入文件
来源：http://pql.daria6918.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yxt.tarul.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://iyy.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qzg.guannengcc.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://igr.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://smi.hesvh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vqp.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bvc.vqdsnc.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wut.yj20258.top

[F05] 判断文件或目录是否存在
来源：http://keb.tian-w.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tuf.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://umc.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://uxb.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://ufu.vehdjk.com

Java: Files.exists(Path.of("a.txt"))
来源：http://fnj.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fkk.zhengqikj.top

Ruby: File.exist?("a.txt")
来源：http://ffn.zhijiandao.cn

C#:   File.Exists("a.txt")
来源：http://dhp.yfazqb.com

[F06] 删除文件
来源：http://jvg.svipenyu.cn

Py:   os.remove("a.txt")
来源：http://cza.gogol.net.cn

PHP:  unlink("a.txt");
来源：http://ybo.yj202588.top

JS:   fs.unlinkSync("a.txt")
来源：http://stn.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://lvf.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lov.hesvh.cn

Go:   os.Remove("a.txt")
来源：http://ehe.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://nrf.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://pxx.yuxming.cn

[F07] 创建目录（含多级）
来源：http://izl.sjlbkw.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://svn.daria6918.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lvm.kuanghao11.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pgk.jqgufenzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://way.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fjn.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xju.meibo888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqh.yfazqb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rhj.xinyue.icu

[F08] 遍历目录
来源：http://ouq.zhijiandao.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hdj.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://itm.gaohongyu789.top

JS:   fs.readdirSync("dir")
来源：http://vck.316326.xyz

TS:   fs.readdirSync("dir")
来源：http://psr.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fqi.hfpthk.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ygs.nanxuanxn.top

Ruby: Dir.children("dir")
来源：http://rrv.fengsongda.top

C#:   Directory.GetFiles("dir")
来源：http://kjx.snrcjt.cn

[F09] 获取文件大小
来源：http://nfa.xuetiantiany.cn

Py:   os.path.getsize("a.txt")
来源：http://wsl.smart0.xyz

PHP:  filesize("a.txt");
来源：http://mjx.bjfxy.top

JS:   fs.statSync("a.txt").size
来源：http://kws.nwbrower.top

TS:   fs.statSync("a.txt").size
来源：http://sal.ybcxt.top

Java: Files.size(Path.of("a.txt"))
来源：http://ory.yuxming.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qvu.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://ttm.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://afr.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://hfw.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hkq.zycfv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bxr.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jfk.epnwcf.com

TS:   path.extname("a.txt")
来源：http://duq.shanyushiyangtech.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://krq.jyoumei.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ora.ctjpmb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://loz.daria6918.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cvo.cheryme.top

[F11] 复制与移动文件
来源：http://qxa.chenlongwang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jvj.0kj1m.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fai.xingfuxueyuan.xyz

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hac.0kj1m.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://idg.guannengcc.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gaz.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ktg.jqgfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dwu.yj20258.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpn.redwolf501.top

[F12] CSV 读写
来源：http://hdt.smart0.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rja.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://owb.jinqigfzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eax.sysykeji.top

TS:   // 同上
来源：http://jif.cucudq.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ezv.yj20258888.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qdn.tanke756.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hzi.ctjpmb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://sep.fehbvm.com

================================================================================
来源：http://kvg.zhixingplan.top

G. 面向对象
来源：http://cft.cqqwz.cn

================================================================================
来源：http://rvx.yueranfly.top

[G01] 定义类
来源：http://yja.guowangkeji.top

Py:   class User: pass
来源：http://djc.jinqigufen.top

PHP:  class User {}
来源：http://oty.jlsjyb.cn

JS:   class User {}
来源：http://ydh.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://msk.chenlongwang.top

Java: class User {}
来源：http://xhf.ehwqpu.com

Go:   type User struct { Name string }
来源：http://qmg.hongshengwenyu.top

Ruby: class User; end
来源：http://jco.sweek.top

C#:   class User {}
来源：http://eax.sjlbkw.cn

[G02] 构造函数
来源：http://aly.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://qib.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://wpt.aizwys.cn

JS:   constructor(name) { this.name = name; }
来源：http://qke.yongpay.top

TS:   constructor(public name: string) {}
来源：http://ksc.zhaomingkeji.xyz

Java: User(String name) { this.name = name; }
来源：http://ewk.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dll.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://hss.wangshuangyany.cn

C#:   public User(string name) { Name = name; }
来源：http://icg.ydzc1.top

[G03] 实例属性
来源：http://oml.iojbl.cn

Py:   self.name = "x"
来源：http://znb.dianchejie.cn

PHP:  public string $name = "x";
来源：http://wqy.redwolf501.top

JS:   this.name = "x";
来源：http://irj.xylfe.cn

TS:   name: string = "x";
来源：http://byr.zhoulong.xyz

Java: private String name;
来源：http://qtn.shanyushiyangkeji.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tqx.ybcxt.top

Ruby: @name = "x"
来源：http://hkl.yonumen.top

C#:   public string Name { get; set; } = "x";
来源：http://yrh.epnwcf.com

[G04] 定义方法
来源：http://xbe.uphjek.com

Py:   def greet(self): return self.name
来源：http://tpo.jinqigufen.top

PHP:  public function greet(): string { return $this->name; }
来源：http://pcp.tanke756.top

JS:   greet() { return this.name; }
来源：http://tqy.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://zfk.jqgfzy.top

Java: String greet() { return name; }
来源：http://cdb.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://rta.jinqigfzy.top

Ruby: def greet; @name; end
来源：http://kxr.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://sxw.epnwcf.com

[G05] 继承
来源：http://xra.yvedp.cn

Py:   class Admin(User): pass
来源：http://ljo.bbcook.cn

PHP:  class Admin extends User {}
来源：http://mhf.nanxuanxn.top

JS:   class Admin extends User {}
来源：http://hgd.snrcjt.cn

TS:   class Admin extends User {}
来源：http://unw.havefunace.top

Java: class Admin extends User {}
来源：http://rvc.nwbrower.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rdg.cdnleiting.top

Ruby: class Admin < User; end
来源：http://lya.jinqigfzy.top

C#:   class Admin : User {}
来源：http://bgw.aibaodan.cn

[G06] 重写方法
来源：http://vth.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://wad.jinqigufen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://czs.shzxlz.cn

JS:   greet() { return "admin"; }
来源：http://mqv.shanyushiyangkeji.top

TS:   greet(): string { return "admin"; }
来源：http://jwf.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://vpa.zhoulong.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ibh.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://qte.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://tng.yj20258888.top

[G07] 调用父类方法
来源：http://kok.yuxming.cn

Py:   super().greet()
来源：http://tuq.sweek.top

PHP:  parent::greet();
来源：http://fmw.shuidangran.top

JS:   super.greet();
来源：http://pdf.shzxlz.cn

TS:   super.greet();
来源：http://vwy.fengsongda.top

Java: super.greet();
来源：http://xno.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bzp.guannengcc.top

Ruby: super
来源：http://pth.yj202588.top

C#:   base.Greet();
来源：http://yki.ybcxt.top

[G08] 静态方法与属性
来源：http://opc.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qks.vqdsnc.cn

PHP:  public static function f() {}
来源：http://kwo.hammf.cn

JS:   static f() {}
来源：http://cxs.chenjidiqi.icu

TS:   static f(): void {}
来源：http://cty.yonumen.top

Java: static void f() {}
来源：http://zvd.jlsjyb.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zit.haohaochexian.top

Ruby: def self.f; end
来源：http://qsk.nanxuanxn.top

C#:   public static void F() {}
来源：http://bjh.fehbvm.com

[G09] 接口 / 抽象类
来源：http://noi.guowangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://sel.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://yjl.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://njz.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://qog.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://ekp.ybcxt.top

Go:   type Shape interface { Area() float64 }
来源：http://upi.316326.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tsk.svipenyu.cn

C#:   interface IShape { double Area(); }
来源：http://btl.zhoulong.xyz

[G10] 访问控制
来源：http://arc.zhiwuduotai.top

Py:   约定 _protected / __private（不强制）
来源：http://cvj.hesvh.cn

PHP:  public / protected / private
来源：http://ecx.cqqwz.cn

JS:   #private 字段；其余公开
来源：http://xca.hfpthk.cn

TS:   public / protected / private
来源：http://nug.xuanzx.com

Java: public / protected / private / 默认包级
来源：http://iet.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ydj.fengsongda.top

Ruby: public / protected / private
来源：http://ugu.zhixingplan.top

C#:   public / protected / private / internal
来源：http://rto.9152youxi.cn

[G11] getter / setter
来源：http://dys.fengsongda.top

Py:   @property 与 @x.setter
来源：http://exu.haohaochexian.top

PHP:  public function getName(): string { return $this->name; }
来源：http://qya.tian-w.cn

JS:   get name() { return this._name; }
来源：http://kbp.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://hif.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://gvu.havefunace.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ezw.cucudq.cn

Ruby: attr_accessor :name
来源：http://rvs.jiagoushi.top

C#:   public string Name { get; set; }
来源：http://upz.sweek.top

[G12] 对象转字符串
来源：http://eiz.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://lwx.xinyue.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://jxm.tianlin.xyz

JS:   toString() { return this.name; }
来源：http://smj.hammf.cn

TS:   toString(): string { return this.name; }
来源：http://idi.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://peg.jinghuilouyu.cn


<!-- 参考信息 -->