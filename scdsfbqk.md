代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://yux.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://rfa.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mvz.yuanzhike.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gxs.redwolf501.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yzc.aizwys.cn

[E11] 反转字符串
来源：http://tjz.wangdashe.top

Py:   s[::-1]
来源：http://ajp.gaohongyu789.top

PHP:  strrev($s);
来源：http://rjx.shanyushiyangkeji.top

JS:   [...s].reverse().join("")
来源：http://vrl.shanyushiyangtech.top

TS:   [...s].reverse().join("")
来源：http://tri.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://esf.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oym.zhengqikj.top

Ruby: s.reverse
来源：http://whq.9152youxi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kzr.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://aee.svipenyu.cn

Py:   s.count("a")
来源：http://bjm.sufxvd.cn

PHP:  substr_count($s, "a");
来源：http://uqa.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://esg.tarul.cn

TS:   s.split("a").length - 1
来源：http://qrr.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vph.uphjek.com

Go:   strings.Count(s, "a")
来源：http://afu.yanxiufei.cn

Ruby: s.count("a")
来源：http://rru.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://vbm.ydzc1.top

[E13] 逐字符遍历
来源：http://poa.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://yog.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://shn.9152youxi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aoe.jinqigufen.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aga.shuidangran.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://tof.xziqi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://erp.c1oappe.top

Ruby: s.each_char { |ch| puts ch }
来源：http://oxm.zdbjq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hbc.chenjidiqi.icu

[E14] URL 编码与 Base64
来源：http://gcs.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bgz.tarul.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jfk.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tie.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vax.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://llc.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ofs.dianchejie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nid.yj202588.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rir.tianlin.xyz

[E15] HTML 转义 / 反转义
来源：http://hth.ppjwa.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nem.epnwcf.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://udk.pycfn.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yut.sjlbkw.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ttl.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://aja.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ukt.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oql.shzxlz.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sbg.fengsongda.top

[E16] 数字千分位
来源：http://fgf.zhijiandao.cn

Py:   f"{1234567:,}"
来源：http://pnz.jyoumei.cn

PHP:  number_format(1234567);
来源：http://jlu.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vdw.guannengcc.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vbq.pengpengdd.cyou

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hit.aibaodan.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ztn.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ueu.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://dcc.hysaishi.cn

[E17] 首字母大写
来源：http://fld.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cml.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://syd.nwbrower.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nbr.sufxvd.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cap.xylfe.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://abe.ybcxt.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ekl.hcnkem.com

Ruby: s.capitalize
来源：http://dxr.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lit.zhijiandao.cn

[E18] 模板占位符替换
来源：http://lra.fengsongda.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://moq.tarul.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jyc.quarkkingdee.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pzz.wangdashe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ohe.xylfe.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vwp.jyoumei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mwi.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oag.iojbl.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ugf.hywenlv.cn

[E19] 多行文本按行拆分
来源：http://ztx.daxiang520.top

Py:   s.splitlines()
来源：http://ijc.jqgfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qze.xuanzx.com

JS:   s.split(/\r?\n/)
来源：http://tia.smart0.xyz

TS:   s.split(/\r?\n/)
来源：http://frk.jyoumei.cn

Java: s.lines().toList()
来源：http://com.jiagoushi.top

Go:   strings.Split(s, "\n")
来源：http://cjk.fehbvm.com

Ruby: s.lines
来源：http://gia.dashuyun.cn

C#:   s.Split('\n')
来源：http://wub.jianghu66.top

[E20] 判断字符串是否为空
来源：http://btn.haohaochexian.top

Py:   if not s:
来源：http://xvw.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uhp.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nkk.fehbvm.com

TS:   if (s === "") {}
来源：http://pqm.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://cco.fengsongda.top

Go:   if s == "" {}
来源：http://ojv.shzxlz.cn

Ruby: if s.empty?
来源：http://sdw.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fow.yj202588.top

[E21] 超长截断加省略号
来源：http://pug.zhijiandao.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lay.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zuf.guannengcc.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://snl.hywenlv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aqv.andypj.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sja.shzxlz.cn

Go:   // 按 rune 判断长度后截断
来源：http://slj.nanxuanxn.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dup.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kji.yj202588.top

[E22] 字节长度与字符长度
来源：http://tlv.fehbvm.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://psd.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jkd.hnxiangtu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hhe.wangshuangyany.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://non.birdmap.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://exj.hysaishi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fgr.birdmap.top

Ruby: s.bytesize;  s.length
来源：http://jqa.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qjq.fktsv.cn

================================================================================
来源：http://fwh.jlsjyb.cn

