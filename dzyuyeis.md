代发 wailian999

Go:   strings.Count(s, "a")
来源：http://neg.sysykeji.top

Ruby: s.count("a")
来源：http://bks.yuanzhike.top

C#:   s.Count(c => c == 'a')
来源：http://nan.ehwqpu.com

[E13] 逐字符遍历
来源：http://ekz.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://xke.xinyue.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bpz.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xni.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tia.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ujd.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pqh.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://zzn.yuxming.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cnp.meibo888.top

[E14] URL 编码与 Base64
来源：http://hbe.ywan-chungtsiang.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ack.316326.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://eyx.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qap.hysaishi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://orp.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ewq.yfazqb.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oef.zdbjq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://daz.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://var.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://tbf.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xsv.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kyu.dianchejie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dka.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wyy.yj20258.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://szj.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gvp.xylfe.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://owe.yj20258888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vox.chenlongwang.top

[E16] 数字千分位
来源：http://bcx.feifeiyinyue.top

Py:   f"{1234567:,}"
来源：http://zrn.guannengcc.top

PHP:  number_format(1234567);
来源：http://gcr.shangyingyoupin.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mnl.guannengcc.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cci.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yds.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fud.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nty.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://fck.hnxiangtu.top

[E17] 首字母大写
来源：http://hpb.fktsv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jkk.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mdr.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ose.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fwn.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hgv.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vnu.zhiwuduotai.top

Ruby: s.capitalize
来源：http://hdk.fktsv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dsw.wangdashe.top

[E18] 模板占位符替换
来源：http://tep.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uhs.sysykeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xwg.redwolf501.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pfl.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ycp.quarkkingdee.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eui.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ivt.shuidangran.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sms.jinghuilouyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xxh.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://qva.hnxiangtu.top

Py:   s.splitlines()
来源：http://jpl.yueranfly.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qpd.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://gvm.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://exa.havefunace.top

Java: s.lines().toList()
来源：http://gzc.zhaomingkeji.xyz

Go:   strings.Split(s, "\n")
来源：http://tac.sweek.top

Ruby: s.lines
来源：http://roe.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://hsz.svipenyu.cn

[E20] 判断字符串是否为空
来源：http://yrx.epnwcf.com

Py:   if not s:
来源：http://yiy.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tyd.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wwk.vqdsnc.cn

TS:   if (s === "") {}
来源：http://tak.jinghuilouyu.cn

Java: if (s.isEmpty()) {}
来源：http://zlv.meibo888.top

Go:   if s == "" {}
来源：http://vrf.yj202588.top

Ruby: if s.empty?
来源：http://loe.fengsongda.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kdi.zhaomingkeji.xyz

[E21] 超长截断加省略号
来源：http://niu.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mxg.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wvz.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://izj.sxryk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhw.tianlin.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dqb.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://gbu.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sag.cdnleiting.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lyp.andypj.xyz

[E22] 字节长度与字符长度
来源：http://ggx.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cjl.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rue.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bjc.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xyq.hywenlv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sgz.iojbl.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wvg.yj202588.top

Ruby: s.bytesize;  s.length
来源：http://lxv.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://owy.hysaishi.cn

================================================================================
来源：http://xcl.yvedp.cn

F. 文件与目录
来源：http://fgl.smart0.xyz

================================================================================
来源：http://oxs.yuxming.cn

[F01] 读取整个文件
来源：http://dkx.nwbrower.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xxl.shuidangran.top

PHP:  file_get_contents("a.txt");
来源：http://wcy.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wzu.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xmt.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ieh.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ygd.feifeiyinyue.top

Ruby: File.read("a.txt")
来源：http://ifx.jyoumei.cn

C#:   File.ReadAllText("a.txt");
来源：http://eoc.bjfxy.top

[F02] 逐行读取文件
来源：http://xbd.epnwcf.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://esd.sjlbkw.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://knc.zhixingplan.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pbu.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gwb.ybcxt.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xrq.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pnr.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dak.jyoumei.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cys.daria6918.cn

[F03] 写入文件（覆盖）
来源：http://vih.snrcjt.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zck.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://aas.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://skw.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlk.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fas.hnxiangtu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cqm.cheryme.top

Ruby: File.write("a.txt", "hi")
来源：http://joy.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yby.sjlbkw.cn

