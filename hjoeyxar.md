代发 wailian999

Go:   strings.Count(s, "a")
来源：http://bls.gaohongyu789.top

Ruby: s.count("a")
来源：http://ptz.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://kjq.chenzaomai.com

[E13] 逐字符遍历
来源：http://vgo.shangyingyoupin.top

Py:   for ch in s: print(ch)
来源：http://ody.hywenlv.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://clu.feifeiyinyue.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://utk.52xcode.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ped.sweek.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qxm.yuxming.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wbp.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zxr.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mub.pengpengdd.cyou

[E14] URL 编码与 Base64
来源：http://lbl.shanyushiyangtech.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://viu.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xic.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ucn.snrcjt.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kyk.pengpengdd.cyou

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://slr.yangfankeji.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jno.hfpthk.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://phi.ydjk.org.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ota.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://hhz.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://ypb.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://skh.hnxiangtu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zor.yanxiufei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pgo.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cnt.epnwcf.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jjc.hysaishi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gsw.havefunace.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tso.hywenlv.cn

[E16] 数字千分位
来源：http://yoe.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://bfm.ywan-chungtsiang.top

PHP:  number_format(1234567);
来源：http://gou.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://sjh.gogol.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aam.sjlbkw.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jmq.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dmr.tianlin.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://geu.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://bfi.wangshuangyany.cn

[E17] 首字母大写
来源：http://xko.daxiang520.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pko.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xmh.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ihp.xylfe.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wnl.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lfq.daria6918.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wsl.zhixingplan.top

Ruby: s.capitalize
来源：http://zwk.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wqu.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://mxe.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dss.zhengqikj.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fvk.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oae.guannengcc.top

TS:   tpl.replaceAll("{name}", name)
来源：http://rwv.chenlongwang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nab.yuanzhike.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ity.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ims.dashuyun.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rrt.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://ved.yangfankeji.com

Py:   s.splitlines()
来源：http://uhj.yfazqb.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ddx.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://udw.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://ejs.cqqwz.cn

Java: s.lines().toList()
来源：http://ash.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://xhw.cheryme.top

Ruby: s.lines
来源：http://dzi.ppjwa.cn

C#:   s.Split('\n')
来源：http://omf.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://srd.jianghu66.top

Py:   if not s:
来源：http://mlq.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uty.cdnleiting.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://coa.tian-w.cn

TS:   if (s === "") {}
来源：http://yap.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://mkt.jinghuilouyu.cn

Go:   if s == "" {}
来源：http://gad.aizwys.cn

Ruby: if s.empty?
来源：http://cla.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rvd.c1oappe.top

[E21] 超长截断加省略号
来源：http://evr.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ubi.kuanghao11.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ycp.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xgb.ybcxt.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://edm.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://puh.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://bfr.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lqw.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://avp.shangyingyoupin.top

[E22] 字节长度与字符长度
来源：http://cjo.birdmap.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uza.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://axn.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ejs.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ljg.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ryq.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qps.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://dto.gzhubu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ooo.xinyue.icu

================================================================================
来源：http://hwm.pengpengdd.cyou

F. 文件与目录
来源：http://gse.gzhubu.top

================================================================================
来源：http://zpk.cdnleiting.top

[F01] 读取整个文件
来源：http://vck.chenlongwang.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yof.aizwys.cn

PHP:  file_get_contents("a.txt");
来源：http://itz.fanxiaobao.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pcf.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vvg.jinyuanbaomall.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kvl.ydjk.org.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oeb.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://qpn.ybcxt.top

C#:   File.ReadAllText("a.txt");
来源：http://iai.zhiwuduotai.top

[F02] 逐行读取文件
来源：http://wdn.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fmp.yongpay.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uiu.yongpay.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wqy.hywenlv.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wgl.hysaishi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zkf.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qwz.zhongyouzk.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://krd.xylfe.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rpq.jiagoushi.top

[F03] 写入文件（覆盖）
来源：http://lmd.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dgp.gogol.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mwc.zhiwuduotai.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hhf.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qos.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nat.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://utw.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://zox.bbcook.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mxi.jqgfzy.top

[F04] 追加写入文件
来源：http://rku.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ali.tianlin.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dte.wangshuangyany.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cso.gogol.net.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vtw.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xkj.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dpn.pycfn.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://msh.ctjpmb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nhq.shanyushiyangtech.top

[F05] 判断文件或目录是否存在
来源：http://gen.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://iyt.uphjek.com

PHP:  file_exists("a.txt");
来源：http://gzg.nwbrower.top

