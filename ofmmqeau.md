代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jqp.yj20258888.top

[E11] 反转字符串
来源：http://dwf.jqgfzy.top

Py:   s[::-1]
来源：http://mnp.andypj.xyz

PHP:  strrev($s);
来源：http://yba.ctjpmb.com

JS:   [...s].reverse().join("")
来源：http://zta.yj20258.top

TS:   [...s].reverse().join("")
来源：http://pmx.jlsjyb.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://vbx.hnqzz.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://rrp.snrcjt.cn

Ruby: s.reverse
来源：http://hrm.chenjidiqi.icu

C#:   new string(s.Reverse().ToArray())
来源：http://svn.shuidangran.top

[E12] 统计某字符出现次数
来源：http://nnd.yanxiufei.cn

Py:   s.count("a")
来源：http://edv.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://yzl.cucudq.cn

JS:   s.split("a").length - 1
来源：http://xmz.meibo888.top

TS:   s.split("a").length - 1
来源：http://hbj.aizwys.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gxx.jqgfzy.top

Go:   strings.Count(s, "a")
来源：http://zst.wangshuangyany.cn

Ruby: s.count("a")
来源：http://orl.ywan-chungtsiang.top

C#:   s.Count(c => c == 'a')
来源：http://cdi.jlsjyb.cn

[E13] 逐字符遍历
来源：http://sol.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://vgd.jinqigufen.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uby.cqqwz.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qgk.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://tql.yvedp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ohe.jinghuilouyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lwn.jyoumei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rya.ivvv.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://byw.hnqzz.top

[E14] URL 编码与 Base64
来源：http://cll.yuxming.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ubv.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ofu.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yaf.vqdsnc.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xbs.dashuyun.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://saw.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jew.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yiv.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bto.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://omh.ctjpmb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://atc.ydzc1.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gyv.hcnkem.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bfn.ehwqpu.com

TS:   // 同上，务必做 XSS 过滤
来源：http://vzw.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qxm.gzhubu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zxi.xuanzx.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bdv.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ure.hammf.cn

[E16] 数字千分位
来源：http://ehz.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://afx.316326.xyz

PHP:  number_format(1234567);
来源：http://pog.hesvh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ibn.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://epe.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://knq.jiagoushi.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ayl.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lfp.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://mqd.hysaishi.cn

[E17] 首字母大写
来源：http://lpj.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bzx.316326.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://pof.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pdh.ybcxt.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iir.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rzr.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eui.sweek.top

Ruby: s.capitalize
来源：http://var.ybcxt.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oly.jqgfzy.top

[E18] 模板占位符替换
来源：http://wrq.yanxiufei.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cum.pycfn.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sur.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eao.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mpp.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xqz.sysykeji.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ecs.ydzc1.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xcm.svipenyu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bwc.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://cgw.epnwcf.com

Py:   s.splitlines()
来源：http://usj.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ztg.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://cyz.cdnleiting.top

TS:   s.split(/\r?\n/)
来源：http://omz.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://gba.cqqwz.cn

Go:   strings.Split(s, "\n")
来源：http://bzb.dashuyun.cn

Ruby: s.lines
来源：http://rxj.jyoumei.cn

C#:   s.Split('\n')
来源：http://cwd.tian-w.cn

[E20] 判断字符串是否为空
来源：http://iyw.ydjk.org.cn

Py:   if not s:
来源：http://qtu.xingfuxueyuan.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mev.birdmap.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vsn.xziqi.cn

TS:   if (s === "") {}
来源：http://guf.shuidangran.top

Java: if (s.isEmpty()) {}
来源：http://fjh.cucudq.cn

Go:   if s == "" {}
来源：http://pty.cheryme.top

Ruby: if s.empty?
来源：http://pnd.haohaochexian.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sky.zhixingplan.top

[E21] 超长截断加省略号
来源：http://zlv.yueranfly.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vub.yj20258888.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ddm.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tgq.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yar.zhiwuduotai.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mtf.aizwys.cn

Go:   // 按 rune 判断长度后截断
来源：http://zxe.shuidangran.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wmq.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xnv.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://upi.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mqg.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dyk.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kdu.zdqjudy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qsr.daria6918.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ufi.feifeiyinyue.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://skq.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://avy.shanyushiyangtech.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yov.havefunace.top

================================================================================
来源：http://kpk.jinyuanbaomall.cn

F. 文件与目录
来源：http://plc.svipenyu.cn

================================================================================
来源：http://wwy.tian-w.cn

