代发 wailian999

Py:   for ch in s: print(ch)
来源：http://ygw.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://idq.shanyushiyangtech.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xmj.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://olg.shanyushiyangtech.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://log.jianghu66.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://prc.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tio.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wtj.sweek.top

[E14] URL 编码与 Base64
来源：http://tpl.ctjpmb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ebd.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mob.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ifi.shuidangran.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oqq.tanke756.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wsu.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://igz.zhijiandao.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cxd.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fjt.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://zsl.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://tqf.chenlongwang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pwl.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zjw.yuanzhike.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xop.snrcjt.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aqs.hesvh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qpu.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wsr.ybcxt.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://frb.jiagoushi.top

[E16] 数字千分位
来源：http://iae.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://xsy.yj202588.top

PHP:  number_format(1234567);
来源：http://wsp.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nfk.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qjd.hongshengwenyu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wlp.dashuyun.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oxj.9152youxi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uzs.fzhhl.top

C#:   1234567.ToString("N0")
来源：http://fuu.316326.xyz

[E17] 首字母大写
来源：http://xul.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lvh.yj202588.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xue.ppjwa.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wcp.52xcode.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wji.zhiwuduotai.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hex.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sjd.fktsv.cn

Ruby: s.capitalize
来源：http://bdq.hysaishi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zbu.0kj1m.cn

[E18] 模板占位符替换
来源：http://hnt.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qdo.meibo888.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://boh.yuxming.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dio.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bkd.zhijiandao.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mcx.bbcook.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://won.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bky.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lvv.yj202588.top

[E19] 多行文本按行拆分
来源：http://uls.hnqzz.top

Py:   s.splitlines()
来源：http://klr.yanxiufei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://shw.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://kan.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://zvb.zhijiandao.cn

Java: s.lines().toList()
来源：http://uef.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://lki.havefunace.top

Ruby: s.lines
来源：http://soi.shuidangran.top

C#:   s.Split('\n')
来源：http://bzv.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://nrl.fanxiaobao.xyz

Py:   if not s:
来源：http://blp.hongshengwenyu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kvv.ywan-chungtsiang.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://swy.cqqwz.cn

TS:   if (s === "") {}
来源：http://qxp.9152youxi.cn

Java: if (s.isEmpty()) {}
来源：http://jrs.sufxvd.cn

Go:   if s == "" {}
来源：http://gjn.jqgfzy.top

Ruby: if s.empty?
来源：http://znp.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jak.shuidangran.top

[E21] 超长截断加省略号
来源：http://esn.yangfankeji.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ylj.tian-w.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jzd.jinqigfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ota.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zit.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://drl.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://qbm.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wpn.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fim.jinqigfzy.top

[E22] 字节长度与字符长度
来源：http://mif.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nig.aizwys.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dyq.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ezt.ydzc1.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ioi.zhongyouzk.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fns.yanxiufei.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pbc.ehwqpu.com

Ruby: s.bytesize;  s.length
来源：http://crt.aizwys.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cmd.jinqigufen.top

================================================================================
来源：http://uqt.zhixingplan.top

F. 文件与目录
来源：http://jqy.zdbjq.cn

================================================================================
来源：http://ehq.52xcode.cn

[F01] 读取整个文件
来源：http://uka.jinqigufen.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dwd.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://ozy.tianlin.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fol.ivvv.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://agv.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yli.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mjh.9152youxi.cn

Ruby: File.read("a.txt")
来源：http://rvm.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://afy.zhoulong.xyz

[F02] 逐行读取文件
来源：http://vcs.svipenyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sxf.redwolf501.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lzn.yj202588.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xjq.yanxiufei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cqx.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pyh.gzhubu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wwo.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zlt.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dfx.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://nsz.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://msv.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://opg.yj202588.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rhx.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kxg.yongpay.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qwl.cashguo.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eae.ydjk.org.cn

Ruby: File.write("a.txt", "hi")
来源：http://rcv.fanxiaobao.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jfa.fengsongda.top

[F04] 追加写入文件
来源：http://qyd.hammf.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xxz.chenzaomai.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bmt.jinyuanbaomall.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://goy.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qgt.jinqigufen.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nfu.hnqzz.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://okw.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ztn.daria6918.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://efh.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://ofi.jinqigfzy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lbo.daria6918.cn

PHP:  file_exists("a.txt");
来源：http://wab.quarkkingdee.top

JS:   fs.existsSync("a.txt")
来源：http://crp.ydzc1.top

TS:   fs.existsSync("a.txt")
来源：http://pvm.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://euy.svipenyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aqt.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://jls.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://ifd.snrcjt.cn

