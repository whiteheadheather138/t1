代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://igi.nanxinkj.top

[E11] 反转字符串
来源：http://wdm.jqgufenzy.top

Py:   s[::-1]
来源：http://ely.zdbjq.cn

PHP:  strrev($s);
来源：http://dbo.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://nlu.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://nna.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tbw.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dzo.vehdjk.com

Ruby: s.reverse
来源：http://zdq.nanxuanxn.top

C#:   new string(s.Reverse().ToArray())
来源：http://pgj.tianlin.xyz

[E12] 统计某字符出现次数
来源：http://dph.52xcode.cn

Py:   s.count("a")
来源：http://yub.pengpengdd.cyou

PHP:  substr_count($s, "a");
来源：http://idl.ppjwa.cn

JS:   s.split("a").length - 1
来源：http://fow.yonumen.top

TS:   s.split("a").length - 1
来源：http://dmz.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rbx.yueranfly.top

Go:   strings.Count(s, "a")
来源：http://ujr.haohaochexian.top

Ruby: s.count("a")
来源：http://rsx.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://fra.c1oappe.top

[E13] 逐字符遍历
来源：http://gxo.zhaomingkeji.xyz

Py:   for ch in s: print(ch)
来源：http://lmo.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jxz.hcnkem.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ruw.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lah.gogol.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://olz.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://muc.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rzd.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jqh.gaohongyu789.top

[E14] URL 编码与 Base64
来源：http://rtp.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://njq.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://trq.kuanghao11.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rhp.bbcook.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jcy.fengsongda.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xfc.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xvc.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ahp.aizwys.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nif.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://ttd.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://svm.aizwys.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://crv.tarul.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mfh.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://igr.yvedp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sbq.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://esw.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://szh.316326.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tft.sjlbkw.cn

[E16] 数字千分位
来源：http://uns.pengpengdd.cyou

Py:   f"{1234567:,}"
来源：http://nde.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://wws.yj202588.top

JS:   (1234567).toLocaleString("en-US")
来源：http://htw.kuanghao11.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ded.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lgv.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wik.hongshengwenyu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tdi.xinyue.icu

C#:   1234567.ToString("N0")
来源：http://sih.ydzc1.top

[E17] 首字母大写
来源：http://vsh.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hbz.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lon.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gve.jiagoushi.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mvs.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qdg.zhiwuduotai.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://plt.quarkkingdee.top

Ruby: s.capitalize
来源：http://xsu.cdnleiting.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aif.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://wkp.aibaodan.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xyz.pengpengdd.cyou

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tkg.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uqs.cqqwz.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bgt.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zgk.yfazqb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zlk.wangshuangyany.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://car.jinqigufen.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://isc.ppjwa.cn

[E19] 多行文本按行拆分
来源：http://ity.xuanzx.com

Py:   s.splitlines()
来源：http://lve.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hsn.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://lnd.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://ice.316326.xyz

Java: s.lines().toList()
来源：http://mfb.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://bor.cucudq.cn

Ruby: s.lines
来源：http://dyp.guannengcc.top

C#:   s.Split('\n')
来源：http://ukm.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://fos.kuanghao11.cn

Py:   if not s:
来源：http://tqs.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hws.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://joj.yuanzhike.top

TS:   if (s === "") {}
来源：http://ybx.nanxuanxn.top

Java: if (s.isEmpty()) {}
来源：http://tbw.yangfankeji.com

Go:   if s == "" {}
来源：http://gcu.ehwqpu.com

Ruby: if s.empty?
来源：http://qao.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vji.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://tyi.jiagoushi.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bpl.jlsjyb.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zmw.epnwcf.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vct.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eax.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pjm.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://feb.ydjk.org.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zdu.daxiang520.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xyd.xinyue.icu

[E22] 字节长度与字符长度
来源：http://dbg.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nsm.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ruz.9152youxi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ial.zhijiandao.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hdr.pengpengdd.cyou

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qua.quarkkingdee.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fhy.zycfv.cn

Ruby: s.bytesize;  s.length
来源：http://hav.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://puv.uphjek.com

================================================================================
来源：http://xyw.shanyushiyangtech.top

F. 文件与目录
来源：http://gzs.bbcook.cn

================================================================================
来源：http://rir.hnqzz.top

[F01] 读取整个文件
来源：http://ifc.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mqi.hammf.cn

PHP:  file_get_contents("a.txt");
来源：http://lks.pengpengdd.cyou

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ypg.yonumen.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mxp.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rhf.tian-w.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ftb.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://vxu.aibaodan.cn

