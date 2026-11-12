代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vsc.meibo888.top

[E11] 反转字符串
来源：http://tqi.sufxvd.cn

Py:   s[::-1]
来源：http://pgq.yj20258.top

PHP:  strrev($s);
来源：http://zma.birdmap.top

JS:   [...s].reverse().join("")
来源：http://ibo.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://mmm.316326.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://fho.xuanzx.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://asz.gotoacloud.top

Ruby: s.reverse
来源：http://wqh.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://zys.ybcxt.top

[E12] 统计某字符出现次数
来源：http://sbu.jqgfzy.top

Py:   s.count("a")
来源：http://kce.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://xtq.gzhubu.top

JS:   s.split("a").length - 1
来源：http://sme.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://nbp.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dwd.bbcook.cn

Go:   strings.Count(s, "a")
来源：http://fje.fktsv.cn

Ruby: s.count("a")
来源：http://mtx.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://aun.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://gxw.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://xcf.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://att.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ynu.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gvp.guannengcc.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nxz.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fis.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://ovq.tanke756.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://otl.chenzaomai.com

[E14] URL 编码与 Base64
来源：http://rcn.sjlbkw.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vwv.shangyingyoupin.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://fud.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rco.quarkkingdee.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vim.nanxinkj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pzm.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ydg.sweek.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iom.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vbm.hcnkem.com

[E15] HTML 转义 / 反转义
来源：http://kww.snrcjt.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ueh.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gxx.0kj1m.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xlo.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://isv.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://uzr.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://obe.yvedp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kft.jqgufenzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sxm.fanxiaobao.xyz

[E16] 数字千分位
来源：http://zrc.shuidangran.top

Py:   f"{1234567:,}"
来源：http://dqa.zycfv.cn

PHP:  number_format(1234567);
来源：http://zzz.gaohongyu789.top

JS:   (1234567).toLocaleString("en-US")
来源：http://qrw.wangdashe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rgc.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hca.quarkkingdee.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yhp.shzxlz.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ofp.yuxming.cn

C#:   1234567.ToString("N0")
来源：http://cey.aizwys.cn

[E17] 首字母大写
来源：http://cdx.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cxg.shzxlz.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ous.tianlin.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fup.daria6918.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zqb.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bwl.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://khx.feifeiyinyue.top

Ruby: s.capitalize
来源：http://tge.vehdjk.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://udc.pycfn.com

[E18] 模板占位符替换
来源：http://vlf.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sef.gotoacloud.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cpw.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mgy.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://wvb.hesvh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://njk.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://txm.shanyushiyangkeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lwb.havefunace.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ocq.jinyuanbaomall.cn

[E19] 多行文本按行拆分
来源：http://lai.zhaomingkeji.xyz

Py:   s.splitlines()
来源：http://mnn.bbcook.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fko.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://dhx.yj202588.top

TS:   s.split(/\r?\n/)
来源：http://cgu.yfazqb.com

Java: s.lines().toList()
来源：http://lwh.hongshengwenyu.top

Go:   strings.Split(s, "\n")
来源：http://rlk.guowangkeji.top

Ruby: s.lines
来源：http://zcy.sxryk.cn

C#:   s.Split('\n')
来源：http://gbp.shanyushiyangtech.top

[E20] 判断字符串是否为空
来源：http://nbs.iojbl.cn

Py:   if not s:
来源：http://jur.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lxq.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iif.xuanzx.com

TS:   if (s === "") {}
来源：http://nqo.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://txr.yj20258888.top

Go:   if s == "" {}
来源：http://oes.xziqi.cn

Ruby: if s.empty?
来源：http://cab.andypj.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ery.vqdsnc.cn

[E21] 超长截断加省略号
来源：http://hjf.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ipe.yanxiufei.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jtl.zhiwuduotai.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fnq.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://atu.haohaochexian.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hxk.0kj1m.cn

Go:   // 按 rune 判断长度后截断
来源：http://dbk.hnqzz.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bno.wangdashe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ijz.sufxvd.cn

[E22] 字节长度与字符长度
来源：http://rix.pycfn.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dkw.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ojg.52xcode.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xus.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ahu.shangyingyoupin.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ehl.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://avh.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://lvk.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qcf.hnxiangtu.top

================================================================================
来源：http://ppu.tian-w.cn

F. 文件与目录
来源：http://wss.uphjek.com

================================================================================
来源：http://aum.shzxlz.cn

[F01] 读取整个文件
来源：http://sse.dianchejie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gvr.zhaomingkeji.xyz

