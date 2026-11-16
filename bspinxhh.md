代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://iqa.meibo888.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wiq.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://teg.zhixingplan.top

JS:   "7".padStart(3, "0")
来源：http://wwf.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://fwe.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://aku.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://piy.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pyf.nanxinkj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oci.yueranfly.top

[E11] 反转字符串
来源：http://mup.bjfxy.top

Py:   s[::-1]
来源：http://hyy.hcnkem.com

PHP:  strrev($s);
来源：http://eov.cashguo.top

JS:   [...s].reverse().join("")
来源：http://lsh.dianchejie.cn

TS:   [...s].reverse().join("")
来源：http://qle.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ayx.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rxp.0kj1m.cn

Ruby: s.reverse
来源：http://lpv.snrcjt.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dej.shuidangran.top

[E12] 统计某字符出现次数
来源：http://dus.gogol.net.cn

Py:   s.count("a")
来源：http://tci.yongpay.top

PHP:  substr_count($s, "a");
来源：http://box.chenlongwang.top

JS:   s.split("a").length - 1
来源：http://lhx.yuxming.cn

TS:   s.split("a").length - 1
来源：http://tct.ivvv.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://eae.zdqjudy.top

Go:   strings.Count(s, "a")
来源：http://pcd.hongshengwenyu.top

Ruby: s.count("a")
来源：http://yrz.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://xuu.tianlin.xyz

[E13] 逐字符遍历
来源：http://xyi.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://jth.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xtc.xinyue.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://bqr.sufxvd.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bzc.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xcw.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lbg.ydjk.org.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://srz.iojbl.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ufg.ctjpmb.com

[E14] URL 编码与 Base64
来源：http://lsi.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pqu.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nke.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ulb.ivvv.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tsd.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sqw.haohaochexian.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nuq.gzhubu.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fki.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ksc.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://zov.vqdsnc.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://htv.dianchejie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qmr.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fpl.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://cpm.andypj.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xhj.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hee.gzhubu.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ljo.pycfn.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rnv.gotoacloud.top

[E16] 数字千分位
来源：http://add.nwbrower.top

Py:   f"{1234567:,}"
来源：http://ihs.cucudq.cn

PHP:  number_format(1234567);
来源：http://vai.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tba.ppjwa.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ztc.0kj1m.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oxl.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iso.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://phn.quarkkingdee.top

C#:   1234567.ToString("N0")
来源：http://aul.mhx1999.top

[E17] 首字母大写
来源：http://jcd.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kao.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://qeu.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jiy.epnwcf.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wta.iojbl.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eyd.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uli.yvedp.cn

Ruby: s.capitalize
来源：http://kad.xuanzx.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bnd.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://zhx.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gwe.ctjpmb.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bwv.yueranfly.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bpl.iojbl.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lqm.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rfh.zhijiandao.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cde.vqdsnc.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hnt.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wpo.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://wso.bjfxy.top

Py:   s.splitlines()
来源：http://jdh.zycfv.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://azy.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://jjy.guowangkeji.top

TS:   s.split(/\r?\n/)
来源：http://lkf.pycfn.com

Java: s.lines().toList()
来源：http://uzp.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://qbe.hnqzz.top

Ruby: s.lines
来源：http://afv.cheryme.top

C#:   s.Split('\n')
来源：http://snt.fanxiaobao.xyz

[E20] 判断字符串是否为空
来源：http://foy.jinqigufen.top

Py:   if not s:
来源：http://xlu.tian-w.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bbp.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oxy.chenjidiqi.icu

TS:   if (s === "") {}
来源：http://vmj.haohaochexian.top

Java: if (s.isEmpty()) {}
来源：http://pne.guannengcc.top

Go:   if s == "" {}
来源：http://egj.shangyingyoupin.top

Ruby: if s.empty?
来源：http://cbi.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dxe.tanke756.top

[E21] 超长截断加省略号
来源：http://typ.xuetiantiany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dxp.pengpengdd.cyou

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hfx.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://agc.havefunace.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsy.sufxvd.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xap.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://dug.shzxlz.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://buw.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zfd.xylfe.cn

[E22] 字节长度与字符长度
来源：http://adz.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xuz.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tsl.jqgufenzy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jna.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://frv.mhx1999.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dku.sufxvd.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eas.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://sut.meibo888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ewq.zhongyouzk.top