C#:   File.ReadAllText("a.txt");
来源：http://aks.ctjpmb.com

[F02] 逐行读取文件
来源：http://uxz.uphjek.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cde.quarkkingdee.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wqw.redwolf501.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cyk.jqgfzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dkc.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mey.52xcode.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kbe.dianchejie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rxg.jinghuilouyu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rnx.cashguo.top

[F03] 写入文件（覆盖）
来源：http://eok.nwbrower.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eck.wangshuangyany.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://awc.hongshengwenyu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oqr.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sdx.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uht.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yfh.cashguo.top

Ruby: File.write("a.txt", "hi")
来源：http://kzt.chenlongwang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qkh.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://oxf.ybcxt.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xvw.cucudq.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bqr.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xdw.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fct.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://skr.hnxiangtu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://imq.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pfc.shzxlz.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dmt.yj20258888.top

[F05] 判断文件或目录是否存在
来源：http://cjn.hfpthk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oue.cdnleiting.top

PHP:  file_exists("a.txt");
来源：http://rtw.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://tlk.uphjek.com

TS:   fs.existsSync("a.txt")
来源：http://sxu.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fec.yuxming.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qwc.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://jan.shanyushiyangtech.top

C#:   File.Exists("a.txt")
来源：http://ddm.chenjidiqi.icu

[F06] 删除文件
来源：http://utf.zhoulong.xyz

Py:   os.remove("a.txt")
来源：http://awh.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://asz.chenlongwang.top

JS:   fs.unlinkSync("a.txt")
来源：http://tgj.xuetiantiany.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uzg.nwbrower.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rkx.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://bmr.nwbrower.top

Ruby: File.delete("a.txt")
来源：http://qgc.daxiang520.top

C#:   File.Delete("a.txt");
来源：http://lya.jianghu66.top

[F07] 创建目录（含多级）
来源：http://urn.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sit.ppjwa.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cts.chenzaomai.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://etb.andypj.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kip.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vvc.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kdn.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qfr.fzhhl.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aqm.pycfn.com

[F08] 遍历目录
来源：http://xah.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://arv.dashuyun.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mvx.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://ser.uphjek.com

TS:   fs.readdirSync("dir")
来源：http://dwo.sufxvd.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zsb.guowangkeji.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://vxf.yfazqb.com

Ruby: Dir.children("dir")
来源：http://qdc.pycfn.com

C#:   Directory.GetFiles("dir")
来源：http://iht.fzhhl.top

[F09] 获取文件大小
来源：http://trk.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://hbt.birdmap.top

PHP:  filesize("a.txt");
来源：http://imz.yj20258888.top

JS:   fs.statSync("a.txt").size
来源：http://sfr.feifeiyinyue.top

TS:   fs.statSync("a.txt").size
来源：http://iez.mhx1999.top

Java: Files.size(Path.of("a.txt"))
来源：http://vos.chenlongwang.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gzn.nwbrower.top

Ruby: File.size("a.txt")
来源：http://pou.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://tft.hywenlv.cn

[F10] 取文件扩展名 / 文件名
来源：http://wsk.tarul.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sdw.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kko.ydzc1.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tou.yj20258.top

TS:   path.extname("a.txt")
来源：http://zqk.ywan-chungtsiang.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tkj.haohaochexian.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jpm.zhengqikj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://spt.xylfe.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://egf.chenjidiqi.icu

[F11] 复制与移动文件
来源：http://zod.fktsv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jco.chenlongwang.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lcc.yueranfly.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ork.hnqzz.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qsn.yuanzhike.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lrw.gotoacloud.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wip.shzxlz.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eli.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nnt.wangdashe.top

[F12] CSV 读写
来源：http://vua.sufxvd.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rqy.redwolf501.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nqz.hnqzz.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egk.tanke756.top

TS:   // 同上
来源：http://jcg.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://plb.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://oco.chenjidiqi.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://coi.hcnkem.com

C#:   // 无内置：用 CsvHelper 库
来源：http://tbp.sufxvd.cn

================================================================================
来源：http://lnc.yj202588.top

G. 面向对象
来源：http://xnu.iojbl.cn

================================================================================
来源：http://kwr.jinqigufen.top

[G01] 定义类
来源：http://zzu.jiagoushi.top

Py:   class User: pass
来源：http://fcl.yueranfly.top

PHP:  class User {}
来源：http://qia.fktsv.cn

JS:   class User {}
来源：http://yxi.ydzc1.top

