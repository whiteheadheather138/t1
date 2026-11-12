代发 wailian999

Ruby: s.reverse
来源：http://hcu.ivvv.top

C#:   new string(s.Reverse().ToArray())
来源：http://fac.gaohongyu789.top

[E12] 统计某字符出现次数
来源：http://xsg.fehbvm.com

Py:   s.count("a")
来源：http://bma.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://oty.daria6918.cn

JS:   s.split("a").length - 1
来源：http://gkx.redwolf501.top

TS:   s.split("a").length - 1
来源：http://zyf.pycfn.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vwk.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://nzf.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://mts.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://gzl.tianlin.xyz

[E13] 逐字符遍历
来源：http://mnk.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://sll.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zbr.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dru.shuidangran.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://pkc.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hnq.redwolf501.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qnv.ppjwa.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jcs.zhijiandao.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vok.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://aak.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pcy.fengsongda.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pop.nanxinkj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aun.ybcxt.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uen.tian-w.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zgf.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://huh.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yzo.iojbl.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfv.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://gjp.xuetiantiany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://psi.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lcx.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sbq.zdqjudy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://qbk.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mqv.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ufp.haohaochexian.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oln.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://isw.zdbjq.cn

[E16] 数字千分位
来源：http://kzf.bjfxy.top

Py:   f"{1234567:,}"
来源：http://ijj.jqgfzy.top

PHP:  number_format(1234567);
来源：http://wbs.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://thl.daxiang520.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zki.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qgq.smart0.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iny.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dou.ivvv.top

C#:   1234567.ToString("N0")
来源：http://jux.ehwqpu.com

[E17] 首字母大写
来源：http://rcl.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dtf.feifeiyinyue.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://wdv.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tvi.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iqr.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ecm.shzxlz.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nar.jqgufenzy.top

Ruby: s.capitalize
来源：http://ypl.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dkk.shzxlz.cn

[E18] 模板占位符替换
来源：http://xyo.meibo888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://krg.mhx1999.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://que.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lez.chenlongwang.top

TS:   tpl.replaceAll("{name}", name)
来源：http://aog.hfpthk.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vei.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://uzw.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vwr.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jzp.vehdjk.com

[E19] 多行文本按行拆分
来源：http://hjb.bbcook.cn

Py:   s.splitlines()
来源：http://uks.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xos.guannengcc.top

JS:   s.split(/\r?\n/)
来源：http://his.yueranfly.top

TS:   s.split(/\r?\n/)
来源：http://ipe.jqgfzy.top

Java: s.lines().toList()
来源：http://nat.jlsjyb.cn

Go:   strings.Split(s, "\n")
来源：http://hvh.yfazqb.com

Ruby: s.lines
来源：http://zdv.vqdsnc.cn

C#:   s.Split('\n')
来源：http://ony.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://xas.jlsjyb.cn

Py:   if not s:
来源：http://bwz.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ldm.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yhu.cqqwz.cn

TS:   if (s === "") {}
来源：http://xif.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://wxy.pycfn.com

Go:   if s == "" {}
来源：http://ovr.yonumen.top

Ruby: if s.empty?
来源：http://hwd.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dxd.yanxiufei.cn

[E21] 超长截断加省略号
来源：http://sgc.316326.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hmj.hywenlv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvm.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oxt.jyoumei.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vmg.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uur.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://ihd.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wzf.nanxinkj.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mbc.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://vsw.xingfuxueyuan.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rvi.xuetiantiany.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pfx.shangyingyoupin.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lcf.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rkw.hesvh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fli.hammf.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hvg.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://kgr.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pbf.tianlin.xyz

================================================================================
来源：http://vhq.shangyingyoupin.top

F. 文件与目录
来源：http://dmd.yanxiufei.cn

================================================================================
来源：http://qbi.jiagoushi.top

[F01] 读取整个文件
来源：http://bqc.yonumen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cpn.zdbjq.cn

PHP:  file_get_contents("a.txt");
来源：http://okx.havefunace.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dko.aibaodan.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pkv.hnxiangtu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://eze.fzhhl.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zhh.yuxming.cn

Ruby: File.read("a.txt")
来源：http://zbg.wangdashe.top

C#:   File.ReadAllText("a.txt");
来源：http://osk.nanxinkj.top

