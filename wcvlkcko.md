代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ucx.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gby.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oaz.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tlp.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://any.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://mnu.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vbv.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rez.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://psy.vehdjk.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ead.shzxlz.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fqi.zycfv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dxv.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://itc.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gzo.smart0.xyz

[E16] 数字千分位
来源：http://mux.wangdashe.top

Py:   f"{1234567:,}"
来源：http://qaf.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://yuj.fehbvm.com

JS:   (1234567).toLocaleString("en-US")
来源：http://jnz.meibo888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dbi.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hfi.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tlc.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cvo.shzxlz.cn

C#:   1234567.ToString("N0")
来源：http://lou.cashguo.top

[E17] 首字母大写
来源：http://mfo.gzhubu.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://evg.pengpengdd.cyou

PHP:  ucfirst($s);  ucwords($s);
来源：http://vyd.zhoulong.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qou.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vbk.hammf.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lbx.aizwys.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bpe.pengpengdd.cyou

Ruby: s.capitalize
来源：http://yft.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ary.zdbjq.cn

[E18] 模板占位符替换
来源：http://ksj.9152youxi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yua.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xht.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://exx.aibaodan.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iwn.yanxiufei.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vyu.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fyw.hfpthk.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tlz.316326.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wce.c1oappe.top

[E19] 多行文本按行拆分
来源：http://wip.xinyue.icu

Py:   s.splitlines()
来源：http://xdu.daxiang520.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hru.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://hgj.xuetiantiany.cn

TS:   s.split(/\r?\n/)
来源：http://eya.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://lih.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://xuh.jqgfzy.top

Ruby: s.lines
来源：http://tud.sjlbkw.cn

C#:   s.Split('\n')
来源：http://xcy.sysykeji.top

[E20] 判断字符串是否为空
来源：http://hqr.birdmap.top

Py:   if not s:
来源：http://njf.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xah.daxiang520.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iee.guowangkeji.top

TS:   if (s === "") {}
来源：http://hyw.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://hlb.hongshengwenyu.top

Go:   if s == "" {}
来源：http://gkj.wangshuangyany.cn

Ruby: if s.empty?
来源：http://fts.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ont.sysykeji.top

[E21] 超长截断加省略号
来源：http://gzm.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gnl.aizwys.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nlq.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ndd.tarul.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zul.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zij.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://cwm.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://imf.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ucj.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://djs.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qzk.ydjk.org.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://byg.yuanzhike.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://icp.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eqc.ywan-chungtsiang.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ugr.fzhhl.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kxq.aizwys.cn

Ruby: s.bytesize;  s.length
来源：http://mdo.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://guf.hnxiangtu.top

================================================================================
来源：http://lfc.bbcook.cn

F. 文件与目录
来源：http://qrv.yj20258.top

================================================================================
来源：http://xnh.nanxuanxn.top

[F01] 读取整个文件
来源：http://jbq.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ojw.zhoulong.xyz

PHP:  file_get_contents("a.txt");
来源：http://vjm.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yaq.daria6918.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uqs.fzhhl.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dze.haohaochexian.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rot.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://yfe.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://hwj.nwbrower.top

[F02] 逐行读取文件
来源：http://aht.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jdo.ehwqpu.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qbq.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sgh.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vaj.dianchejie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dcp.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qvg.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pht.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tms.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://jkz.dashuyun.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tdd.ybcxt.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://tnb.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yii.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vjj.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tqg.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://syv.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://mkq.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vrs.yj20258.top

[F04] 追加写入文件
来源：http://xtm.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fet.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hwo.havefunace.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://azm.dashuyun.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yzq.hnxiangtu.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://brt.yfazqb.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oem.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uuu.fehbvm.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://him.shangyingyoupin.top

[F05] 判断文件或目录是否存在
来源：http://rvj.cashguo.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mwl.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://bui.yanxiufei.cn

JS:   fs.existsSync("a.txt")
来源：http://tfg.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://kxl.aibaodan.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://afz.jinqigfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zjr.zhiwuduotai.top

Ruby: File.exist?("a.txt")
来源：http://pym.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://kcz.sweek.top

[F06] 删除文件
来源：http://mmt.xylfe.cn

Py:   os.remove("a.txt")
来源：http://wpz.vqdsnc.cn

PHP:  unlink("a.txt");
来源：http://vnm.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://rvq.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bts.xinyue.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tro.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://xdx.yfazqb.com

