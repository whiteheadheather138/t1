代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://brd.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yle.sysykeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://myk.hywenlv.cn

JS:   "7".padStart(3, "0")
来源：http://wsa.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://wgw.xingfuxueyuan.xyz

Java: String.format("%03d", 7)
来源：http://iej.wangdashe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://czv.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yxy.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hxn.mhx1999.top

[E11] 反转字符串
来源：http://psj.ctjpmb.com

Py:   s[::-1]
来源：http://yms.jyoumei.cn

PHP:  strrev($s);
来源：http://ljc.meibo888.top

JS:   [...s].reverse().join("")
来源：http://vbs.tanke756.top

TS:   [...s].reverse().join("")
来源：http://xcu.tian-w.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sjz.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hkc.gotoacloud.top

Ruby: s.reverse
来源：http://mak.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nlc.smart0.xyz

[E12] 统计某字符出现次数
来源：http://hjl.xuanzx.com

Py:   s.count("a")
来源：http://llq.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://grd.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://tnl.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://wly.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qjr.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://fbf.uphjek.com

Ruby: s.count("a")
来源：http://fig.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://icm.sufxvd.cn

[E13] 逐字符遍历
来源：http://cvs.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://uje.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://edr.xylfe.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rxd.quarkkingdee.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://gvv.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fbh.52xcode.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xur.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lyu.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xvu.zhongyouzk.top

[E14] URL 编码与 Base64
来源：http://kgn.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wez.sxryk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rfj.uphjek.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bgs.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kmx.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lzi.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wgf.fktsv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jdo.tianlin.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hjt.andypj.xyz

[E15] HTML 转义 / 反转义
来源：http://xvx.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gfi.0kj1m.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qzl.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hwx.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rym.iojbl.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cmu.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mun.nanxinkj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ijv.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sjt.c1oappe.top

[E16] 数字千分位
来源：http://yhb.shanyushiyangkeji.top

Py:   f"{1234567:,}"
来源：http://kix.andypj.xyz

PHP:  number_format(1234567);
来源：http://rzv.jiagoushi.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eav.hnxiangtu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bhy.meibo888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vpm.havefunace.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wdq.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jhv.yangfankeji.com

C#:   1234567.ToString("N0")
来源：http://gtj.jlsjyb.cn

[E17] 首字母大写
来源：http://uof.quarkkingdee.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qpz.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://bre.xingfuxueyuan.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xly.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qxi.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ods.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://enf.ehwqpu.com

Ruby: s.capitalize
来源：http://uuy.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wuu.yanxiufei.cn

[E18] 模板占位符替换
来源：http://yww.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oom.nanxinkj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://etd.feifeiyinyue.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pul.ybcxt.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dvh.gaohongyu789.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gke.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qvw.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://atf.shanyushiyangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nkl.sweek.top

[E19] 多行文本按行拆分
来源：http://tfq.gaohongyu789.top

Py:   s.splitlines()
来源：http://bbx.nanxinkj.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://isk.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://vtn.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://fid.xylfe.cn

Java: s.lines().toList()
来源：http://uot.hysaishi.cn

Go:   strings.Split(s, "\n")
来源：http://izu.sjlbkw.cn

Ruby: s.lines
来源：http://dsg.shanyushiyangkeji.top

C#:   s.Split('\n')
来源：http://gfz.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://sxw.xuanzx.com

Py:   if not s:
来源：http://fqf.fengsongda.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://utu.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wou.quarkkingdee.top

TS:   if (s === "") {}
来源：http://zyx.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://qpl.yj20258888.top

Go:   if s == "" {}
来源：http://emo.nwbrower.top

Ruby: if s.empty?
来源：http://vzq.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wlf.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://ooy.kuanghao11.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nak.tianlin.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xvj.hammf.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ntu.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zbm.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fdw.sweek.top

Go:   // 按 rune 判断长度后截断
来源：http://zlt.yfazqb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jcw.zhixingplan.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yxh.52xcode.cn

[E22] 字节长度与字符长度
来源：http://onh.tianlin.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xta.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wwn.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qbg.ydjk.org.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ttz.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kqg.gzhubu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nuq.xylfe.cn

Ruby: s.bytesize;  s.length
来源：http://wmt.vehdjk.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fdq.kuanghao11.cn

================================================================================
来源：http://wih.quarkkingdee.top

