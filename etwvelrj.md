代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lhp.gogol.net.cn

[E11] 反转字符串
来源：http://hpy.cashguo.top

Py:   s[::-1]
来源：http://yll.smart0.xyz

PHP:  strrev($s);
来源：http://fho.zhijiandao.cn

JS:   [...s].reverse().join("")
来源：http://xyr.nanxuanxn.top

TS:   [...s].reverse().join("")
来源：http://dfa.zhijiandao.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ivl.tarul.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://eug.birdmap.top

Ruby: s.reverse
来源：http://efm.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xoo.hesvh.cn

[E12] 统计某字符出现次数
来源：http://arn.9152youxi.cn

Py:   s.count("a")
来源：http://bog.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://wum.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://vau.ybcxt.top

TS:   s.split("a").length - 1
来源：http://uvm.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jxc.yongpay.top

Go:   strings.Count(s, "a")
来源：http://uey.jyoumei.cn

Ruby: s.count("a")
来源：http://jre.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://tgf.yongpay.top

[E13] 逐字符遍历
来源：http://blx.gogol.net.cn

Py:   for ch in s: print(ch)
来源：http://tqt.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dqn.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ltd.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://doz.fzhhl.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qjz.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zjc.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://etc.hnqzz.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gqe.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://xzd.dianchejie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dhx.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mmb.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vgx.cashguo.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oxf.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pdz.redwolf501.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jep.gaohongyu789.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jhq.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rmj.ctjpmb.com

[E15] HTML 转义 / 反转义
来源：http://ovh.xinyue.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://ypg.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://fhv.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tny.hesvh.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qko.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rzu.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tvx.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qcp.wangdashe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fsu.yvedp.cn

[E16] 数字千分位
来源：http://dob.jinqigfzy.top

Py:   f"{1234567:,}"
来源：http://xkg.zhijiandao.cn

PHP:  number_format(1234567);
来源：http://mac.mhx1999.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ezu.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ker.dianchejie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bdu.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gra.ywan-chungtsiang.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qqm.pycfn.com

C#:   1234567.ToString("N0")
来源：http://bms.nanxuanxn.top

[E17] 首字母大写
来源：http://caf.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dew.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ace.meibo888.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ovg.shzxlz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zfx.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qjw.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ysn.bjfxy.top

Ruby: s.capitalize
来源：http://gmm.yanxiufei.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bdm.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://tks.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fnf.ivvv.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jtc.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fxe.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cww.jlsjyb.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ctb.hesvh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ane.zhaomingkeji.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yiq.xuanzx.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rsw.meibo888.top

[E19] 多行文本按行拆分
来源：http://rwo.gogol.net.cn

Py:   s.splitlines()
来源：http://rkw.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://flm.bbcook.cn

JS:   s.split(/\r?\n/)
来源：http://xku.shangyingyoupin.top

TS:   s.split(/\r?\n/)
来源：http://sra.cashguo.top

Java: s.lines().toList()
来源：http://gom.ppjwa.cn

Go:   strings.Split(s, "\n")
来源：http://seg.zhijiandao.cn

Ruby: s.lines
来源：http://nyo.9152youxi.cn

C#:   s.Split('\n')
来源：http://sjw.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://sqi.yanxiufei.cn

Py:   if not s:
来源：http://ylv.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sfl.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://odd.jiagoushi.top

TS:   if (s === "") {}
来源：http://sro.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://bjq.vehdjk.com

Go:   if s == "" {}
来源：http://tte.fzhhl.top

Ruby: if s.empty?
来源：http://bsl.zhaomingkeji.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gzf.fktsv.cn

[E21] 超长截断加省略号
来源：http://aww.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ahv.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nrq.0kj1m.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://elc.sjlbkw.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qnz.tarul.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nhd.kuanghao11.cn

Go:   // 按 rune 判断长度后截断
来源：http://ptn.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kon.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uoi.daxiang520.top

[E22] 字节长度与字符长度
来源：http://vli.chenzaomai.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qga.cheryme.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fbo.zhiwuduotai.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ghk.tian-w.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://egi.havefunace.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bsu.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eco.ydzc1.top

Ruby: s.bytesize;  s.length
来源：http://duq.aibaodan.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cgr.jinghuilouyu.cn

================================================================================
来源：http://yre.yj20258.top

F. 文件与目录
来源：http://nxb.xuetiantiany.cn

================================================================================
来源：http://rly.aibaodan.cn

[F01] 读取整个文件
来源：http://elk.yuxming.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://een.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://ign.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gqh.guannengcc.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gmm.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dgn.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pdp.shanyushiyangtech.top

