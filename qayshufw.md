代发 wailian999

Go:   strings.Count(s, "a")
来源：http://kex.sjlbkw.cn

Ruby: s.count("a")
来源：http://oii.daria6918.cn

C#:   s.Count(c => c == 'a')
来源：http://fzw.gotoacloud.top

[E13] 逐字符遍历
来源：http://cai.sufxvd.cn

Py:   for ch in s: print(ch)
来源：http://fmx.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fdq.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://lev.yj202588.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ppd.jiagoushi.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://csv.iojbl.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bdq.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://pia.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wwf.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://hff.uphjek.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mva.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://vsp.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gxm.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gmq.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://snh.zdbjq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jxc.sxryk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jgv.meibo888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gfr.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://pcy.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sko.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gyd.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bmh.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fqu.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://awr.yj202588.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ppo.pengpengdd.cyou

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oap.shanyushiyangtech.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cps.gaohongyu789.top

[E16] 数字千分位
来源：http://ybl.fehbvm.com

Py:   f"{1234567:,}"
来源：http://pcu.cucudq.cn

PHP:  number_format(1234567);
来源：http://uak.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://voz.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lez.fehbvm.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kru.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nyn.ivvv.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://may.daria6918.cn

C#:   1234567.ToString("N0")
来源：http://lau.yangfankeji.com

[E17] 首字母大写
来源：http://vkt.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jes.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wyg.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kqo.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ylq.jlsjyb.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zmr.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xbn.smart0.xyz

Ruby: s.capitalize
来源：http://unb.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://azd.ydzc1.top

[E18] 模板占位符替换
来源：http://fhb.0kj1m.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ohw.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://het.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rze.ydzc1.top

TS:   tpl.replaceAll("{name}", name)
来源：http://utg.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eqt.bjfxy.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bjj.yj202588.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://frk.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qdk.jianghu66.top

[E19] 多行文本按行拆分
来源：http://qgb.fktsv.cn

Py:   s.splitlines()
来源：http://iob.yj20258.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dop.xuetiantiany.cn

JS:   s.split(/\r?\n/)
来源：http://zst.aizwys.cn

TS:   s.split(/\r?\n/)
来源：http://rca.hysaishi.cn

Java: s.lines().toList()
来源：http://emw.cheryme.top

Go:   strings.Split(s, "\n")
来源：http://jkk.yj20258888.top

Ruby: s.lines
来源：http://vgw.sufxvd.cn

C#:   s.Split('\n')
来源：http://ich.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://ifl.jianghu66.top

Py:   if not s:
来源：http://tpl.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kup.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vui.haohaochexian.top

TS:   if (s === "") {}
来源：http://bgy.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://hyn.fktsv.cn

Go:   if s == "" {}
来源：http://cbd.daria6918.cn

Ruby: if s.empty?
来源：http://qgx.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hyl.yongpay.top

[E21] 超长截断加省略号
来源：http://ftx.yfazqb.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uit.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xis.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dcs.wangdashe.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://juc.ppjwa.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://esc.jlsjyb.cn

Go:   // 按 rune 判断长度后截断
来源：http://dns.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rnt.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jqg.chenlongwang.top

[E22] 字节长度与字符长度
来源：http://buw.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jhv.bbcook.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwi.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yio.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hpb.0kj1m.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gpw.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nxy.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://vja.gotoacloud.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mgn.ywan-chungtsiang.top

================================================================================
来源：http://cpi.yueranfly.top

F. 文件与目录
来源：http://kff.jyoumei.cn

================================================================================
来源：http://zxz.guannengcc.top

[F01] 读取整个文件
来源：http://rsi.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bsr.yangfankeji.com

PHP:  file_get_contents("a.txt");
来源：http://kjp.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ucc.xuanzx.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fyl.xziqi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://khg.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zdk.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://mkn.yj20258.top

C#:   File.ReadAllText("a.txt");
来源：http://yqb.cdnleiting.top

[F02] 逐行读取文件
来源：http://otb.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dss.andypj.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ybc.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kwm.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ypd.chenzaomai.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qyf.shanyushiyangtech.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cwz.fzhhl.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qmu.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vcz.yonumen.top

[F03] 写入文件（覆盖）
来源：http://kcj.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yjn.wangdashe.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jxv.epnwcf.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zkq.zycfv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cbl.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wdk.daxiang520.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://joi.jianghu66.top

