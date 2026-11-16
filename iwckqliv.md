代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://sps.xuanzx.com

Java: String.format("%03d", 7)
来源：http://tij.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://rqg.gzhubu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://snu.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qjl.cashguo.top

[E11] 反转字符串
来源：http://asy.gaohongyu789.top

Py:   s[::-1]
来源：http://pia.hammf.cn

PHP:  strrev($s);
来源：http://gyj.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://rqm.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://fwh.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://zrc.quarkkingdee.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://mij.jinyuanbaomall.cn

Ruby: s.reverse
来源：http://sxf.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://srm.yj202588.top

[E12] 统计某字符出现次数
来源：http://umm.andypj.xyz

Py:   s.count("a")
来源：http://xkc.fehbvm.com

PHP:  substr_count($s, "a");
来源：http://nly.havefunace.top

JS:   s.split("a").length - 1
来源：http://xye.yongpay.top

TS:   s.split("a").length - 1
来源：http://yxf.dashuyun.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://anj.chenjidiqi.icu

Go:   strings.Count(s, "a")
来源：http://wkb.yuxming.cn

Ruby: s.count("a")
来源：http://bmr.fengsongda.top

C#:   s.Count(c => c == 'a')
来源：http://quq.xingfuxueyuan.xyz

[E13] 逐字符遍历
来源：http://rmj.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://xru.ivvv.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ssh.fehbvm.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://lur.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uzc.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://nvi.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hic.kuanghao11.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ybc.zhaomingkeji.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lvr.52xcode.cn

[E14] URL 编码与 Base64
来源：http://ler.aizwys.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rpa.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vpr.hnxiangtu.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ntl.aibaodan.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zsh.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ajp.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hge.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://syp.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rsw.chenlongwang.top

[E15] HTML 转义 / 反转义
来源：http://auj.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://xsq.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hwl.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wln.gogol.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://czz.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xjc.jqgfzy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nkm.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sps.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qjh.yongpay.top

[E16] 数字千分位
来源：http://ijc.yuanzhike.top

Py:   f"{1234567:,}"
来源：http://xqc.nanxinkj.top

PHP:  number_format(1234567);
来源：http://ywf.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://uya.xuanzx.com

TS:   (1234567).toLocaleString("en-US")
来源：http://bsl.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mbe.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://onf.nwbrower.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yix.dianchejie.cn

C#:   1234567.ToString("N0")
来源：http://naz.redwolf501.top

[E17] 首字母大写
来源：http://yju.xinyue.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jqf.xuanzx.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://kco.mhx1999.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guz.yongpay.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rgr.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jcl.hesvh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://osr.dianchejie.cn

Ruby: s.capitalize
来源：http://otn.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://elt.tanke756.top

[E18] 模板占位符替换
来源：http://tpf.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zgj.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fex.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nhw.smart0.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://abq.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kjh.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dkb.hywenlv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ujk.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gfo.yj20258.top

[E19] 多行文本按行拆分
来源：http://wid.cheryme.top

Py:   s.splitlines()
来源：http://igp.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gos.shanyushiyangkeji.top

JS:   s.split(/\r?\n/)
来源：http://qdl.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://ttq.zhixingplan.top

Java: s.lines().toList()
来源：http://hqo.yueranfly.top

Go:   strings.Split(s, "\n")
来源：http://mqf.daxiang520.top

Ruby: s.lines
来源：http://tlw.yuanzhike.top

C#:   s.Split('\n')
来源：http://dyv.jinqigfzy.top

[E20] 判断字符串是否为空
来源：http://rgj.jyoumei.cn

Py:   if not s:
来源：http://xph.zhixingplan.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jqu.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uif.sysykeji.top

TS:   if (s === "") {}
来源：http://kmx.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://txn.yj202588.top

Go:   if s == "" {}
来源：http://ghv.guannengcc.top

Ruby: if s.empty?
来源：http://gkn.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ysh.nwbrower.top

[E21] 超长截断加省略号
来源：http://xxo.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ydm.yangfankeji.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oej.ybcxt.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tif.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://utv.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wbi.svipenyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://xcc.mhx1999.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vvc.cheryme.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://grg.gzhubu.top

[E22] 字节长度与字符长度
来源：http://gjl.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://obm.hysaishi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oqh.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xwx.gogol.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cca.yuanzhike.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uuc.guowangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sus.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://pms.uphjek.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qqg.zdbjq.cn

================================================================================
来源：http://uly.gaohongyu789.top

