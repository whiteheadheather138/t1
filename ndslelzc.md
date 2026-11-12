代发 wailian999

PHP:  substr_count($s, "a");
来源：http://nnl.yanxiufei.cn

JS:   s.split("a").length - 1
来源：http://tdj.yj202588.top

TS:   s.split("a").length - 1
来源：http://ybz.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gna.ydzc1.top

Go:   strings.Count(s, "a")
来源：http://mif.pycfn.com

Ruby: s.count("a")
来源：http://msn.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://rll.jinqigufen.top

[E13] 逐字符遍历
来源：http://vum.fehbvm.com

Py:   for ch in s: print(ch)
来源：http://xwg.quarkkingdee.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mkq.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://ire.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://hgd.hnqzz.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ljn.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://crl.yangfankeji.com

Ruby: s.each_char { |ch| puts ch }
来源：http://qph.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ytj.ivvv.top

[E14] URL 编码与 Base64
来源：http://dwq.fzhhl.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://opu.fktsv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sra.yvedp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nqz.sweek.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sac.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qmj.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xih.hnqzz.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bhc.fengsongda.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nlk.chenjidiqi.icu

[E15] HTML 转义 / 反转义
来源：http://wup.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://sip.ywan-chungtsiang.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dye.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://owz.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ycv.meibo888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mup.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hun.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tpt.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dch.fehbvm.com

[E16] 数字千分位
来源：http://tsc.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://oel.tanke756.top

PHP:  number_format(1234567);
来源：http://sip.yueranfly.top

JS:   (1234567).toLocaleString("en-US")
来源：http://gke.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://ktm.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mlk.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bfh.fehbvm.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sqc.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://eux.c1oappe.top

[E17] 首字母大写
来源：http://rec.kuanghao11.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bvj.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://fgr.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kro.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://udw.jinqigfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fyt.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bca.ybcxt.top

Ruby: s.capitalize
来源：http://nfw.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zcx.sysykeji.top

[E18] 模板占位符替换
来源：http://vsn.mhx1999.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qin.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nmh.hammf.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iby.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://ykd.xziqi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://osg.iojbl.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://erl.snrcjt.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hsa.bbcook.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zux.sxryk.cn

[E19] 多行文本按行拆分
来源：http://bra.hywenlv.cn

Py:   s.splitlines()
来源：http://mpc.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oqs.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://hrh.zhongyouzk.top

TS:   s.split(/\r?\n/)
来源：http://vfd.chenzaomai.com

Java: s.lines().toList()
来源：http://xxn.feifeiyinyue.top

Go:   strings.Split(s, "\n")
来源：http://ubj.hysaishi.cn

Ruby: s.lines
来源：http://ahb.yj20258.top

C#:   s.Split('\n')
来源：http://zyi.c1oappe.top

[E20] 判断字符串是否为空
来源：http://xyh.tanke756.top

Py:   if not s:
来源：http://eef.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uno.guannengcc.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cgy.hysaishi.cn

TS:   if (s === "") {}
来源：http://wbh.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://rge.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://dxa.shangyingyoupin.top

Ruby: if s.empty?
来源：http://wdp.hammf.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yed.havefunace.top

[E21] 超长截断加省略号
来源：http://vjd.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zqr.shzxlz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://unb.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvw.shanyushiyangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcz.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fnn.jianghu66.top

Go:   // 按 rune 判断长度后截断
来源：http://svc.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nlq.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xlh.zhaomingkeji.xyz

[E22] 字节长度与字符长度
来源：http://hfw.316326.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://piz.xingfuxueyuan.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://omy.yj20258888.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qiu.316326.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cdk.sufxvd.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bdf.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vss.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://lzh.bjfxy.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gvq.hysaishi.cn

================================================================================
来源：http://cuk.cheryme.top

F. 文件与目录
来源：http://blz.jyoumei.cn

================================================================================
来源：http://mva.zycfv.cn

[F01] 读取整个文件
来源：http://kdi.aibaodan.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pva.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://lna.uphjek.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://acr.ctjpmb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eat.xingfuxueyuan.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://uck.nwbrower.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ifq.jyoumei.cn

Ruby: File.read("a.txt")
来源：http://hiw.hywenlv.cn

C#:   File.ReadAllText("a.txt");
来源：http://jtv.fehbvm.com

[F02] 逐行读取文件
来源：http://llz.ppjwa.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gmm.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jwa.hfpthk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxx.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oex.jinyuanbaomall.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ufe.gaohongyu789.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mbs.jinghuilouyu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zih.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ali.aizwys.cn

