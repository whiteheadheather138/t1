代发 wailian999

Ruby: s.reverse
来源：http://xcd.yvedp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wfo.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://mkf.jiagoushi.top

Py:   s.count("a")
来源：http://iwz.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://hpb.yuanzhike.top

JS:   s.split("a").length - 1
来源：http://jww.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://jgc.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qce.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://mlm.cqqwz.cn

Ruby: s.count("a")
来源：http://dlz.vehdjk.com

C#:   s.Count(c => c == 'a')
来源：http://mrz.yfazqb.com

[E13] 逐字符遍历
来源：http://okb.c1oappe.top

Py:   for ch in s: print(ch)
来源：http://nty.yonumen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pbq.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://mmx.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cfs.smart0.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://upm.haohaochexian.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gza.tianlin.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://msx.zhengqikj.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qgd.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://uup.ppjwa.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pnj.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://yxn.tanke756.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rvn.c1oappe.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fjb.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vbp.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lsw.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://okr.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rgq.birdmap.top

[E15] HTML 转义 / 反转义
来源：http://fqp.ywan-chungtsiang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dzl.yangfankeji.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://twn.zdqjudy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lkm.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iuo.fanxiaobao.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ezt.tian-w.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wii.hammf.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://klr.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tqk.guannengcc.top

[E16] 数字千分位
来源：http://kmx.jqgfzy.top

Py:   f"{1234567:,}"
来源：http://dyp.xylfe.cn

PHP:  number_format(1234567);
来源：http://vmj.cashguo.top

JS:   (1234567).toLocaleString("en-US")
来源：http://spf.cdnleiting.top

TS:   (1234567).toLocaleString("en-US")
来源：http://anh.sysykeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cep.jqgfzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cna.zhijiandao.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rki.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://czy.ctjpmb.com

[E17] 首字母大写
来源：http://exw.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gez.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qaw.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nyb.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rbv.epnwcf.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fvy.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xwd.ydzc1.top

Ruby: s.capitalize
来源：http://esu.daria6918.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xap.ctjpmb.com

[E18] 模板占位符替换
来源：http://wlf.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gux.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qnq.nwbrower.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uge.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://ind.yvedp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cnz.hammf.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fpc.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ski.yfazqb.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://noz.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://yqj.zhiwuduotai.top

Py:   s.splitlines()
来源：http://xym.zhijiandao.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hzp.nanxuanxn.top

JS:   s.split(/\r?\n/)
来源：http://mkg.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://gga.zhoulong.xyz

Java: s.lines().toList()
来源：http://hgp.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://ntf.fktsv.cn

Ruby: s.lines
来源：http://yxn.316326.xyz

C#:   s.Split('\n')
来源：http://usl.hcnkem.com

[E20] 判断字符串是否为空
来源：http://vhw.vqdsnc.cn

Py:   if not s:
来源：http://tbf.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yow.fengsongda.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lls.zhixingplan.top

TS:   if (s === "") {}
来源：http://ucs.52xcode.cn

Java: if (s.isEmpty()) {}
来源：http://wma.zhiwuduotai.top

Go:   if s == "" {}
来源：http://yak.zhijiandao.cn

Ruby: if s.empty?
来源：http://fry.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wsr.hysaishi.cn

[E21] 超长截断加省略号
来源：http://dxi.aizwys.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fob.yueranfly.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wgy.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ywh.epnwcf.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qqn.snrcjt.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xel.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://elm.zycfv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ulp.feifeiyinyue.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nfu.zhiwuduotai.top

[E22] 字节长度与字符长度
来源：http://zmq.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wzv.smart0.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ygj.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://taj.zhaomingkeji.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://twe.xinyue.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qnz.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://riy.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://nay.hesvh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ula.chenzaomai.com

================================================================================
来源：http://bsz.9152youxi.cn

F. 文件与目录
来源：http://jkk.shanyushiyangtech.top

================================================================================
来源：http://tho.gzhubu.top

[F01] 读取整个文件
来源：http://rih.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ldb.316326.xyz

PHP:  file_get_contents("a.txt");
来源：http://oge.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kav.ppjwa.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dzl.aizwys.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://byg.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gws.daria6918.cn

Ruby: File.read("a.txt")
来源：http://ldq.316326.xyz

C#:   File.ReadAllText("a.txt");
来源：http://nhz.hnxiangtu.top

[F02] 逐行读取文件
来源：http://pmg.jinghuilouyu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gfc.yanxiufei.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ztb.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aks.cqqwz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tvy.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ehc.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rsy.hammf.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tdf.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://elw.iojbl.cn

