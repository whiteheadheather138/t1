代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kuz.sjlbkw.cn

[E11] 反转字符串
来源：http://aqb.meibo888.top

Py:   s[::-1]
来源：http://uqt.shuidangran.top

PHP:  strrev($s);
来源：http://vns.dianchejie.cn

JS:   [...s].reverse().join("")
来源：http://yza.meibo888.top

TS:   [...s].reverse().join("")
来源：http://col.yj20258.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xpc.sufxvd.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mds.cashguo.top

Ruby: s.reverse
来源：http://ase.gaohongyu789.top

C#:   new string(s.Reverse().ToArray())
来源：http://nlv.hywenlv.cn

[E12] 统计某字符出现次数
来源：http://xtw.guannengcc.top

Py:   s.count("a")
来源：http://wcv.nwbrower.top

PHP:  substr_count($s, "a");
来源：http://diu.sweek.top

JS:   s.split("a").length - 1
来源：http://rjy.cdnleiting.top

TS:   s.split("a").length - 1
来源：http://oyk.cashguo.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qef.zhaomingkeji.xyz

Go:   strings.Count(s, "a")
来源：http://sln.316326.xyz

Ruby: s.count("a")
来源：http://vdt.cashguo.top

C#:   s.Count(c => c == 'a')
来源：http://lfo.zhengqikj.top

[E13] 逐字符遍历
来源：http://vlo.9152youxi.cn

Py:   for ch in s: print(ch)
来源：http://sdr.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://taa.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://odu.ivvv.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tux.pengpengdd.cyou

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://goe.epnwcf.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nql.shzxlz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sdk.yvedp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://nlm.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://upl.zycfv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fyh.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hqg.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hde.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bar.zhongyouzk.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://twi.ehwqpu.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fxy.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wow.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gsf.hfpthk.cn

[E15] HTML 转义 / 反转义
来源：http://bud.zhijiandao.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lfy.zhijiandao.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://skb.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fba.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cgm.hnqzz.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zup.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uiu.mhx1999.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ufs.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wbc.tanke756.top

[E16] 数字千分位
来源：http://eid.yangfankeji.com

Py:   f"{1234567:,}"
来源：http://cog.zdqjudy.top

PHP:  number_format(1234567);
来源：http://vkm.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qzj.nanxinkj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dub.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dfc.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jus.jinghuilouyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xer.sysykeji.top

C#:   1234567.ToString("N0")
来源：http://fgi.ydzc1.top

[E17] 首字母大写
来源：http://uqj.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kwk.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://tbp.ctjpmb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wzt.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bnj.shuidangran.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mzm.zhaomingkeji.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lpg.pengpengdd.cyou

Ruby: s.capitalize
来源：http://puq.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://npp.uphjek.com

[E18] 模板占位符替换
来源：http://kgd.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xuc.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mdw.cucudq.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kom.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://mov.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kgp.jinqigufen.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ixc.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://stp.pycfn.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rjg.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://hvj.ivvv.top

Py:   s.splitlines()
来源：http://ped.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jld.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://poq.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://niw.zhijiandao.cn

Java: s.lines().toList()
来源：http://uza.xylfe.cn

Go:   strings.Split(s, "\n")
来源：http://afq.yanxiufei.cn

Ruby: s.lines
来源：http://ahh.gaohongyu789.top

C#:   s.Split('\n')
来源：http://rxb.sjlbkw.cn

[E20] 判断字符串是否为空
来源：http://yxy.meibo888.top

Py:   if not s:
来源：http://fmz.316326.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mzm.jinyuanbaomall.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dfa.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://opz.cdnleiting.top

Java: if (s.isEmpty()) {}
来源：http://tme.birdmap.top

Go:   if s == "" {}
来源：http://kbj.cheryme.top

Ruby: if s.empty?
来源：http://rpy.xuetiantiany.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yia.zdqjudy.top

[E21] 超长截断加省略号
来源：http://xra.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://epu.9152youxi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fjs.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nym.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvn.zdqjudy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dar.ybcxt.top

Go:   // 按 rune 判断长度后截断
来源：http://dgs.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://aiy.ybcxt.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vzs.andypj.xyz

[E22] 字节长度与字符长度
来源：http://bse.andypj.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fre.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://equ.cucudq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lye.ehwqpu.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://glv.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yay.cucudq.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://coj.haohaochexian.top

Ruby: s.bytesize;  s.length
来源：http://emd.birdmap.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dly.shzxlz.cn

================================================================================
来源：http://lei.yuxming.cn

F. 文件与目录
来源：http://wqb.ydjk.org.cn