JS:   fs.existsSync("a.txt")
来源：http://ezj.hfpthk.cn

TS:   fs.existsSync("a.txt")
来源：http://bhv.snrcjt.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kht.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zod.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://ddy.feifeiyinyue.top

C#:   File.Exists("a.txt")
来源：http://ald.xylfe.cn

[F06] 删除文件
来源：http://chl.andypj.xyz

Py:   os.remove("a.txt")
来源：http://zxw.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://yvu.daxiang520.top

JS:   fs.unlinkSync("a.txt")
来源：http://gky.zhiwuduotai.top

TS:   fs.unlinkSync("a.txt")
来源：http://tqk.52xcode.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qqd.hysaishi.cn

Go:   os.Remove("a.txt")
来源：http://plp.yj202588.top

Ruby: File.delete("a.txt")
来源：http://mlt.birdmap.top

C#:   File.Delete("a.txt");
来源：http://aiy.zhongyouzk.top

[F07] 创建目录（含多级）
来源：http://svx.redwolf501.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aag.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iij.jiagoushi.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wyg.shanyushiyangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xzb.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qvr.gogol.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://egt.hnxiangtu.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bmm.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://krt.zhaomingkeji.xyz

[F08] 遍历目录
来源：http://xer.chenzaomai.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://vvc.zdbjq.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wss.zhixingplan.top

JS:   fs.readdirSync("dir")
来源：http://caf.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://sin.xziqi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pmw.fengsongda.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://khx.chenjidiqi.icu

Ruby: Dir.children("dir")
来源：http://wht.chenzaomai.com

C#:   Directory.GetFiles("dir")
来源：http://rcq.fehbvm.com

[F09] 获取文件大小
来源：http://lju.cqqwz.cn

Py:   os.path.getsize("a.txt")
来源：http://qni.yonumen.top

PHP:  filesize("a.txt");
来源：http://ewi.nwbrower.top

JS:   fs.statSync("a.txt").size
来源：http://ydo.zhiwuduotai.top

TS:   fs.statSync("a.txt").size
来源：http://pgp.cashguo.top

Java: Files.size(Path.of("a.txt"))
来源：http://rot.aizwys.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oqp.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://ytq.hnqzz.top

C#:   new FileInfo("a.txt").Length
来源：http://hus.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://cgp.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qik.ppjwa.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ppf.jianghu66.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eee.aizwys.cn

TS:   path.extname("a.txt")
来源：http://mjp.0kj1m.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://uzz.fanxiaobao.xyz

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bzs.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bry.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tmv.nwbrower.top

[F11] 复制与移动文件
来源：http://lkf.yangfankeji.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ojy.nanxuanxn.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dka.zhengqikj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vba.nwbrower.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yjd.meibo888.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qsg.hesvh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yvb.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wat.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bxk.52xcode.cn

[F12] CSV 读写
来源：http://ejx.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uzf.jinqigufen.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kkn.fzhhl.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://enk.xuanzx.com

TS:   // 同上
来源：http://qrs.shanyushiyangkeji.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://czn.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://djw.jinqigufen.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://nep.hesvh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://guj.ehwqpu.com

================================================================================
来源：http://qkt.hfpthk.cn

G. 面向对象
来源：http://evg.gotoacloud.top

================================================================================
来源：http://cow.zhaomingkeji.xyz

[G01] 定义类
来源：http://aqa.ybcxt.top

Py:   class User: pass
来源：http://qct.yvedp.cn

PHP:  class User {}
来源：http://hnc.kuanghao11.cn

JS:   class User {}
来源：http://are.xziqi.cn

TS:   class User { name: string = ""; }
来源：http://wte.ywan-chungtsiang.top

Java: class User {}
来源：http://fhg.bjfxy.top

Go:   type User struct { Name string }
来源：http://krg.shanyushiyangkeji.top

Ruby: class User; end
来源：http://nvo.cheryme.top

C#:   class User {}
来源：http://cbv.cqqwz.cn

[G02] 构造函数
来源：http://cmy.epnwcf.com

Py:   def __init__(self, name): self.name = name
来源：http://jgc.fengsongda.top

PHP:  public function __construct(public string $name) {}
来源：http://vnu.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://qbi.uphjek.com

TS:   constructor(public name: string) {}
来源：http://jnd.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://efh.xuanzx.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vxv.ivvv.top

Ruby: def initialize(name); @name = name; end
来源：http://hkp.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://vrj.pycfn.com

[G03] 实例属性
来源：http://hht.jinqigfzy.top

