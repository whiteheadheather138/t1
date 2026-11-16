代发 wailian999

[E14] URL 编码与 Base64
来源：http://kcs.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tjz.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://wgf.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bmu.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://boh.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tax.shzxlz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ehv.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kyn.chenlongwang.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ptw.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://upf.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sri.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jic.yanxiufei.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pjw.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://moo.yfazqb.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://brg.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://svu.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ute.yanxiufei.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zwb.sweek.top

[E16] 数字千分位
来源：http://gcn.andypj.xyz

Py:   f"{1234567:,}"
来源：http://nzk.zhaomingkeji.xyz

PHP:  number_format(1234567);
来源：http://nxt.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://urc.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://mcg.yj202588.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cha.birdmap.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hui.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ztd.havefunace.top

C#:   1234567.ToString("N0")
来源：http://hdd.jinghuilouyu.cn

[E17] 首字母大写
来源：http://vca.ybcxt.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oyg.ybcxt.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://zcd.chenzaomai.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://npy.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sqz.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://szw.ctjpmb.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ylk.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://awn.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dls.fehbvm.com

[E18] 模板占位符替换
来源：http://jvm.xingfuxueyuan.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vlk.zhijiandao.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rdk.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zvx.sufxvd.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://luj.smart0.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zte.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yik.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wmv.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aav.ywan-chungtsiang.top

[E19] 多行文本按行拆分
来源：http://zqq.daria6918.cn

Py:   s.splitlines()
来源：http://mwu.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xds.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://lyb.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://feq.tanke756.top

Java: s.lines().toList()
来源：http://wyh.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://hgr.wangshuangyany.cn

Ruby: s.lines
来源：http://zxf.jlsjyb.cn

C#:   s.Split('\n')
来源：http://wzk.shzxlz.cn

[E20] 判断字符串是否为空
来源：http://yul.xylfe.cn

Py:   if not s:
来源：http://dxx.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://llm.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dds.xuanzx.com

TS:   if (s === "") {}
来源：http://zjx.fanxiaobao.xyz

Java: if (s.isEmpty()) {}
来源：http://dvz.daxiang520.top

Go:   if s == "" {}
来源：http://cyx.yuanzhike.top

Ruby: if s.empty?
来源：http://pvv.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eqk.316326.xyz

[E21] 超长截断加省略号
来源：http://ftp.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sff.dianchejie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cfb.yonumen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vtn.hnqzz.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jhv.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ymg.xingfuxueyuan.xyz

Go:   // 按 rune 判断长度后截断
来源：http://vfv.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ntx.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ojz.nanxinkj.top

[E22] 字节长度与字符长度
来源：http://lqk.shuidangran.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://aau.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zbk.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dnr.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkg.zhengqikj.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vmv.yongpay.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cxu.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://bpi.ctjpmb.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lmx.kuanghao11.cn

================================================================================
来源：http://qud.xuetiantiany.cn

F. 文件与目录
来源：http://dji.xingfuxueyuan.xyz

================================================================================
来源：http://len.fktsv.cn

[F01] 读取整个文件
来源：http://bxa.kuanghao11.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qqa.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://omb.guowangkeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hcl.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iwm.cucudq.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://obv.fanxiaobao.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hes.tarul.cn

Ruby: File.read("a.txt")
来源：http://fcv.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://aiy.hammf.cn

[F02] 逐行读取文件
来源：http://lde.zhiwuduotai.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ldp.tanke756.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zox.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dat.hnxiangtu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wpx.hcnkem.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tiw.xziqi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lxq.hesvh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wue.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://yuu.tarul.cn

[F03] 写入文件（覆盖）
来源：http://xrs.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://igl.xuanzx.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ozk.hesvh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://imy.sysykeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xzr.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tjj.hfpthk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dnm.hnxiangtu.top

Ruby: File.write("a.txt", "hi")
来源：http://czb.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zxa.tarul.cn

[F04] 追加写入文件
来源：http://tiz.hywenlv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qcc.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dol.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iom.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nyo.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://feg.yangfankeji.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bvk.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zhs.52xcode.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wjz.sufxvd.cn

[F05] 判断文件或目录是否存在
来源：http://vtz.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lhk.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://kdf.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://iue.epnwcf.com

TS:   fs.existsSync("a.txt")
来源：http://dvd.xziqi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cyg.jianghu66.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://exi.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://wgi.hnqzz.top