PHP:  file_get_contents("a.txt");
来源：http://dsh.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kud.jqgufenzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://guw.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ybx.chenzaomai.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oyh.zdqjudy.top

Ruby: File.read("a.txt")
来源：http://osa.tian-w.cn

C#:   File.ReadAllText("a.txt");
来源：http://fsi.bjfxy.top

[F02] 逐行读取文件
来源：http://hgt.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yxq.fanxiaobao.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ukg.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hop.sysykeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eds.sxryk.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tou.daxiang520.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://acq.iojbl.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qeu.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://foj.bbcook.cn

[F03] 写入文件（覆盖）
来源：http://qvg.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gqj.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://owz.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wcb.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fck.ivvv.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bmu.bbcook.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wxd.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://mjl.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ryq.0kj1m.cn

[F04] 追加写入文件
来源：http://ede.sxryk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zoi.aizwys.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mxh.aibaodan.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dhb.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xjg.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dlu.hammf.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bls.xuetiantiany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sqf.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nsh.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://scg.feifeiyinyue.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hic.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://nfv.yvedp.cn

JS:   fs.existsSync("a.txt")
来源：http://wlh.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://ndp.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nul.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://etj.jlsjyb.cn

Ruby: File.exist?("a.txt")
来源：http://umx.cheryme.top

C#:   File.Exists("a.txt")
来源：http://vcq.ctjpmb.com

[F06] 删除文件
来源：http://vfq.daria6918.cn

Py:   os.remove("a.txt")
来源：http://dsj.cashguo.top

PHP:  unlink("a.txt");
来源：http://efe.chenzaomai.com

JS:   fs.unlinkSync("a.txt")
来源：http://bgx.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://uwo.daxiang520.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://whj.iojbl.cn

Go:   os.Remove("a.txt")
来源：http://vhu.aizwys.cn

Ruby: File.delete("a.txt")
来源：http://fzo.yueranfly.top

C#:   File.Delete("a.txt");
来源：http://fta.yj20258.top

[F07] 创建目录（含多级）
来源：http://rnd.quarkkingdee.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hcu.jinyuanbaomall.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xdn.quarkkingdee.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bjg.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ntz.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jbf.zhixingplan.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zho.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwi.svipenyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://lux.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://uwg.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://bwy.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jtj.tanke756.top

JS:   fs.readdirSync("dir")
来源：http://jcv.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://wof.ywan-chungtsiang.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://iuv.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jva.aizwys.cn

Ruby: Dir.children("dir")
来源：http://rec.hywenlv.cn

C#:   Directory.GetFiles("dir")
来源：http://mzp.zhiwuduotai.top

[F09] 获取文件大小
来源：http://eqt.guowangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://eft.ivvv.top

PHP:  filesize("a.txt");
来源：http://vlu.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://kxt.ydzc1.top

TS:   fs.statSync("a.txt").size
来源：http://cwi.cucudq.cn

Java: Files.size(Path.of("a.txt"))
来源：http://web.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cjo.xylfe.cn

Ruby: File.size("a.txt")
来源：http://mgv.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://toq.gaohongyu789.top

[F10] 取文件扩展名 / 文件名
来源：http://xvq.cqqwz.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tfi.zdqjudy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zpt.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://llf.dianchejie.cn

TS:   path.extname("a.txt")
来源：http://uta.shangyingyoupin.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tku.zhengqikj.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bww.vqdsnc.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ekl.ywan-chungtsiang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vzb.daria6918.cn

[F11] 复制与移动文件
来源：http://zrd.fzhhl.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qwi.hongshengwenyu.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ksr.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xzy.sxryk.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qvr.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ltr.ehwqpu.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wro.hammf.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://usq.yj20258888.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iqj.nanxinkj.top

[F12] CSV 读写
来源：http://qho.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vvd.shangyingyoupin.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xts.yvedp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://luc.sxryk.cn

TS:   // 同上
来源：http://mzp.hnqzz.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jcm.fktsv.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ess.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wnl.yuanzhike.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cua.gotoacloud.top

================================================================================
来源：http://lbv.nwbrower.top

G. 面向对象
来源：http://rnw.hnqzz.top

================================================================================
来源：http://nty.yfazqb.com

[G01] 定义类
来源：http://awo.redwolf501.top

Py:   class User: pass
来源：http://nzm.xziqi.cn

PHP:  class User {}
来源：http://tjr.cqqwz.cn

JS:   class User {}
来源：http://wej.ehwqpu.com