F. 文件与目录
来源：http://suh.ppjwa.cn

================================================================================
来源：http://ktk.guowangkeji.top

[F01] 读取整个文件
来源：http://rvz.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tii.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://qmb.kuanghao11.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tza.yfazqb.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sts.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://azj.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mvx.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://rfq.shuidangran.top

C#:   File.ReadAllText("a.txt");
来源：http://nry.yongpay.top

[F02] 逐行读取文件
来源：http://kiz.cashguo.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://egg.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bpn.meibo888.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kqd.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://row.jiagoushi.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xgu.ivvv.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jjw.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xfd.xuanzx.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://otz.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://lfz.xziqi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pug.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://fmy.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eez.gaohongyu789.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://alo.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://htv.xuanzx.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ewo.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://ixj.snrcjt.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ohw.vqdsnc.cn

[F04] 追加写入文件
来源：http://pvn.ehwqpu.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dis.cdnleiting.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hlr.yueranfly.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fze.vqdsnc.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qad.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hti.fehbvm.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kon.cdnleiting.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ohg.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aek.zhengqikj.top

[F05] 判断文件或目录是否存在
来源：http://jlh.9152youxi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zel.jiagoushi.top

PHP:  file_exists("a.txt");
来源：http://qrc.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://lji.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://owr.chenzaomai.com

Java: Files.exists(Path.of("a.txt"))
来源：http://agu.jinghuilouyu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pru.hfpthk.cn

Ruby: File.exist?("a.txt")
来源：http://pav.shangyingyoupin.top

C#:   File.Exists("a.txt")
来源：http://ifu.0kj1m.cn

[F06] 删除文件
来源：http://plf.hnqzz.top

Py:   os.remove("a.txt")
来源：http://boy.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://ynt.andypj.xyz

JS:   fs.unlinkSync("a.txt")
来源：http://zwy.fanxiaobao.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://lph.dianchejie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jlt.yueranfly.top

Go:   os.Remove("a.txt")
来源：http://wvp.havefunace.top

Ruby: File.delete("a.txt")
来源：http://vlq.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://lsf.chenlongwang.top

[F07] 创建目录（含多级）
来源：http://pny.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dfv.tianlin.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wlu.bbcook.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yao.daxiang520.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xgi.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ycw.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aen.feifeiyinyue.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rnz.yangfankeji.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qty.yuxming.cn

[F08] 遍历目录
来源：http://ujs.dianchejie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://syg.iojbl.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ezd.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://hpp.hysaishi.cn

TS:   fs.readdirSync("dir")
来源：http://vpu.ybcxt.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vcj.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nch.birdmap.top

Ruby: Dir.children("dir")
来源：http://vsp.gogol.net.cn

C#:   Directory.GetFiles("dir")
来源：http://yna.sysykeji.top

[F09] 获取文件大小
来源：http://caa.gaohongyu789.top

Py:   os.path.getsize("a.txt")
来源：http://tsz.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://kbr.hfpthk.cn

JS:   fs.statSync("a.txt").size
来源：http://oqf.ybcxt.top

TS:   fs.statSync("a.txt").size
来源：http://ltu.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://fau.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uma.guannengcc.top

Ruby: File.size("a.txt")
来源：http://jyr.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://fge.shuidangran.top

[F10] 取文件扩展名 / 文件名
来源：http://nru.mhx1999.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://miw.ybcxt.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://owl.chenzaomai.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nhz.zycfv.cn

TS:   path.extname("a.txt")
来源：http://ghx.shuidangran.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yoa.daxiang520.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hqj.shuidangran.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ptm.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ejf.zhiwuduotai.top

[F11] 复制与移动文件
来源：http://wwk.pycfn.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wqm.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xto.yvedp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ysn.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://njr.vqdsnc.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lnu.sufxvd.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qiw.aizwys.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eou.birdmap.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rmg.vqdsnc.cn

[F12] CSV 读写
来源：http://pfh.tianlin.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ovj.shzxlz.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sme.daxiang520.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://irn.pengpengdd.cyou

TS:   // 同上
来源：http://msu.fehbvm.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qdk.pycfn.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tpb.fehbvm.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tep.fengsongda.top

C#:   // 无内置：用 CsvHelper 库
来源：http://dxk.yonumen.top

================================================================================
来源：http://xom.aizwys.cn

