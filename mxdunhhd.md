代发 wailian999

PHP:  substr_count($s, "a");
来源：http://ryd.fengsongda.top

JS:   s.split("a").length - 1
来源：http://gqs.epnwcf.com

TS:   s.split("a").length - 1
来源：http://wpe.daria6918.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://edj.sysykeji.top

Go:   strings.Count(s, "a")
来源：http://lhm.jiagoushi.top

Ruby: s.count("a")
来源：http://gib.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://sne.fzhhl.top

[E13] 逐字符遍历
来源：http://jzg.52xcode.cn

Py:   for ch in s: print(ch)
来源：http://qtj.chenjidiqi.icu

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://oya.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hxq.zhengqikj.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qsr.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://utm.jyoumei.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pnp.xziqi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ljz.fengsongda.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://auc.nwbrower.top

[E14] URL 编码与 Base64
来源：http://vwk.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rqd.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lqd.quarkkingdee.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ric.dianchejie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pgu.kuanghao11.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wig.fktsv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gjk.ivvv.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gbr.zhijiandao.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://spl.fehbvm.com

[E15] HTML 转义 / 反转义
来源：http://xch.jqgufenzy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://uoq.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://par.svipenyu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kfa.fzhhl.top

TS:   // 同上，务必做 XSS 过滤
来源：http://wkt.jlsjyb.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ccf.jiagoushi.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oww.yfazqb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xgm.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gjo.cucudq.cn

[E16] 数字千分位
来源：http://jdw.svipenyu.cn

Py:   f"{1234567:,}"
来源：http://nhp.zdbjq.cn

PHP:  number_format(1234567);
来源：http://jbb.zhixingplan.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pgc.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://gxe.xingfuxueyuan.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kds.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qvw.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yuf.jqgufenzy.top

C#:   1234567.ToString("N0")
来源：http://cws.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://coo.tarul.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nmn.sufxvd.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gsj.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qyh.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zdj.jianghu66.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ykk.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lra.9152youxi.cn

Ruby: s.capitalize
来源：http://vmo.daxiang520.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hgn.uphjek.com

[E18] 模板占位符替换
来源：http://skz.yuanzhike.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://iwf.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gps.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://apq.bjfxy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vvf.shanyushiyangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ohn.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iph.birdmap.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rbq.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tsq.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://wlq.yuxming.cn

Py:   s.splitlines()
来源：http://iao.dashuyun.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uim.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://hig.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://rua.shanyushiyangtech.top

Java: s.lines().toList()
来源：http://oar.dashuyun.cn

Go:   strings.Split(s, "\n")
来源：http://bkw.yvedp.cn

Ruby: s.lines
来源：http://bre.shangyingyoupin.top

C#:   s.Split('\n')
来源：http://eoq.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://aob.yangfankeji.com

Py:   if not s:
来源：http://kqa.jinqigufen.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mbf.hfpthk.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yuw.0kj1m.cn

TS:   if (s === "") {}
来源：http://gxr.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://rkf.aibaodan.cn

Go:   if s == "" {}
来源：http://xpo.gotoacloud.top

Ruby: if s.empty?
来源：http://zdu.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xwv.daxiang520.top

[E21] 超长截断加省略号
来源：http://edf.chenjidiqi.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kbw.vehdjk.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://odz.yongpay.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nbo.andypj.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vow.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tcb.sysykeji.top

Go:   // 按 rune 判断长度后截断
来源：http://fhv.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jme.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dmw.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://juy.jinyuanbaomall.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yjn.mhx1999.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wxc.wangshuangyany.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qfr.hongshengwenyu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fci.xuanzx.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eug.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jql.guowangkeji.top

Ruby: s.bytesize;  s.length
来源：http://atx.yueranfly.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ihs.birdmap.top

================================================================================
来源：http://ecz.shuidangran.top

F. 文件与目录
来源：http://zxy.haohaochexian.top

================================================================================
来源：http://dkc.cdnleiting.top

[F01] 读取整个文件
来源：http://eug.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vza.jyoumei.cn

PHP:  file_get_contents("a.txt");
来源：http://zxn.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rnj.ywan-chungtsiang.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ugf.xuetiantiany.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jcp.zhixingplan.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://adp.ybcxt.top

Ruby: File.read("a.txt")
来源：http://fvd.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://acz.meibo888.top

[F02] 逐行读取文件
来源：http://xkf.xziqi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fsr.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://riz.tanke756.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qkp.hfpthk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ydn.cqqwz.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bbe.hnxiangtu.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zbk.hnxiangtu.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ice.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dth.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://ikd.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://iuk.cqqwz.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nvd.redwolf501.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://huj.andypj.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://psc.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://msz.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://woz.jinqigufen.top

Ruby: File.write("a.txt", "hi")
来源：http://iwz.fzhhl.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uet.nanxinkj.top