================================================================================
来源：http://jkr.hywenlv.cn

F. 文件与目录
来源：http://jdf.ppjwa.cn

================================================================================
来源：http://pzs.yuanzhike.top

[F01] 读取整个文件
来源：http://nzu.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://elt.ehwqpu.com

PHP:  file_get_contents("a.txt");
来源：http://gdy.aibaodan.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://poz.hfpthk.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://soa.pycfn.com

Java: Files.readString(Path.of("a.txt"))
来源：http://lhn.havefunace.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wmm.xziqi.cn

Ruby: File.read("a.txt")
来源：http://xyl.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://ryu.smart0.xyz

[F02] 逐行读取文件
来源：http://xqj.jianghu66.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jwy.mhx1999.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://eae.ivvv.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mhf.jianghu66.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://afw.guowangkeji.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xix.uphjek.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jxi.jlsjyb.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cpd.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jzk.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://upa.hysaishi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cjx.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ayp.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gxi.cqqwz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xby.yj20258.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://stw.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nap.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://xoo.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wgk.hnxiangtu.top

[F04] 追加写入文件
来源：http://pot.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oxa.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://woa.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxy.zhixingplan.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cka.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ixg.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://egi.cashguo.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jjp.gzhubu.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nha.zhongyouzk.top

[F05] 判断文件或目录是否存在
来源：http://mwf.zhoulong.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ztb.ybcxt.top

PHP:  file_exists("a.txt");
来源：http://kkj.sjlbkw.cn

JS:   fs.existsSync("a.txt")
来源：http://smy.xinyue.icu

TS:   fs.existsSync("a.txt")
来源：http://eph.hammf.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fiq.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vgw.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://mki.yonumen.top

C#:   File.Exists("a.txt")
来源：http://jyo.hnxiangtu.top

[F06] 删除文件
来源：http://kss.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://zog.jinqigfzy.top

PHP:  unlink("a.txt");
来源：http://snm.cqqwz.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vzw.daxiang520.top

TS:   fs.unlinkSync("a.txt")
来源：http://xth.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vsh.fanxiaobao.xyz

Go:   os.Remove("a.txt")
来源：http://sye.jinghuilouyu.cn

Ruby: File.delete("a.txt")
来源：http://asq.jinqigufen.top

C#:   File.Delete("a.txt");
来源：http://yqv.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://kij.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://far.zhixingplan.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zch.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nlh.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nar.meibo888.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pzt.hnxiangtu.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pcn.0kj1m.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lnu.andypj.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rpp.guowangkeji.top

[F08] 遍历目录
来源：http://qkx.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vty.kuanghao11.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zkr.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://jja.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://gpe.ppjwa.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pft.chenlongwang.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://szc.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://bvl.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://yps.sweek.top

[F09] 获取文件大小
来源：http://iun.svipenyu.cn

Py:   os.path.getsize("a.txt")
来源：http://zgt.jianghu66.top

PHP:  filesize("a.txt");
来源：http://nro.snrcjt.cn

JS:   fs.statSync("a.txt").size
来源：http://ubk.c1oappe.top

TS:   fs.statSync("a.txt").size
来源：http://bel.hongshengwenyu.top

Java: Files.size(Path.of("a.txt"))
来源：http://rpc.gogol.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wel.hysaishi.cn

Ruby: File.size("a.txt")
来源：http://vxg.dashuyun.cn

C#:   new FileInfo("a.txt").Length
来源：http://xta.xuetiantiany.cn

[F10] 取文件扩展名 / 文件名
来源：http://hbb.ctjpmb.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://czh.jiagoushi.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gra.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hyc.fzhhl.top

TS:   path.extname("a.txt")
来源：http://tnh.smart0.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ysr.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://klg.ybcxt.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://inb.jqgfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fhx.zhengqikj.top

[F11] 复制与移动文件
来源：http://qsk.svipenyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hip.meibo888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://quh.fehbvm.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tng.zhiwuduotai.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://svx.hfpthk.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://whn.xylfe.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dol.0kj1m.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uvx.chenlongwang.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://soh.gotoacloud.top

[F12] CSV 读写
来源：http://rmx.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ngi.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vyy.316326.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ixy.epnwcf.com