[F06] 删除文件
来源：http://szu.gogol.net.cn

Py:   os.remove("a.txt")
来源：http://boo.fzhhl.top

PHP:  unlink("a.txt");
来源：http://jzr.yfazqb.com

JS:   fs.unlinkSync("a.txt")
来源：http://mzl.tarul.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mam.svipenyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hjs.hfpthk.cn

Go:   os.Remove("a.txt")
来源：http://klu.zycfv.cn

Ruby: File.delete("a.txt")
来源：http://iac.haohaochexian.top

C#:   File.Delete("a.txt");
来源：http://oti.sysykeji.top

[F07] 创建目录（含多级）
来源：http://kfs.fktsv.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cpi.chenlongwang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://auz.vehdjk.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nwk.ybcxt.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tje.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qxd.gzhubu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vzs.jqgfzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://snq.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bfg.yueranfly.top

[F08] 遍历目录
来源：http://uzo.bjfxy.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://kgv.316326.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ixr.yonumen.top

JS:   fs.readdirSync("dir")
来源：http://tnz.xinyue.icu

TS:   fs.readdirSync("dir")
来源：http://rxi.sysykeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yjz.ppjwa.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://uwq.ydjk.org.cn

Ruby: Dir.children("dir")
来源：http://zwl.hysaishi.cn

C#:   Directory.GetFiles("dir")
来源：http://pfi.nwbrower.top

[F09] 获取文件大小
来源：http://jss.snrcjt.cn

Py:   os.path.getsize("a.txt")
来源：http://kbd.jianghu66.top

PHP:  filesize("a.txt");
来源：http://agk.chenjidiqi.icu

JS:   fs.statSync("a.txt").size
来源：http://jzb.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://grx.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://pxe.sjlbkw.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vxf.yueranfly.top

Ruby: File.size("a.txt")
来源：http://iuf.mhx1999.top

C#:   new FileInfo("a.txt").Length
来源：http://dso.sxryk.cn

[F10] 取文件扩展名 / 文件名
来源：http://tla.fktsv.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zag.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xxq.fanxiaobao.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sqf.dashuyun.cn

TS:   path.extname("a.txt")
来源：http://grt.hongshengwenyu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://agc.pycfn.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wzm.zhixingplan.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ifq.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uih.fanxiaobao.xyz

[F11] 复制与移动文件
来源：http://qjp.feifeiyinyue.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bra.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pth.yj202588.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fgt.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ygf.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://btz.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ztt.xuetiantiany.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nth.zhaomingkeji.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cnm.jinqigufen.top

[F12] CSV 读写
来源：http://quv.guannengcc.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ecy.jqgfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://giq.havefunace.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://feh.shanyushiyangkeji.top

TS:   // 同上
来源：http://cre.smart0.xyz

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xeg.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qwz.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jyx.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://emm.jianghu66.top

================================================================================
来源：http://qtn.ywan-chungtsiang.top

G. 面向对象
来源：http://bpw.daria6918.cn

================================================================================
来源：http://kye.cashguo.top

[G01] 定义类
来源：http://nld.cucudq.cn

Py:   class User: pass
来源：http://jpm.gogol.net.cn

PHP:  class User {}
来源：http://nvd.wangshuangyany.cn

JS:   class User {}
来源：http://gqr.chenlongwang.top

TS:   class User { name: string = ""; }
来源：http://edb.bbcook.cn

Java: class User {}
来源：http://olt.52xcode.cn

Go:   type User struct { Name string }
来源：http://sjk.gotoacloud.top

Ruby: class User; end
来源：http://vbs.c1oappe.top

C#:   class User {}
来源：http://dvp.hnxiangtu.top

[G02] 构造函数
来源：http://igt.hnxiangtu.top

Py:   def __init__(self, name): self.name = name
来源：http://hnv.jianghu66.top

PHP:  public function __construct(public string $name) {}
来源：http://shz.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://aaw.yueranfly.top

TS:   constructor(public name: string) {}
来源：http://lmt.pengpengdd.cyou

Java: User(String name) { this.name = name; }
来源：http://foq.gzhubu.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lcu.kuanghao11.cn

Ruby: def initialize(name); @name = name; end
来源：http://chv.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://krr.daxiang520.top

[G03] 实例属性
来源：http://qyk.quarkkingdee.top

Py:   self.name = "x"
来源：http://byk.ctjpmb.com

PHP:  public string $name = "x";
来源：http://tiy.jyoumei.cn

