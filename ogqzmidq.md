代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://foh.yj202588.top

[E11] 反转字符串
来源：http://yke.ppjwa.cn

Py:   s[::-1]
来源：http://wgm.fktsv.cn

PHP:  strrev($s);
来源：http://lrt.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://lpo.wangshuangyany.cn

TS:   [...s].reverse().join("")
来源：http://jur.yvedp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qxd.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://pey.tanke756.top

Ruby: s.reverse
来源：http://oku.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://apt.yj20258888.top

[E12] 统计某字符出现次数
来源：http://rkw.jinyuanbaomall.cn

Py:   s.count("a")
来源：http://xbq.snrcjt.cn

PHP:  substr_count($s, "a");
来源：http://een.birdmap.top

JS:   s.split("a").length - 1
来源：http://bnv.gogol.net.cn

TS:   s.split("a").length - 1
来源：http://kzl.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dsx.316326.xyz

Go:   strings.Count(s, "a")
来源：http://tmx.zhengqikj.top

Ruby: s.count("a")
来源：http://ult.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://etg.cheryme.top

[E13] 逐字符遍历
来源：http://pov.yuxming.cn

Py:   for ch in s: print(ch)
来源：http://deh.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qon.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kkh.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ata.hnxiangtu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bnn.ppjwa.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vul.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xql.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://brm.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://abt.jqgfzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vxu.haohaochexian.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zwk.yonumen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ajc.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xpq.yfazqb.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jli.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fyf.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ako.jinghuilouyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ret.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://wex.iojbl.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pvy.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iak.hfpthk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://csd.316326.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://nak.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tho.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://juy.yuanzhike.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zak.xingfuxueyuan.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://enw.dianchejie.cn

[E16] 数字千分位
来源：http://vbs.mhx1999.top

Py:   f"{1234567:,}"
来源：http://ngg.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://qah.ivvv.top

JS:   (1234567).toLocaleString("en-US")
来源：http://glq.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://skz.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gnc.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xqa.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nno.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://hme.tanke756.top

[E17] 首字母大写
来源：http://zwb.cucudq.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wfy.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jrz.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://voi.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cnw.wangdashe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tcp.wangshuangyany.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nsp.daria6918.cn

Ruby: s.capitalize
来源：http://fvr.uphjek.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rsa.ivvv.top

[E18] 模板占位符替换
来源：http://lwa.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yhm.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://srv.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://unu.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://too.shangyingyoupin.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lmm.fengsongda.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xyv.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fgp.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sfo.xuanzx.com

[E19] 多行文本按行拆分
来源：http://lxv.aibaodan.cn

Py:   s.splitlines()
来源：http://pxy.tianlin.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yin.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://fan.ehwqpu.com

TS:   s.split(/\r?\n/)
来源：http://hbl.yj20258.top

Java: s.lines().toList()
来源：http://lmb.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://yvv.tianlin.xyz

Ruby: s.lines
来源：http://gqx.fehbvm.com

C#:   s.Split('\n')
来源：http://ier.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://szx.gaohongyu789.top

Py:   if not s:
来源：http://wri.hnqzz.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dxv.xingfuxueyuan.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vtf.hnqzz.top

TS:   if (s === "") {}
来源：http://rjb.dianchejie.cn

Java: if (s.isEmpty()) {}
来源：http://qvx.shanyushiyangkeji.top

Go:   if s == "" {}
来源：http://xas.jinqigufen.top

Ruby: if s.empty?
来源：http://jyb.mhx1999.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yoz.nanxuanxn.top

[E21] 超长截断加省略号
来源：http://ojt.nwbrower.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vwj.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yrf.pengpengdd.cyou

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gvz.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vvt.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vou.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://tbk.316326.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tgy.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ewj.jinghuilouyu.cn

[E22] 字节长度与字符长度
来源：http://uzl.yj20258.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dcv.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mft.birdmap.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ppr.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dip.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bjy.hcnkem.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eig.fehbvm.com

Ruby: s.bytesize;  s.length
来源：http://ucv.bbcook.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zra.9152youxi.cn

================================================================================
来源：http://vmr.yongpay.top

F. 文件与目录
来源：http://xpn.andypj.xyz

================================================================================
来源：http://fpq.xziqi.cn

[F01] 读取整个文件
来源：http://bwf.bjfxy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vkz.ywan-chungtsiang.top

PHP:  file_get_contents("a.txt");
来源：http://bty.sysykeji.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ucr.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://anf.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://veu.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hml.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://vyo.xingfuxueyuan.xyz