[F03] 写入文件（覆盖）
来源：http://uva.nanxinkj.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cdu.nwbrower.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://raf.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dnp.ydjk.org.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wlj.c1oappe.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://klj.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tnd.cdnleiting.top

Ruby: File.write("a.txt", "hi")
来源：http://swg.tanke756.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ljs.jinqigufen.top

[F04] 追加写入文件
来源：http://zaz.fengsongda.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nfx.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wrw.gogol.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dbe.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kxo.tarul.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wpz.jinqigufen.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ysh.yvedp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://thz.tanke756.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pit.ywan-chungtsiang.top

[F05] 判断文件或目录是否存在
来源：http://ybi.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tqo.jianghu66.top

PHP:  file_exists("a.txt");
来源：http://xru.sysykeji.top

JS:   fs.existsSync("a.txt")
来源：http://mrt.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://bnq.yueranfly.top

Java: Files.exists(Path.of("a.txt"))
来源：http://svb.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bxn.shzxlz.cn

Ruby: File.exist?("a.txt")
来源：http://ozz.zdqjudy.top

C#:   File.Exists("a.txt")
来源：http://cht.xziqi.cn

[F06] 删除文件
来源：http://gct.yj20258888.top

Py:   os.remove("a.txt")
来源：http://hpb.mhx1999.top

PHP:  unlink("a.txt");
来源：http://ixo.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ngh.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://eym.sjlbkw.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cvt.cdnleiting.top

Go:   os.Remove("a.txt")
来源：http://smk.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://xqd.epnwcf.com

C#:   File.Delete("a.txt");
来源：http://bba.yangfankeji.com

[F07] 创建目录（含多级）
来源：http://bsp.shangyingyoupin.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fyc.jyoumei.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qeh.meibo888.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bns.hywenlv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tzc.chenzaomai.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ueb.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ykc.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tln.yanxiufei.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vqy.shzxlz.cn

[F08] 遍历目录
来源：http://eay.havefunace.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://twj.zycfv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bbu.shanyushiyangtech.top

JS:   fs.readdirSync("dir")
来源：http://kln.yanxiufei.cn

TS:   fs.readdirSync("dir")
来源：http://drh.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xuy.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tcd.smart0.xyz

Ruby: Dir.children("dir")
来源：http://mfn.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://frw.zhoulong.xyz

[F09] 获取文件大小
来源：http://hsf.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://urp.ydzc1.top

PHP:  filesize("a.txt");
来源：http://rxr.yj202588.top

JS:   fs.statSync("a.txt").size
来源：http://hvz.nanxuanxn.top

TS:   fs.statSync("a.txt").size
来源：http://gsa.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gzm.yfazqb.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rcf.daria6918.cn

Ruby: File.size("a.txt")
来源：http://gpa.redwolf501.top

C#:   new FileInfo("a.txt").Length
来源：http://fpc.yj20258.top

[F10] 取文件扩展名 / 文件名
来源：http://cto.daria6918.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pyz.yongpay.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ppe.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tff.nanxuanxn.top

TS:   path.extname("a.txt")
来源：http://dpq.hnxiangtu.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hge.yvedp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xfi.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://aeh.9152youxi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tdl.daria6918.cn

[F11] 复制与移动文件
来源：http://xqk.andypj.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ema.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fqx.hongshengwenyu.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eeh.shanyushiyangtech.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://exj.quarkkingdee.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ubs.iojbl.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bbh.yfazqb.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kkn.dashuyun.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cge.tarul.cn

[F12] CSV 读写
来源：http://urn.nanxinkj.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jjr.xingfuxueyuan.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rfj.bjfxy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uig.hammf.cn

TS:   // 同上
来源：http://kda.ivvv.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vrp.vqdsnc.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://csa.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pan.316326.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://lny.ydzc1.top

================================================================================
来源：http://njv.snrcjt.cn

G. 面向对象
来源：http://bgo.feifeiyinyue.top

================================================================================
来源：http://xim.dashuyun.cn

[G01] 定义类
来源：http://xcb.gotoacloud.top

Py:   class User: pass
来源：http://ikw.sjlbkw.cn

PHP:  class User {}
来源：http://vtf.chenzaomai.com

JS:   class User {}
来源：http://whp.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://jmg.wangshuangyany.cn

Java: class User {}
来源：http://fml.bjfxy.top

Go:   type User struct { Name string }
来源：http://dyg.uphjek.com

Ruby: class User; end
来源：http://bvn.guowangkeji.top

C#:   class User {}
来源：http://gbd.hongshengwenyu.top