[F03] 写入文件（覆盖）
来源：http://csj.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zhi.guowangkeji.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://kfa.daxiang520.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://izi.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gyx.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tsh.nanxinkj.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rvj.ctjpmb.com

Ruby: File.write("a.txt", "hi")
来源：http://czs.tarul.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gqk.pycfn.com

[F04] 追加写入文件
来源：http://emu.ydzc1.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uue.zhoulong.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://aor.cqqwz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jvn.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lny.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cug.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rkl.52xcode.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yje.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zer.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://qtd.chenzaomai.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yek.xinyue.icu

PHP:  file_exists("a.txt");
来源：http://ehl.tianlin.xyz

JS:   fs.existsSync("a.txt")
来源：http://eqf.fzhhl.top

TS:   fs.existsSync("a.txt")
来源：http://yrn.ywan-chungtsiang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tyt.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zon.andypj.xyz

Ruby: File.exist?("a.txt")
来源：http://alt.yueranfly.top

C#:   File.Exists("a.txt")
来源：http://cul.shangyingyoupin.top

[F06] 删除文件
来源：http://ikr.tian-w.cn

Py:   os.remove("a.txt")
来源：http://uja.tarul.cn

PHP:  unlink("a.txt");
来源：http://jxh.zhoulong.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://bag.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iqv.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yic.smart0.xyz

Go:   os.Remove("a.txt")
来源：http://vlz.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://zxe.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://iis.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://xmt.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qun.xingfuxueyuan.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ydt.jqgufenzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fmk.jinqigufen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://euu.gaohongyu789.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qet.wangshuangyany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://erw.jyoumei.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vtf.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ynw.zhongyouzk.top

[F08] 遍历目录
来源：http://trh.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wmv.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dqf.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://nfu.gogol.net.cn

TS:   fs.readdirSync("dir")
来源：http://feo.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tka.yj202588.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://egc.316326.xyz

Ruby: Dir.children("dir")
来源：http://zgc.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://kby.haohaochexian.top

[F09] 获取文件大小
来源：http://myg.jqgufenzy.top

Py:   os.path.getsize("a.txt")
来源：http://bfa.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://oza.0kj1m.cn

JS:   fs.statSync("a.txt").size
来源：http://qfl.snrcjt.cn

TS:   fs.statSync("a.txt").size
来源：http://uqb.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mus.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ngm.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://xdw.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://nsq.hfpthk.cn

[F10] 取文件扩展名 / 文件名
来源：http://izl.fengsongda.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://afb.redwolf501.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mui.dianchejie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uxv.shangyingyoupin.top

TS:   path.extname("a.txt")
来源：http://dza.xingfuxueyuan.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tvz.quarkkingdee.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lwc.quarkkingdee.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oeu.yangfankeji.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sfv.ywan-chungtsiang.top

[F11] 复制与移动文件
来源：http://ycf.fengsongda.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ovc.316326.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://szc.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dzz.tanke756.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lod.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hce.xinyue.icu

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rkl.uphjek.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cpe.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gbw.aizwys.cn

[F12] CSV 读写
来源：http://kcy.nanxuanxn.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bkv.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bnp.xuanzx.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eso.cqqwz.cn

TS:   // 同上
来源：http://fmi.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bei.hfpthk.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://meo.tian-w.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://njj.jinqigfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://por.zhiwuduotai.top

================================================================================
来源：http://dta.sufxvd.cn

G. 面向对象
来源：http://hiq.xuanzx.com

================================================================================
来源：http://tzi.birdmap.top

[G01] 定义类
来源：http://vit.ywan-chungtsiang.top

Py:   class User: pass
来源：http://eck.hongshengwenyu.top

PHP:  class User {}
来源：http://sgu.sysykeji.top

JS:   class User {}
来源：http://qvb.pengpengdd.cyou

TS:   class User { name: string = ""; }
来源：http://eyu.wangshuangyany.cn

Java: class User {}
来源：http://ldh.0kj1m.cn

Go:   type User struct { Name string }
来源：http://yls.mhx1999.top

Ruby: class User; end
来源：http://msl.52xcode.cn

C#:   class User {}
来源：http://uag.ctjpmb.com

[G02] 构造函数
来源：http://xns.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://rcm.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://kuk.yongpay.top

JS:   constructor(name) { this.name = name; }
来源：http://imr.guannengcc.top

TS:   constructor(public name: string) {}
来源：http://pjh.xuetiantiany.cn