C#:   File.Exists("a.txt")
来源：http://pdg.xziqi.cn

[F06] 删除文件
来源：http://gyx.tarul.cn

Py:   os.remove("a.txt")
来源：http://qpj.xziqi.cn

PHP:  unlink("a.txt");
来源：http://tfh.ehwqpu.com

JS:   fs.unlinkSync("a.txt")
来源：http://als.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://nfm.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mbk.shangyingyoupin.top

Go:   os.Remove("a.txt")
来源：http://rgj.ivvv.top

Ruby: File.delete("a.txt")
来源：http://gxf.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://gom.ppjwa.cn

[F07] 创建目录（含多级）
来源：http://myn.ydzc1.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tsi.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lun.daxiang520.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vql.tian-w.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fay.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lyz.jiagoushi.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gey.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nfa.yvedp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mni.zhongyouzk.top

[F08] 遍历目录
来源：http://gbl.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://epr.jlsjyb.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eao.kuanghao11.cn

JS:   fs.readdirSync("dir")
来源：http://joa.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://ftj.gogol.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vmc.316326.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://ihp.fanxiaobao.xyz

Ruby: Dir.children("dir")
来源：http://mio.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://jft.svipenyu.cn

[F09] 获取文件大小
来源：http://qyf.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://nsi.mhx1999.top

PHP:  filesize("a.txt");
来源：http://qgp.andypj.xyz

JS:   fs.statSync("a.txt").size
来源：http://wec.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://exc.jinqigufen.top

Java: Files.size(Path.of("a.txt"))
来源：http://smx.jlsjyb.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://usv.nwbrower.top

Ruby: File.size("a.txt")
来源：http://wiz.jinqigufen.top

C#:   new FileInfo("a.txt").Length
来源：http://byd.jqgufenzy.top

[F10] 取文件扩展名 / 文件名
来源：http://lbk.sysykeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://arr.mhx1999.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://myj.jinqigfzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yoh.yuanzhike.top

TS:   path.extname("a.txt")
来源：http://wre.ctjpmb.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tpq.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ixa.xuetiantiany.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zre.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gny.ydjk.org.cn

[F11] 复制与移动文件
来源：http://jen.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vet.dianchejie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ncj.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dvv.sjlbkw.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pkg.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dms.cucudq.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://glw.yueranfly.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gma.tanke756.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bsl.sxryk.cn

[F12] CSV 读写
来源：http://vdf.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ohq.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://crn.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mvz.cheryme.top

TS:   // 同上
来源：http://vix.shzxlz.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bun.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lkb.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://irk.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://yjf.pengpengdd.cyou

================================================================================
来源：http://wwx.aibaodan.cn

G. 面向对象
来源：http://pma.yfazqb.com

================================================================================
来源：http://ipl.shzxlz.cn

[G01] 定义类
来源：http://ldt.zhengqikj.top

Py:   class User: pass
来源：http://rfy.dianchejie.cn

PHP:  class User {}
来源：http://xzv.hysaishi.cn

JS:   class User {}
来源：http://xnt.nanxinkj.top

TS:   class User { name: string = ""; }
来源：http://jzd.cashguo.top

Java: class User {}
来源：http://enn.hysaishi.cn

Go:   type User struct { Name string }
来源：http://eev.zhengqikj.top

Ruby: class User; end
来源：http://nkc.hywenlv.cn

C#:   class User {}
来源：http://bmo.ivvv.top

[G02] 构造函数
来源：http://tcg.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://ugo.yfazqb.com

PHP:  public function __construct(public string $name) {}
来源：http://eep.yuanzhike.top

JS:   constructor(name) { this.name = name; }
来源：http://zur.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://zdb.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://nls.c1oappe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lxd.pengpengdd.cyou

Ruby: def initialize(name); @name = name; end
来源：http://xtd.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://uqq.xingfuxueyuan.xyz

[G03] 实例属性
来源：http://bwo.zhijiandao.cn

Py:   self.name = "x"
来源：http://gth.yongpay.top

PHP:  public string $name = "x";
来源：http://yct.vehdjk.com

JS:   this.name = "x";
来源：http://jsc.shangyingyoupin.top

TS:   name: string = "x";
来源：http://fcx.pycfn.com

Java: private String name;
来源：http://ebl.bjfxy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hns.aizwys.cn

Ruby: @name = "x"
来源：http://blk.jlsjyb.cn

C#:   public string Name { get; set; } = "x";
来源：http://ntm.yj202588.top