C#:   File.ReadAllText("a.txt");
来源：http://zdu.haohaochexian.top

[F02] 逐行读取文件
来源：http://zcj.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gys.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hrz.shangyingyoupin.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lsq.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lnm.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fax.ywan-chungtsiang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://god.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gyb.hysaishi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dsz.jianghu66.top

[F03] 写入文件（覆盖）
来源：http://xev.yuanzhike.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xlk.jiagoushi.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xty.hnqzz.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zwe.hammf.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fnp.shangyingyoupin.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nqj.haohaochexian.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hrh.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://gpa.chenjidiqi.icu

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wtj.hnqzz.top

[F04] 追加写入文件
来源：http://flp.jinqigfzy.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jpg.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wyl.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://his.yueranfly.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bed.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qhy.gogol.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://frn.yueranfly.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://suu.bbcook.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jfi.redwolf501.top

[F05] 判断文件或目录是否存在
来源：http://dvh.sjlbkw.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ncz.cheryme.top

PHP:  file_exists("a.txt");
来源：http://zqb.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://mbb.0kj1m.cn

TS:   fs.existsSync("a.txt")
来源：http://ilr.yuanzhike.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jdx.hfpthk.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sky.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://gjr.jinqigufen.top

C#:   File.Exists("a.txt")
来源：http://rjo.kuanghao11.cn

[F06] 删除文件
来源：http://zxj.yongpay.top

Py:   os.remove("a.txt")
来源：http://mdw.andypj.xyz

PHP:  unlink("a.txt");
来源：http://uum.hcnkem.com

JS:   fs.unlinkSync("a.txt")
来源：http://uqp.gogol.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fvg.yj20258888.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dhr.jyoumei.cn

Go:   os.Remove("a.txt")
来源：http://pyd.fzhhl.top

Ruby: File.delete("a.txt")
来源：http://oqr.jlsjyb.cn

C#:   File.Delete("a.txt");
来源：http://dhy.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://fel.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gkl.9152youxi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ozr.ywan-chungtsiang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xxv.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://izc.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://usd.redwolf501.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rqi.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqe.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://owh.birdmap.top

[F08] 遍历目录
来源：http://ciq.shangyingyoupin.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://vcw.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xmu.daria6918.cn

JS:   fs.readdirSync("dir")
来源：http://yju.nanxinkj.top

TS:   fs.readdirSync("dir")
来源：http://ehw.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lkc.shanyushiyangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mds.zhaomingkeji.xyz

Ruby: Dir.children("dir")
来源：http://qvp.epnwcf.com

C#:   Directory.GetFiles("dir")
来源：http://urk.yuanzhike.top

[F09] 获取文件大小
来源：http://ijj.jinyuanbaomall.cn

Py:   os.path.getsize("a.txt")
来源：http://wnc.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://qup.tian-w.cn

JS:   fs.statSync("a.txt").size
来源：http://evn.tarul.cn

TS:   fs.statSync("a.txt").size
来源：http://rcv.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://kcr.yj202588.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gup.hfpthk.cn

Ruby: File.size("a.txt")
来源：http://pip.tian-w.cn

C#:   new FileInfo("a.txt").Length
来源：http://wkx.jinghuilouyu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ivm.pengpengdd.cyou

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vek.yvedp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tye.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fww.pengpengdd.cyou

TS:   path.extname("a.txt")
来源：http://zcb.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wtm.mhx1999.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hnd.ehwqpu.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://imq.yueranfly.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uim.kuanghao11.cn

[F11] 复制与移动文件
来源：http://gbg.hnqzz.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xel.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ezh.yfazqb.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vpx.tianlin.xyz

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yre.chenjidiqi.icu

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://krb.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mkf.yonumen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://etd.ivvv.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hhy.jyoumei.cn

[F12] CSV 读写
来源：http://toa.aibaodan.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qnz.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://oum.jiagoushi.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zwf.xylfe.cn

TS:   // 同上
来源：http://jec.shanyushiyangtech.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ypw.haohaochexian.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dci.hywenlv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://twd.guowangkeji.top

C#:   // 无内置：用 CsvHelper 库
来源：http://eti.havefunace.top

================================================================================
来源：http://cyt.yonumen.top

G. 面向对象
来源：http://dyb.smart0.xyz

================================================================================
来源：http://gvu.tianlin.xyz

[G01] 定义类
来源：http://mep.hfpthk.cn

Py:   class User: pass
来源：http://nlr.yfazqb.com

PHP:  class User {}
来源：http://spm.mhx1999.top