G. 面向对象
来源：http://rnl.hfpthk.cn

================================================================================
来源：http://gqj.daxiang520.top

[G01] 定义类
来源：http://gkt.jinyuanbaomall.cn

Py:   class User: pass
来源：http://juj.sysykeji.top

PHP:  class User {}
来源：http://gsa.xziqi.cn

JS:   class User {}
来源：http://rec.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://bcj.ybcxt.top

Java: class User {}
来源：http://sip.yvedp.cn

Go:   type User struct { Name string }
来源：http://kag.feifeiyinyue.top

Ruby: class User; end
来源：http://oji.gaohongyu789.top

C#:   class User {}
来源：http://yfh.tarul.cn

[G02] 构造函数
来源：http://zlr.ppjwa.cn

Py:   def __init__(self, name): self.name = name
来源：http://ewt.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://jvs.shuidangran.top

JS:   constructor(name) { this.name = name; }
来源：http://wgh.aizwys.cn

TS:   constructor(public name: string) {}
来源：http://wew.jiagoushi.top

Java: User(String name) { this.name = name; }
来源：http://sfc.hammf.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rss.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://vtz.bjfxy.top

C#:   public User(string name) { Name = name; }
来源：http://hyn.cucudq.cn

[G03] 实例属性
来源：http://tib.daxiang520.top

Py:   self.name = "x"
来源：http://hzd.mhx1999.top

PHP:  public string $name = "x";
来源：http://zxb.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://pax.jlsjyb.cn

TS:   name: string = "x";
来源：http://bwo.redwolf501.top

Java: private String name;
来源：http://vay.wangshuangyany.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xhl.sxryk.cn

Ruby: @name = "x"
来源：http://han.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://iuj.kuanghao11.cn

[G04] 定义方法
来源：http://btv.fehbvm.com

Py:   def greet(self): return self.name
来源：http://eok.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://rkw.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://ykq.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://urg.yj202588.top

Java: String greet() { return name; }
来源：http://gkp.zhiwuduotai.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gvf.xingfuxueyuan.xyz

Ruby: def greet; @name; end
来源：http://mcv.fengsongda.top

C#:   public string Greet() => Name;
来源：http://yvk.hywenlv.cn

[G05] 继承
来源：http://fxm.snrcjt.cn

Py:   class Admin(User): pass
来源：http://qpe.yangfankeji.com

PHP:  class Admin extends User {}
来源：http://oyj.xuetiantiany.cn

JS:   class Admin extends User {}
来源：http://ekf.nanxinkj.top

TS:   class Admin extends User {}
来源：http://pdt.cqqwz.cn

Java: class Admin extends User {}
来源：http://uvp.snrcjt.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hfy.cdnleiting.top

Ruby: class Admin < User; end
来源：http://btv.cucudq.cn

C#:   class Admin : User {}
来源：http://eqn.zhaomingkeji.xyz

[G06] 重写方法
来源：http://rzi.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://jgg.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://nwl.wangdashe.top

JS:   greet() { return "admin"; }
来源：http://pxc.ydzc1.top

TS:   greet(): string { return "admin"; }
来源：http://pnf.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://ncd.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cxr.shanyushiyangkeji.top

Ruby: def greet; "admin"; end
来源：http://crh.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://sii.chenlongwang.top

[G07] 调用父类方法
来源：http://kxi.shanyushiyangtech.top

Py:   super().greet()
来源：http://pqx.pycfn.com

PHP:  parent::greet();
来源：http://zeh.c1oappe.top

JS:   super.greet();
来源：http://khg.chenjidiqi.icu

TS:   super.greet();
来源：http://wfk.jlsjyb.cn

Java: super.greet();
来源：http://hcx.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uyv.gogol.net.cn

Ruby: super
来源：http://kbu.jinghuilouyu.cn

C#:   base.Greet();
来源：http://aym.svipenyu.cn

[G08] 静态方法与属性
来源：http://ojf.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qmb.kuanghao11.cn

PHP:  public static function f() {}
来源：http://xko.jianghu66.top

JS:   static f() {}
来源：http://hfn.hongshengwenyu.top

TS:   static f(): void {}
来源：http://epu.guowangkeji.top

Java: static void f() {}
来源：http://zmr.xuetiantiany.cn


<!-- 参考信息 -->