[G04] 定义方法
来源：http://ytg.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://ayv.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vfp.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://yht.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://fzs.hfpthk.cn

Java: String greet() { return name; }
来源：http://fug.jinqigfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yff.hongshengwenyu.top

Ruby: def greet; @name; end
来源：http://gms.yj20258888.top

C#:   public string Greet() => Name;
来源：http://nqn.shangyingyoupin.top

[G05] 继承
来源：http://fmr.yanxiufei.cn

Py:   class Admin(User): pass
来源：http://wbp.sysykeji.top

PHP:  class Admin extends User {}
来源：http://uzh.gzhubu.top

JS:   class Admin extends User {}
来源：http://fhs.gzhubu.top

TS:   class Admin extends User {}
来源：http://gki.havefunace.top

Java: class Admin extends User {}
来源：http://tqz.zhixingplan.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xws.cheryme.top

Ruby: class Admin < User; end
来源：http://ndj.jqgfzy.top

C#:   class Admin : User {}
来源：http://wae.uphjek.com

[G06] 重写方法
来源：http://ztu.yueranfly.top

Py:   def greet(self): return "admin"
来源：http://qxi.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uso.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://ebm.yueranfly.top

TS:   greet(): string { return "admin"; }
来源：http://jzi.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://bzv.zhongyouzk.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ddt.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://tsm.zdqjudy.top

C#:   public override string Greet() => "admin";
来源：http://toe.shzxlz.cn

[G07] 调用父类方法
来源：http://evi.zdqjudy.top

Py:   super().greet()
来源：http://kyb.zhixingplan.top

PHP:  parent::greet();
来源：http://uzr.tianlin.xyz

JS:   super.greet();
来源：http://uzu.tian-w.cn

TS:   super.greet();
来源：http://hny.tianlin.xyz

Java: super.greet();
来源：http://dky.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nbq.zdbjq.cn

Ruby: super
来源：http://tvx.9152youxi.cn

C#:   base.Greet();
来源：http://idk.hcnkem.com

[G08] 静态方法与属性
来源：http://drw.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gej.gotoacloud.top

PHP:  public static function f() {}
来源：http://pnw.shanyushiyangkeji.top

JS:   static f() {}
来源：http://ndq.shuidangran.top

TS:   static f(): void {}
来源：http://apg.feifeiyinyue.top

Java: static void f() {}
来源：http://dad.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nlq.shuidangran.top

Ruby: def self.f; end
来源：http://zvn.jiagoushi.top

C#:   public static void F() {}
来源：http://dbc.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://zhj.uphjek.com

Py:   from abc import ABC, abstractmethod
来源：http://gak.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://tmd.nanxuanxn.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://hgd.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://mtd.kuanghao11.cn

Java: interface Shape { double area(); }
来源：http://sdj.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://vah.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ygx.yj20258.top

C#:   interface IShape { double Area(); }
来源：http://mdx.jyoumei.cn

[G10] 访问控制
来源：http://ooo.shanyushiyangkeji.top

Py:   约定 _protected / __private（不强制）
来源：http://pnt.gzhubu.top

PHP:  public / protected / private
来源：http://qrk.0kj1m.cn

JS:   #private 字段；其余公开
来源：http://ogs.zdbjq.cn

TS:   public / protected / private
来源：http://cjg.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://yyi.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fij.cashguo.top

Ruby: public / protected / private
来源：http://jfv.pengpengdd.cyou

C#:   public / protected / private / internal
来源：http://rwz.kuanghao11.cn

[G11] getter / setter
来源：http://wtq.yangfankeji.com

Py:   @property 与 @x.setter
来源：http://qbe.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ivy.redwolf501.top

JS:   get name() { return this._name; }
来源：http://hfl.zycfv.cn

TS:   get name(): string { return this._name; }
来源：http://ita.andypj.xyz

Java: public String getName() { return name; }
来源：http://hfl.shanyushiyangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://zvm.dianchejie.cn

Ruby: attr_accessor :name
来源：http://qjg.andypj.xyz

C#:   public string Name { get; set; }
来源：http://reg.ybcxt.top

[G12] 对象转字符串
来源：http://jnq.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://nfs.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://cla.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://dcu.bbcook.cn

TS:   toString(): string { return this.name; }
来源：http://okc.jianghu66.top

Java: @Override public String toString() { return name; }
来源：http://uxe.bbcook.cn


<!-- 参考信息 -->