[F04] 追加写入文件
来源：http://bgh.hcnkem.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uzl.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rew.dashuyun.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eyz.zycfv.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hqa.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dvj.zhixingplan.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jbm.birdmap.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mpx.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zqg.quarkkingdee.top

[F05] 判断文件或目录是否存在
来源：http://bwz.hcnkem.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://plg.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://ifn.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://dfs.yj202588.top

TS:   fs.existsSync("a.txt")
来源：http://xrp.xuanzx.com

Java: Files.exists(Path.of("a.txt"))
来源：http://ysl.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mvz.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://lid.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://ynp.hfpthk.cn

[F06] 删除文件
来源：http://kjn.316326.xyz

Py:   os.remove("a.txt")
来源：http://oee.jianghu66.top

PHP:  unlink("a.txt");
来源：http://ktt.tian-w.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zmy.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://way.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mqr.ppjwa.cn

Go:   os.Remove("a.txt")
来源：http://swr.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://kqx.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://krc.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://hyp.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://brw.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nba.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kgs.yanxiufei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dop.hcnkem.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vzy.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mfh.jinyuanbaomall.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cda.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mzz.vehdjk.com

[F08] 遍历目录
来源：http://nbs.bbcook.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://clo.sxryk.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hol.bjfxy.top

JS:   fs.readdirSync("dir")
来源：http://sqp.pengpengdd.cyou

TS:   fs.readdirSync("dir")
来源：http://glt.yuanzhike.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bdb.zdbjq.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vel.jianghu66.top

Ruby: Dir.children("dir")
来源：http://cyv.jinqigufen.top

C#:   Directory.GetFiles("dir")
来源：http://kpz.zhoulong.xyz

[F09] 获取文件大小
来源：http://mmd.yj20258.top

Py:   os.path.getsize("a.txt")
来源：http://ibn.bbcook.cn

PHP:  filesize("a.txt");
来源：http://rvm.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://hrt.ctjpmb.com

TS:   fs.statSync("a.txt").size
来源：http://reu.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cib.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qdz.xingfuxueyuan.xyz

Ruby: File.size("a.txt")
来源：http://upj.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://gju.shangyingyoupin.top

[F10] 取文件扩展名 / 文件名
来源：http://xkk.zdqjudy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qyn.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mcf.shanyushiyangtech.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ydw.svipenyu.cn

TS:   path.extname("a.txt")
来源：http://xke.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gkv.vqdsnc.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vjd.fzhhl.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wth.fzhhl.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zgj.meibo888.top

[F11] 复制与移动文件
来源：http://dxi.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mgc.hnxiangtu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oot.pengpengdd.cyou

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ymr.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rdi.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dbj.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lcu.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nen.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rvt.gaohongyu789.top

[F12] CSV 读写
来源：http://pef.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hyd.0kj1m.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gic.hysaishi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yvc.zhongyouzk.top

TS:   // 同上
来源：http://ror.haohaochexian.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sta.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ddu.zhoulong.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wgq.52xcode.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mmx.hysaishi.cn

================================================================================
来源：http://feb.0kj1m.cn

G. 面向对象
来源：http://osz.jinghuilouyu.cn

================================================================================
来源：http://gax.yuxming.cn

[G01] 定义类
来源：http://njh.yj202588.top

Py:   class User: pass
来源：http://lev.ydjk.org.cn

PHP:  class User {}
来源：http://mma.52xcode.cn

JS:   class User {}
来源：http://nhk.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://mkz.cqqwz.cn

Java: class User {}
来源：http://qhd.fzhhl.top

Go:   type User struct { Name string }
来源：http://sqv.bbcook.cn

Ruby: class User; end
来源：http://icz.hfpthk.cn

C#:   class User {}
来源：http://ceo.guowangkeji.top

[G02] 构造函数
来源：http://qet.daria6918.cn

Py:   def __init__(self, name): self.name = name
来源：http://evk.yj202588.top

PHP:  public function __construct(public string $name) {}
来源：http://oup.daxiang520.top

JS:   constructor(name) { this.name = name; }
来源：http://bub.ivvv.top

TS:   constructor(public name: string) {}
来源：http://nvu.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://cik.cqqwz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://siv.xuanzx.com

