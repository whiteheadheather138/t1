代发 wailian999

Ruby: s.reverse
来源：http://mxu.quarkkingdee.top

C#:   new string(s.Reverse().ToArray())
来源：http://yyl.yuanzhike.top

[E12] 统计某字符出现次数
来源：http://oit.guannengcc.top

Py:   s.count("a")
来源：http://ibq.fktsv.cn

PHP:  substr_count($s, "a");
来源：http://nlx.jinqigufen.top

JS:   s.split("a").length - 1
来源：http://zcu.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://hzm.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rxb.yj20258.top

Go:   strings.Count(s, "a")
来源：http://rsp.pengpengdd.cyou

Ruby: s.count("a")
来源：http://crl.52xcode.cn

C#:   s.Count(c => c == 'a')
来源：http://szv.ppjwa.cn

[E13] 逐字符遍历
来源：http://dla.hysaishi.cn

Py:   for ch in s: print(ch)
来源：http://wtq.ctjpmb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tsl.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://loa.smart0.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://tvs.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vpm.tarul.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nhf.haohaochexian.top

Ruby: s.each_char { |ch| puts ch }
来源：http://cxx.gaohongyu789.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ixd.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://dxs.shangyingyoupin.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pkr.jinqigfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ldq.zhiwuduotai.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://diw.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vwl.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zgs.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://owe.haohaochexian.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bxi.guannengcc.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fqc.hongshengwenyu.top

[E15] HTML 转义 / 反转义
来源：http://fdc.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://hpj.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://erw.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zuh.52xcode.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qyj.yj20258888.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://obg.iojbl.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjj.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rlk.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ywe.uphjek.com

[E16] 数字千分位
来源：http://aje.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://ssy.cdnleiting.top

PHP:  number_format(1234567);
来源：http://dfl.gogol.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://akk.bjfxy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jzr.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zxc.316326.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jjf.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mvj.zhixingplan.top

C#:   1234567.ToString("N0")
来源：http://glq.0kj1m.cn

[E17] 首字母大写
来源：http://bnb.jqgfzy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qwp.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://hqj.yanxiufei.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://trk.yueranfly.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ewu.hfpthk.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mez.chenzaomai.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ioh.ppjwa.cn

Ruby: s.capitalize
来源：http://rds.shuidangran.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xdl.fehbvm.com

[E18] 模板占位符替换
来源：http://ibf.chenlongwang.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://srk.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fex.mhx1999.top

JS:   tpl.replaceAll("{name}", name)
来源：http://tfe.nanxuanxn.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pmz.vqdsnc.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xio.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bns.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sof.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fqs.epnwcf.com

[E19] 多行文本按行拆分
来源：http://nqk.hesvh.cn

Py:   s.splitlines()
来源：http://ttq.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://que.svipenyu.cn

JS:   s.split(/\r?\n/)
来源：http://wvh.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://btk.cucudq.cn

Java: s.lines().toList()
来源：http://okr.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://ojk.ydzc1.top

Ruby: s.lines
来源：http://kcl.xinyue.icu

C#:   s.Split('\n')
来源：http://rbr.nanxuanxn.top

[E20] 判断字符串是否为空
来源：http://xio.snrcjt.cn

Py:   if not s:
来源：http://pfp.yonumen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kqw.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rvz.andypj.xyz

TS:   if (s === "") {}
来源：http://eqw.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://moj.dashuyun.cn

Go:   if s == "" {}
来源：http://dkg.zycfv.cn

Ruby: if s.empty?
来源：http://pdc.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qvs.tanke756.top

[E21] 超长截断加省略号
来源：http://gzl.sysykeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vkn.ywan-chungtsiang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lbg.sweek.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://igm.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jut.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xna.hfpthk.cn

Go:   // 按 rune 判断长度后截断
来源：http://ihg.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tcn.jiagoushi.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nep.kuanghao11.cn

[E22] 字节长度与字符长度
来源：http://sjg.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvn.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bsm.sweek.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dit.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iig.shuidangran.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wqo.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pmu.jyoumei.cn

Ruby: s.bytesize;  s.length
来源：http://brv.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kbz.hnqzz.top

================================================================================
来源：http://vxq.yvedp.cn

F. 文件与目录
来源：http://yxl.kuanghao11.cn

================================================================================
来源：http://nvk.kuanghao11.cn

[F01] 读取整个文件
来源：http://ind.jinqigfzy.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lia.nwbrower.top

PHP:  file_get_contents("a.txt");
来源：http://xpx.hysaishi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gqs.9152youxi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bpk.bjfxy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://nof.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://smt.andypj.xyz

Ruby: File.read("a.txt")
来源：http://uux.shanyushiyangtech.top

C#:   File.ReadAllText("a.txt");
来源：http://ger.yuanzhike.top