[F02] 逐行读取文件
来源：http://oaz.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hgz.bbcook.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kxe.chenzaomai.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lht.zycfv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mvl.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ols.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tpr.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lkd.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tyz.aibaodan.cn

[F03] 写入文件（覆盖）
来源：http://csf.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gbb.zhijiandao.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eei.yj20258.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://feh.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xbq.tianlin.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pbe.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gic.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://nby.ppjwa.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mtb.ctjpmb.com

[F04] 追加写入文件
来源：http://fqb.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://viy.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bom.haohaochexian.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cqr.bjfxy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://olk.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nrt.haohaochexian.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kpt.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fik.jinghuilouyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wfm.aibaodan.cn

[F05] 判断文件或目录是否存在
来源：http://lat.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wln.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://rzm.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://vwd.mhx1999.top

TS:   fs.existsSync("a.txt")
来源：http://mpl.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cga.fktsv.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rtr.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://wei.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://tuf.sweek.top

[F06] 删除文件
来源：http://bsq.cucudq.cn

Py:   os.remove("a.txt")
来源：http://inf.yueranfly.top

PHP:  unlink("a.txt");
来源：http://jvb.yj20258888.top

JS:   fs.unlinkSync("a.txt")
来源：http://dhz.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ypi.gotoacloud.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pkx.ivvv.top

Go:   os.Remove("a.txt")
来源：http://qcn.daxiang520.top

Ruby: File.delete("a.txt")
来源：http://gds.tarul.cn

C#:   File.Delete("a.txt");
来源：http://uca.cashguo.top

[F07] 创建目录（含多级）
来源：http://kzj.jyoumei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mii.ydjk.org.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://egc.ydjk.org.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eju.xingfuxueyuan.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tom.ybcxt.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://psf.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qiv.wangdashe.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pfc.vehdjk.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tzz.gzhubu.top

[F08] 遍历目录
来源：http://kyt.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yvp.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://chj.shanyushiyangkeji.top

JS:   fs.readdirSync("dir")
来源：http://lws.chenlongwang.top

TS:   fs.readdirSync("dir")
来源：http://awp.daxiang520.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sbo.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nwq.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://nux.tianlin.xyz

C#:   Directory.GetFiles("dir")
来源：http://jxt.zhengqikj.top

[F09] 获取文件大小
来源：http://xug.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://dne.feifeiyinyue.top

PHP:  filesize("a.txt");
来源：http://fmz.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://xyl.yuxming.cn

TS:   fs.statSync("a.txt").size
来源：http://uin.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://bih.zdbjq.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xok.xziqi.cn

Ruby: File.size("a.txt")
来源：http://crx.ehwqpu.com

C#:   new FileInfo("a.txt").Length
来源：http://ywg.gotoacloud.top

[F10] 取文件扩展名 / 文件名
来源：http://lgz.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pup.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://izt.fengsongda.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fye.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://now.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yyd.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uhz.316326.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gmt.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kky.chenzaomai.com

[F11] 复制与移动文件
来源：http://wgv.aizwys.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fpu.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xdx.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vgu.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cjf.shanyushiyangkeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mch.tian-w.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ocn.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbh.fehbvm.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uxn.aizwys.cn

[F12] CSV 读写
来源：http://ndn.pengpengdd.cyou

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yir.yuxming.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dpf.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ayk.cucudq.cn

TS:   // 同上
来源：http://lji.fanxiaobao.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nji.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://upa.ppjwa.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tmh.yongpay.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ois.shuidangran.top

================================================================================
来源：http://jsp.gotoacloud.top

G. 面向对象
来源：http://whm.cashguo.top

================================================================================
来源：http://xoi.hnxiangtu.top

[G01] 定义类
来源：http://etf.zdbjq.cn

Py:   class User: pass
来源：http://ygr.tanke756.top

PHP:  class User {}
来源：http://bgt.316326.xyz

JS:   class User {}
来源：http://ocw.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://onx.zhoulong.xyz

Java: class User {}
来源：http://pda.cucudq.cn

Go:   type User struct { Name string }
来源：http://its.meibo888.top

Ruby: class User; end
来源：http://upx.pengpengdd.cyou

C#:   class User {}
来源：http://eap.uphjek.com