TS:   class User { name: string = ""; }
来源：http://heq.9152youxi.cn

Java: class User {}
来源：http://mro.ydjk.org.cn

Go:   type User struct { Name string }
来源：http://gqq.havefunace.top

Ruby: class User; end
来源：http://xdh.tianlin.xyz

C#:   class User {}
来源：http://gjj.vqdsnc.cn

[G02] 构造函数
来源：http://bfj.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://csn.zdqjudy.top

PHP:  public function __construct(public string $name) {}
来源：http://zxa.ppjwa.cn

JS:   constructor(name) { this.name = name; }
来源：http://ynr.hammf.cn

TS:   constructor(public name: string) {}
来源：http://hrq.jinyuanbaomall.cn

Java: User(String name) { this.name = name; }
来源：http://leh.yonumen.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://thy.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://dgn.yuxming.cn

C#:   public User(string name) { Name = name; }
来源：http://ahn.iojbl.cn

[G03] 实例属性
来源：http://vzo.smart0.xyz

Py:   self.name = "x"
来源：http://fvz.yanxiufei.cn

PHP:  public string $name = "x";
来源：http://bjy.chenlongwang.top

JS:   this.name = "x";
来源：http://plf.yangfankeji.com

TS:   name: string = "x";
来源：http://lfo.jinqigfzy.top

Java: private String name;
来源：http://prf.yuanzhike.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hsj.andypj.xyz

Ruby: @name = "x"
来源：http://ptb.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://msm.fengsongda.top

[G04] 定义方法
来源：http://wun.smart0.xyz

Py:   def greet(self): return self.name
来源：http://dso.fzhhl.top

PHP:  public function greet(): string { return $this->name; }
来源：http://aqm.yj20258888.top

JS:   greet() { return this.name; }
来源：http://upt.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://cmi.shzxlz.cn

Java: String greet() { return name; }
来源：http://vlj.yuanzhike.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://glv.haohaochexian.top

Ruby: def greet; @name; end
来源：http://usb.gogol.net.cn

C#:   public string Greet() => Name;
来源：http://mcx.chenzaomai.com

[G05] 继承
来源：http://ech.zhixingplan.top

Py:   class Admin(User): pass
来源：http://aqz.cqqwz.cn

PHP:  class Admin extends User {}
来源：http://uwc.iojbl.cn

JS:   class Admin extends User {}
来源：http://nix.zhixingplan.top

TS:   class Admin extends User {}
来源：http://ljl.hfpthk.cn

Java: class Admin extends User {}
来源：http://vlk.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zae.yuxming.cn

Ruby: class Admin < User; end
来源：http://hyt.hfpthk.cn

C#:   class Admin : User {}
来源：http://qcn.quarkkingdee.top

[G06] 重写方法
来源：http://grd.jqgfzy.top

Py:   def greet(self): return "admin"
来源：http://mkv.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mob.jiagoushi.top

JS:   greet() { return "admin"; }
来源：http://ypn.ehwqpu.com

TS:   greet(): string { return "admin"; }
来源：http://vwp.gogol.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://nvf.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ivz.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://dkz.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://bzu.andypj.xyz

[G07] 调用父类方法
来源：http://kom.jyoumei.cn

Py:   super().greet()
来源：http://ipo.bbcook.cn

PHP:  parent::greet();
来源：http://fwp.yangfankeji.com

JS:   super.greet();
来源：http://xca.bjfxy.top

TS:   super.greet();
来源：http://leo.gotoacloud.top

Java: super.greet();
来源：http://foo.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sqm.zhixingplan.top

Ruby: super
来源：http://anh.birdmap.top

C#:   base.Greet();
来源：http://bud.ehwqpu.com

[G08] 静态方法与属性
来源：http://ave.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ovh.tarul.cn

PHP:  public static function f() {}
来源：http://lte.yfazqb.com

JS:   static f() {}
来源：http://foo.guannengcc.top

TS:   static f(): void {}
来源：http://czi.jiagoushi.top

Java: static void f() {}
来源：http://niz.zhengqikj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://eip.52xcode.cn

Ruby: def self.f; end
来源：http://qrk.meibo888.top

C#:   public static void F() {}
来源：http://xuv.daria6918.cn

[G09] 接口 / 抽象类
来源：http://qme.meibo888.top

Py:   from abc import ABC, abstractmethod
来源：http://wwc.zhijiandao.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fli.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://cpz.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://aaq.yonumen.top


<!-- 参考信息 -->