[F02] 逐行读取文件
来源：http://bkx.chenzaomai.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pqx.hysaishi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hja.birdmap.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vue.jqgufenzy.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mwz.tanke756.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ljq.yvedp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ylh.vqdsnc.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vjh.jinqigfzy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tna.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://xvq.shangyingyoupin.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hyp.tian-w.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uiq.fengsongda.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rjc.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbq.dianchejie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zqk.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ixa.ybcxt.top

Ruby: File.write("a.txt", "hi")
来源：http://xcz.sxryk.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qwx.zhongyouzk.top

[F04] 追加写入文件
来源：http://ugd.ydjk.org.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vbi.andypj.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cfc.feifeiyinyue.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hiz.cheryme.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://urh.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://squ.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yzs.guowangkeji.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wqe.hysaishi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qqb.bbcook.cn

[F05] 判断文件或目录是否存在
来源：http://hwl.pengpengdd.cyou

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://exm.tarul.cn

PHP:  file_exists("a.txt");
来源：http://nmt.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://vjz.zhijiandao.cn

TS:   fs.existsSync("a.txt")
来源：http://uri.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ykr.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://why.52xcode.cn

Ruby: File.exist?("a.txt")
来源：http://wuz.vehdjk.com

C#:   File.Exists("a.txt")
来源：http://tvz.hesvh.cn

[F06] 删除文件
来源：http://gte.yanxiufei.cn

Py:   os.remove("a.txt")
来源：http://lxg.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://glz.nanxinkj.top

JS:   fs.unlinkSync("a.txt")
来源：http://lmv.bbcook.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qop.sxryk.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dll.yonumen.top

Go:   os.Remove("a.txt")
来源：http://joh.chenlongwang.top

Ruby: File.delete("a.txt")
来源：http://mgp.zhengqikj.top

C#:   File.Delete("a.txt");
来源：http://xvi.yj20258.top

[F07] 创建目录（含多级）
来源：http://ssq.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cnt.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://yeo.jinyuanbaomall.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://peg.ydjk.org.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://afa.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pdb.shangyingyoupin.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kzm.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://naf.sxryk.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://irt.yvedp.cn

[F08] 遍历目录
来源：http://wfw.jinyuanbaomall.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xus.xuetiantiany.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qos.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://nkc.epnwcf.com

TS:   fs.readdirSync("dir")
来源：http://hxm.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wjm.zhaomingkeji.xyz

Go:   entries, _ := os.ReadDir("dir")
来源：http://cng.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://bnf.gaohongyu789.top

C#:   Directory.GetFiles("dir")
来源：http://zzx.hesvh.cn

[F09] 获取文件大小
来源：http://upl.gotoacloud.top

Py:   os.path.getsize("a.txt")
来源：http://ire.hfpthk.cn

PHP:  filesize("a.txt");
来源：http://jni.quarkkingdee.top

JS:   fs.statSync("a.txt").size
来源：http://rmd.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://gzp.xingfuxueyuan.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://dtm.snrcjt.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://srf.xziqi.cn

Ruby: File.size("a.txt")
来源：http://tce.feifeiyinyue.top

C#:   new FileInfo("a.txt").Length
来源：http://lmb.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://xxi.wangdashe.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gcz.c1oappe.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gyo.316326.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cyk.jinyuanbaomall.cn

TS:   path.extname("a.txt")
来源：http://utb.zhaomingkeji.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zvb.ctjpmb.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pjn.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nrq.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pqt.ehwqpu.com

[F11] 复制与移动文件
来源：http://beo.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wel.cucudq.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wag.chenzaomai.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zuy.snrcjt.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rbk.jinqigufen.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fvy.yongpay.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dtv.ybcxt.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lgy.chenjidiqi.icu

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lup.gotoacloud.top

[F12] CSV 读写
来源：http://kgs.xinyue.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://emv.xziqi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ant.52xcode.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egg.ywan-chungtsiang.top

TS:   // 同上
来源：http://tsn.chenjidiqi.icu

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lhq.tianlin.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dxp.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ncy.jinqigufen.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xuj.pengpengdd.cyou

================================================================================
来源：http://yzo.tarul.cn

G. 面向对象
来源：http://ays.316326.xyz

================================================================================
来源：http://ipw.epnwcf.com

[G01] 定义类
来源：http://iry.xziqi.cn

Py:   class User: pass
来源：http://xdw.ppjwa.cn

PHP:  class User {}
来源：http://ptk.yongpay.top

JS:   class User {}
来源：http://iho.dianchejie.cn

TS:   class User { name: string = ""; }
来源：http://nnh.yonumen.top

Java: class User {}
来源：http://qsc.0kj1m.cn

Go:   type User struct { Name string }
来源：http://vhw.vqdsnc.cn

Ruby: class User; end
来源：http://tai.guannengcc.top