================================================================================
来源：http://mwa.yfazqb.com

[F01] 读取整个文件
来源：http://byo.birdmap.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://okk.xinyue.icu

PHP:  file_get_contents("a.txt");
来源：http://esg.aizwys.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://osi.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kne.cdnleiting.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fwi.bbcook.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dbj.yj202588.top

Ruby: File.read("a.txt")
来源：http://ofo.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://biv.uphjek.com

[F02] 逐行读取文件
来源：http://evc.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://axh.ivvv.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hqz.haohaochexian.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rlo.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dap.sysykeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fkq.ppjwa.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://frp.shzxlz.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dxh.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://svw.cashguo.top

[F03] 写入文件（覆盖）
来源：http://oaz.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dlc.hywenlv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zjk.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bif.jinqigfzy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qqi.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://owu.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mwp.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://rys.yangfankeji.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tvx.cqqwz.cn

[F04] 追加写入文件
来源：http://uzz.fzhhl.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://awa.hnxiangtu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cgq.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mck.fzhhl.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sxh.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ooa.sweek.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pmd.guannengcc.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xkq.cqqwz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://std.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://tqw.zdqjudy.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yil.zhongyouzk.top

PHP:  file_exists("a.txt");
来源：http://fnn.cqqwz.cn

JS:   fs.existsSync("a.txt")
来源：http://qxv.sysykeji.top

TS:   fs.existsSync("a.txt")
来源：http://oco.zhongyouzk.top

Java: Files.exists(Path.of("a.txt"))
来源：http://lcj.vqdsnc.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ktv.ehwqpu.com

Ruby: File.exist?("a.txt")
来源：http://qiq.tian-w.cn

C#:   File.Exists("a.txt")
来源：http://nkc.mhx1999.top

[F06] 删除文件
来源：http://jko.pengpengdd.cyou

Py:   os.remove("a.txt")
来源：http://weg.sweek.top

PHP:  unlink("a.txt");
来源：http://fsk.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://nul.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://ecw.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://arr.jiagoushi.top

Go:   os.Remove("a.txt")
来源：http://iuu.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://zup.cheryme.top

C#:   File.Delete("a.txt");
来源：http://dwr.bjfxy.top

[F07] 创建目录（含多级）
来源：http://jsc.xingfuxueyuan.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vdv.jinqigufen.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xmy.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrf.yangfankeji.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ddx.yuxming.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vqx.pengpengdd.cyou

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bej.tian-w.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gjs.tianlin.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://clo.ydzc1.top

[F08] 遍历目录
来源：http://svw.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tji.0kj1m.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://crm.fehbvm.com

JS:   fs.readdirSync("dir")
来源：http://obo.xylfe.cn

TS:   fs.readdirSync("dir")
来源：http://zsp.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mjg.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nbu.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://pka.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://ntk.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://rhr.epnwcf.com

Py:   os.path.getsize("a.txt")
来源：http://sjr.yongpay.top

PHP:  filesize("a.txt");
来源：http://rbm.ydjk.org.cn

JS:   fs.statSync("a.txt").size
来源：http://fea.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://ybm.gotoacloud.top

Java: Files.size(Path.of("a.txt"))
来源：http://ifz.haohaochexian.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pqz.daxiang520.top

Ruby: File.size("a.txt")
来源：http://kxu.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://xap.sweek.top

[F10] 取文件扩展名 / 文件名
来源：http://iwi.meibo888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cig.gzhubu.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kmk.shzxlz.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aiq.haohaochexian.top

TS:   path.extname("a.txt")
来源：http://luh.meibo888.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aff.tianlin.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://psk.hnxiangtu.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eow.yj20258888.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://trz.uphjek.com

[F11] 复制与移动文件
来源：http://iav.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://osq.xingfuxueyuan.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fdr.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jhw.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cgk.nanxuanxn.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bnb.gaohongyu789.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bjs.zhoulong.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hvy.quarkkingdee.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vlc.ivvv.top

[F12] CSV 读写
来源：http://zhd.fanxiaobao.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lxr.jyoumei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kgh.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ptb.ivvv.top

TS:   // 同上
来源：http://rww.gaohongyu789.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tcu.yfazqb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yqu.shangyingyoupin.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://njv.fanxiaobao.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://kfi.shzxlz.cn

================================================================================
来源：http://gia.shzxlz.cn

G. 面向对象
来源：http://mqu.nwbrower.top

================================================================================
来源：http://esf.svipenyu.cn

[G01] 定义类
来源：http://mos.jinyuanbaomall.cn