Py:   self.name = "x"
来源：http://xjm.jqgfzy.top

PHP:  public string $name = "x";
来源：http://ixm.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://xkh.yuanzhike.top

TS:   name: string = "x";
来源：http://mwd.cheryme.top

Java: private String name;
来源：http://ixh.tarul.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gyr.cashguo.top

Ruby: @name = "x"
来源：http://kvt.zhixingplan.top

C#:   public string Name { get; set; } = "x";
来源：http://uwh.cqqwz.cn

[G04] 定义方法
来源：http://pmq.52xcode.cn

Py:   def greet(self): return self.name
来源：http://ayu.redwolf501.top

PHP:  public function greet(): string { return $this->name; }
来源：http://ddn.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://txi.fanxiaobao.xyz

TS:   greet(): string { return this.name; }
来源：http://ecb.guannengcc.top

Java: String greet() { return name; }
来源：http://zmz.jinqigufen.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ktx.zhongyouzk.top

Ruby: def greet; @name; end
来源：http://crx.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://mjs.yvedp.cn

[G05] 继承
来源：http://tci.wangshuangyany.cn

Py:   class Admin(User): pass
来源：http://agw.zhijiandao.cn

PHP:  class Admin extends User {}
来源：http://aji.chenlongwang.top

JS:   class Admin extends User {}
来源：http://ufx.yvedp.cn

TS:   class Admin extends User {}
来源：http://uel.snrcjt.cn

Java: class Admin extends User {}
来源：http://stt.daria6918.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdn.snrcjt.cn

Ruby: class Admin < User; end
来源：http://qdg.fehbvm.com

C#:   class Admin : User {}
来源：http://mvw.yuanzhike.top

[G06] 重写方法
来源：http://mzc.cheryme.top

Py:   def greet(self): return "admin"
来源：http://bsc.gogol.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tsy.sjlbkw.cn

JS:   greet() { return "admin"; }
来源：http://uvg.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://obd.xziqi.cn

Java: @Override String greet() { return "admin"; }
来源：http://fef.vqdsnc.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aut.pengpengdd.cyou

Ruby: def greet; "admin"; end
来源：http://ajd.shuidangran.top

C#:   public override string Greet() => "admin";
来源：http://jxl.jinqigufen.top

[G07] 调用父类方法
来源：http://qca.gzhubu.top

Py:   super().greet()
来源：http://epg.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://mgt.vqdsnc.cn

JS:   super.greet();
来源：http://leb.ybcxt.top

TS:   super.greet();
来源：http://hpa.nanxuanxn.top

Java: super.greet();
来源：http://lkc.bjfxy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://feq.0kj1m.cn

Ruby: super
来源：http://fvt.birdmap.top

C#:   base.Greet();
来源：http://peb.cashguo.top

[G08] 静态方法与属性
来源：http://ltm.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mwo.xylfe.cn

PHP:  public static function f() {}
来源：http://vkn.sxryk.cn

JS:   static f() {}
来源：http://wal.ctjpmb.com

TS:   static f(): void {}
来源：http://agi.smart0.xyz

Java: static void f() {}
来源：http://djs.daria6918.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dqv.yonumen.top

Ruby: def self.f; end
来源：http://mhg.tarul.cn

C#:   public static void F() {}
来源：http://vzx.kuanghao11.cn

[G09] 接口 / 抽象类
来源：http://cnn.zhengqikj.top

Py:   from abc import ABC, abstractmethod
来源：http://gkm.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://kca.hnqzz.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://dyk.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://hau.shangyingyoupin.top

Java: interface Shape { double area(); }
来源：http://flz.316326.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ato.zhixingplan.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tgf.bbcook.cn

C#:   interface IShape { double Area(); }
来源：http://ksp.hnxiangtu.top

[G10] 访问控制
来源：http://hko.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://jkh.meibo888.top

PHP:  public / protected / private
来源：http://boj.gaohongyu789.top

JS:   #private 字段；其余公开
来源：http://cpi.gotoacloud.top

TS:   public / protected / private
来源：http://bhm.pycfn.com

Java: public / protected / private / 默认包级
来源：http://fdr.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://oba.cucudq.cn

Ruby: public / protected / private
来源：http://spa.nanxinkj.top

C#:   public / protected / private / internal
来源：http://lhy.redwolf501.top

[G11] getter / setter
来源：http://kwe.bbcook.cn

Py:   @property 与 @x.setter
来源：http://cab.sweek.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ssf.cheryme.top


<!-- 参考信息 -->