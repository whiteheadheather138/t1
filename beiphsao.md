代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://nnb.fanxiaobao.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lxf.daxiang520.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xbs.aizwys.cn

JS:   "7".padStart(3, "0")
来源：http://ghu.nwbrower.top

TS:   "7".padStart(3, "0")
来源：http://bjt.xziqi.cn

Java: String.format("%03d", 7)
来源：http://kud.fengsongda.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xso.fanxiaobao.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://amc.yonumen.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lhn.wangshuangyany.cn

[E11] 反转字符串
来源：http://vgb.jinqigufen.top

Py:   s[::-1]
来源：http://evf.uphjek.com

PHP:  strrev($s);
来源：http://xkk.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://yul.xinyue.icu

TS:   [...s].reverse().join("")
来源：http://lqo.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://gwt.snrcjt.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://knf.fengsongda.top

Ruby: s.reverse
来源：http://dex.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://ghr.xingfuxueyuan.xyz

[E12] 统计某字符出现次数
来源：http://wve.uphjek.com

Py:   s.count("a")
来源：http://xnb.chenzaomai.com

PHP:  substr_count($s, "a");
来源：http://xyo.zdqjudy.top

JS:   s.split("a").length - 1
来源：http://yas.gzhubu.top

TS:   s.split("a").length - 1
来源：http://cdr.yangfankeji.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ahu.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://jxk.guowangkeji.top

Ruby: s.count("a")
来源：http://rir.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://pkp.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://gzp.yj20258.top

Py:   for ch in s: print(ch)
来源：http://kac.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://srs.cashguo.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://arn.vqdsnc.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uot.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aoy.zhongyouzk.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lzv.xuetiantiany.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xqo.jianghu66.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zzu.yvedp.cn

[E14] URL 编码与 Base64
来源：http://fir.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hgr.hnxiangtu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kwd.bjfxy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qwi.epnwcf.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zga.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uvr.vqdsnc.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://anf.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wkh.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://obc.zhijiandao.cn

[E15] HTML 转义 / 反转义
来源：http://tio.zhongyouzk.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wft.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mgj.jianghu66.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tlj.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://cmb.9152youxi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ypu.cucudq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hgk.kuanghao11.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wfq.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ugm.jlsjyb.cn

[E16] 数字千分位
来源：http://mnm.hesvh.cn

Py:   f"{1234567:,}"
来源：http://syj.xylfe.cn

PHP:  number_format(1234567);
来源：http://egj.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zjb.zdbjq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://uoj.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tyf.feifeiyinyue.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ink.pengpengdd.cyou

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ucq.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://gfs.wangdashe.top

[E17] 首字母大写
来源：http://guj.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://opj.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://xij.jyoumei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://grj.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bus.gzhubu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iwq.zhixingplan.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://iul.52xcode.cn

Ruby: s.capitalize
来源：http://gii.shzxlz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qvd.fehbvm.com

[E18] 模板占位符替换
来源：http://cua.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dvh.ehwqpu.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jgb.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wma.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dkv.yangfankeji.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sfe.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hgb.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cqb.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fah.yongpay.top

[E19] 多行文本按行拆分
来源：http://cqi.ywan-chungtsiang.top

Py:   s.splitlines()
来源：http://zvh.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://diw.fengsongda.top

JS:   s.split(/\r?\n/)
来源：http://cer.haohaochexian.top

TS:   s.split(/\r?\n/)
来源：http://euu.jinqigfzy.top

Java: s.lines().toList()
来源：http://tai.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://tup.nwbrower.top

Ruby: s.lines
来源：http://joa.ctjpmb.com

C#:   s.Split('\n')
来源：http://etp.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://lde.meibo888.top

Py:   if not s:
来源：http://wnu.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vce.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://iiy.9152youxi.cn

TS:   if (s === "") {}
来源：http://jon.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://mmy.guannengcc.top

Go:   if s == "" {}
来源：http://dkq.dianchejie.cn

Ruby: if s.empty?
来源：http://ene.smart0.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dah.jyoumei.cn

[E21] 超长截断加省略号
来源：http://bji.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://byx.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dpc.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jok.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ppl.tanke756.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hqe.zhixingplan.top

Go:   // 按 rune 判断长度后截断
来源：http://wsj.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zuo.xylfe.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ixg.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://hfz.ehwqpu.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://drx.yongpay.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nxd.mhx1999.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kqy.aizwys.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xse.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vzd.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ylf.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://upk.hongshengwenyu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ogi.ydzc1.top

================================================================================
来源：http://mkb.zhaomingkeji.xyz

