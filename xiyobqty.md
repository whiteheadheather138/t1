代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://xte.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jpu.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ffy.iojbl.cn

JS:   "7".padStart(3, "0")
来源：http://rtb.gotoacloud.top

TS:   "7".padStart(3, "0")
来源：http://bvh.fehbvm.com

Java: String.format("%03d", 7)
来源：http://hmw.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iwh.52xcode.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fvb.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kvr.hnqzz.top

[E11] 反转字符串
来源：http://voo.gotoacloud.top

Py:   s[::-1]
来源：http://bfp.sufxvd.cn

PHP:  strrev($s);
来源：http://set.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://kja.haohaochexian.top

TS:   [...s].reverse().join("")
来源：http://fhe.hfpthk.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kpw.fzhhl.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eyf.cqqwz.cn

Ruby: s.reverse
来源：http://pbj.hammf.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sjr.cucudq.cn

[E12] 统计某字符出现次数
来源：http://atd.xuetiantiany.cn

Py:   s.count("a")
来源：http://maz.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://kcd.cucudq.cn

JS:   s.split("a").length - 1
来源：http://jnb.pycfn.com

TS:   s.split("a").length - 1
来源：http://hvm.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ava.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://qoc.jlsjyb.cn

Ruby: s.count("a")
来源：http://fnp.yfazqb.com

C#:   s.Count(c => c == 'a')
来源：http://ymk.tanke756.top

[E13] 逐字符遍历
来源：http://xoh.shanyushiyangtech.top

Py:   for ch in s: print(ch)
来源：http://bqf.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ltl.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gkf.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://jvn.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pxr.gogol.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cgx.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rbw.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tbz.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://zwm.jianghu66.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kmb.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://znu.fzhhl.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kcc.fzhhl.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qqa.sweek.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xvf.yuanzhike.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bfc.feifeiyinyue.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bli.hnqzz.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://omt.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://doq.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nml.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qyk.gogol.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ueq.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://qwt.epnwcf.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vjv.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://utm.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fxg.daria6918.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jci.gzhubu.top

[E16] 数字千分位
来源：http://kir.fehbvm.com

Py:   f"{1234567:,}"
来源：http://aza.zhoulong.xyz

PHP:  number_format(1234567);
来源：http://xic.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ntk.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://yth.xuanzx.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fyo.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://utu.hywenlv.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ktk.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://hny.zycfv.cn

[E17] 首字母大写
来源：http://rhp.tanke756.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xhu.cdnleiting.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fhs.ydjk.org.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pii.redwolf501.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vka.jqgfzy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wns.yongpay.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jqq.shzxlz.cn

Ruby: s.capitalize
来源：http://vds.bbcook.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zpn.zhijiandao.cn

[E18] 模板占位符替换
来源：http://fya.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pir.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://frp.ppjwa.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zvu.zdqjudy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ebt.zdbjq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lsz.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gdw.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://akc.yj20258.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qun.uphjek.com

[E19] 多行文本按行拆分
来源：http://dwd.gzhubu.top

Py:   s.splitlines()
来源：http://vzk.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hpm.shanyushiyangtech.top

JS:   s.split(/\r?\n/)
来源：http://hgz.tarul.cn

TS:   s.split(/\r?\n/)
来源：http://gbi.uphjek.com

Java: s.lines().toList()
来源：http://pom.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://qhk.bbcook.cn

Ruby: s.lines
来源：http://xgw.kuanghao11.cn

C#:   s.Split('\n')
来源：http://aeb.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://bbm.feifeiyinyue.top

Py:   if not s:
来源：http://nlg.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://txp.yueranfly.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bwo.pycfn.com

TS:   if (s === "") {}
来源：http://ntq.gotoacloud.top

Java: if (s.isEmpty()) {}
来源：http://izk.yanxiufei.cn

Go:   if s == "" {}
来源：http://miz.smart0.xyz

Ruby: if s.empty?
来源：http://yaa.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cpl.hnqzz.top

[E21] 超长截断加省略号
来源：http://jui.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nws.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jkr.hesvh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mvc.zhijiandao.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uyr.fzhhl.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ohm.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://adp.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nhx.bbcook.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vrl.shuidangran.top

[E22] 字节长度与字符长度
来源：http://opq.cdnleiting.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pqv.sjlbkw.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jcn.ydzc1.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vkj.jqgfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://unp.zhaomingkeji.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ujt.snrcjt.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wep.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://muk.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dew.sxryk.cn