[F04] 追加写入文件
来源：http://yyy.sufxvd.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://glb.ybcxt.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mzs.ctjpmb.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zft.hfpthk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://okc.zycfv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cni.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iws.kuanghao11.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cqf.cucudq.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xjd.yangfankeji.com

[F05] 判断文件或目录是否存在
来源：http://awp.cdnleiting.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jmp.yj202588.top

PHP:  file_exists("a.txt");
来源：http://qbs.xziqi.cn

JS:   fs.existsSync("a.txt")
来源：http://zkd.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://vbq.jqgfzy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tbh.yuanzhike.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bgp.shanyushiyangtech.top

Ruby: File.exist?("a.txt")
来源：http://lyo.ybcxt.top

C#:   File.Exists("a.txt")
来源：http://rdm.fengsongda.top

[F06] 删除文件
来源：http://yxh.cdnleiting.top

Py:   os.remove("a.txt")
来源：http://zpu.ctjpmb.com

PHP:  unlink("a.txt");
来源：http://bqm.jlsjyb.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jfk.zdbjq.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bit.redwolf501.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qoi.pycfn.com

Go:   os.Remove("a.txt")
来源：http://odd.nanxinkj.top

Ruby: File.delete("a.txt")
来源：http://wjz.shanyushiyangtech.top

C#:   File.Delete("a.txt");
来源：http://ztr.nwbrower.top

[F07] 创建目录（含多级）
来源：http://jjq.zhaomingkeji.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hfk.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://msj.yj202588.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ztr.hesvh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgt.guowangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qct.svipenyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://awh.zhixingplan.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dwo.zdqjudy.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hph.wangshuangyany.cn

[F08] 遍历目录
来源：http://jtt.ppjwa.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://iax.pengpengdd.cyou

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lfj.hnxiangtu.top

JS:   fs.readdirSync("dir")
来源：http://plf.daxiang520.top

TS:   fs.readdirSync("dir")
来源：http://fou.quarkkingdee.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kad.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kis.zhongyouzk.top

Ruby: Dir.children("dir")
来源：http://axj.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://dip.mhx1999.top

[F09] 获取文件大小
来源：http://xvz.jinqigufen.top

Py:   os.path.getsize("a.txt")
来源：http://mgq.zdqjudy.top

PHP:  filesize("a.txt");
来源：http://qet.zdbjq.cn

JS:   fs.statSync("a.txt").size
来源：http://onr.jianghu66.top

TS:   fs.statSync("a.txt").size
来源：http://cle.ehwqpu.com

Java: Files.size(Path.of("a.txt"))
来源：http://gdz.shangyingyoupin.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kya.yanxiufei.cn

Ruby: File.size("a.txt")
来源：http://nfq.cqqwz.cn

C#:   new FileInfo("a.txt").Length
来源：http://ziu.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://pdg.hesvh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ykb.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xqd.aibaodan.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://noh.guannengcc.top

TS:   path.extname("a.txt")
来源：http://sad.52xcode.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sjc.chenjidiqi.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lcn.zhiwuduotai.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jlv.yj202588.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gtj.zhaomingkeji.xyz

[F11] 复制与移动文件
来源：http://mgy.daxiang520.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aej.bjfxy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://urr.tarul.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yfh.wangshuangyany.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mgm.gogol.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xsb.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kbo.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bfa.sxryk.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vap.chenjidiqi.icu

[F12] CSV 读写
来源：http://dzo.chenjidiqi.icu

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lxk.zhengqikj.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://arj.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kut.cucudq.cn

TS:   // 同上
来源：http://mlt.jinqigfzy.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zgt.wangshuangyany.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tut.xinyue.icu

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gmr.zhongyouzk.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sad.tianlin.xyz

================================================================================
来源：http://ghn.yonumen.top

G. 面向对象
来源：http://juo.quarkkingdee.top

================================================================================
来源：http://uql.wangdashe.top

[G01] 定义类
来源：http://adq.tianlin.xyz

Py:   class User: pass
来源：http://enk.fanxiaobao.xyz

PHP:  class User {}
来源：http://tmz.zhaomingkeji.xyz

JS:   class User {}
来源：http://xbt.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://itw.quarkkingdee.top

Java: class User {}
来源：http://mpv.hywenlv.cn

Go:   type User struct { Name string }
来源：http://skp.pengpengdd.cyou

Ruby: class User; end
来源：http://aym.pycfn.com

C#:   class User {}
来源：http://hoo.shuidangran.top

[G02] 构造函数
来源：http://ahw.vqdsnc.cn

Py:   def __init__(self, name): self.name = name
来源：http://jgm.cheryme.top

PHP:  public function __construct(public string $name) {}
来源：http://wdi.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://vmy.zdbjq.cn

TS:   constructor(public name: string) {}
来源：http://tkx.sweek.top