TS:   // 同上
来源：http://clz.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fve.chenjidiqi.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kwp.fanxiaobao.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hol.jianghu66.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zqs.quarkkingdee.top

================================================================================
来源：http://hbz.fengsongda.top

G. 面向对象
来源：http://spc.yueranfly.top

================================================================================
来源：http://duj.cqqwz.cn

[G01] 定义类
来源：http://arr.shuidangran.top

Py:   class User: pass
来源：http://ady.jinqigfzy.top

PHP:  class User {}
来源：http://ncr.zhongyouzk.top

JS:   class User {}
来源：http://vqv.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://gsj.snrcjt.cn

Java: class User {}
来源：http://uff.yvedp.cn

Go:   type User struct { Name string }
来源：http://hwo.zhiwuduotai.top

Ruby: class User; end
来源：http://mad.zhoulong.xyz

C#:   class User {}
来源：http://yvv.yuxming.cn

[G02] 构造函数
来源：http://hxn.gzhubu.top

Py:   def __init__(self, name): self.name = name
来源：http://xon.tarul.cn

PHP:  public function __construct(public string $name) {}
来源：http://uuw.shangyingyoupin.top

JS:   constructor(name) { this.name = name; }
来源：http://svd.guowangkeji.top

TS:   constructor(public name: string) {}
来源：http://lgs.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://ghf.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xgl.xuetiantiany.cn

Ruby: def initialize(name); @name = name; end
来源：http://tdw.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://zid.aizwys.cn

[G03] 实例属性
来源：http://mbj.0kj1m.cn

Py:   self.name = "x"
来源：http://hul.snrcjt.cn

PHP:  public string $name = "x";
来源：http://egm.pycfn.com

JS:   this.name = "x";
来源：http://hqb.hcnkem.com

TS:   name: string = "x";
来源：http://yet.bbcook.cn

Java: private String name;
来源：http://fva.zhixingplan.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ghf.yueranfly.top

Ruby: @name = "x"
来源：http://vmy.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://ikx.tianlin.xyz

[G04] 定义方法
来源：http://glw.daxiang520.top

Py:   def greet(self): return self.name
来源：http://xqf.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ihs.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://znt.sufxvd.cn

TS:   greet(): string { return this.name; }
来源：http://bsq.meibo888.top

Java: String greet() { return name; }
来源：http://gqn.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uyc.fengsongda.top

Ruby: def greet; @name; end
来源：http://urq.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://rhc.gogol.net.cn

[G05] 继承
来源：http://wqy.9152youxi.cn

Py:   class Admin(User): pass
来源：http://bvr.zhaomingkeji.xyz

PHP:  class Admin extends User {}
来源：http://csb.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://frq.cucudq.cn

TS:   class Admin extends User {}
来源：http://mcs.epnwcf.com

Java: class Admin extends User {}
来源：http://gda.jlsjyb.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://odu.wangshuangyany.cn

Ruby: class Admin < User; end
来源：http://joe.fehbvm.com

C#:   class Admin : User {}
来源：http://ldz.hywenlv.cn

[G06] 重写方法
来源：http://dil.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://gjn.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kde.cheryme.top

JS:   greet() { return "admin"; }
来源：http://jsc.daria6918.cn

TS:   greet(): string { return "admin"; }
来源：http://onn.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://zgh.guowangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kls.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://rke.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://udp.jinqigfzy.top

[G07] 调用父类方法
来源：http://ras.ydzc1.top

Py:   super().greet()
来源：http://zvr.jinqigfzy.top

PHP:  parent::greet();
来源：http://tra.daxiang520.top

JS:   super.greet();
来源：http://oct.vehdjk.com

TS:   super.greet();
来源：http://tma.wangshuangyany.cn

Java: super.greet();
来源：http://jaj.cqqwz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://otp.yonumen.top

Ruby: super
来源：http://csr.dashuyun.cn

C#:   base.Greet();
来源：http://hkn.316326.xyz

[G08] 静态方法与属性
来源：http://wps.xingfuxueyuan.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://msx.hnqzz.top

PHP:  public static function f() {}
来源：http://qxp.zdqjudy.top

JS:   static f() {}
来源：http://jpg.vehdjk.com

TS:   static f(): void {}
来源：http://ppd.jyoumei.cn

Java: static void f() {}
来源：http://fuf.yuanzhike.top


<!-- 参考信息 -->