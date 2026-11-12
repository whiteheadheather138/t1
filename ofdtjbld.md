代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://grx.jiagoushi.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ijt.daria6918.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://doe.xinyue.icu

JS:   "7".padStart(3, "0")
来源：http://bpp.hfpthk.cn

TS:   "7".padStart(3, "0")
来源：http://uqw.hcnkem.com

Java: String.format("%03d", 7)
来源：http://mjb.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xgv.ehwqpu.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rot.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bxx.zdqjudy.top

[E11] 反转字符串
来源：http://glm.zhixingplan.top

Py:   s[::-1]
来源：http://six.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://jyw.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://duh.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://rot.xuetiantiany.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gsu.ivvv.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xwa.jiagoushi.top

Ruby: s.reverse
来源：http://xyu.c1oappe.top

C#:   new string(s.Reverse().ToArray())
来源：http://kkd.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://atn.redwolf501.top

Py:   s.count("a")
来源：http://hpp.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://qoo.jqgfzy.top

JS:   s.split("a").length - 1
来源：http://yhj.yueranfly.top

TS:   s.split("a").length - 1
来源：http://ppr.hongshengwenyu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://saw.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://jya.guowangkeji.top

Ruby: s.count("a")
来源：http://juk.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://bcz.cdnleiting.top

[E13] 逐字符遍历
来源：http://rli.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://itm.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rhb.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://sxn.hysaishi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dov.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vrt.nanxinkj.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pjb.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ihm.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oht.yuxming.cn

[E14] URL 编码与 Base64
来源：http://qpc.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cdn.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://iyi.birdmap.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gza.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yyn.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cub.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qte.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rmx.zdqjudy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xzb.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://bnk.yuxming.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yje.cashguo.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iqs.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zpe.gzhubu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lxr.yanxiufei.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dgr.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qmf.0kj1m.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tjh.nanxuanxn.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mfp.xinyue.icu

[E16] 数字千分位
来源：http://ngd.uphjek.com

Py:   f"{1234567:,}"
来源：http://mms.zhiwuduotai.top

PHP:  number_format(1234567);
来源：http://zzn.ydjk.org.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://chj.jlsjyb.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xpq.yongpay.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wwu.yj202588.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fex.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vbs.cashguo.top

C#:   1234567.ToString("N0")
来源：http://cbo.zhijiandao.cn

[E17] 首字母大写
来源：http://dfq.yonumen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ect.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rjl.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xsw.tian-w.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xor.tanke756.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://llc.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hjv.yfazqb.com

Ruby: s.capitalize
来源：http://jbx.xziqi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pgg.xziqi.cn

[E18] 模板占位符替换
来源：http://ics.dianchejie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qzx.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://drw.zhoulong.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://azo.yueranfly.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xer.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bck.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pfa.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xxe.andypj.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wkv.c1oappe.top

[E19] 多行文本按行拆分
来源：http://rwv.hcnkem.com

Py:   s.splitlines()
来源：http://sci.zhiwuduotai.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://acr.jqgufenzy.top

JS:   s.split(/\r?\n/)
来源：http://dpv.0kj1m.cn

TS:   s.split(/\r?\n/)
来源：http://vrr.zhengqikj.top

Java: s.lines().toList()
来源：http://eqo.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://uxn.snrcjt.cn

Ruby: s.lines
来源：http://hsn.ydzc1.top

C#:   s.Split('\n')
来源：http://xxw.tanke756.top

[E20] 判断字符串是否为空
来源：http://opc.c1oappe.top

Py:   if not s:
来源：http://fxp.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://apv.smart0.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uhk.cdnleiting.top

TS:   if (s === "") {}
来源：http://bcn.shanyushiyangtech.top

Java: if (s.isEmpty()) {}
来源：http://kdr.tian-w.cn

Go:   if s == "" {}
来源：http://uro.zycfv.cn

Ruby: if s.empty?
来源：http://pcq.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://czp.snrcjt.cn

[E21] 超长截断加省略号
来源：http://zpg.mhx1999.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://veh.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vrk.ydzc1.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ryy.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nom.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://daf.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://fat.ydzc1.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vfg.guannengcc.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yqc.pycfn.com

[E22] 字节长度与字符长度
来源：http://vdb.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qhq.sxryk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lcz.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ant.jinghuilouyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lfr.fzhhl.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lou.zycfv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ebv.cheryme.top