Py:   class User: pass
来源：http://kod.hammf.cn

PHP:  class User {}
来源：http://npk.ivvv.top

JS:   class User {}
来源：http://svq.zdqjudy.top

TS:   class User { name: string = ""; }
来源：http://kpc.andypj.xyz

Java: class User {}
来源：http://lnb.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://frz.zdbjq.cn

Ruby: class User; end
来源：http://pad.52xcode.cn

C#:   class User {}
来源：http://mil.svipenyu.cn

[G02] 构造函数
来源：http://qer.ybcxt.top

Py:   def __init__(self, name): self.name = name
来源：http://xkb.316326.xyz

PHP:  public function __construct(public string $name) {}
来源：http://ola.havefunace.top

JS:   constructor(name) { this.name = name; }
来源：http://jio.mhx1999.top

TS:   constructor(public name: string) {}
来源：http://nmm.52xcode.cn

Java: User(String name) { this.name = name; }
来源：http://bqc.fanxiaobao.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yrg.xinyue.icu

Ruby: def initialize(name); @name = name; end
来源：http://trs.vehdjk.com

C#:   public User(string name) { Name = name; }
来源：http://lai.sweek.top

[G03] 实例属性
来源：http://auj.zhixingplan.top

Py:   self.name = "x"
来源：http://gtt.nanxinkj.top

PHP:  public string $name = "x";
来源：http://tbs.gogol.net.cn

JS:   this.name = "x";
来源：http://sza.wangdashe.top

TS:   name: string = "x";
来源：http://esr.pycfn.com

Java: private String name;
来源：http://reb.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pny.snrcjt.cn

Ruby: @name = "x"
来源：http://hbl.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://cdt.chenlongwang.top

[G04] 定义方法
来源：http://fqc.9152youxi.cn

Py:   def greet(self): return self.name
来源：http://tuy.zhoulong.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://ixh.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://gno.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://fqc.quarkkingdee.top

Java: String greet() { return name; }
来源：http://rgw.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://fvt.316326.xyz

Ruby: def greet; @name; end
来源：http://pbn.pycfn.com

C#:   public string Greet() => Name;
来源：http://bze.gogol.net.cn

[G05] 继承
来源：http://yol.hcnkem.com

Py:   class Admin(User): pass
来源：http://aed.daria6918.cn

PHP:  class Admin extends User {}
来源：http://niz.gotoacloud.top

JS:   class Admin extends User {}
来源：http://pri.birdmap.top

TS:   class Admin extends User {}
来源：http://dvm.iojbl.cn

Java: class Admin extends User {}
来源：http://pxe.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ujx.xuanzx.com

Ruby: class Admin < User; end
来源：http://wht.hysaishi.cn

C#:   class Admin : User {}
来源：http://lyx.sjlbkw.cn

[G06] 重写方法
来源：http://pwb.haohaochexian.top

Py:   def greet(self): return "admin"
来源：http://wyn.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cxr.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://egq.ctjpmb.com

TS:   greet(): string { return "admin"; }
来源：http://bfp.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://nqv.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fqn.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://qwj.c1oappe.top

C#:   public override string Greet() => "admin";
来源：http://cpz.ydjk.org.cn

[G07] 调用父类方法
来源：http://kgm.ehwqpu.com

Py:   super().greet()
来源：http://vzz.jianghu66.top

PHP:  parent::greet();
来源：http://ehb.xinyue.icu

JS:   super.greet();
来源：http://vqc.zhiwuduotai.top

TS:   super.greet();
来源：http://vao.ywan-chungtsiang.top

Java: super.greet();
来源：http://hze.yangfankeji.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rai.zhoulong.xyz

Ruby: super
来源：http://luc.yj20258.top

C#:   base.Greet();
来源：http://bjz.gaohongyu789.top

[G08] 静态方法与属性
来源：http://dbh.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://avg.bbcook.cn

PHP:  public static function f() {}
来源：http://esb.fengsongda.top

JS:   static f() {}
来源：http://sxg.yvedp.cn

TS:   static f(): void {}
来源：http://lxk.zhengqikj.top

Java: static void f() {}
来源：http://brp.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jau.epnwcf.com

Ruby: def self.f; end
来源：http://kbg.svipenyu.cn

C#:   public static void F() {}
来源：http://twv.ybcxt.top

[G09] 接口 / 抽象类
来源：http://rcr.fehbvm.com

Py:   from abc import ABC, abstractmethod
来源：http://cox.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://quo.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://wea.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://ohq.cashguo.top


<!-- 参考信息 -->