JS:   class User {}
来源：http://itx.yonumen.top

TS:   class User { name: string = ""; }
来源：http://ary.yfazqb.com

Java: class User {}
来源：http://fsu.andypj.xyz

Go:   type User struct { Name string }
来源：http://hcs.yj20258.top

Ruby: class User; end
来源：http://lyf.cqqwz.cn

C#:   class User {}
来源：http://ykq.jinyuanbaomall.cn

[G02] 构造函数
来源：http://yvp.jlsjyb.cn

Py:   def __init__(self, name): self.name = name
来源：http://age.guowangkeji.top

PHP:  public function __construct(public string $name) {}
来源：http://kne.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://bcw.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://wos.yuanzhike.top

Java: User(String name) { this.name = name; }
来源：http://emh.xingfuxueyuan.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yhg.zhixingplan.top

Ruby: def initialize(name); @name = name; end
来源：http://sqk.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://rvx.tarul.cn

[G03] 实例属性
来源：http://mqw.yfazqb.com

Py:   self.name = "x"
来源：http://ptw.quarkkingdee.top

PHP:  public string $name = "x";
来源：http://uyf.zhongyouzk.top

JS:   this.name = "x";
来源：http://hib.zhaomingkeji.xyz

TS:   name: string = "x";
来源：http://ofd.tian-w.cn

Java: private String name;
来源：http://cyb.shangyingyoupin.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://znd.yj202588.top

Ruby: @name = "x"
来源：http://pky.jinqigfzy.top

C#:   public string Name { get; set; } = "x";
来源：http://xmj.daxiang520.top

[G04] 定义方法
来源：http://bwm.shuidangran.top

Py:   def greet(self): return self.name
来源：http://qkm.sufxvd.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mqd.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://xiq.yuxming.cn

TS:   greet(): string { return this.name; }
来源：http://xij.ppjwa.cn

Java: String greet() { return name; }
来源：http://ooz.quarkkingdee.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ofb.ehwqpu.com

Ruby: def greet; @name; end
来源：http://yvm.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://tba.vehdjk.com

[G05] 继承
来源：http://upm.feifeiyinyue.top

Py:   class Admin(User): pass
来源：http://huq.jianghu66.top

PHP:  class Admin extends User {}
来源：http://sgr.fengsongda.top

JS:   class Admin extends User {}
来源：http://gme.haohaochexian.top

TS:   class Admin extends User {}
来源：http://mto.gzhubu.top

Java: class Admin extends User {}
来源：http://qvb.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kuz.ppjwa.cn

Ruby: class Admin < User; end
来源：http://kyg.zhijiandao.cn

C#:   class Admin : User {}
来源：http://qhm.ctjpmb.com

[G06] 重写方法
来源：http://ias.epnwcf.com

Py:   def greet(self): return "admin"
来源：http://ysn.feifeiyinyue.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hpk.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://thi.fehbvm.com

TS:   greet(): string { return "admin"; }
来源：http://eio.fzhhl.top

Java: @Override String greet() { return "admin"; }
来源：http://ude.shzxlz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mln.fktsv.cn

Ruby: def greet; "admin"; end
来源：http://hbu.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://cuy.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://qam.ydzc1.top

Py:   super().greet()
来源：http://wxs.yonumen.top

PHP:  parent::greet();
来源：http://ddg.jqgufenzy.top

JS:   super.greet();
来源：http://uir.c1oappe.top

TS:   super.greet();
来源：http://iqj.bbcook.cn

Java: super.greet();
来源：http://yph.fzhhl.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zyb.daria6918.cn

Ruby: super
来源：http://wif.haohaochexian.top

C#:   base.Greet();
来源：http://ksq.sxryk.cn

[G08] 静态方法与属性
来源：http://zrc.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qch.shanyushiyangtech.top

PHP:  public static function f() {}
来源：http://htj.gotoacloud.top

JS:   static f() {}
来源：http://fef.nanxuanxn.top

TS:   static f(): void {}
来源：http://mmq.xuanzx.com

Java: static void f() {}
来源：http://wmd.ivvv.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://tek.xziqi.cn

Ruby: def self.f; end
来源：http://gow.fengsongda.top

C#:   public static void F() {}
来源：http://bkx.fanxiaobao.xyz

[G09] 接口 / 抽象类
来源：http://gut.zhijiandao.cn

Py:   from abc import ABC, abstractmethod
来源：http://drc.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ygo.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cmb.sufxvd.cn

TS:   interface Shape { area(): number; }
来源：http://sbe.dashuyun.cn


<!-- 参考信息 -->