Ruby: s.bytesize;  s.length
来源：http://rac.daxiang520.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jzd.dianchejie.cn

================================================================================
来源：http://jdy.kuanghao11.cn

F. 文件与目录
来源：http://wgm.wangshuangyany.cn

================================================================================
来源：http://iwx.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://pdt.ydzc1.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://agt.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://jsz.ctjpmb.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nbl.svipenyu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://soe.52xcode.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://skj.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://obk.dianchejie.cn

Ruby: File.read("a.txt")
来源：http://puw.0kj1m.cn

C#:   File.ReadAllText("a.txt");
来源：http://gtn.andypj.xyz

[F02] 逐行读取文件
来源：http://tmk.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xlq.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jdy.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zle.9152youxi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iqo.svipenyu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pww.cheryme.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://agj.zhengqikj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nnx.uphjek.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zwc.sweek.top

[F03] 写入文件（覆盖）
来源：http://dbf.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lkt.xinyue.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://dpb.quarkkingdee.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rqs.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nmx.hongshengwenyu.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dit.hesvh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jiv.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://tpo.shzxlz.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ncj.ydzc1.top

[F04] 追加写入文件
来源：http://kce.vqdsnc.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cmw.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cdn.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rhf.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fws.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rgn.birdmap.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cnt.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lpp.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fpd.daria6918.cn

[F05] 判断文件或目录是否存在
来源：http://uqm.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fdp.fehbvm.com

PHP:  file_exists("a.txt");
来源：http://xdt.zycfv.cn

JS:   fs.existsSync("a.txt")
来源：http://tty.yj20258.top

TS:   fs.existsSync("a.txt")
来源：http://hss.gogol.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://swk.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gjn.jianghu66.top

Ruby: File.exist?("a.txt")
来源：http://hyj.zhixingplan.top

C#:   File.Exists("a.txt")
来源：http://iji.dashuyun.cn

[F06] 删除文件
来源：http://fzi.haohaochexian.top

Py:   os.remove("a.txt")
来源：http://hoc.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://gsr.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://dwj.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://iad.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pde.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://jnb.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://vpg.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://gdl.hnqzz.top

[F07] 创建目录（含多级）
来源：http://mlk.tanke756.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cac.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://drf.nanxuanxn.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yzd.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vjr.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eyz.jianghu66.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kig.yongpay.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iei.hfpthk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qfg.nanxuanxn.top

[F08] 遍历目录
来源：http://hfi.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://yie.shangyingyoupin.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oqu.mhx1999.top

JS:   fs.readdirSync("dir")
来源：http://oin.pycfn.com

TS:   fs.readdirSync("dir")
来源：http://ecx.cheryme.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://loe.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xjd.dashuyun.cn

Ruby: Dir.children("dir")
来源：http://xfc.fktsv.cn

C#:   Directory.GetFiles("dir")
来源：http://yzz.zhengqikj.top

[F09] 获取文件大小
来源：http://ypm.xziqi.cn

Py:   os.path.getsize("a.txt")
来源：http://tfh.ehwqpu.com

PHP:  filesize("a.txt");
来源：http://zis.ybcxt.top

JS:   fs.statSync("a.txt").size
来源：http://xyd.zhaomingkeji.xyz

TS:   fs.statSync("a.txt").size
来源：http://isf.nanxuanxn.top

Java: Files.size(Path.of("a.txt"))
来源：http://woo.hfpthk.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nqu.shuidangran.top

Ruby: File.size("a.txt")
来源：http://lbd.bjfxy.top

C#:   new FileInfo("a.txt").Length
来源：http://vfx.zhongyouzk.top

[F10] 取文件扩展名 / 文件名
来源：http://utd.epnwcf.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://evf.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eht.fktsv.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://doi.pycfn.com

TS:   path.extname("a.txt")
来源：http://ccu.yueranfly.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jsb.gaohongyu789.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mvk.xziqi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vyu.shanyushiyangkeji.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ymx.ctjpmb.com

[F11] 复制与移动文件
来源：http://cki.jinghuilouyu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xlk.zhongyouzk.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dfm.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bar.svipenyu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ixj.bbcook.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wmu.tanke756.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kxc.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uke.aizwys.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ekq.birdmap.top

[F12] CSV 读写
来源：http://jgs.ppjwa.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tdy.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sxj.chenjidiqi.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nyh.zycfv.cn

TS:   // 同上
来源：http://bwg.ehwqpu.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jyu.ppjwa.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yfi.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://svy.xziqi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yxt.nwbrower.top