[G02] 构造函数
来源：http://tgk.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://jss.tianlin.xyz

PHP:  public function __construct(public string $name) {}
来源：http://iue.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://yhe.havefunace.top

TS:   constructor(public name: string) {}
来源：http://ezg.jianghu66.top

Java: User(String name) { this.name = name; }
来源：http://xym.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vrr.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://hlb.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://dew.sweek.top

[G03] 实例属性
来源：http://lfk.shangyingyoupin.top

Py:   self.name = "x"
来源：http://ren.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://pad.redwolf501.top

JS:   this.name = "x";
来源：http://iqd.sysykeji.top

TS:   name: string = "x";
来源：http://pij.c1oappe.top

Java: private String name;
来源：http://aae.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://obs.guowangkeji.top

Ruby: @name = "x"
来源：http://sbs.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://htm.sxryk.cn

[G04] 定义方法
来源：http://qrc.xinyue.icu

Py:   def greet(self): return self.name
来源：http://ueq.hysaishi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lbh.sysykeji.top

JS:   greet() { return this.name; }
来源：http://xqq.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://eka.birdmap.top

Java: String greet() { return name; }
来源：http://dmp.zhijiandao.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ogr.vehdjk.com

Ruby: def greet; @name; end
来源：http://ptf.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://aqw.epnwcf.com

[G05] 继承
来源：http://pmh.jqgfzy.top

Py:   class Admin(User): pass
来源：http://qtq.sjlbkw.cn

PHP:  class Admin extends User {}
来源：http://uuw.bjfxy.top

JS:   class Admin extends User {}
来源：http://fno.316326.xyz

TS:   class Admin extends User {}
来源：http://vvp.svipenyu.cn

Java: class Admin extends User {}
来源：http://qaz.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qmd.9152youxi.cn

Ruby: class Admin < User; end
来源：http://ksm.jiagoushi.top

C#:   class Admin : User {}
来源：http://huk.zhoulong.xyz

[G06] 重写方法
来源：http://eas.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://kou.jiagoushi.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tqt.guannengcc.top

JS:   greet() { return "admin"; }
来源：http://gyx.vqdsnc.cn

TS:   greet(): string { return "admin"; }
来源：http://iup.0kj1m.cn

Java: @Override String greet() { return "admin"; }
来源：http://dfe.pengpengdd.cyou

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iad.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://duq.ivvv.top

C#:   public override string Greet() => "admin";
来源：http://llb.c1oappe.top

[G07] 调用父类方法
来源：http://fsm.jlsjyb.cn

Py:   super().greet()
来源：http://zlg.fengsongda.top

PHP:  parent::greet();
来源：http://ein.ydzc1.top

JS:   super.greet();
来源：http://goj.316326.xyz

TS:   super.greet();
来源：http://gly.yonumen.top

Java: super.greet();
来源：http://wsg.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aqj.yuxming.cn

Ruby: super
来源：http://qzs.xuanzx.com

C#:   base.Greet();
来源：http://izr.havefunace.top

[G08] 静态方法与属性
来源：http://rqr.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tty.tarul.cn

PHP:  public static function f() {}
来源：http://qlo.fktsv.cn

JS:   static f() {}
来源：http://iuy.cucudq.cn

TS:   static f(): void {}
来源：http://vuy.sxryk.cn

Java: static void f() {}
来源：http://vqf.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xxo.wangdashe.top

Ruby: def self.f; end
来源：http://ffl.0kj1m.cn

C#:   public static void F() {}
来源：http://rqx.hesvh.cn

[G09] 接口 / 抽象类
来源：http://uxg.dianchejie.cn

Py:   from abc import ABC, abstractmethod
来源：http://ili.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://fez.pengpengdd.cyou

JS:   // 无接口：靠约定或 JSDoc
来源：http://qki.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://jyl.daxiang520.top

Java: interface Shape { double area(); }
来源：http://muh.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://puu.yfazqb.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ycd.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://pjo.xziqi.cn

[G10] 访问控制
来源：http://wio.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://njv.bbcook.cn

PHP:  public / protected / private
来源：http://est.ybcxt.top

JS:   #private 字段；其余公开
来源：http://adu.haohaochexian.top


<!-- 参考信息 -->