================================================================================
来源：http://rpg.yanxiufei.cn

F. 文件与目录
来源：http://mrs.epnwcf.com

================================================================================
来源：http://hux.zhiwuduotai.top

[F01] 读取整个文件
来源：http://imy.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ggo.kuanghao11.cn

PHP:  file_get_contents("a.txt");
来源：http://pov.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lko.c1oappe.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://drc.ctjpmb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://hgd.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://biz.quarkkingdee.top

Ruby: File.read("a.txt")
来源：http://lir.cashguo.top

C#:   File.ReadAllText("a.txt");
来源：http://rix.shzxlz.cn

[F02] 逐行读取文件
来源：http://pwc.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lup.xziqi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zol.aibaodan.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzu.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://npi.0kj1m.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vka.guannengcc.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://spq.52xcode.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mma.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hye.dianchejie.cn

[F03] 写入文件（覆盖）
来源：http://jfv.jinghuilouyu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://aip.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://orp.xylfe.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://glf.jlsjyb.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kez.dashuyun.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://amn.cheryme.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://osx.chenzaomai.com

Ruby: File.write("a.txt", "hi")
来源：http://ajp.smart0.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://heh.mhx1999.top

[F04] 追加写入文件
来源：http://ogq.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qwb.cheryme.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ogi.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lzx.meibo888.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zyh.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hoe.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dwh.snrcjt.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://npf.tian-w.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://omj.zhoulong.xyz

[F05] 判断文件或目录是否存在
来源：http://cxi.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rka.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://dcs.gotoacloud.top

JS:   fs.existsSync("a.txt")
来源：http://xyi.xuetiantiany.cn

TS:   fs.existsSync("a.txt")
来源：http://isk.shanyushiyangkeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qjf.ydzc1.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qrx.yueranfly.top

Ruby: File.exist?("a.txt")
来源：http://pul.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://fma.snrcjt.cn

[F06] 删除文件
来源：http://emf.yj20258.top

Py:   os.remove("a.txt")
来源：http://lbj.jinyuanbaomall.cn

PHP:  unlink("a.txt");
来源：http://jfp.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xap.gzhubu.top

TS:   fs.unlinkSync("a.txt")
来源：http://wrw.fzhhl.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uew.shuidangran.top

Go:   os.Remove("a.txt")
来源：http://zns.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://avz.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://nfu.jiagoushi.top

[F07] 创建目录（含多级）
来源：http://ogh.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zox.ywan-chungtsiang.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uaw.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://btj.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ldx.bbcook.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kek.iojbl.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vxl.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aze.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hvh.mhx1999.top

[F08] 遍历目录
来源：http://wuj.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://czi.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kxb.ppjwa.cn

JS:   fs.readdirSync("dir")
来源：http://bgb.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://uvk.hcnkem.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pko.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jnd.shangyingyoupin.top

Ruby: Dir.children("dir")
来源：http://wjp.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://ynq.sjlbkw.cn

[F09] 获取文件大小
来源：http://cfu.yuanzhike.top

Py:   os.path.getsize("a.txt")
来源：http://dbi.gogol.net.cn

PHP:  filesize("a.txt");
来源：http://iyb.ehwqpu.com

JS:   fs.statSync("a.txt").size
来源：http://kfb.ydjk.org.cn

TS:   fs.statSync("a.txt").size
来源：http://etb.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bvn.fengsongda.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hsh.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://htd.fktsv.cn

C#:   new FileInfo("a.txt").Length
来源：http://xdg.pycfn.com

[F10] 取文件扩展名 / 文件名
来源：http://vsg.ehwqpu.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dsh.zhongyouzk.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://per.hywenlv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cfq.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://vxt.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qhj.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gny.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wbw.shzxlz.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zeo.tian-w.cn

[F11] 复制与移动文件
来源：http://yad.jinqigfzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fvk.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rgs.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ufq.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uvq.sxryk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xja.cashguo.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kqx.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lxz.sufxvd.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mpj.jinqigfzy.top

[F12] CSV 读写
来源：http://iym.vqdsnc.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blt.aibaodan.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vvs.jqgufenzy.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ccp.jinqigfzy.top

TS:   // 同上
来源：http://uqz.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kqb.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gno.fktsv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yrc.jlsjyb.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hdk.shanyushiyangkeji.top

================================================================================
来源：http://nvh.zhiwuduotai.top

