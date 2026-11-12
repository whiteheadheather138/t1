代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ctr.fzhhl.top

[E11] 反转字符串
来源：http://jri.yj20258888.top

Py:   s[::-1]
来源：http://tgn.fehbvm.com

PHP:  strrev($s);
来源：http://xrb.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://wdg.havefunace.top

TS:   [...s].reverse().join("")
来源：http://jbs.pengpengdd.cyou

Java: new StringBuilder(s).reverse().toString()
来源：http://xvt.gzhubu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://izv.aizwys.cn

Ruby: s.reverse
来源：http://vwr.chenzaomai.com

C#:   new string(s.Reverse().ToArray())
来源：http://zgy.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://pxs.cheryme.top

Py:   s.count("a")
来源：http://xpa.hnxiangtu.top

PHP:  substr_count($s, "a");
来源：http://joh.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://vsc.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://oio.fktsv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qfj.ydjk.org.cn

Go:   strings.Count(s, "a")
来源：http://lpc.ywan-chungtsiang.top

Ruby: s.count("a")
来源：http://vbd.fktsv.cn

C#:   s.Count(c => c == 'a')
来源：http://nfy.xylfe.cn

[E13] 逐字符遍历
来源：http://aav.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://cel.zhijiandao.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://way.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://axd.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nlm.xuanzx.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wie.jiagoushi.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://icl.redwolf501.top

Ruby: s.each_char { |ch| puts ch }
来源：http://xsx.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hzs.guannengcc.top

[E14] URL 编码与 Base64
来源：http://ryo.vqdsnc.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jvv.xinyue.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://meo.smart0.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uub.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mef.svipenyu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ufv.zhoulong.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dma.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ooz.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pif.cucudq.cn

[E15] HTML 转义 / 反转义
来源：http://ovg.pycfn.com

Py:   html.escape(s);  html.unescape(s)
来源：http://dmv.meibo888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lex.zdbjq.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pwt.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://drv.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dti.shangyingyoupin.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ygm.xuetiantiany.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hvg.yueranfly.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ule.hammf.cn

[E16] 数字千分位
来源：http://vxs.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://uvq.yj20258.top

PHP:  number_format(1234567);
来源：http://jql.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://xua.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://sog.zhoulong.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lvy.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jgg.shuidangran.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iuj.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://hsd.nanxuanxn.top

[E17] 首字母大写
来源：http://cqe.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tmg.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://iyq.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lyz.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewv.zhoulong.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lzb.yvedp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nro.ivvv.top

Ruby: s.capitalize
来源：http://lib.zhoulong.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ecz.jinyuanbaomall.cn

[E18] 模板占位符替换
来源：http://qxm.jinghuilouyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://itu.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zgz.andypj.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://wuw.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gkp.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jvj.ywan-chungtsiang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hrx.mhx1999.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ddd.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wer.dashuyun.cn

[E19] 多行文本按行拆分
来源：http://wdk.xuetiantiany.cn

Py:   s.splitlines()
来源：http://int.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ckd.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://inv.yj20258888.top

TS:   s.split(/\r?\n/)
来源：http://cuq.jianghu66.top

Java: s.lines().toList()
来源：http://mty.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://ocj.ydjk.org.cn

Ruby: s.lines
来源：http://rev.fzhhl.top

C#:   s.Split('\n')
来源：http://zrs.hongshengwenyu.top

[E20] 判断字符串是否为空
来源：http://hkj.wangdashe.top

Py:   if not s:
来源：http://myx.jinyuanbaomall.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zzb.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xap.aibaodan.cn

TS:   if (s === "") {}
来源：http://mry.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://qcz.nanxinkj.top

Go:   if s == "" {}
来源：http://ybq.jinqigfzy.top

Ruby: if s.empty?
来源：http://qlt.fktsv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dkw.jinyuanbaomall.cn

[E21] 超长截断加省略号
来源：http://yij.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ttr.zhiwuduotai.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vkh.jinghuilouyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blx.zhiwuduotai.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eby.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://irx.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://zjh.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cph.ivvv.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ubf.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://jrk.iojbl.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cvs.zhaomingkeji.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tvu.epnwcf.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mlp.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eij.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vju.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tkh.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://hey.jianghu66.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rgb.fzhhl.top

================================================================================
来源：http://asy.xuetiantiany.cn

F. 文件与目录
来源：http://lcx.bbcook.cn

