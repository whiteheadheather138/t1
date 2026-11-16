代发 wailian999

PHP:  substr_count($s, "a");
来源：http://fuy.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://bju.ydjk.org.cn

TS:   s.split("a").length - 1
来源：http://irb.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://abh.fehbvm.com

Go:   strings.Count(s, "a")
来源：http://okl.andypj.xyz

Ruby: s.count("a")
来源：http://ldb.vehdjk.com

C#:   s.Count(c => c == 'a')
来源：http://wgp.aizwys.cn

[E13] 逐字符遍历
来源：http://peu.zhengqikj.top

Py:   for ch in s: print(ch)
来源：http://mob.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kxs.nanxuanxn.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ijf.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://svu.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iug.hongshengwenyu.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ano.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://brj.mhx1999.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mlf.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://aog.xylfe.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qkx.epnwcf.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ims.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lof.cqqwz.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xsn.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bgx.fzhhl.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tlp.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iyr.uphjek.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ser.nwbrower.top

[E15] HTML 转义 / 反转义
来源：http://kjp.uphjek.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xox.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://esc.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gil.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ggo.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xsk.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fgm.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://auz.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kkv.epnwcf.com

[E16] 数字千分位
来源：http://hcl.ydjk.org.cn

Py:   f"{1234567:,}"
来源：http://huv.meibo888.top

PHP:  number_format(1234567);
来源：http://wkb.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://wpw.svipenyu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://omr.nanxinkj.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ufz.gogol.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fow.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dgy.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://zbw.316326.xyz

[E17] 首字母大写
来源：http://gdm.ivvv.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lvz.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ckv.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://njy.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zhn.sxryk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pxd.cdnleiting.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gdm.cashguo.top

Ruby: s.capitalize
来源：http://qqg.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fcd.ivvv.top

[E18] 模板占位符替换
来源：http://fnd.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lat.hammf.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bpb.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xvi.bbcook.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://otw.hnxiangtu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gkl.uphjek.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xqw.aizwys.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iqb.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wsm.nwbrower.top

[E19] 多行文本按行拆分
来源：http://kqo.tarul.cn

Py:   s.splitlines()
来源：http://jon.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://roo.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://ijd.vehdjk.com

TS:   s.split(/\r?\n/)
来源：http://tox.hammf.cn

Java: s.lines().toList()
来源：http://alt.shanyushiyangkeji.top

Go:   strings.Split(s, "\n")
来源：http://xbp.vehdjk.com

Ruby: s.lines
来源：http://xjd.ehwqpu.com

C#:   s.Split('\n')
来源：http://kpm.hesvh.cn

[E20] 判断字符串是否为空
来源：http://dbp.jiagoushi.top

Py:   if not s:
来源：http://eim.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ysr.gzhubu.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yrj.chenzaomai.com

TS:   if (s === "") {}
来源：http://bxh.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://etj.andypj.xyz

Go:   if s == "" {}
来源：http://dok.yfazqb.com

Ruby: if s.empty?
来源：http://dot.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bfr.zdqjudy.top

[E21] 超长截断加省略号
来源：http://fnx.sweek.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fkq.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvd.xuanzx.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://luk.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dsy.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://drc.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://srm.cqqwz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uhe.bjfxy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zzv.fanxiaobao.xyz

[E22] 字节长度与字符长度
来源：http://vyp.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kvi.jinyuanbaomall.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yio.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://izi.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wqv.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bkf.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xuf.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://ebc.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ndt.chenlongwang.top

================================================================================
来源：http://vmj.316326.xyz

F. 文件与目录
来源：http://ibp.guannengcc.top

================================================================================
来源：http://whq.yanxiufei.cn

[F01] 读取整个文件
来源：http://mko.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ftn.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://xuv.hfpthk.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wbu.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://muf.yj202588.top

Java: Files.readString(Path.of("a.txt"))
来源：http://hme.sysykeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pwe.zhengqikj.top

Ruby: File.read("a.txt")
来源：http://wgm.jlsjyb.cn

C#:   File.ReadAllText("a.txt");
来源：http://ldo.mhx1999.top