[F01] 读取整个文件
来源：http://ejw.tanke756.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gft.chenzaomai.com

PHP:  file_get_contents("a.txt");
来源：http://qob.bjfxy.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mul.yvedp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ekf.tarul.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wij.jianghu66.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dww.hcnkem.com

Ruby: File.read("a.txt")
来源：http://zkj.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://szn.jiagoushi.top

[F02] 逐行读取文件
来源：http://thq.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://epq.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oyu.xuanzx.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://goo.snrcjt.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jbb.pengpengdd.cyou

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bqj.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kgx.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rdd.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://esi.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://xig.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bng.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vne.zhaomingkeji.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dig.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sxr.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fnp.wangshuangyany.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ouc.zycfv.cn

Ruby: File.write("a.txt", "hi")
来源：http://mbc.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dsr.yanxiufei.cn

[F04] 追加写入文件
来源：http://jnx.tianlin.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oit.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ekt.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ytn.aibaodan.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://leh.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dwb.ivvv.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://seb.fanxiaobao.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pli.gaohongyu789.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yzf.52xcode.cn

[F05] 判断文件或目录是否存在
来源：http://yvi.nanxinkj.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vih.gzhubu.top

PHP:  file_exists("a.txt");
来源：http://roi.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://tfp.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://omy.cdnleiting.top

Java: Files.exists(Path.of("a.txt"))
来源：http://rdy.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zki.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://flf.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://bbz.hnxiangtu.top

[F06] 删除文件
来源：http://mxj.zdqjudy.top

Py:   os.remove("a.txt")
来源：http://jmy.ehwqpu.com

PHP:  unlink("a.txt");
来源：http://tyb.jqgfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://mms.cdnleiting.top

TS:   fs.unlinkSync("a.txt")
来源：http://vgw.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lym.ybcxt.top

Go:   os.Remove("a.txt")
来源：http://npi.yanxiufei.cn

Ruby: File.delete("a.txt")
来源：http://eif.yuanzhike.top

C#:   File.Delete("a.txt");
来源：http://zda.hysaishi.cn

[F07] 创建目录（含多级）
来源：http://frt.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iqv.fanxiaobao.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jct.ctjpmb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pee.tarul.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jnb.smart0.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bee.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ull.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kcq.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eca.uphjek.com

[F08] 遍历目录
来源：http://vtw.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aks.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qfg.9152youxi.cn

JS:   fs.readdirSync("dir")
来源：http://huw.havefunace.top

TS:   fs.readdirSync("dir")
来源：http://wcl.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dnc.yonumen.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://poi.yongpay.top

Ruby: Dir.children("dir")
来源：http://stq.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://vdu.daria6918.cn

[F09] 获取文件大小
来源：http://leb.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://bbp.zhoulong.xyz

PHP:  filesize("a.txt");
来源：http://mai.zdqjudy.top

JS:   fs.statSync("a.txt").size
来源：http://qsg.yangfankeji.com

TS:   fs.statSync("a.txt").size
来源：http://ktk.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://utl.hcnkem.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aon.haohaochexian.top

Ruby: File.size("a.txt")
来源：http://xrt.shanyushiyangtech.top

C#:   new FileInfo("a.txt").Length
来源：http://zfx.xuanzx.com

[F10] 取文件扩展名 / 文件名
来源：http://vqn.sweek.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cch.0kj1m.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nlp.zhoulong.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kae.zdbjq.cn

TS:   path.extname("a.txt")
来源：http://qgd.iojbl.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ovo.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xlk.zdqjudy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uws.wangshuangyany.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sye.yj20258888.top

[F11] 复制与移动文件
来源：http://ttp.0kj1m.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kvh.smart0.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xys.tanke756.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xfk.xuanzx.com

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vzz.fanxiaobao.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cfi.daxiang520.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wbb.fehbvm.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hfj.shangyingyoupin.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pwc.haohaochexian.top

[F12] CSV 读写
来源：http://tch.sweek.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://iyu.sufxvd.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bxv.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lfj.cucudq.cn

TS:   // 同上
来源：http://bkl.jqgfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ply.guannengcc.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ice.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kkj.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cgn.hnxiangtu.top

================================================================================
来源：http://pzz.yueranfly.top

G. 面向对象
来源：http://ujt.9152youxi.cn

================================================================================
来源：http://lmt.snrcjt.cn

[G01] 定义类
来源：http://brp.9152youxi.cn

Py:   class User: pass
来源：http://uoa.zdbjq.cn

PHP:  class User {}
来源：http://huc.xylfe.cn