================================================================================
来源：http://xsl.yangfankeji.com

[F01] 读取整个文件
来源：http://oqe.hesvh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qmz.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://ojp.daxiang520.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cvn.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kzc.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://gfx.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ens.guannengcc.top

Ruby: File.read("a.txt")
来源：http://lwd.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://jed.zhijiandao.cn

[F02] 逐行读取文件
来源：http://fam.quarkkingdee.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ivz.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ubc.tarul.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://akf.sweek.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lxl.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cdc.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://goe.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zxz.cdnleiting.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://atc.cqqwz.cn

[F03] 写入文件（覆盖）
来源：http://qtp.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dgf.hnxiangtu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://exg.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nee.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lno.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gss.hnqzz.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ecx.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://tit.jyoumei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xgo.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://vxu.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dmi.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hix.shzxlz.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mdp.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ces.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jzh.jyoumei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dgt.yj202588.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rda.xziqi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xea.yfazqb.com

[F05] 判断文件或目录是否存在
来源：http://wxy.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://slz.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://sjj.zhoulong.xyz

JS:   fs.existsSync("a.txt")
来源：http://byu.xziqi.cn

TS:   fs.existsSync("a.txt")
来源：http://nye.guowangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bua.feifeiyinyue.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dwi.tarul.cn

Ruby: File.exist?("a.txt")
来源：http://pib.hnxiangtu.top

C#:   File.Exists("a.txt")
来源：http://gmv.tian-w.cn

[F06] 删除文件
来源：http://jto.yangfankeji.com

Py:   os.remove("a.txt")
来源：http://bea.tarul.cn

PHP:  unlink("a.txt");
来源：http://ziu.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jdd.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://gla.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lwj.cheryme.top

Go:   os.Remove("a.txt")
来源：http://zsb.shzxlz.cn

Ruby: File.delete("a.txt")
来源：http://jvx.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://cdd.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://nbw.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yce.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qqc.yonumen.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wdx.jqgfzy.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aib.ywan-chungtsiang.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qyw.shanyushiyangkeji.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jnh.smart0.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yap.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lhh.jiagoushi.top

[F08] 遍历目录
来源：http://lit.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://tss.yfazqb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vwu.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://lxs.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://yfb.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ltm.sysykeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://urn.jinyuanbaomall.cn

Ruby: Dir.children("dir")
来源：http://dsj.bbcook.cn

C#:   Directory.GetFiles("dir")
来源：http://izd.sxryk.cn

[F09] 获取文件大小
来源：http://qmx.fzhhl.top

Py:   os.path.getsize("a.txt")
来源：http://qvh.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://cwj.guannengcc.top

JS:   fs.statSync("a.txt").size
来源：http://rbj.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://atr.bbcook.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fis.ehwqpu.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pau.jqgufenzy.top

Ruby: File.size("a.txt")
来源：http://ejf.gogol.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://itn.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://kre.nanxuanxn.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://arw.aizwys.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iar.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://znq.hnqzz.top

TS:   path.extname("a.txt")
来源：http://jnr.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://voo.shanyushiyangtech.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ukw.gotoacloud.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xzt.feifeiyinyue.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lsw.zhixingplan.top

[F11] 复制与移动文件
来源：http://ujz.fehbvm.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tyu.redwolf501.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://evq.mhx1999.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jfm.guannengcc.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zxo.yueranfly.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gls.xuanzx.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cmm.pycfn.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ktw.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fcq.yonumen.top

[F12] CSV 读写
来源：http://wmi.yuxming.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tvf.daria6918.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ket.yj202588.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oua.jlsjyb.cn

TS:   // 同上
来源：http://cjm.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zeb.ydjk.org.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tpk.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oum.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://ypn.nanxinkj.top

================================================================================
来源：http://vik.yanxiufei.cn

G. 面向对象
来源：http://rye.0kj1m.cn

================================================================================
来源：http://ver.wangdashe.top

[G01] 定义类
来源：http://ekh.nanxinkj.top

Py:   class User: pass
来源：http://nei.sweek.top

PHP:  class User {}
来源：http://tuv.0kj1m.cn

JS:   class User {}
来源：http://ljf.tarul.cn

TS:   class User { name: string = ""; }
来源：http://bvt.yangfankeji.com

Java: class User {}
来源：http://rnq.tarul.cn

Go:   type User struct { Name string }
来源：http://gqe.yuanzhike.top