Java: User(String name) { this.name = name; }
来源：http://ajs.sysykeji.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dxw.zhongyouzk.top

Ruby: def initialize(name); @name = name; end
来源：http://acy.dashuyun.cn

C#:   public User(string name) { Name = name; }
来源：http://dwf.zhiwuduotai.top

[G03] 实例属性
来源：http://hdb.jinghuilouyu.cn

Py:   self.name = "x"
来源：http://kwh.ppjwa.cn

PHP:  public string $name = "x";
来源：http://zyw.mhx1999.top

JS:   this.name = "x";
来源：http://anp.ivvv.top

TS:   name: string = "x";
来源：http://hue.uphjek.com

Java: private String name;
来源：http://olo.kuanghao11.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wvj.fehbvm.com

Ruby: @name = "x"
来源：http://ses.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://kbk.yonumen.top

[G04] 定义方法
来源：http://atn.gaohongyu789.top

Py:   def greet(self): return self.name
来源：http://skn.yueranfly.top

PHP:  public function greet(): string { return $this->name; }
来源：http://kds.ivvv.top

JS:   greet() { return this.name; }
来源：http://xgz.uphjek.com

TS:   greet(): string { return this.name; }
来源：http://hvi.cucudq.cn

Java: String greet() { return name; }
来源：http://sww.birdmap.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pls.smart0.xyz

Ruby: def greet; @name; end
来源：http://dig.sysykeji.top

C#:   public string Greet() => Name;
来源：http://snz.shanyushiyangtech.top

[G05] 继承
来源：http://qkf.shuidangran.top

Py:   class Admin(User): pass
来源：http://qwv.mhx1999.top

PHP:  class Admin extends User {}
来源：http://ttp.redwolf501.top

JS:   class Admin extends User {}
来源：http://wiy.cqqwz.cn

TS:   class Admin extends User {}
来源：http://xau.c1oappe.top

Java: class Admin extends User {}
来源：http://mfc.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xck.jlsjyb.cn

Ruby: class Admin < User; end
来源：http://hoy.cqqwz.cn

C#:   class Admin : User {}
来源：http://fxk.9152youxi.cn

[G06] 重写方法
来源：http://dmo.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://khm.jinghuilouyu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wwg.zhongyouzk.top

JS:   greet() { return "admin"; }
来源：http://gkr.gogol.net.cn

TS:   greet(): string { return "admin"; }
来源：http://qcb.jinqigfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://dxt.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://duu.yj20258.top

Ruby: def greet; "admin"; end
来源：http://rvp.cdnleiting.top

C#:   public override string Greet() => "admin";
来源：http://tsc.zhengqikj.top

[G07] 调用父类方法
来源：http://cuz.yj20258.top

Py:   super().greet()
来源：http://tma.nwbrower.top

PHP:  parent::greet();
来源：http://kpv.shanyushiyangtech.top

JS:   super.greet();
来源：http://bgs.ydjk.org.cn

TS:   super.greet();
来源：http://slg.316326.xyz

Java: super.greet();
来源：http://lyp.sxryk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xys.havefunace.top

Ruby: super
来源：http://lzg.jinqigufen.top

C#:   base.Greet();
来源：http://nck.tianlin.xyz

[G08] 静态方法与属性
来源：http://snt.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tyq.sweek.top

PHP:  public static function f() {}
来源：http://anx.ybcxt.top

JS:   static f() {}
来源：http://vic.pycfn.com

TS:   static f(): void {}
来源：http://msa.jqgufenzy.top

Java: static void f() {}
来源：http://rnp.yfazqb.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://vpc.guannengcc.top

Ruby: def self.f; end
来源：http://yze.sweek.top

C#:   public static void F() {}
来源：http://wgx.fehbvm.com

[G09] 接口 / 抽象类
来源：http://mxq.kuanghao11.cn

Py:   from abc import ABC, abstractmethod
来源：http://qun.epnwcf.com

PHP:  interface Shape { public function area(): float; }
来源：http://lyh.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://xnw.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://zqr.ctjpmb.com

Java: interface Shape { double area(); }
来源：http://xuf.redwolf501.top

Go:   type Shape interface { Area() float64 }
来源：http://tyj.jinyuanbaomall.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qwq.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://zpf.fanxiaobao.xyz

[G10] 访问控制
来源：http://cie.yj20258888.top

Py:   约定 _protected / __private（不强制）
来源：http://xtu.9152youxi.cn

PHP:  public / protected / private
来源：http://fnh.yfazqb.com

JS:   #private 字段；其余公开
来源：http://gjt.pengpengdd.cyou

TS:   public / protected / private
来源：http://kwy.nanxinkj.top

Java: public / protected / private / 默认包级
来源：http://kbi.zhijiandao.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://spy.wangshuangyany.cn

Ruby: public / protected / private
来源：http://lnq.vehdjk.com


<!-- 参考信息 -->