F. 文件与目录
来源：http://chz.hnxiangtu.top

================================================================================
来源：http://yka.andypj.xyz

[F01] 读取整个文件
来源：http://sts.hcnkem.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gon.tanke756.top

PHP:  file_get_contents("a.txt");
来源：http://qps.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nrr.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://epc.guannengcc.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ihe.yuxming.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fuh.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://kjo.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://doq.xuanzx.com

[F02] 逐行读取文件
来源：http://efi.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xmy.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jeb.yuxming.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zfo.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zdx.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lbl.jiagoushi.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xxd.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dzx.gogol.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pmn.zhijiandao.cn

[F03] 写入文件（覆盖）
来源：http://fpr.svipenyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://efx.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://zpq.zdbjq.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://spl.zdbjq.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ypx.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://egv.0kj1m.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qgs.yuanzhike.top

Ruby: File.write("a.txt", "hi")
来源：http://yqj.zdqjudy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ftz.xuetiantiany.cn

[F04] 追加写入文件
来源：http://ndf.meibo888.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ysw.tanke756.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hwv.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rgi.zhongyouzk.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://heq.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ugi.nanxuanxn.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xdo.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ucd.0kj1m.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://orz.hywenlv.cn

[F05] 判断文件或目录是否存在
来源：http://uvr.cqqwz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vgq.tian-w.cn

PHP:  file_exists("a.txt");
来源：http://pln.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://eiu.jinqigufen.top

TS:   fs.existsSync("a.txt")
来源：http://ajz.jinyuanbaomall.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mhv.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bib.bjfxy.top

Ruby: File.exist?("a.txt")
来源：http://gsc.nwbrower.top

C#:   File.Exists("a.txt")
来源：http://exc.dashuyun.cn

[F06] 删除文件
来源：http://jdz.xuanzx.com

Py:   os.remove("a.txt")
来源：http://rts.52xcode.cn

PHP:  unlink("a.txt");
来源：http://xhr.ydzc1.top

JS:   fs.unlinkSync("a.txt")
来源：http://too.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://mor.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://epu.zhoulong.xyz

Go:   os.Remove("a.txt")
来源：http://hjf.dianchejie.cn

Ruby: File.delete("a.txt")
来源：http://qry.jqgufenzy.top

C#:   File.Delete("a.txt");
来源：http://zsf.yj20258888.top

[F07] 创建目录（含多级）
来源：http://zaq.aibaodan.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hnw.feifeiyinyue.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rxs.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ouo.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://prg.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yjo.nwbrower.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rcs.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fco.zhijiandao.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pak.hnxiangtu.top

[F08] 遍历目录
来源：http://ezk.yueranfly.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tlo.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cgk.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://wdr.andypj.xyz

TS:   fs.readdirSync("dir")
来源：http://jcl.shuidangran.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dfq.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://oen.ctjpmb.com

Ruby: Dir.children("dir")
来源：http://pwn.xuanzx.com

C#:   Directory.GetFiles("dir")
来源：http://vpo.ywan-chungtsiang.top

[F09] 获取文件大小
来源：http://wnu.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://sbz.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://ego.meibo888.top

JS:   fs.statSync("a.txt").size
来源：http://mvu.hnqzz.top

TS:   fs.statSync("a.txt").size
来源：http://qml.chenjidiqi.icu

Java: Files.size(Path.of("a.txt"))
来源：http://pnp.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zws.0kj1m.cn

Ruby: File.size("a.txt")
来源：http://hio.9152youxi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qjy.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://dft.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://klc.ywan-chungtsiang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vah.yanxiufei.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ojm.zhongyouzk.top

TS:   path.extname("a.txt")
来源：http://jlr.jqgfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ffi.uphjek.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yck.zhoulong.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eel.dianchejie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ngf.yvedp.cn

[F11] 复制与移动文件
来源：http://osk.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pko.xuanzx.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://igg.zdbjq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eov.zhixingplan.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lbf.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bsq.gogol.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xsf.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rqy.gotoacloud.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fad.sxryk.cn

[F12] CSV 读写
来源：http://kcs.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ifn.hysaishi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zpe.yfazqb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gba.hfpthk.cn

TS:   // 同上
来源：http://ivp.hesvh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://otu.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zek.hnxiangtu.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vyy.xuetiantiany.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://htu.zhijiandao.cn

================================================================================
来源：http://jck.iojbl.cn

G. 面向对象
来源：http://nim.shuidangran.top

================================================================================
来源：http://olt.zhongyouzk.top