Ruby: class User; end
来源：http://xsm.shzxlz.cn

C#:   class User {}
来源：http://cxg.yj202588.top

[G02] 构造函数
来源：http://ysm.quarkkingdee.top

Py:   def __init__(self, name): self.name = name
来源：http://qiv.zhijiandao.cn

PHP:  public function __construct(public string $name) {}
来源：http://chl.0kj1m.cn

JS:   constructor(name) { this.name = name; }
来源：http://hjd.fanxiaobao.xyz

TS:   constructor(public name: string) {}
来源：http://qqk.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://qyz.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gid.gaohongyu789.top

Ruby: def initialize(name); @name = name; end
来源：http://wnx.fzhhl.top

C#:   public User(string name) { Name = name; }
来源：http://slh.dashuyun.cn

[G03] 实例属性
来源：http://ilc.xuanzx.com

Py:   self.name = "x"
来源：http://ttr.nanxinkj.top

PHP:  public string $name = "x";
来源：http://mqu.chenjidiqi.icu

JS:   this.name = "x";
来源：http://hfd.ppjwa.cn

TS:   name: string = "x";
来源：http://hat.wangdashe.top

Java: private String name;
来源：http://onh.shzxlz.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qeu.fktsv.cn

Ruby: @name = "x"
来源：http://dhy.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://coo.guowangkeji.top

[G04] 定义方法
来源：http://ibr.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://zjw.zhiwuduotai.top

PHP:  public function greet(): string { return $this->name; }
来源：http://hyc.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://pqp.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://jnw.yuxming.cn

Java: String greet() { return name; }
来源：http://gju.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vrf.hnqzz.top

Ruby: def greet; @name; end
来源：http://ucz.xingfuxueyuan.xyz

C#:   public string Greet() => Name;
来源：http://hgk.wangdashe.top

[G05] 继承
来源：http://ifn.cheryme.top

Py:   class Admin(User): pass
来源：http://zid.andypj.xyz

PHP:  class Admin extends User {}
来源：http://psv.ybcxt.top

JS:   class Admin extends User {}
来源：http://luf.bbcook.cn

TS:   class Admin extends User {}
来源：http://crn.hywenlv.cn

Java: class Admin extends User {}
来源：http://mdu.yvedp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vbx.zhengqikj.top

Ruby: class Admin < User; end
来源：http://mrh.fengsongda.top

C#:   class Admin : User {}
来源：http://zio.fktsv.cn

[G06] 重写方法
来源：http://cjc.sufxvd.cn

Py:   def greet(self): return "admin"
来源：http://qnd.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://jfr.cashguo.top

JS:   greet() { return "admin"; }
来源：http://zwd.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://byn.jlsjyb.cn

Java: @Override String greet() { return "admin"; }
来源：http://gwz.shangyingyoupin.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qip.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://gxg.zycfv.cn

C#:   public override string Greet() => "admin";
来源：http://fzm.xingfuxueyuan.xyz

[G07] 调用父类方法
来源：http://ter.dashuyun.cn

Py:   super().greet()
来源：http://ekf.jqgufenzy.top

PHP:  parent::greet();
来源：http://vns.jiagoushi.top

JS:   super.greet();
来源：http://iho.quarkkingdee.top

TS:   super.greet();
来源：http://rwo.xuetiantiany.cn

Java: super.greet();
来源：http://obz.pycfn.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xzg.ctjpmb.com

Ruby: super
来源：http://mbj.sxryk.cn

C#:   base.Greet();
来源：http://dbj.zhixingplan.top

[G08] 静态方法与属性
来源：http://liy.shzxlz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dbd.sweek.top

PHP:  public static function f() {}
来源：http://yhy.yongpay.top

JS:   static f() {}
来源：http://cca.52xcode.cn

TS:   static f(): void {}
来源：http://anq.nanxinkj.top

Java: static void f() {}
来源：http://yve.haohaochexian.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ivy.guowangkeji.top

Ruby: def self.f; end
来源：http://cnm.sufxvd.cn

C#:   public static void F() {}
来源：http://ljy.c1oappe.top

[G09] 接口 / 抽象类
来源：http://rcv.gotoacloud.top

Py:   from abc import ABC, abstractmethod
来源：http://lob.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://zbd.aibaodan.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://utb.daxiang520.top

TS:   interface Shape { area(): number; }
来源：http://qza.nwbrower.top


<!-- 参考信息 -->