Ruby: def initialize(name); @name = name; end
来源：http://uvn.xuetiantiany.cn

C#:   public User(string name) { Name = name; }
来源：http://znx.aibaodan.cn

[G03] 实例属性
来源：http://wkh.andypj.xyz

Py:   self.name = "x"
来源：http://zhp.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://pva.feifeiyinyue.top

JS:   this.name = "x";
来源：http://jqr.fktsv.cn

TS:   name: string = "x";
来源：http://ixh.yangfankeji.com

Java: private String name;
来源：http://dce.svipenyu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://enj.zhongyouzk.top

Ruby: @name = "x"
来源：http://rbh.gotoacloud.top

C#:   public string Name { get; set; } = "x";
来源：http://lac.xylfe.cn

[G04] 定义方法
来源：http://euw.yj20258.top

Py:   def greet(self): return self.name
来源：http://zgg.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bsp.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://nzx.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://qlt.0kj1m.cn

Java: String greet() { return name; }
来源：http://okr.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bvy.zycfv.cn

Ruby: def greet; @name; end
来源：http://znl.chenjidiqi.icu

C#:   public string Greet() => Name;
来源：http://qxe.gzhubu.top

[G05] 继承
来源：http://jhx.zhijiandao.cn

Py:   class Admin(User): pass
来源：http://gne.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://dep.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://aio.tianlin.xyz

TS:   class Admin extends User {}
来源：http://koi.c1oappe.top

Java: class Admin extends User {}
来源：http://sac.guowangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xef.tarul.cn

Ruby: class Admin < User; end
来源：http://oay.yonumen.top

C#:   class Admin : User {}
来源：http://hts.nanxinkj.top

[G06] 重写方法
来源：http://dtj.guowangkeji.top

Py:   def greet(self): return "admin"
来源：http://fvu.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cjk.shanyushiyangtech.top

JS:   greet() { return "admin"; }
来源：http://nrm.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://xog.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://xiz.gzhubu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://via.yuxming.cn

Ruby: def greet; "admin"; end
来源：http://rqc.yongpay.top

C#:   public override string Greet() => "admin";
来源：http://wsk.pycfn.com

[G07] 调用父类方法
来源：http://gat.zhaomingkeji.xyz

Py:   super().greet()
来源：http://sxg.xuanzx.com

PHP:  parent::greet();
来源：http://xyx.xylfe.cn

JS:   super.greet();
来源：http://hnt.zhoulong.xyz

TS:   super.greet();
来源：http://jic.chenzaomai.com

Java: super.greet();
来源：http://ewt.wangdashe.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yux.yuanzhike.top

Ruby: super
来源：http://ceg.cdnleiting.top

C#:   base.Greet();
来源：http://kyr.yanxiufei.cn

[G08] 静态方法与属性
来源：http://ttp.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xwr.hnqzz.top

PHP:  public static function f() {}
来源：http://hxp.ydzc1.top

JS:   static f() {}
来源：http://apo.zdqjudy.top

TS:   static f(): void {}
来源：http://fxc.cashguo.top

Java: static void f() {}
来源：http://hdx.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://czp.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://mem.jlsjyb.cn

C#:   public static void F() {}
来源：http://snz.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://kdb.ehwqpu.com

Py:   from abc import ABC, abstractmethod
来源：http://fjg.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://fcx.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://czc.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://kvo.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://dkz.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://nwu.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uxh.sweek.top

C#:   interface IShape { double Area(); }
来源：http://nwa.zhaomingkeji.xyz

[G10] 访问控制
来源：http://dya.jiagoushi.top

Py:   约定 _protected / __private（不强制）
来源：http://cnq.zdbjq.cn

PHP:  public / protected / private
来源：http://uzl.yj202588.top

JS:   #private 字段；其余公开
来源：http://dkz.gzhubu.top

TS:   public / protected / private
来源：http://kns.yueranfly.top

Java: public / protected / private / 默认包级
来源：http://cin.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://zzq.havefunace.top

Ruby: public / protected / private
来源：http://liz.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://mnc.uphjek.com

[G11] getter / setter
来源：http://ktd.zdqjudy.top

Py:   @property 与 @x.setter
来源：http://gso.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ykw.mhx1999.top


<!-- 参考信息 -->