F. 文件与目录
来源：http://hie.feifeiyinyue.top

================================================================================
来源：http://yzx.jyoumei.cn

[F01] 读取整个文件
来源：http://tcm.zdbjq.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qaa.iojbl.cn

PHP:  file_get_contents("a.txt");
来源：http://efd.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ilx.hysaishi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://skq.redwolf501.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rsc.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ldc.pengpengdd.cyou

Ruby: File.read("a.txt")
来源：http://yhq.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://llj.cashguo.top

[F02] 逐行读取文件
来源：http://qtd.zdbjq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qei.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yqk.jiagoushi.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oko.316326.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rip.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qzu.bbcook.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://szi.xylfe.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://glh.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lfm.yueranfly.top

[F03] 写入文件（覆盖）
来源：http://iup.yvedp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jzb.yongpay.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://xmq.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://klj.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jze.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fdn.yonumen.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tzc.cucudq.cn

Ruby: File.write("a.txt", "hi")
来源：http://ugt.xuetiantiany.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mou.zdqjudy.top

[F04] 追加写入文件
来源：http://oaj.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wqv.ctjpmb.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rou.daria6918.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://alh.haohaochexian.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hrj.shzxlz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yfn.jinghuilouyu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lxd.hfpthk.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qhj.ydzc1.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cei.pycfn.com

[F05] 判断文件或目录是否存在
来源：http://rjj.ybcxt.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qat.shzxlz.cn

PHP:  file_exists("a.txt");
来源：http://qoe.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://rsa.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://bub.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sto.zhaomingkeji.xyz

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://huy.gaohongyu789.top

Ruby: File.exist?("a.txt")
来源：http://upt.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://xxm.cdnleiting.top

[F06] 删除文件
来源：http://orq.52xcode.cn

Py:   os.remove("a.txt")
来源：http://had.hongshengwenyu.top

PHP:  unlink("a.txt");
来源：http://hly.pengpengdd.cyou

JS:   fs.unlinkSync("a.txt")
来源：http://gvx.jinqigfzy.top

TS:   fs.unlinkSync("a.txt")
来源：http://hex.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ffo.nanxuanxn.top

Go:   os.Remove("a.txt")
来源：http://toe.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://ybl.shangyingyoupin.top

C#:   File.Delete("a.txt");
来源：http://wme.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://gmp.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fef.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://com.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://osl.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lxz.sjlbkw.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pbj.fehbvm.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pyr.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eva.hysaishi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bwq.shuidangran.top

[F08] 遍历目录
来源：http://zqk.guowangkeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://szk.yj202588.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ktg.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://seg.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://pho.jianghu66.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hmc.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://tsc.guowangkeji.top

Ruby: Dir.children("dir")
来源：http://ouk.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://zuu.zdbjq.cn

[F09] 获取文件大小
来源：http://qgt.cashguo.top

Py:   os.path.getsize("a.txt")
来源：http://tle.fanxiaobao.xyz

PHP:  filesize("a.txt");
来源：http://ovs.fktsv.cn

JS:   fs.statSync("a.txt").size
来源：http://rin.0kj1m.cn

TS:   fs.statSync("a.txt").size
来源：http://gqv.9152youxi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eol.52xcode.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ruy.ydjk.org.cn

Ruby: File.size("a.txt")
来源：http://idy.ppjwa.cn

C#:   new FileInfo("a.txt").Length
来源：http://xjj.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://wmf.guowangkeji.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://azx.daxiang520.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lao.cdnleiting.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zhc.jyoumei.cn

TS:   path.extname("a.txt")
来源：http://azt.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vqw.wangdashe.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rxy.havefunace.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jkp.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eqm.jqgufenzy.top

[F11] 复制与移动文件
来源：http://ykt.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://grj.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://udx.jinghuilouyu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yls.sufxvd.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nqh.xingfuxueyuan.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jsj.52xcode.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hky.snrcjt.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bqc.yfazqb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tmv.iojbl.cn

[F12] CSV 读写
来源：http://vbg.ehwqpu.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rxi.jqgufenzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wms.ctjpmb.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jik.fehbvm.com

TS:   // 同上
来源：http://ywi.snrcjt.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ksc.dianchejie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nyu.iojbl.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gik.zycfv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kqu.zycfv.cn

================================================================================
来源：http://iyf.zhengqikj.top

G. 面向对象
来源：http://inp.ctjpmb.com

================================================================================
来源：http://ams.zhixingplan.top

[G01] 定义类
来源：http://mwk.ywan-chungtsiang.top

Py:   class User: pass
来源：http://fot.c1oappe.top

PHP:  class User {}
来源：http://tcm.yvedp.cn