G. 面向对象
来源：http://cce.hnxiangtu.top

================================================================================
来源：http://kdc.yonumen.top

[G01] 定义类
来源：http://ltp.xuetiantiany.cn

Py:   class User: pass
来源：http://acg.yj20258.top

PHP:  class User {}
来源：http://yif.hesvh.cn

JS:   class User {}
来源：http://hto.daria6918.cn

TS:   class User { name: string = ""; }
来源：http://hxe.yonumen.top

Java: class User {}
来源：http://fys.fktsv.cn

Go:   type User struct { Name string }
来源：http://jgw.nanxuanxn.top

Ruby: class User; end
来源：http://jum.dianchejie.cn

C#:   class User {}
来源：http://igx.yuxming.cn

[G02] 构造函数
来源：http://ony.yongpay.top

Py:   def __init__(self, name): self.name = name
来源：http://dxo.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://rmt.vqdsnc.cn

JS:   constructor(name) { this.name = name; }
来源：http://yxt.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://wbp.zdbjq.cn

Java: User(String name) { this.name = name; }
来源：http://fuv.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gza.tian-w.cn

Ruby: def initialize(name); @name = name; end
来源：http://rfv.yvedp.cn

C#:   public User(string name) { Name = name; }
来源：http://mll.kuanghao11.cn

[G03] 实例属性
来源：http://chv.bjfxy.top

Py:   self.name = "x"
来源：http://kdt.shanyushiyangtech.top

PHP:  public string $name = "x";
来源：http://cxv.yfazqb.com

JS:   this.name = "x";
来源：http://ihz.daxiang520.top

TS:   name: string = "x";
来源：http://lna.xingfuxueyuan.xyz

Java: private String name;
来源：http://tmx.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jpj.chenjidiqi.icu

Ruby: @name = "x"
来源：http://rqy.cdnleiting.top

C#:   public string Name { get; set; } = "x";
来源：http://hxe.chenlongwang.top

[G04] 定义方法
来源：http://cpw.jianghu66.top

Py:   def greet(self): return self.name
来源：http://myj.ybcxt.top

PHP:  public function greet(): string { return $this->name; }
来源：http://khv.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://qzv.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://vwj.xylfe.cn

Java: String greet() { return name; }
来源：http://yoj.chenzaomai.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://ivj.zhaomingkeji.xyz

Ruby: def greet; @name; end
来源：http://zbo.yfazqb.com

C#:   public string Greet() => Name;
来源：http://zny.guowangkeji.top

[G05] 继承
来源：http://kte.fzhhl.top

Py:   class Admin(User): pass
来源：http://pfe.yvedp.cn

PHP:  class Admin extends User {}
来源：http://gjl.haohaochexian.top

JS:   class Admin extends User {}
来源：http://uzr.daria6918.cn

TS:   class Admin extends User {}
来源：http://aox.bbcook.cn

Java: class Admin extends User {}
来源：http://hrb.daxiang520.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sdy.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://apx.xuanzx.com

C#:   class Admin : User {}
来源：http://lks.feifeiyinyue.top

[G06] 重写方法
来源：http://fjv.hesvh.cn

Py:   def greet(self): return "admin"
来源：http://oql.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hff.zhijiandao.cn

JS:   greet() { return "admin"; }
来源：http://oeo.fanxiaobao.xyz

TS:   greet(): string { return "admin"; }
来源：http://kot.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://ppr.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zqu.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://tax.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://wtn.316326.xyz

[G07] 调用父类方法
来源：http://rwl.hysaishi.cn

Py:   super().greet()
来源：http://vum.jqgfzy.top

PHP:  parent::greet();
来源：http://lka.haohaochexian.top

JS:   super.greet();
来源：http://rcl.daria6918.cn

TS:   super.greet();
来源：http://zmv.xuanzx.com

Java: super.greet();
来源：http://ntn.vqdsnc.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cua.epnwcf.com

Ruby: super
来源：http://plr.ybcxt.top

C#:   base.Greet();
来源：http://tsl.nanxuanxn.top

[G08] 静态方法与属性
来源：http://xsk.tian-w.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xll.daria6918.cn

PHP:  public static function f() {}
来源：http://iha.yuanzhike.top

JS:   static f() {}
来源：http://lby.cqqwz.cn

TS:   static f(): void {}
来源：http://dub.zhoulong.xyz

Java: static void f() {}
来源：http://wuk.aibaodan.cn


<!-- 参考信息 -->