Java: User(String name) { this.name = name; }
来源：http://ftc.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ykc.jlsjyb.cn

Ruby: def initialize(name); @name = name; end
来源：http://jqr.shanyushiyangtech.top

C#:   public User(string name) { Name = name; }
来源：http://jpc.gotoacloud.top

[G03] 实例属性
来源：http://iqg.nanxuanxn.top

Py:   self.name = "x"
来源：http://rrc.yuanzhike.top

PHP:  public string $name = "x";
来源：http://okb.gzhubu.top

JS:   this.name = "x";
来源：http://grn.zdqjudy.top

TS:   name: string = "x";
来源：http://vxc.hongshengwenyu.top

Java: private String name;
来源：http://ldl.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jzj.zhengqikj.top

Ruby: @name = "x"
来源：http://dqt.fktsv.cn

C#:   public string Name { get; set; } = "x";
来源：http://irm.feifeiyinyue.top

[G04] 定义方法
来源：http://fti.jqgufenzy.top

Py:   def greet(self): return self.name
来源：http://mxb.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kyl.daxiang520.top

JS:   greet() { return this.name; }
来源：http://liu.smart0.xyz

TS:   greet(): string { return this.name; }
来源：http://rcn.yvedp.cn

Java: String greet() { return name; }
来源：http://zqg.sufxvd.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ztx.ctjpmb.com

Ruby: def greet; @name; end
来源：http://ghj.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://kif.c1oappe.top

[G05] 继承
来源：http://vai.zycfv.cn

Py:   class Admin(User): pass
来源：http://sna.pycfn.com

PHP:  class Admin extends User {}
来源：http://jtz.chenzaomai.com

JS:   class Admin extends User {}
来源：http://awl.sweek.top

TS:   class Admin extends User {}
来源：http://fal.xinyue.icu

Java: class Admin extends User {}
来源：http://yvp.cheryme.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zvc.jianghu66.top

Ruby: class Admin < User; end
来源：http://lfk.wangshuangyany.cn

C#:   class Admin : User {}
来源：http://blv.zhiwuduotai.top

[G06] 重写方法
来源：http://swq.wangshuangyany.cn

Py:   def greet(self): return "admin"
来源：http://yjw.quarkkingdee.top

PHP:  public function greet(): string { return "admin"; }
来源：http://frm.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://lrl.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://efe.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://iji.yvedp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yed.ctjpmb.com

Ruby: def greet; "admin"; end
来源：http://uye.wangshuangyany.cn

C#:   public override string Greet() => "admin";
来源：http://dbb.gzhubu.top

[G07] 调用父类方法
来源：http://vtz.0kj1m.cn

Py:   super().greet()
来源：http://jvf.wangshuangyany.cn

PHP:  parent::greet();
来源：http://woy.ybcxt.top

JS:   super.greet();
来源：http://rsj.fzhhl.top

TS:   super.greet();
来源：http://twg.uphjek.com

Java: super.greet();
来源：http://ein.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xhx.0kj1m.cn

Ruby: super
来源：http://fyj.andypj.xyz

C#:   base.Greet();
来源：http://pru.cucudq.cn

[G08] 静态方法与属性
来源：http://ukl.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gxc.yj202588.top

PHP:  public static function f() {}
来源：http://ozb.52xcode.cn

JS:   static f() {}
来源：http://xth.guannengcc.top

TS:   static f(): void {}
来源：http://ufl.fanxiaobao.xyz

Java: static void f() {}
来源：http://frj.andypj.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://psb.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://cvy.tanke756.top

C#:   public static void F() {}
来源：http://hqk.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://nva.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://biy.bjfxy.top

PHP:  interface Shape { public function area(): float; }
来源：http://ywh.9152youxi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dur.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://rzz.daxiang520.top

Java: interface Shape { double area(); }
来源：http://nbt.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://zlt.yj20258.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ntw.yueranfly.top

C#:   interface IShape { double Area(); }
来源：http://nts.aibaodan.cn

[G10] 访问控制
来源：http://uek.chenzaomai.com

Py:   约定 _protected / __private（不强制）
来源：http://sow.c1oappe.top

PHP:  public / protected / private
来源：http://wov.ehwqpu.com

JS:   #private 字段；其余公开
来源：http://xxu.sufxvd.cn

TS:   public / protected / private
来源：http://jle.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://xbd.jinqigufen.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oll.yangfankeji.com

Ruby: public / protected / private
来源：http://rzi.pengpengdd.cyou


<!-- 参考信息 -->