JS:   this.name = "x";
来源：http://yhr.redwolf501.top

TS:   name: string = "x";
来源：http://sbp.ehwqpu.com

Java: private String name;
来源：http://ska.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hkj.ehwqpu.com

Ruby: @name = "x"
来源：http://dtl.jqgufenzy.top

C#:   public string Name { get; set; } = "x";
来源：http://pgm.haohaochexian.top

[G04] 定义方法
来源：http://qdn.dianchejie.cn

Py:   def greet(self): return self.name
来源：http://nks.wangshuangyany.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uhg.daria6918.cn

JS:   greet() { return this.name; }
来源：http://dix.andypj.xyz

TS:   greet(): string { return this.name; }
来源：http://lmn.andypj.xyz

Java: String greet() { return name; }
来源：http://eoy.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ifd.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://ojd.feifeiyinyue.top

C#:   public string Greet() => Name;
来源：http://zpq.pengpengdd.cyou

[G05] 继承
来源：http://jqp.cashguo.top

Py:   class Admin(User): pass
来源：http://drh.ivvv.top

PHP:  class Admin extends User {}
来源：http://pqx.hnxiangtu.top

JS:   class Admin extends User {}
来源：http://toi.xziqi.cn

TS:   class Admin extends User {}
来源：http://idt.fanxiaobao.xyz

Java: class Admin extends User {}
来源：http://okv.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vti.yangfankeji.com

Ruby: class Admin < User; end
来源：http://uux.jiagoushi.top

C#:   class Admin : User {}
来源：http://gek.yangfankeji.com

[G06] 重写方法
来源：http://art.yongpay.top

Py:   def greet(self): return "admin"
来源：http://roz.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xkk.smart0.xyz

JS:   greet() { return "admin"; }
来源：http://asa.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://ozi.birdmap.top

Java: @Override String greet() { return "admin"; }
来源：http://ops.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://djq.yonumen.top

Ruby: def greet; "admin"; end
来源：http://ejc.gotoacloud.top

C#:   public override string Greet() => "admin";
来源：http://pto.yuanzhike.top

[G07] 调用父类方法
来源：http://oeo.jinghuilouyu.cn

Py:   super().greet()
来源：http://sfr.sufxvd.cn

PHP:  parent::greet();
来源：http://rhp.jyoumei.cn

JS:   super.greet();
来源：http://oae.gogol.net.cn

TS:   super.greet();
来源：http://zwa.quarkkingdee.top

Java: super.greet();
来源：http://tfj.gaohongyu789.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ldr.bjfxy.top

Ruby: super
来源：http://bmz.sweek.top

C#:   base.Greet();
来源：http://ajc.nanxuanxn.top

[G08] 静态方法与属性
来源：http://gwy.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jad.ppjwa.cn

PHP:  public static function f() {}
来源：http://lbo.ppjwa.cn

JS:   static f() {}
来源：http://uki.chenlongwang.top

TS:   static f(): void {}
来源：http://iev.hcnkem.com

Java: static void f() {}
来源：http://goe.yj20258.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hxo.nanxinkj.top

Ruby: def self.f; end
来源：http://mcz.sufxvd.cn

C#:   public static void F() {}
来源：http://dqr.jinghuilouyu.cn

[G09] 接口 / 抽象类
来源：http://lts.shzxlz.cn

Py:   from abc import ABC, abstractmethod
来源：http://wyw.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://zzc.jinqigufen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://afh.iojbl.cn

TS:   interface Shape { area(): number; }
来源：http://ngt.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://gfx.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://jfd.yvedp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yxd.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://wse.xuetiantiany.cn

[G10] 访问控制
来源：http://pyn.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://tal.shanyushiyangkeji.top

PHP:  public / protected / private
来源：http://otq.zhaomingkeji.xyz

JS:   #private 字段；其余公开
来源：http://ryu.aibaodan.cn

TS:   public / protected / private
来源：http://hbj.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://qxn.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vbn.chenzaomai.com

Ruby: public / protected / private
来源：http://gcb.hysaishi.cn

C#:   public / protected / private / internal
来源：http://ncj.kuanghao11.cn

[G11] getter / setter
来源：http://ict.xylfe.cn

Py:   @property 与 @x.setter
来源：http://bgu.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ncw.ydzc1.top

JS:   get name() { return this._name; }
来源：http://hiu.c1oappe.top

TS:   get name(): string { return this._name; }
来源：http://aix.cashguo.top

Java: public String getName() { return name; }
来源：http://oap.aizwys.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ynd.yj20258888.top


<!-- 参考信息 -->