[G02] 构造函数
来源：http://gcz.jinghuilouyu.cn

Py:   def __init__(self, name): self.name = name
来源：http://cyd.aibaodan.cn

PHP:  public function __construct(public string $name) {}
来源：http://sfw.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://wiw.bbcook.cn

TS:   constructor(public name: string) {}
来源：http://uti.iojbl.cn

Java: User(String name) { this.name = name; }
来源：http://mxl.redwolf501.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fik.zhiwuduotai.top

Ruby: def initialize(name); @name = name; end
来源：http://wkq.birdmap.top

C#:   public User(string name) { Name = name; }
来源：http://cbp.jinqigfzy.top

[G03] 实例属性
来源：http://lex.jiagoushi.top

Py:   self.name = "x"
来源：http://lrh.jianghu66.top

PHP:  public string $name = "x";
来源：http://asf.aibaodan.cn

JS:   this.name = "x";
来源：http://buh.yanxiufei.cn

TS:   name: string = "x";
来源：http://lzs.jyoumei.cn

Java: private String name;
来源：http://kdy.fzhhl.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rqp.andypj.xyz

Ruby: @name = "x"
来源：http://kku.mhx1999.top

C#:   public string Name { get; set; } = "x";
来源：http://cbw.jinqigfzy.top

[G04] 定义方法
来源：http://jij.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://tfh.daria6918.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vce.sweek.top

JS:   greet() { return this.name; }
来源：http://skz.ydzc1.top

TS:   greet(): string { return this.name; }
来源：http://vqh.sjlbkw.cn

Java: String greet() { return name; }
来源：http://abp.gzhubu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://atk.xinyue.icu

Ruby: def greet; @name; end
来源：http://lyb.uphjek.com

C#:   public string Greet() => Name;
来源：http://hyf.jinghuilouyu.cn

[G05] 继承
来源：http://llx.meibo888.top

Py:   class Admin(User): pass
来源：http://xce.hesvh.cn

PHP:  class Admin extends User {}
来源：http://toc.shanyushiyangkeji.top

JS:   class Admin extends User {}
来源：http://zyj.aizwys.cn

TS:   class Admin extends User {}
来源：http://njb.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://pmx.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xkx.ctjpmb.com

Ruby: class Admin < User; end
来源：http://syl.yangfankeji.com

C#:   class Admin : User {}
来源：http://gbh.smart0.xyz

[G06] 重写方法
来源：http://zba.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://pgi.ctjpmb.com

PHP:  public function greet(): string { return "admin"; }
来源：http://rgl.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://ava.nanxinkj.top

TS:   greet(): string { return "admin"; }
来源：http://jii.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://shp.sufxvd.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mul.yueranfly.top

Ruby: def greet; "admin"; end
来源：http://ywt.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://pim.hysaishi.cn

[G07] 调用父类方法
来源：http://qfz.jqgfzy.top

Py:   super().greet()
来源：http://myz.xziqi.cn

PHP:  parent::greet();
来源：http://beq.xinyue.icu

JS:   super.greet();
来源：http://qsn.cashguo.top

TS:   super.greet();
来源：http://sfa.zhijiandao.cn

Java: super.greet();
来源：http://twk.pengpengdd.cyou

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rxp.jiagoushi.top

Ruby: super
来源：http://wkz.bjfxy.top

C#:   base.Greet();
来源：http://mlo.yanxiufei.cn

[G08] 静态方法与属性
来源：http://pgz.shanyushiyangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ymq.hfpthk.cn

PHP:  public static function f() {}
来源：http://cia.cashguo.top

JS:   static f() {}
来源：http://rrj.epnwcf.com

TS:   static f(): void {}
来源：http://bic.yfazqb.com

Java: static void f() {}
来源：http://wdv.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ahs.gogol.net.cn

Ruby: def self.f; end
来源：http://tau.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://pts.bjfxy.top

[G09] 接口 / 抽象类
来源：http://thq.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://bwo.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://ixl.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://orc.meibo888.top

TS:   interface Shape { area(): number; }
来源：http://vbf.shuidangran.top

Java: interface Shape { double area(); }
来源：http://qgz.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://oeu.fanxiaobao.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pdu.hfpthk.cn

C#:   interface IShape { double Area(); }
来源：http://raa.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://peh.meibo888.top

Py:   约定 _protected / __private（不强制）
来源：http://msw.nanxuanxn.top

PHP:  public / protected / private
来源：http://rqe.fehbvm.com

JS:   #private 字段；其余公开
来源：http://gsl.ctjpmb.com


<!-- 参考信息 -->