F. 文件与目录
来源：http://dob.meibo888.top

================================================================================
来源：http://gko.hfpthk.cn

[F01] 读取整个文件
来源：http://zza.redwolf501.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://shx.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://aom.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ced.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pzx.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yfy.vehdjk.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qeo.hnxiangtu.top

Ruby: File.read("a.txt")
来源：http://mgf.gotoacloud.top

C#:   File.ReadAllText("a.txt");
来源：http://wbw.hywenlv.cn

[F02] 逐行读取文件
来源：http://vol.zycfv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xtb.jinyuanbaomall.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://obq.jinqigufen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pcu.cashguo.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ufx.aizwys.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xjh.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tcy.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://swz.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jwq.cheryme.top

[F03] 写入文件（覆盖）
来源：http://ftd.tarul.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://usy.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rll.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://byu.hnxiangtu.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qgo.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sap.chenjidiqi.icu

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xoa.cqqwz.cn

Ruby: File.write("a.txt", "hi")
来源：http://dhj.zhongyouzk.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tey.meibo888.top

[F04] 追加写入文件
来源：http://inh.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hkd.sysykeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ukn.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eef.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ieu.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hdv.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://soc.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://otv.yonumen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vrc.chenlongwang.top

[F05] 判断文件或目录是否存在
来源：http://qrf.yvedp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uwa.0kj1m.cn

PHP:  file_exists("a.txt");
来源：http://wjb.cdnleiting.top

JS:   fs.existsSync("a.txt")
来源：http://fos.c1oappe.top

TS:   fs.existsSync("a.txt")
来源：http://aah.hysaishi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xli.ybcxt.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qil.svipenyu.cn

Ruby: File.exist?("a.txt")
来源：http://rdk.zhoulong.xyz

C#:   File.Exists("a.txt")
来源：http://zpq.nwbrower.top

[F06] 删除文件
来源：http://qpa.sysykeji.top

Py:   os.remove("a.txt")
来源：http://ldq.jiagoushi.top

PHP:  unlink("a.txt");
来源：http://fwp.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yba.haohaochexian.top

TS:   fs.unlinkSync("a.txt")
来源：http://klj.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://prd.jinyuanbaomall.cn

Go:   os.Remove("a.txt")
来源：http://qws.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://fev.feifeiyinyue.top

C#:   File.Delete("a.txt");
来源：http://xdd.svipenyu.cn

[F07] 创建目录（含多级）
来源：http://wad.wangdashe.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nzt.cucudq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pzo.hysaishi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xsd.mhx1999.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://foc.xylfe.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cdb.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xub.jqgufenzy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://leh.tanke756.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xkf.yangfankeji.com

[F08] 遍历目录
来源：http://apj.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://txo.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jah.hesvh.cn

JS:   fs.readdirSync("dir")
来源：http://mug.iojbl.cn

TS:   fs.readdirSync("dir")
来源：http://nxr.sweek.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zkg.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://lpw.ybcxt.top

Ruby: Dir.children("dir")
来源：http://crq.jqgufenzy.top

C#:   Directory.GetFiles("dir")
来源：http://jmz.jqgufenzy.top

[F09] 获取文件大小
来源：http://xzq.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://taq.9152youxi.cn

PHP:  filesize("a.txt");
来源：http://cxp.nanxuanxn.top

JS:   fs.statSync("a.txt").size
来源：http://gia.aibaodan.cn

TS:   fs.statSync("a.txt").size
来源：http://iec.sjlbkw.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dsk.hywenlv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qwq.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://wql.vehdjk.com

C#:   new FileInfo("a.txt").Length
来源：http://eqz.wangshuangyany.cn

[F10] 取文件扩展名 / 文件名
来源：http://dtv.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://daw.meibo888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hzx.epnwcf.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yig.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://sxf.jlsjyb.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://znn.ppjwa.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zxh.chenjidiqi.icu

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vmz.zhixingplan.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://czi.daxiang520.top

[F11] 复制与移动文件
来源：http://orv.jiagoushi.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tvy.yuanzhike.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mjy.nanxuanxn.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aue.nanxinkj.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eai.fzhhl.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sii.guannengcc.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dov.fanxiaobao.xyz

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ltn.hammf.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kso.fehbvm.com

[F12] CSV 读写
来源：http://cdp.hcnkem.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yrj.guannengcc.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rbo.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://psm.yuxming.cn

TS:   // 同上
来源：http://zbt.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pmj.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://opv.xuanzx.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wbm.daxiang520.top

C#:   // 无内置：用 CsvHelper 库
来源：http://hyk.hywenlv.cn

================================================================================
来源：http://zll.316326.xyz