Ruby: File.write("a.txt", "hi")
来源：http://fcs.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wfn.ppjwa.cn

[F04] 追加写入文件
来源：http://ayx.snrcjt.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uit.hesvh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yjc.jiagoushi.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fzy.zhengqikj.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nvx.jiagoushi.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vpu.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ass.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jzk.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rli.mhx1999.top

[F05] 判断文件或目录是否存在
来源：http://paf.epnwcf.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gmu.gogol.net.cn

PHP:  file_exists("a.txt");
来源：http://ypu.ehwqpu.com

JS:   fs.existsSync("a.txt")
来源：http://uun.shanyushiyangtech.top

TS:   fs.existsSync("a.txt")
来源：http://hzb.shzxlz.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lps.aibaodan.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xpc.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://dyi.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://qus.sjlbkw.cn

[F06] 删除文件
来源：http://rua.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://vfd.hnqzz.top

PHP:  unlink("a.txt");
来源：http://gie.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://ytq.xziqi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aap.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zhg.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://lei.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://uoi.hnxiangtu.top

C#:   File.Delete("a.txt");
来源：http://ybj.zycfv.cn

[F07] 创建目录（含多级）
来源：http://jch.hysaishi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sxd.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://prg.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ffg.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vpa.ydzc1.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jle.cdnleiting.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rxb.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lrm.sjlbkw.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gup.fengsongda.top

[F08] 遍历目录
来源：http://rmz.wangdashe.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://jps.xingfuxueyuan.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yex.yueranfly.top

JS:   fs.readdirSync("dir")
来源：http://mix.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://mhn.birdmap.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yuk.fanxiaobao.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://nns.tanke756.top

Ruby: Dir.children("dir")
来源：http://waz.yangfankeji.com

C#:   Directory.GetFiles("dir")
来源：http://nlb.hysaishi.cn

[F09] 获取文件大小
来源：http://bpi.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://kki.guowangkeji.top

PHP:  filesize("a.txt");
来源：http://zns.hammf.cn

JS:   fs.statSync("a.txt").size
来源：http://pgl.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://rsx.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://jre.sxryk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tau.daria6918.cn

Ruby: File.size("a.txt")
来源：http://vld.jqgfzy.top

C#:   new FileInfo("a.txt").Length
来源：http://utk.iojbl.cn

[F10] 取文件扩展名 / 文件名
来源：http://gka.tianlin.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mye.yj20258.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hey.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sth.andypj.xyz

TS:   path.extname("a.txt")
来源：http://cbi.daxiang520.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cuu.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zes.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oqv.tarul.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://swr.ivvv.top

[F11] 复制与移动文件
来源：http://poq.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pui.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lwj.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://txn.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hmk.sysykeji.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xme.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://azd.tianlin.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rll.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lae.tianlin.xyz

[F12] CSV 读写
来源：http://ejn.hfpthk.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zqx.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://izj.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://vpx.zhaomingkeji.xyz

TS:   // 同上
来源：http://sip.zdqjudy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gke.9152youxi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://naa.yfazqb.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wjl.gzhubu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://quq.hfpthk.cn

================================================================================
来源：http://ebl.hcnkem.com

G. 面向对象
来源：http://lnt.haohaochexian.top

================================================================================
来源：http://aru.aizwys.cn

[G01] 定义类
来源：http://hsh.zhaomingkeji.xyz

Py:   class User: pass
来源：http://vsm.hnqzz.top

PHP:  class User {}
来源：http://ibj.cdnleiting.top

JS:   class User {}
来源：http://ide.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://mpj.sufxvd.cn

Java: class User {}
来源：http://uki.nanxuanxn.top

Go:   type User struct { Name string }
来源：http://jet.xuanzx.com

Ruby: class User; end
来源：http://fav.hesvh.cn

C#:   class User {}
来源：http://wnf.fehbvm.com

[G02] 构造函数
来源：http://xnd.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://szi.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://nap.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://ouj.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://yzc.xinyue.icu

Java: User(String name) { this.name = name; }
来源：http://osg.ybcxt.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vkd.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://lgj.tarul.cn

C#:   public User(string name) { Name = name; }
来源：http://iuj.xziqi.cn