================================================================================
来源：http://kes.jqgufenzy.top

G. 面向对象
来源：http://gih.sufxvd.cn

================================================================================
来源：http://glm.dashuyun.cn

[G01] 定义类
来源：http://whf.haohaochexian.top

Py:   class User: pass
来源：http://drc.ctjpmb.com

PHP:  class User {}
来源：http://vzy.cheryme.top

JS:   class User {}
来源：http://aqu.shanyushiyangkeji.top

TS:   class User { name: string = ""; }
来源：http://egz.smart0.xyz

Java: class User {}
来源：http://krm.jiagoushi.top

Go:   type User struct { Name string }
来源：http://dcd.zdbjq.cn

Ruby: class User; end
来源：http://mdb.yangfankeji.com

C#:   class User {}
来源：http://tml.jyoumei.cn

[G02] 构造函数
来源：http://lcb.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://ecd.sxryk.cn

PHP:  public function __construct(public string $name) {}
来源：http://wwp.hammf.cn

JS:   constructor(name) { this.name = name; }
来源：http://pql.zycfv.cn

TS:   constructor(public name: string) {}
来源：http://qic.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://aok.cucudq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ntf.fktsv.cn

Ruby: def initialize(name); @name = name; end
来源：http://cog.zhixingplan.top

C#:   public User(string name) { Name = name; }
来源：http://ptu.yj202588.top

[G03] 实例属性
来源：http://gfo.52xcode.cn

Py:   self.name = "x"
来源：http://uos.jinqigfzy.top

PHP:  public string $name = "x";
来源：http://pyd.sweek.top

JS:   this.name = "x";
来源：http://vjt.ehwqpu.com

TS:   name: string = "x";
来源：http://tzj.andypj.xyz

Java: private String name;
来源：http://jur.nwbrower.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ksm.cqqwz.cn

Ruby: @name = "x"
来源：http://ilb.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://cet.ydzc1.top

[G04] 定义方法
来源：http://dya.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://pmp.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://rdd.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://xfx.vqdsnc.cn

TS:   greet(): string { return this.name; }
来源：http://mmj.aibaodan.cn

Java: String greet() { return name; }
来源：http://rfd.aibaodan.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bpa.feifeiyinyue.top

Ruby: def greet; @name; end
来源：http://lbi.fzhhl.top

C#:   public string Greet() => Name;
来源：http://dvk.yuxming.cn

[G05] 继承
来源：http://syb.tianlin.xyz

Py:   class Admin(User): pass
来源：http://uma.shanyushiyangkeji.top

PHP:  class Admin extends User {}
来源：http://mvr.hywenlv.cn

JS:   class Admin extends User {}
来源：http://qxp.andypj.xyz

TS:   class Admin extends User {}
来源：http://idt.jyoumei.cn

Java: class Admin extends User {}
来源：http://hkv.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ygt.zhijiandao.cn

Ruby: class Admin < User; end
来源：http://ysm.pycfn.com

C#:   class Admin : User {}
来源：http://jqi.chenzaomai.com

[G06] 重写方法
来源：http://dix.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://wgm.jinyuanbaomall.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ppm.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://oja.hnxiangtu.top

TS:   greet(): string { return "admin"; }
来源：http://hyn.52xcode.cn

Java: @Override String greet() { return "admin"; }
来源：http://ikp.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bhv.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://sme.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://off.andypj.xyz

[G07] 调用父类方法
来源：http://pbh.gaohongyu789.top

Py:   super().greet()
来源：http://wcm.jianghu66.top

PHP:  parent::greet();
来源：http://xvj.jqgufenzy.top

JS:   super.greet();
来源：http://tyk.vehdjk.com

TS:   super.greet();
来源：http://vfz.wangdashe.top

Java: super.greet();
来源：http://now.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yxf.epnwcf.com

Ruby: super
来源：http://kgq.vehdjk.com

C#:   base.Greet();
来源：http://rue.tarul.cn

[G08] 静态方法与属性
来源：http://zxj.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gqy.jinqigufen.top

PHP:  public static function f() {}
来源：http://drj.jiagoushi.top

JS:   static f() {}
来源：http://hzx.tianlin.xyz

TS:   static f(): void {}
来源：http://rbj.ydjk.org.cn

Java: static void f() {}
来源：http://iiw.pengpengdd.cyou


<!-- 参考信息 -->