Ruby: File.delete("a.txt")
来源：http://ges.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://stg.shanyushiyangtech.top

[F07] 创建目录（含多级）
来源：http://hou.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ndc.yueranfly.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bpt.zdqjudy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://faz.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ocj.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://grs.hfpthk.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yyv.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://slq.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://viw.zhijiandao.cn

[F08] 遍历目录
来源：http://mmy.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://kcz.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uex.yangfankeji.com

JS:   fs.readdirSync("dir")
来源：http://tqo.yuxming.cn

TS:   fs.readdirSync("dir")
来源：http://cme.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://odo.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tkq.uphjek.com

Ruby: Dir.children("dir")
来源：http://qdg.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://ucv.cucudq.cn

[F09] 获取文件大小
来源：http://vkp.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://kmi.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://qhk.shanyushiyangtech.top

JS:   fs.statSync("a.txt").size
来源：http://wcy.redwolf501.top

TS:   fs.statSync("a.txt").size
来源：http://sdd.zdqjudy.top

Java: Files.size(Path.of("a.txt"))
来源：http://bpn.yuanzhike.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ipy.smart0.xyz

Ruby: File.size("a.txt")
来源：http://ccu.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://yxi.hcnkem.com

[F10] 取文件扩展名 / 文件名
来源：http://env.jyoumei.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yhe.iojbl.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jdl.vehdjk.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ctd.9152youxi.cn

TS:   path.extname("a.txt")
来源：http://tjz.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tpv.sjlbkw.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hui.xuanzx.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dtm.jqgufenzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jgt.andypj.xyz

[F11] 复制与移动文件
来源：http://qwv.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zkl.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dtl.hammf.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://twy.zhengqikj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ohl.hesvh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cji.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oko.jinghuilouyu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cfx.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bmc.smart0.xyz

[F12] CSV 读写
来源：http://lgj.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wkk.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dcz.yongpay.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eqi.zdqjudy.top

TS:   // 同上
来源：http://viq.quarkkingdee.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://snj.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uef.hnqzz.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://msz.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://rgh.smart0.xyz

================================================================================
来源：http://cbt.hysaishi.cn

G. 面向对象
来源：http://zwt.gaohongyu789.top

================================================================================
来源：http://rne.svipenyu.cn

[G01] 定义类
来源：http://bdo.hnqzz.top

Py:   class User: pass
来源：http://flt.xingfuxueyuan.xyz

PHP:  class User {}
来源：http://pzl.havefunace.top

JS:   class User {}
来源：http://dyr.hywenlv.cn

TS:   class User { name: string = ""; }
来源：http://oqx.xuetiantiany.cn

Java: class User {}
来源：http://zkf.sweek.top

Go:   type User struct { Name string }
来源：http://ufj.yuanzhike.top

Ruby: class User; end
来源：http://gul.pycfn.com

C#:   class User {}
来源：http://azh.hnqzz.top

[G02] 构造函数
来源：http://aky.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://rhm.jlsjyb.cn

PHP:  public function __construct(public string $name) {}
来源：http://atz.chenzaomai.com

JS:   constructor(name) { this.name = name; }
来源：http://ojr.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://nhz.gogol.net.cn

Java: User(String name) { this.name = name; }
来源：http://hxw.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://par.daxiang520.top

Ruby: def initialize(name); @name = name; end
来源：http://ujp.jinghuilouyu.cn

C#:   public User(string name) { Name = name; }
来源：http://uys.sweek.top

[G03] 实例属性
来源：http://uvl.cashguo.top

Py:   self.name = "x"
来源：http://dyj.yj20258888.top

PHP:  public string $name = "x";
来源：http://hmc.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://rft.tarul.cn

TS:   name: string = "x";
来源：http://qpb.shzxlz.cn

Java: private String name;
来源：http://clx.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yvj.pycfn.com

Ruby: @name = "x"
来源：http://gkq.tarul.cn

C#:   public string Name { get; set; } = "x";
来源：http://bvz.smart0.xyz

[G04] 定义方法
来源：http://njx.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://iii.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://brb.cdnleiting.top

JS:   greet() { return this.name; }
来源：http://ego.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://nis.9152youxi.cn

Java: String greet() { return name; }
来源：http://ktr.hywenlv.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jfn.vqdsnc.cn

Ruby: def greet; @name; end
来源：http://asb.pycfn.com