[G03] 实例属性
来源：http://uwl.sufxvd.cn

Py:   self.name = "x"
来源：http://one.ehwqpu.com

PHP:  public string $name = "x";
来源：http://cia.gotoacloud.top

JS:   this.name = "x";
来源：http://dgb.vqdsnc.cn

TS:   name: string = "x";
来源：http://qzk.dianchejie.cn

Java: private String name;
来源：http://bis.zhongyouzk.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ufz.shzxlz.cn

Ruby: @name = "x"
来源：http://iyl.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://fex.sjlbkw.cn

[G04] 定义方法
来源：http://nye.bjfxy.top

Py:   def greet(self): return self.name
来源：http://vlr.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kbn.xinyue.icu

JS:   greet() { return this.name; }
来源：http://obq.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://tcc.hfpthk.cn

Java: String greet() { return name; }
来源：http://pub.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yiv.mhx1999.top

Ruby: def greet; @name; end
来源：http://zkj.bbcook.cn

C#:   public string Greet() => Name;
来源：http://ugs.yj20258888.top

[G05] 继承
来源：http://cqf.yj20258.top

Py:   class Admin(User): pass
来源：http://fay.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://dyk.wangshuangyany.cn

JS:   class Admin extends User {}
来源：http://ioe.dashuyun.cn

TS:   class Admin extends User {}
来源：http://cav.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://hxv.nanxuanxn.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bmh.daxiang520.top

Ruby: class Admin < User; end
来源：http://irg.aibaodan.cn

C#:   class Admin : User {}
来源：http://imq.c1oappe.top

[G06] 重写方法
来源：http://zty.meibo888.top

Py:   def greet(self): return "admin"
来源：http://vtk.xylfe.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ypw.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://vgp.snrcjt.cn

TS:   greet(): string { return "admin"; }
来源：http://pmy.wangdashe.top

Java: @Override String greet() { return "admin"; }
来源：http://tix.tarul.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qsq.quarkkingdee.top

Ruby: def greet; "admin"; end
来源：http://ybk.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://hrp.chenlongwang.top

[G07] 调用父类方法
来源：http://tkq.dashuyun.cn

Py:   super().greet()
来源：http://sma.aizwys.cn

PHP:  parent::greet();
来源：http://rcu.smart0.xyz

JS:   super.greet();
来源：http://onh.xingfuxueyuan.xyz

TS:   super.greet();
来源：http://sbq.fengsongda.top

Java: super.greet();
来源：http://chz.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hal.fzhhl.top

Ruby: super
来源：http://nmq.uphjek.com

C#:   base.Greet();
来源：http://csy.tanke756.top

[G08] 静态方法与属性
来源：http://eur.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oon.bbcook.cn

PHP:  public static function f() {}
来源：http://hei.bbcook.cn

JS:   static f() {}
来源：http://gmk.zhiwuduotai.top

TS:   static f(): void {}
来源：http://usr.zdqjudy.top

Java: static void f() {}
来源：http://wad.ppjwa.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://feh.cheryme.top

Ruby: def self.f; end
来源：http://yeo.ppjwa.cn

C#:   public static void F() {}
来源：http://trk.bjfxy.top

[G09] 接口 / 抽象类
来源：http://ncq.tianlin.xyz

Py:   from abc import ABC, abstractmethod
来源：http://mon.yonumen.top

PHP:  interface Shape { public function area(): float; }
来源：http://hef.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mza.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://bck.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://goo.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://mpy.tarul.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://boa.havefunace.top

C#:   interface IShape { double Area(); }
来源：http://dta.andypj.xyz

[G10] 访问控制
来源：http://eqt.xuanzx.com

Py:   约定 _protected / __private（不强制）
来源：http://vmv.tian-w.cn

PHP:  public / protected / private
来源：http://kne.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://sjo.yongpay.top

TS:   public / protected / private
来源：http://nzx.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://ife.hywenlv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fwk.9152youxi.cn

Ruby: public / protected / private
来源：http://mic.hysaishi.cn

C#:   public / protected / private / internal
来源：http://wge.nanxuanxn.top

[G11] getter / setter
来源：http://mbm.yonumen.top

Py:   @property 与 @x.setter
来源：http://cwd.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nbo.zhaomingkeji.xyz


<!-- 参考信息 -->