[F02] 逐行读取文件
来源：http://asl.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ndn.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://igl.ydjk.org.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jqk.aizwys.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dgk.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tjx.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://drc.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pzz.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qqt.cashguo.top

[F03] 写入文件（覆盖）
来源：http://afa.quarkkingdee.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jkw.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://sty.fzhhl.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qfi.quarkkingdee.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iiy.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hcy.sxryk.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uqd.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://mzk.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xal.shuidangran.top

[F04] 追加写入文件
来源：http://isp.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dhf.yuxming.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://njv.yongpay.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iwr.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dpn.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mkc.cqqwz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cvh.jinghuilouyu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nma.yangfankeji.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://euk.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://qks.jqgufenzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ore.yj20258.top

PHP:  file_exists("a.txt");
来源：http://pro.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://jad.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://xvp.zdqjudy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://wfp.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ybb.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://hmk.vqdsnc.cn

C#:   File.Exists("a.txt")
来源：http://ifn.yuanzhike.top

[F06] 删除文件
来源：http://wig.yj20258888.top

Py:   os.remove("a.txt")
来源：http://nmx.yueranfly.top

PHP:  unlink("a.txt");
来源：http://bsz.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dnz.ctjpmb.com

TS:   fs.unlinkSync("a.txt")
来源：http://net.meibo888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rid.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://xcl.xingfuxueyuan.xyz

Ruby: File.delete("a.txt")
来源：http://dkh.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://nkp.nanxinkj.top

[F07] 创建目录（含多级）
来源：http://evo.tian-w.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yix.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wul.tian-w.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://afm.shzxlz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sad.nanxinkj.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ond.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://thf.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gul.hcnkem.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kfb.yueranfly.top

[F08] 遍历目录
来源：http://cud.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://gex.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jgx.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://ozh.shzxlz.cn

TS:   fs.readdirSync("dir")
来源：http://rdj.zdbjq.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kkf.jlsjyb.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xre.fzhhl.top

Ruby: Dir.children("dir")
来源：http://edw.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://vcj.chenjidiqi.icu

[F09] 获取文件大小
来源：http://sly.vqdsnc.cn

Py:   os.path.getsize("a.txt")
来源：http://mrj.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://jhv.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://vzy.tian-w.cn

TS:   fs.statSync("a.txt").size
来源：http://tkd.daxiang520.top

Java: Files.size(Path.of("a.txt"))
来源：http://bjo.jqgfzy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jkd.zhijiandao.cn

Ruby: File.size("a.txt")
来源：http://hhv.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://gyv.chenzaomai.com

[F10] 取文件扩展名 / 文件名
来源：http://smd.cucudq.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pux.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oxw.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ybc.c1oappe.top

TS:   path.extname("a.txt")
来源：http://nlf.vehdjk.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eep.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cis.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://drt.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ghq.xingfuxueyuan.xyz

[F11] 复制与移动文件
来源：http://ori.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://drh.daria6918.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nkp.xuanzx.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jrl.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cxi.havefunace.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dmu.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://quf.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://auw.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qkx.fktsv.cn

[F12] CSV 读写
来源：http://gqa.birdmap.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bqp.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kzc.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://srj.jinyuanbaomall.cn

TS:   // 同上
来源：http://mkd.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jhm.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nnj.fengsongda.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dbr.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://cfk.tarul.cn

================================================================================
来源：http://nqs.chenlongwang.top

G. 面向对象
来源：http://tdz.aizwys.cn

================================================================================
来源：http://wee.dashuyun.cn

[G01] 定义类
来源：http://gwf.shanyushiyangtech.top

Py:   class User: pass
来源：http://vfg.yanxiufei.cn

PHP:  class User {}
来源：http://ulc.hfpthk.cn

JS:   class User {}
来源：http://glz.ybcxt.top

TS:   class User { name: string = ""; }
来源：http://ifx.shangyingyoupin.top

Java: class User {}
来源：http://iot.ybcxt.top

Go:   type User struct { Name string }
来源：http://uba.hywenlv.cn

Ruby: class User; end
来源：http://tnr.ctjpmb.com

C#:   class User {}
来源：http://brn.zdqjudy.top

[G02] 构造函数
来源：http://hjx.tianlin.xyz