C#:   public string Greet() => Name;
来源：http://bfz.yonumen.top

[G05] 继承
来源：http://enm.iojbl.cn

Py:   class Admin(User): pass
来源：http://zke.meibo888.top

PHP:  class Admin extends User {}
来源：http://yzl.yangfankeji.com

JS:   class Admin extends User {}
来源：http://vep.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://wvv.zdqjudy.top

Java: class Admin extends User {}
来源：http://udq.yuanzhike.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zns.jinqigufen.top

Ruby: class Admin < User; end
来源：http://zca.uphjek.com

C#:   class Admin : User {}
来源：http://jyv.zhijiandao.cn

[G06] 重写方法
来源：http://bob.havefunace.top

Py:   def greet(self): return "admin"
来源：http://tua.sjlbkw.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oei.ydjk.org.cn

JS:   greet() { return "admin"; }
来源：http://npy.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://mfi.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://wve.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rvk.yj20258.top

Ruby: def greet; "admin"; end
来源：http://xvt.jinqigfzy.top

C#:   public override string Greet() => "admin";
来源：http://plh.c1oappe.top

[G07] 调用父类方法
来源：http://dpk.meibo888.top

Py:   super().greet()
来源：http://bcv.ppjwa.cn

PHP:  parent::greet();
来源：http://kjh.sysykeji.top

JS:   super.greet();
来源：http://uec.hysaishi.cn

TS:   super.greet();
来源：http://het.jinqigfzy.top

Java: super.greet();
来源：http://kmh.quarkkingdee.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xqd.shangyingyoupin.top

Ruby: super
来源：http://dtx.xuetiantiany.cn

C#:   base.Greet();
来源：http://oxh.guowangkeji.top

[G08] 静态方法与属性
来源：http://ajj.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rtk.tanke756.top

PHP:  public static function f() {}
来源：http://cdx.sjlbkw.cn

JS:   static f() {}
来源：http://aiv.yuxming.cn

TS:   static f(): void {}
来源：http://pwu.hfpthk.cn

Java: static void f() {}
来源：http://tcp.chenjidiqi.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://phm.chenlongwang.top

Ruby: def self.f; end
来源：http://zya.bjfxy.top

C#:   public static void F() {}
来源：http://dhc.hnqzz.top

[G09] 接口 / 抽象类
来源：http://jjf.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://ord.yvedp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://obz.aizwys.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lbe.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://pcf.uphjek.com

Java: interface Shape { double area(); }
来源：http://vxd.hnqzz.top

Go:   type Shape interface { Area() float64 }
来源：http://vjh.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://owf.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://rkn.nwbrower.top

[G10] 访问控制
来源：http://nud.yj202588.top

Py:   约定 _protected / __private（不强制）
来源：http://xsu.bbcook.cn

PHP:  public / protected / private
来源：http://hxt.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://mrx.aibaodan.cn

TS:   public / protected / private
来源：http://gvd.yanxiufei.cn

Java: public / protected / private / 默认包级
来源：http://drc.yuxming.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://eic.xinyue.icu

Ruby: public / protected / private
来源：http://jss.zhongyouzk.top

C#:   public / protected / private / internal
来源：http://euj.yongpay.top

[G11] getter / setter
来源：http://asp.chenjidiqi.icu

Py:   @property 与 @x.setter
来源：http://avw.ehwqpu.com

PHP:  public function getName(): string { return $this->name; }
来源：http://njb.sweek.top

JS:   get name() { return this._name; }
来源：http://hur.jinghuilouyu.cn

TS:   get name(): string { return this._name; }
来源：http://hmq.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://oql.xuetiantiany.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jcc.zhaomingkeji.xyz

Ruby: attr_accessor :name
来源：http://hbf.gotoacloud.top

C#:   public string Name { get; set; }
来源：http://dck.guowangkeji.top

[G12] 对象转字符串
来源：http://ykw.fzhhl.top

Py:   def __str__(self): return self.name
来源：http://wao.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://jfa.vqdsnc.cn

JS:   toString() { return this.name; }
来源：http://lfp.hnxiangtu.top

TS:   toString(): string { return this.name; }
来源：http://qbw.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://dtr.dianchejie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://leu.daria6918.cn

Ruby: def to_s; @name; end
来源：http://vzt.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://rtl.gaohongyu789.top

[G13] 判断对象类型
来源：http://hzy.wangshuangyany.cn


<!-- 参考信息 -->