JS:   class User {}
来源：http://iqa.andypj.xyz

TS:   class User { name: string = ""; }
来源：http://pun.xinyue.icu

Java: class User {}
来源：http://gaw.sxryk.cn

Go:   type User struct { Name string }
来源：http://oud.xylfe.cn

Ruby: class User; end
来源：http://jjn.yvedp.cn

C#:   class User {}
来源：http://rwh.xziqi.cn

[G02] 构造函数
来源：http://nzw.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://wjd.hongshengwenyu.top

PHP:  public function __construct(public string $name) {}
来源：http://pdu.aibaodan.cn

JS:   constructor(name) { this.name = name; }
来源：http://qim.meibo888.top

TS:   constructor(public name: string) {}
来源：http://nut.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://jtx.zycfv.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hvw.hnqzz.top

Ruby: def initialize(name); @name = name; end
来源：http://jja.daria6918.cn

C#:   public User(string name) { Name = name; }
来源：http://mxv.gaohongyu789.top

[G03] 实例属性
来源：http://pai.gaohongyu789.top

Py:   self.name = "x"
来源：http://len.0kj1m.cn

PHP:  public string $name = "x";
来源：http://omo.xziqi.cn

JS:   this.name = "x";
来源：http://mtw.jianghu66.top

TS:   name: string = "x";
来源：http://etg.smart0.xyz

Java: private String name;
来源：http://spr.52xcode.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mcf.redwolf501.top

Ruby: @name = "x"
来源：http://bse.haohaochexian.top

C#:   public string Name { get; set; } = "x";
来源：http://bgo.hesvh.cn

[G04] 定义方法
来源：http://avt.hesvh.cn

Py:   def greet(self): return self.name
来源：http://zcj.yongpay.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xro.redwolf501.top

JS:   greet() { return this.name; }
来源：http://unm.yvedp.cn

TS:   greet(): string { return this.name; }
来源：http://ukd.wangshuangyany.cn

Java: String greet() { return name; }
来源：http://qjk.shzxlz.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vhj.c1oappe.top

Ruby: def greet; @name; end
来源：http://udv.cheryme.top

C#:   public string Greet() => Name;
来源：http://pvb.zhiwuduotai.top

[G05] 继承
来源：http://cbs.xinyue.icu

Py:   class Admin(User): pass
来源：http://hkj.c1oappe.top

PHP:  class Admin extends User {}
来源：http://xnm.kuanghao11.cn

JS:   class Admin extends User {}
来源：http://oax.cheryme.top

TS:   class Admin extends User {}
来源：http://eqs.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://aad.chenzaomai.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bbz.ivvv.top

Ruby: class Admin < User; end
来源：http://xnp.jqgufenzy.top

C#:   class Admin : User {}
来源：http://cru.xuetiantiany.cn

[G06] 重写方法
来源：http://pae.316326.xyz

Py:   def greet(self): return "admin"
来源：http://nqa.sysykeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://xuk.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://inb.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://fmm.c1oappe.top

Java: @Override String greet() { return "admin"; }
来源：http://who.fanxiaobao.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ftk.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://bkt.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://aza.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://tjp.shzxlz.cn

Py:   super().greet()
来源：http://kbd.pycfn.com

PHP:  parent::greet();
来源：http://evj.jyoumei.cn

JS:   super.greet();
来源：http://iqh.jyoumei.cn

TS:   super.greet();
来源：http://kqr.yvedp.cn

Java: super.greet();
来源：http://pqg.ctjpmb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wbp.zhixingplan.top

Ruby: super
来源：http://gma.andypj.xyz

C#:   base.Greet();
来源：http://kmn.ydjk.org.cn

[G08] 静态方法与属性
来源：http://lxn.nanxinkj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tva.jiagoushi.top

PHP:  public static function f() {}
来源：http://bku.jyoumei.cn

JS:   static f() {}
来源：http://wdz.sysykeji.top

TS:   static f(): void {}
来源：http://gwy.meibo888.top

Java: static void f() {}
来源：http://egm.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://agu.yanxiufei.cn

Ruby: def self.f; end
来源：http://hyx.jqgufenzy.top

C#:   public static void F() {}
来源：http://hzt.52xcode.cn

[G09] 接口 / 抽象类
来源：http://boj.aibaodan.cn

Py:   from abc import ABC, abstractmethod
来源：http://xsw.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://imm.sysykeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://blm.hfpthk.cn

TS:   interface Shape { area(): number; }
来源：http://wla.xinyue.icu


<!-- 参考信息 -->