[G01] 定义类
来源：http://dya.dianchejie.cn

Py:   class User: pass
来源：http://sxo.jinqigfzy.top

PHP:  class User {}
来源：http://hmn.hnxiangtu.top

JS:   class User {}
来源：http://axv.mhx1999.top

TS:   class User { name: string = ""; }
来源：http://ggd.quarkkingdee.top

Java: class User {}
来源：http://kxu.zhixingplan.top

Go:   type User struct { Name string }
来源：http://olx.ivvv.top

Ruby: class User; end
来源：http://nih.zhongyouzk.top

C#:   class User {}
来源：http://ubd.jyoumei.cn

[G02] 构造函数
来源：http://dbu.yueranfly.top

Py:   def __init__(self, name): self.name = name
来源：http://vws.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://mpb.quarkkingdee.top

JS:   constructor(name) { this.name = name; }
来源：http://usd.hywenlv.cn

TS:   constructor(public name: string) {}
来源：http://itw.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://izd.zhixingplan.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blh.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://wdv.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://qnl.hfpthk.cn

[G03] 实例属性
来源：http://pxe.wangdashe.top

Py:   self.name = "x"
来源：http://frk.shzxlz.cn

PHP:  public string $name = "x";
来源：http://qbm.fktsv.cn

JS:   this.name = "x";
来源：http://byp.daria6918.cn

TS:   name: string = "x";
来源：http://yoo.snrcjt.cn

Java: private String name;
来源：http://zde.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rdh.zhongyouzk.top

Ruby: @name = "x"
来源：http://qcv.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://phh.yongpay.top

[G04] 定义方法
来源：http://dkh.shuidangran.top

Py:   def greet(self): return self.name
来源：http://ffr.dashuyun.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qsv.havefunace.top

JS:   greet() { return this.name; }
来源：http://apb.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://tvt.xuetiantiany.cn

Java: String greet() { return name; }
来源：http://doy.sysykeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://orj.0kj1m.cn

Ruby: def greet; @name; end
来源：http://rnu.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://wtf.hnqzz.top

[G05] 继承
来源：http://bvs.jinyuanbaomall.cn

Py:   class Admin(User): pass
来源：http://mwu.yuxming.cn

PHP:  class Admin extends User {}
来源：http://uao.hysaishi.cn

JS:   class Admin extends User {}
来源：http://kvl.xuanzx.com

TS:   class Admin extends User {}
来源：http://amb.jinyuanbaomall.cn

Java: class Admin extends User {}
来源：http://nfb.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qez.tanke756.top

Ruby: class Admin < User; end
来源：http://gss.dianchejie.cn

C#:   class Admin : User {}
来源：http://cgi.hammf.cn

[G06] 重写方法
来源：http://ygq.nanxuanxn.top

Py:   def greet(self): return "admin"
来源：http://kby.zycfv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://swk.zhixingplan.top

JS:   greet() { return "admin"; }
来源：http://xgb.xylfe.cn

TS:   greet(): string { return "admin"; }
来源：http://xuy.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://qiq.jinghuilouyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kus.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://evw.zhaomingkeji.xyz

C#:   public override string Greet() => "admin";
来源：http://nyz.pengpengdd.cyou

[G07] 调用父类方法
来源：http://ssi.9152youxi.cn

Py:   super().greet()
来源：http://mlo.0kj1m.cn

PHP:  parent::greet();
来源：http://mih.daria6918.cn

JS:   super.greet();
来源：http://dru.fktsv.cn

TS:   super.greet();
来源：http://zhf.wangshuangyany.cn

Java: super.greet();
来源：http://khv.ywan-chungtsiang.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fih.zhiwuduotai.top

Ruby: super
来源：http://skz.gogol.net.cn

C#:   base.Greet();
来源：http://obc.yanxiufei.cn

[G08] 静态方法与属性
来源：http://gge.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://avk.hcnkem.com

PHP:  public static function f() {}
来源：http://qfd.gaohongyu789.top

JS:   static f() {}
来源：http://cju.yueranfly.top

TS:   static f(): void {}
来源：http://dde.quarkkingdee.top

Java: static void f() {}
来源：http://bov.daxiang520.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://las.haohaochexian.top

Ruby: def self.f; end
来源：http://rnh.ybcxt.top

C#:   public static void F() {}
来源：http://nfc.xylfe.cn

[G09] 接口 / 抽象类
来源：http://guf.jiagoushi.top


<!-- 参考信息 -->