C#:   class User {}
来源：http://clf.wangshuangyany.cn

[G02] 构造函数
来源：http://fni.iojbl.cn

Py:   def __init__(self, name): self.name = name
来源：http://bgs.gaohongyu789.top

PHP:  public function __construct(public string $name) {}
来源：http://yau.nwbrower.top

JS:   constructor(name) { this.name = name; }
来源：http://kql.chenjidiqi.icu

TS:   constructor(public name: string) {}
来源：http://oev.tanke756.top

Java: User(String name) { this.name = name; }
来源：http://cox.shuidangran.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pyv.xziqi.cn

Ruby: def initialize(name); @name = name; end
来源：http://mzl.hesvh.cn

C#:   public User(string name) { Name = name; }
来源：http://gaa.shuidangran.top

[G03] 实例属性
来源：http://ryn.sysykeji.top

Py:   self.name = "x"
来源：http://rur.hywenlv.cn

PHP:  public string $name = "x";
来源：http://hoa.jinqigfzy.top

JS:   this.name = "x";
来源：http://nrg.yueranfly.top

TS:   name: string = "x";
来源：http://cde.ydjk.org.cn

Java: private String name;
来源：http://jhv.daxiang520.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bra.jinghuilouyu.cn

Ruby: @name = "x"
来源：http://ajb.guowangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://viz.cqqwz.cn

[G04] 定义方法
来源：http://bvp.tian-w.cn

Py:   def greet(self): return self.name
来源：http://jsi.chenlongwang.top

PHP:  public function greet(): string { return $this->name; }
来源：http://abq.jianghu66.top

JS:   greet() { return this.name; }
来源：http://hdf.tianlin.xyz

TS:   greet(): string { return this.name; }
来源：http://iiz.haohaochexian.top

Java: String greet() { return name; }
来源：http://mhf.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ysh.jyoumei.cn

Ruby: def greet; @name; end
来源：http://pzv.fengsongda.top

C#:   public string Greet() => Name;
来源：http://hhw.zdqjudy.top

[G05] 继承
来源：http://rjf.jiagoushi.top

Py:   class Admin(User): pass
来源：http://xlf.xinyue.icu

PHP:  class Admin extends User {}
来源：http://onu.cqqwz.cn

JS:   class Admin extends User {}
来源：http://mbz.jqgufenzy.top

TS:   class Admin extends User {}
来源：http://ews.fktsv.cn

Java: class Admin extends User {}
来源：http://tom.smart0.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pgx.ppjwa.cn

Ruby: class Admin < User; end
来源：http://jap.xingfuxueyuan.xyz

C#:   class Admin : User {}
来源：http://fff.fehbvm.com

[G06] 重写方法
来源：http://tdj.yj20258.top

Py:   def greet(self): return "admin"
来源：http://nib.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dzd.yj202588.top

JS:   greet() { return "admin"; }
来源：http://ogr.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://zws.kuanghao11.cn

Java: @Override String greet() { return "admin"; }
来源：http://uzr.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nvk.vehdjk.com

Ruby: def greet; "admin"; end
来源：http://ghi.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://xxl.jqgufenzy.top

[G07] 调用父类方法
来源：http://cpj.hnxiangtu.top

Py:   super().greet()
来源：http://dsi.yuxming.cn

PHP:  parent::greet();
来源：http://kfk.epnwcf.com

JS:   super.greet();
来源：http://yzw.dashuyun.cn

TS:   super.greet();
来源：http://pka.xinyue.icu

Java: super.greet();
来源：http://wzj.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ybf.wangdashe.top

Ruby: super
来源：http://xkk.jinqigfzy.top

C#:   base.Greet();
来源：http://jkb.guannengcc.top

[G08] 静态方法与属性
来源：http://owy.nwbrower.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://khk.hesvh.cn

PHP:  public static function f() {}
来源：http://dcw.sweek.top

JS:   static f() {}
来源：http://gwz.yj202588.top

TS:   static f(): void {}
来源：http://czh.sweek.top

Java: static void f() {}
来源：http://cqx.gogol.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mze.redwolf501.top

Ruby: def self.f; end
来源：http://pja.yueranfly.top

C#:   public static void F() {}
来源：http://aro.jyoumei.cn

[G09] 接口 / 抽象类
来源：http://iob.sufxvd.cn

Py:   from abc import ABC, abstractmethod
来源：http://pqq.jqgfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://sjj.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tyr.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://zby.ivvv.top

Java: interface Shape { double area(); }
来源：http://abs.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://uhs.pycfn.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fin.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://fob.chenzaomai.com

[G10] 访问控制
来源：http://txm.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://aph.snrcjt.cn

PHP:  public / protected / private
来源：http://cws.hammf.cn

JS:   #private 字段；其余公开
来源：http://suv.feifeiyinyue.top


<!-- 参考信息 -->