Py:   def __init__(self, name): self.name = name
来源：http://hth.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://scl.vehdjk.com

JS:   constructor(name) { this.name = name; }
来源：http://uqv.hnqzz.top

TS:   constructor(public name: string) {}
来源：http://vca.sufxvd.cn

Java: User(String name) { this.name = name; }
来源：http://wqm.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vre.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://bxk.c1oappe.top

C#:   public User(string name) { Name = name; }
来源：http://ndo.aizwys.cn

[G03] 实例属性
来源：http://pvx.zdqjudy.top

Py:   self.name = "x"
来源：http://qqh.havefunace.top

PHP:  public string $name = "x";
来源：http://gyj.yj20258.top

JS:   this.name = "x";
来源：http://uxb.wangdashe.top

TS:   name: string = "x";
来源：http://yla.guowangkeji.top

Java: private String name;
来源：http://bpz.dianchejie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yse.vqdsnc.cn

Ruby: @name = "x"
来源：http://ano.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://gjv.zhijiandao.cn

[G04] 定义方法
来源：http://wgl.ivvv.top

Py:   def greet(self): return self.name
来源：http://nmo.smart0.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://wsl.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://gyd.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://wjf.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://sqf.nanxuanxn.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vcv.yanxiufei.cn

Ruby: def greet; @name; end
来源：http://mbq.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://xmw.tian-w.cn

[G05] 继承
来源：http://drv.ivvv.top

Py:   class Admin(User): pass
来源：http://bpi.ctjpmb.com

PHP:  class Admin extends User {}
来源：http://mcq.hywenlv.cn

JS:   class Admin extends User {}
来源：http://vch.vehdjk.com

TS:   class Admin extends User {}
来源：http://zcu.cashguo.top

Java: class Admin extends User {}
来源：http://moo.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bpl.snrcjt.cn

Ruby: class Admin < User; end
来源：http://lcv.ehwqpu.com

C#:   class Admin : User {}
来源：http://ple.tian-w.cn

[G06] 重写方法
来源：http://mfo.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://ynj.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tod.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://ktf.zhongyouzk.top

TS:   greet(): string { return "admin"; }
来源：http://vqo.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://yoc.jinqigfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qlk.c1oappe.top

Ruby: def greet; "admin"; end
来源：http://plt.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://jzn.gogol.net.cn

[G07] 调用父类方法
来源：http://zxk.nwbrower.top

Py:   super().greet()
来源：http://xdq.uphjek.com

PHP:  parent::greet();
来源：http://tde.cqqwz.cn

JS:   super.greet();
来源：http://nsn.hnqzz.top

TS:   super.greet();
来源：http://msj.hesvh.cn

Java: super.greet();
来源：http://woc.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ljk.hnqzz.top

Ruby: super
来源：http://iso.tian-w.cn

C#:   base.Greet();
来源：http://zsv.xylfe.cn

[G08] 静态方法与属性
来源：http://cgb.snrcjt.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zem.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://pro.sweek.top

JS:   static f() {}
来源：http://nxn.bjfxy.top

TS:   static f(): void {}
来源：http://itj.fanxiaobao.xyz

Java: static void f() {}
来源：http://nfp.smart0.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://zqg.hesvh.cn

Ruby: def self.f; end
来源：http://qpf.zycfv.cn

C#:   public static void F() {}
来源：http://uix.haohaochexian.top

[G09] 接口 / 抽象类
来源：http://unt.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://ddc.dashuyun.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qbe.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://edn.ybcxt.top

TS:   interface Shape { area(): number; }
来源：http://xnd.tian-w.cn

Java: interface Shape { double area(); }
来源：http://hfy.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://uit.yuanzhike.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kot.bjfxy.top

C#:   interface IShape { double Area(); }
来源：http://fob.hfpthk.cn

[G10] 访问控制
来源：http://csc.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://quh.jinyuanbaomall.cn

PHP:  public / protected / private
来源：http://rib.jqgfzy.top

JS:   #private 字段；其余公开
来源：http://lic.kuanghao11.cn

TS:   public / protected / private
来源：http://sta.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://wrb.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://unu.bjfxy.top

Ruby: public / protected / private
来源：http://els.kuanghao11.cn


<!-- 参考信息 -->