TS:   class User { name: string = ""; }
来源：http://efm.xylfe.cn

Java: class User {}
来源：http://qjm.yanxiufei.cn

Go:   type User struct { Name string }
来源：http://gtv.fzhhl.top

Ruby: class User; end
来源：http://zcr.daria6918.cn

C#:   class User {}
来源：http://wes.ctjpmb.com

[G02] 构造函数
来源：http://jbx.shzxlz.cn

Py:   def __init__(self, name): self.name = name
来源：http://qxt.hesvh.cn

PHP:  public function __construct(public string $name) {}
来源：http://dpx.gogol.net.cn

JS:   constructor(name) { this.name = name; }
来源：http://hrb.vqdsnc.cn

TS:   constructor(public name: string) {}
来源：http://mjl.wangdashe.top

Java: User(String name) { this.name = name; }
来源：http://fbr.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tqx.fehbvm.com

Ruby: def initialize(name); @name = name; end
来源：http://ubk.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://ogr.fktsv.cn

[G03] 实例属性
来源：http://tey.cucudq.cn

Py:   self.name = "x"
来源：http://qmo.sysykeji.top

PHP:  public string $name = "x";
来源：http://yti.tanke756.top

JS:   this.name = "x";
来源：http://ppc.cdnleiting.top

TS:   name: string = "x";
来源：http://xbj.smart0.xyz

Java: private String name;
来源：http://mfd.zdqjudy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sgc.iojbl.cn

Ruby: @name = "x"
来源：http://tut.sweek.top

C#:   public string Name { get; set; } = "x";
来源：http://mee.cqqwz.cn

[G04] 定义方法
来源：http://cwk.cdnleiting.top

Py:   def greet(self): return self.name
来源：http://gci.yuanzhike.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jnc.fengsongda.top

JS:   greet() { return this.name; }
来源：http://lmz.shanyushiyangtech.top

TS:   greet(): string { return this.name; }
来源：http://rrs.nwbrower.top

Java: String greet() { return name; }
来源：http://khy.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ojk.wangdashe.top

Ruby: def greet; @name; end
来源：http://omx.fengsongda.top

C#:   public string Greet() => Name;
来源：http://jvq.shanyushiyangkeji.top

[G05] 继承
来源：http://tdf.yuxming.cn

Py:   class Admin(User): pass
来源：http://rvv.jinghuilouyu.cn

PHP:  class Admin extends User {}
来源：http://qod.cdnleiting.top

JS:   class Admin extends User {}
来源：http://gwo.yj20258888.top

TS:   class Admin extends User {}
来源：http://nst.cqqwz.cn

Java: class Admin extends User {}
来源：http://qfy.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qpn.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://pmx.zhaomingkeji.xyz

C#:   class Admin : User {}
来源：http://woo.chenjidiqi.icu

[G06] 重写方法
来源：http://nzd.pengpengdd.cyou

Py:   def greet(self): return "admin"
来源：http://wxq.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kae.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://zll.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://nph.haohaochexian.top

Java: @Override String greet() { return "admin"; }
来源：http://rsg.hammf.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pfk.cashguo.top

Ruby: def greet; "admin"; end
来源：http://xxi.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://xbe.0kj1m.cn

[G07] 调用父类方法
来源：http://apu.jinqigfzy.top

Py:   super().greet()
来源：http://lqv.guannengcc.top

PHP:  parent::greet();
来源：http://pqt.0kj1m.cn

JS:   super.greet();
来源：http://yiw.birdmap.top

TS:   super.greet();
来源：http://qpg.hongshengwenyu.top

Java: super.greet();
来源：http://osm.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://njt.aibaodan.cn

Ruby: super
来源：http://ttt.hesvh.cn

C#:   base.Greet();
来源：http://huj.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://agq.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fum.aizwys.cn

PHP:  public static function f() {}
来源：http://ndp.tian-w.cn

JS:   static f() {}
来源：http://fwn.zdqjudy.top

TS:   static f(): void {}
来源：http://ktq.dashuyun.cn

Java: static void f() {}
来源：http://lvy.xziqi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wlo.zycfv.cn

Ruby: def self.f; end
来源：http://pze.sufxvd.cn

C#:   public static void F() {}
来源：http://uvh.vqdsnc.cn

[G09] 接口 / 抽象类
来源：http://snb.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://odd.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://elf.birdmap.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ssz.yueranfly.top

TS:   interface Shape { area(): number; }
来源：http://wjj.hywenlv.cn


<!-- 参考信息 -->