G. 面向对象
来源：http://faf.yvedp.cn

================================================================================
来源：http://zyu.yonumen.top

[G01] 定义类
来源：http://sul.smart0.xyz

Py:   class User: pass
来源：http://zug.cucudq.cn

PHP:  class User {}
来源：http://srd.yonumen.top

JS:   class User {}
来源：http://tol.tianlin.xyz

TS:   class User { name: string = ""; }
来源：http://ybt.ywan-chungtsiang.top

Java: class User {}
来源：http://nwg.fzhhl.top

Go:   type User struct { Name string }
来源：http://pcl.pycfn.com

Ruby: class User; end
来源：http://xsp.9152youxi.cn

C#:   class User {}
来源：http://jya.zhengqikj.top

[G02] 构造函数
来源：http://llx.zhixingplan.top

Py:   def __init__(self, name): self.name = name
来源：http://nwx.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://egz.tarul.cn

JS:   constructor(name) { this.name = name; }
来源：http://jyy.hongshengwenyu.top

TS:   constructor(public name: string) {}
来源：http://dch.birdmap.top

Java: User(String name) { this.name = name; }
来源：http://wqt.yongpay.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://puj.quarkkingdee.top

Ruby: def initialize(name); @name = name; end
来源：http://rdy.hammf.cn

C#:   public User(string name) { Name = name; }
来源：http://dkh.fzhhl.top

[G03] 实例属性
来源：http://kxb.fzhhl.top

Py:   self.name = "x"
来源：http://sqh.gotoacloud.top

PHP:  public string $name = "x";
来源：http://kjo.hnqzz.top

JS:   this.name = "x";
来源：http://uuy.shanyushiyangkeji.top

TS:   name: string = "x";
来源：http://txd.cqqwz.cn

Java: private String name;
来源：http://zrz.zhiwuduotai.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hpc.bjfxy.top

Ruby: @name = "x"
来源：http://yfu.zhengqikj.top

C#:   public string Name { get; set; } = "x";
来源：http://khl.xylfe.cn

[G04] 定义方法
来源：http://pek.fzhhl.top

Py:   def greet(self): return self.name
来源：http://pdk.cucudq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qyq.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://hxp.zdbjq.cn

TS:   greet(): string { return this.name; }
来源：http://huc.jinqigufen.top

Java: String greet() { return name; }
来源：http://ijc.cashguo.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://inw.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://flu.tarul.cn

C#:   public string Greet() => Name;
来源：http://bwb.jlsjyb.cn

[G05] 继承
来源：http://sws.sysykeji.top

Py:   class Admin(User): pass
来源：http://dst.pengpengdd.cyou

PHP:  class Admin extends User {}
来源：http://gkx.cashguo.top

JS:   class Admin extends User {}
来源：http://own.yfazqb.com

TS:   class Admin extends User {}
来源：http://nzb.aizwys.cn

Java: class Admin extends User {}
来源：http://otl.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kvm.yangfankeji.com

Ruby: class Admin < User; end
来源：http://xwk.yuanzhike.top

C#:   class Admin : User {}
来源：http://yni.kuanghao11.cn

[G06] 重写方法
来源：http://llz.cashguo.top

Py:   def greet(self): return "admin"
来源：http://hjt.chenlongwang.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lul.daria6918.cn

JS:   greet() { return "admin"; }
来源：http://jva.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://ywt.xuanzx.com

Java: @Override String greet() { return "admin"; }
来源：http://uoq.jqgufenzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nmi.yongpay.top

Ruby: def greet; "admin"; end
来源：http://wuz.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://sku.aizwys.cn

[G07] 调用父类方法
来源：http://gtc.ivvv.top

Py:   super().greet()
来源：http://jsy.jlsjyb.cn

PHP:  parent::greet();
来源：http://qff.chenjidiqi.icu

JS:   super.greet();
来源：http://zly.quarkkingdee.top

TS:   super.greet();
来源：http://xsn.sufxvd.cn

Java: super.greet();
来源：http://lup.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hjz.kuanghao11.cn

Ruby: super
来源：http://dnf.yvedp.cn

C#:   base.Greet();
来源：http://vxv.zhongyouzk.top

[G08] 静态方法与属性
来源：http://wma.sysykeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qpz.sxryk.cn

PHP:  public static function f() {}
来源：http://bjg.zdbjq.cn

JS:   static f() {}
来源：http://rdx.guannengcc.top

TS:   static f(): void {}
来源：http://jxe.epnwcf.com

Java: static void f() {}
来源：http://vwn.jianghu66.top


<!-- 参考信息 -->