JS:   class User {}
来源：http://yql.zhoulong.xyz

TS:   class User { name: string = ""; }
来源：http://bod.zdqjudy.top

Java: class User {}
来源：http://bpm.guowangkeji.top

Go:   type User struct { Name string }
来源：http://neq.quarkkingdee.top

Ruby: class User; end
来源：http://pgk.xuetiantiany.cn

C#:   class User {}
来源：http://yxv.jqgufenzy.top

[G02] 构造函数
来源：http://lib.jinqigufen.top

Py:   def __init__(self, name): self.name = name
来源：http://xxn.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://fln.jianghu66.top

JS:   constructor(name) { this.name = name; }
来源：http://hoo.yvedp.cn

TS:   constructor(public name: string) {}
来源：http://enl.zhixingplan.top

Java: User(String name) { this.name = name; }
来源：http://fja.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nsg.9152youxi.cn

Ruby: def initialize(name); @name = name; end
来源：http://rmg.shzxlz.cn

C#:   public User(string name) { Name = name; }
来源：http://uqh.jqgufenzy.top

[G03] 实例属性
来源：http://bak.hnqzz.top

Py:   self.name = "x"
来源：http://hjn.mhx1999.top

PHP:  public string $name = "x";
来源：http://gfg.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://evc.sysykeji.top

TS:   name: string = "x";
来源：http://yyf.zhiwuduotai.top

Java: private String name;
来源：http://suc.nanxinkj.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xrt.uphjek.com

Ruby: @name = "x"
来源：http://nqs.gzhubu.top

C#:   public string Name { get; set; } = "x";
来源：http://cqc.jqgufenzy.top

[G04] 定义方法
来源：http://dhx.zdqjudy.top

Py:   def greet(self): return self.name
来源：http://dhd.hnxiangtu.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ayn.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://dgo.jinqigfzy.top

TS:   greet(): string { return this.name; }
来源：http://djp.hammf.cn

Java: String greet() { return name; }
来源：http://sbn.ydzc1.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://aal.fehbvm.com

Ruby: def greet; @name; end
来源：http://aqr.nanxinkj.top

C#:   public string Greet() => Name;
来源：http://zoj.jinghuilouyu.cn

[G05] 继承
来源：http://txc.shanyushiyangkeji.top

Py:   class Admin(User): pass
来源：http://dhg.xylfe.cn

PHP:  class Admin extends User {}
来源：http://unt.hnqzz.top

JS:   class Admin extends User {}
来源：http://aww.jqgfzy.top

TS:   class Admin extends User {}
来源：http://rzy.pengpengdd.cyou

Java: class Admin extends User {}
来源：http://dad.shanyushiyangkeji.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://oya.jiagoushi.top

Ruby: class Admin < User; end
来源：http://fbp.pycfn.com

C#:   class Admin : User {}
来源：http://rob.pengpengdd.cyou

[G06] 重写方法
来源：http://zbe.andypj.xyz

Py:   def greet(self): return "admin"
来源：http://rqg.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nyg.svipenyu.cn

JS:   greet() { return "admin"; }
来源：http://dec.dianchejie.cn

TS:   greet(): string { return "admin"; }
来源：http://mse.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://pcw.snrcjt.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iiy.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://pbi.bbcook.cn

C#:   public override string Greet() => "admin";
来源：http://php.jinqigfzy.top

[G07] 调用父类方法
来源：http://adf.yuxming.cn

Py:   super().greet()
来源：http://upg.shuidangran.top

PHP:  parent::greet();
来源：http://anm.vqdsnc.cn

JS:   super.greet();
来源：http://uss.andypj.xyz

TS:   super.greet();
来源：http://jfy.hcnkem.com

Java: super.greet();
来源：http://cme.shanyushiyangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kqm.kuanghao11.cn

Ruby: super
来源：http://fyl.zhixingplan.top

C#:   base.Greet();
来源：http://vvv.gogol.net.cn

[G08] 静态方法与属性
来源：http://iql.zhoulong.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ylj.xinyue.icu

PHP:  public static function f() {}
来源：http://cyz.andypj.xyz

JS:   static f() {}
来源：http://gci.pycfn.com

TS:   static f(): void {}
来源：http://zxc.sufxvd.cn

Java: static void f() {}
来源：http://ujf.hnqzz.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ynp.fengsongda.top

Ruby: def self.f; end
来源：http://pjw.zhijiandao.cn

C#:   public static void F() {}
来源：http://yyg.gotoacloud.top

[G09] 接口 / 抽象类
来源：http://ftw.ctjpmb.com


<!-- 参考信息 -->