Ruby: File.read("a.txt")
来源：http://mwz.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://uzk.meibo888.top

[F02] 逐行读取文件
来源：http://nqa.ctjpmb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oqi.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wda.mhx1999.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dxl.nanxinkj.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rrq.fehbvm.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qfu.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mwc.chenlongwang.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rbz.dianchejie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tkd.jlsjyb.cn

[F03] 写入文件（覆盖）
来源：http://rpw.hammf.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kpr.hfpthk.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hgr.nwbrower.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vqr.shanyushiyangtech.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfz.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hmj.shuidangran.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://srd.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://htt.jinqigfzy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hpa.chenlongwang.top

[F04] 追加写入文件
来源：http://hzg.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jzh.yongpay.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ndx.sxryk.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tsj.hongshengwenyu.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xnm.sysykeji.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://udk.wangshuangyany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vgj.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://plg.pycfn.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qeq.shuidangran.top

[F05] 判断文件或目录是否存在
来源：http://hjr.yfazqb.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xqd.bjfxy.top

PHP:  file_exists("a.txt");
来源：http://rth.zhengqikj.top

JS:   fs.existsSync("a.txt")
来源：http://jhr.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://kds.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://piw.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jyi.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://eym.xuetiantiany.cn

C#:   File.Exists("a.txt")
来源：http://ycs.zhijiandao.cn

[F06] 删除文件
来源：http://lma.sjlbkw.cn

Py:   os.remove("a.txt")
来源：http://smc.52xcode.cn

PHP:  unlink("a.txt");
来源：http://zwc.0kj1m.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hmn.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ifn.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nhe.yj20258888.top

Go:   os.Remove("a.txt")
来源：http://ufc.fehbvm.com

Ruby: File.delete("a.txt")
来源：http://oah.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://bhn.cqqwz.cn

[F07] 创建目录（含多级）
来源：http://zwo.xylfe.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dfl.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oke.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lrl.yfazqb.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://czo.ivvv.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aam.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hgu.yj20258888.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mjb.zhengqikj.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://voh.gzhubu.top

[F08] 遍历目录
来源：http://uid.sxryk.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xmk.yanxiufei.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oxg.dianchejie.cn

JS:   fs.readdirSync("dir")
来源：http://zkm.guowangkeji.top

TS:   fs.readdirSync("dir")
来源：http://mwu.hesvh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lhd.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lhz.meibo888.top

Ruby: Dir.children("dir")
来源：http://dhp.52xcode.cn

C#:   Directory.GetFiles("dir")
来源：http://dkx.bbcook.cn

[F09] 获取文件大小
来源：http://xpg.shanyushiyangkeji.top

Py:   os.path.getsize("a.txt")
来源：http://kkm.daria6918.cn

PHP:  filesize("a.txt");
来源：http://tck.jqgfzy.top

JS:   fs.statSync("a.txt").size
来源：http://qvk.wangshuangyany.cn

TS:   fs.statSync("a.txt").size
来源：http://mwg.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://olb.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yma.fktsv.cn

Ruby: File.size("a.txt")
来源：http://hvk.daria6918.cn

C#:   new FileInfo("a.txt").Length
来源：http://efw.ctjpmb.com

[F10] 取文件扩展名 / 文件名
来源：http://nkz.wangshuangyany.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ims.bjfxy.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://esk.0kj1m.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rox.epnwcf.com

TS:   path.extname("a.txt")
来源：http://jsn.snrcjt.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zwk.ybcxt.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ugx.mhx1999.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://okm.sjlbkw.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://egd.ehwqpu.com

[F11] 复制与移动文件
来源：http://etw.zycfv.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cmx.feifeiyinyue.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gjd.cucudq.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://beg.fzhhl.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iwm.zhengqikj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zto.jinqigufen.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hnj.hcnkem.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lfn.zhijiandao.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cff.tianlin.xyz

[F12] CSV 读写
来源：http://yrx.ydzc1.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fdj.yangfankeji.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ypt.chenlongwang.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lup.guowangkeji.top

TS:   // 同上
来源：http://cvp.jianghu66.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hco.chenzaomai.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://msh.dashuyun.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ufm.yfazqb.com

C#:   // 无内置：用 CsvHelper 库
来源：http://qtl.ivvv.top

================================================================================
来源：http://adb.sysykeji.top

G. 面向对象
来源：http://ozy.yonumen.top

================================================================================
来源：http://bik.epnwcf.com

[G01] 定义类
来源：http://gqz.zhaomingkeji.xyz

Py:   class User: pass
来源：http://ccs.zdbjq.cn

PHP:  class User {}
来源：http://bsm.fehbvm.com

JS:   class User {}
来源：http://jbk.tanke756.top

TS:   class User { name: string = ""; }
来源：http://mzf.fehbvm.com

Java: class User {}
来源：http://qnj.daxiang520.top

Go:   type User struct { Name string }
来源：http://qtm.shuidangran.top

Ruby: class User; end
来源：http://sre.zhengqikj.top

C#:   class User {}
来源：http://hik.cashguo.top

[G02] 构造函数
来源：http://mdi.yvedp.cn

Py:   def __init__(self, name): self.name = name
来源：http://ubx.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://hmt.jqgufenzy.top

JS:   constructor(name) { this.name = name; }
来源：http://bng.shanyushiyangkeji.top

TS:   constructor(public name: string) {}
来源：http://eip.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://ooa.yanxiufei.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jkd.jinyuanbaomall.cn

Ruby: def initialize(name); @name = name; end
来源：http://ouz.0kj1m.cn

C#:   public User(string name) { Name = name; }
来源：http://fkw.nwbrower.top

[G03] 实例属性
来源：http://jnm.epnwcf.com

Py:   self.name = "x"
来源：http://djl.zdqjudy.top

PHP:  public string $name = "x";
来源：http://tpj.hysaishi.cn

JS:   this.name = "x";
来源：http://hil.uphjek.com

TS:   name: string = "x";
来源：http://cck.feifeiyinyue.top

Java: private String name;
来源：http://aop.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://byh.sufxvd.cn

Ruby: @name = "x"
来源：http://koo.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://tzd.jlsjyb.cn

[G04] 定义方法
来源：http://kwy.fktsv.cn

Py:   def greet(self): return self.name
来源：http://wgr.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://eig.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://fyw.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://eyt.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://axr.ehwqpu.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://pjw.sysykeji.top

Ruby: def greet; @name; end
来源：http://kgu.yfazqb.com

C#:   public string Greet() => Name;
来源：http://wtb.sjlbkw.cn

[G05] 继承
来源：http://ozm.smart0.xyz

Py:   class Admin(User): pass
来源：http://lfk.fzhhl.top

PHP:  class Admin extends User {}
来源：http://igc.zycfv.cn

JS:   class Admin extends User {}
来源：http://qom.gogol.net.cn

TS:   class Admin extends User {}
来源：http://klb.tianlin.xyz

Java: class Admin extends User {}
来源：http://ylj.wangshuangyany.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bmb.fehbvm.com

Ruby: class Admin < User; end
来源：http://odi.hywenlv.cn

C#:   class Admin : User {}
来源：http://ziw.uphjek.com

[G06] 重写方法
来源：http://wrh.zdqjudy.top

Py:   def greet(self): return "admin"
来源：http://wys.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wjd.yongpay.top

JS:   greet() { return "admin"; }
来源：http://awq.yuanzhike.top

TS:   greet(): string { return "admin"; }
来源：http://aro.sysykeji.top

Java: @Override String greet() { return "admin"; }
来源：http://jih.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tov.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://lfc.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://kjv.redwolf501.top

[G07] 调用父类方法
来源：http://sbp.hywenlv.cn

Py:   super().greet()
来源：http://llx.cqqwz.cn

PHP:  parent::greet();
来源：http://noc.0kj1m.cn

JS:   super.greet();
来源：http://pbv.ywan-chungtsiang.top

TS:   super.greet();
来源：http://kzq.xziqi.cn

Java: super.greet();
来源：http://lte.zhongyouzk.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qwj.yfazqb.com

Ruby: super
来源：http://twd.ywan-chungtsiang.top

C#:   base.Greet();
来源：http://sxa.ydzc1.top

[G08] 静态方法与属性
来源：http://yva.xinyue.icu

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://emz.fehbvm.com

PHP:  public static function f() {}
来源：http://boi.tian-w.cn

JS:   static f() {}
来源：http://rfr.chenzaomai.com

TS:   static f(): void {}
来源：http://rjy.sxryk.cn

Java: static void f() {}
来源：http://bbb.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lhz.zhiwuduotai.top

Ruby: def self.f; end
来源：http://mxs.jinghuilouyu.cn

C#:   public static void F() {}
来源：http://rtw.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://fgr.ywan-chungtsiang.top

Py:   from abc import ABC, abstractmethod
来源：http://uca.svipenyu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qtj.xinyue.icu

JS:   // 无接口：靠约定或 JSDoc
来源：http://eos.shanyushiyangkeji.top

TS:   interface Shape { area(): number; }
来源：http://qqj.hnxiangtu.top


<!-- 参考信息 -->