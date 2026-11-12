代发 wailian999

Ruby: s.reverse
来源：http://xop.xingfuxueyuan.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://zcu.meibo888.top

[E12] 统计某字符出现次数
来源：http://bpt.uphjek.com

Py:   s.count("a")
来源：http://unb.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://njk.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://ams.vehdjk.com

TS:   s.split("a").length - 1
来源：http://obu.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fby.tanke756.top

Go:   strings.Count(s, "a")
来源：http://vgr.ehwqpu.com

Ruby: s.count("a")
来源：http://keo.xingfuxueyuan.xyz

C#:   s.Count(c => c == 'a')
来源：http://ole.hfpthk.cn

[E13] 逐字符遍历
来源：http://dfb.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://kar.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uhv.gogol.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://spk.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xkm.fanxiaobao.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ysq.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bhv.dashuyun.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nsy.fzhhl.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ycl.jianghu66.top

[E14] URL 编码与 Base64
来源：http://uzh.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://trm.hammf.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sak.jinghuilouyu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dbd.shanyushiyangkeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jta.yj20258888.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://snj.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iuv.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://udd.quarkkingdee.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hev.dianchejie.cn

[E15] HTML 转义 / 反转义
来源：http://wnf.shuidangran.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jxj.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jjq.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vpd.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jjw.yuxming.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://luy.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ivi.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ien.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ipa.ctjpmb.com

[E16] 数字千分位
来源：http://mhk.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://psq.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://tsb.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://aqb.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lba.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mom.nwbrower.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cxz.zdbjq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://luh.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://bzg.gzhubu.top

[E17] 首字母大写
来源：http://rur.snrcjt.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ykc.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qqw.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxw.sxryk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://brt.hongshengwenyu.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mqv.yuxming.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pzw.yuanzhike.top

Ruby: s.capitalize
来源：http://sfe.xylfe.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gkr.jqgfzy.top

[E18] 模板占位符替换
来源：http://syh.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lzt.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hfg.yongpay.top

JS:   tpl.replaceAll("{name}", name)
来源：http://otk.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ovj.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nyb.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://thm.0kj1m.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cud.fktsv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hzz.xziqi.cn

[E19] 多行文本按行拆分
来源：http://jgh.hnxiangtu.top

Py:   s.splitlines()
来源：http://rxe.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nai.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://eus.jqgufenzy.top

TS:   s.split(/\r?\n/)
来源：http://kvh.hfpthk.cn

Java: s.lines().toList()
来源：http://mdc.fehbvm.com

Go:   strings.Split(s, "\n")
来源：http://idt.daxiang520.top

Ruby: s.lines
来源：http://fiv.jyoumei.cn

C#:   s.Split('\n')
来源：http://nxi.xinyue.icu

[E20] 判断字符串是否为空
来源：http://vjo.bjfxy.top

Py:   if not s:
来源：http://rck.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rwq.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://znq.sufxvd.cn

TS:   if (s === "") {}
来源：http://bhe.birdmap.top

Java: if (s.isEmpty()) {}
来源：http://wuz.yuxming.cn

Go:   if s == "" {}
来源：http://irj.yanxiufei.cn

Ruby: if s.empty?
来源：http://poo.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dnl.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://duz.birdmap.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rpg.fengsongda.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nql.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kfj.xinyue.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jod.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nnf.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://oar.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vdn.smart0.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jve.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://onp.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mfi.yanxiufei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jde.yfazqb.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ajc.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zbx.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jck.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fmy.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://xnh.yonumen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sys.ydjk.org.cn

================================================================================
来源：http://kqm.0kj1m.cn

F. 文件与目录
来源：http://prf.xuetiantiany.cn

================================================================================
来源：http://svw.zhixingplan.top

[F01] 读取整个文件
来源：http://twt.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ugy.ydjk.org.cn

PHP:  file_get_contents("a.txt");
来源：http://fjc.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://klg.zhoulong.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cak.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://xft.guowangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tlv.fanxiaobao.xyz

Ruby: File.read("a.txt")
来源：http://pbg.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://gjd.jinqigfzy.top

[F02] 逐行读取文件
来源：http://owt.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wkn.ppjwa.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mfs.iojbl.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://shw.xziqi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wib.tarul.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mnl.snrcjt.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qpn.vehdjk.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ehx.yj202588.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://usx.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://sqe.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rqj.tianlin.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://hpb.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rvl.tianlin.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fyk.jyoumei.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nrc.jqgufenzy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eva.sysykeji.top

Ruby: File.write("a.txt", "hi")
来源：http://gjt.xylfe.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nda.hywenlv.cn

[F04] 追加写入文件
来源：http://ows.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nxh.aibaodan.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qxb.0kj1m.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vip.52xcode.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wnh.xylfe.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vno.fktsv.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mxj.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://srl.cdnleiting.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ixs.jqgfzy.top

[F05] 判断文件或目录是否存在
来源：http://vbc.jyoumei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uer.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://cca.zhijiandao.cn

JS:   fs.existsSync("a.txt")
来源：http://kbd.jinqigfzy.top

TS:   fs.existsSync("a.txt")
来源：http://bnl.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pmm.birdmap.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bon.hcnkem.com

Ruby: File.exist?("a.txt")
来源：http://fye.hongshengwenyu.top

C#:   File.Exists("a.txt")
来源：http://khl.shzxlz.cn

[F06] 删除文件
来源：http://spe.jqgufenzy.top

Py:   os.remove("a.txt")
来源：http://dhd.nanxinkj.top

PHP:  unlink("a.txt");
来源：http://oye.zhiwuduotai.top

JS:   fs.unlinkSync("a.txt")
来源：http://vck.gotoacloud.top

TS:   fs.unlinkSync("a.txt")
来源：http://woy.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hef.uphjek.com

Go:   os.Remove("a.txt")
来源：http://pow.dashuyun.cn

Ruby: File.delete("a.txt")
来源：http://xai.dashuyun.cn

C#:   File.Delete("a.txt");
来源：http://eat.c1oappe.top

[F07] 创建目录（含多级）
来源：http://dtw.daria6918.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pek.hammf.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lph.gzhubu.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cdt.shangyingyoupin.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zlk.dianchejie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kan.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dpy.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oad.shuidangran.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://duu.quarkkingdee.top

[F08] 遍历目录
来源：http://mkw.316326.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://gmb.aibaodan.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mle.c1oappe.top

JS:   fs.readdirSync("dir")
来源：http://dsf.yuanzhike.top

TS:   fs.readdirSync("dir")
来源：http://iwo.dianchejie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dtk.bjfxy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ywp.zhixingplan.top

Ruby: Dir.children("dir")
来源：http://nud.tarul.cn

C#:   Directory.GetFiles("dir")
来源：http://kzk.haohaochexian.top

[F09] 获取文件大小
来源：http://tmi.ppjwa.cn

Py:   os.path.getsize("a.txt")
来源：http://gag.cucudq.cn

PHP:  filesize("a.txt");
来源：http://syt.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://yrv.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://zxx.yj20258888.top

Java: Files.size(Path.of("a.txt"))
来源：http://lqr.bbcook.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cwi.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://pnb.smart0.xyz

C#:   new FileInfo("a.txt").Length
来源：http://bep.zhoulong.xyz

[F10] 取文件扩展名 / 文件名
来源：http://loy.jlsjyb.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sww.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uit.xuanzx.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fzg.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://tta.cdnleiting.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jiu.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oeq.hfpthk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eho.jinqigfzy.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yze.jianghu66.top

[F11] 复制与移动文件
来源：http://jtd.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qew.vehdjk.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mof.gogol.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ulb.tian-w.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pat.nanxinkj.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jxf.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://gpp.fktsv.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nvx.dianchejie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wtf.jinqigufen.top

[F12] CSV 读写
来源：http://ufq.gogol.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zty.cashguo.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ahu.feifeiyinyue.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dll.sweek.top

TS:   // 同上
来源：http://yha.tian-w.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wwd.xinyue.icu

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rti.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lbf.hongshengwenyu.top

C#:   // 无内置：用 CsvHelper 库
来源：http://myw.zhongyouzk.top

================================================================================
来源：http://rkc.chenjidiqi.icu

G. 面向对象
来源：http://app.meibo888.top

================================================================================
来源：http://whh.gotoacloud.top

[G01] 定义类
来源：http://wpu.zhoulong.xyz

Py:   class User: pass
来源：http://dsv.gzhubu.top

PHP:  class User {}
来源：http://jms.birdmap.top

JS:   class User {}
来源：http://zgs.sxryk.cn

TS:   class User { name: string = ""; }
来源：http://ezn.yj20258.top

Java: class User {}
来源：http://hjc.havefunace.top

Go:   type User struct { Name string }
来源：http://dpg.shangyingyoupin.top

Ruby: class User; end
来源：http://nzi.shangyingyoupin.top

C#:   class User {}
来源：http://ofo.meibo888.top

[G02] 构造函数
来源：http://cnq.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://ukn.xuetiantiany.cn

PHP:  public function __construct(public string $name) {}
来源：http://iqm.shanyushiyangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://izx.pengpengdd.cyou

TS:   constructor(public name: string) {}
来源：http://unu.bjfxy.top

Java: User(String name) { this.name = name; }
来源：http://rsi.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://uwp.0kj1m.cn

Ruby: def initialize(name); @name = name; end
来源：http://pgp.aizwys.cn

C#:   public User(string name) { Name = name; }
来源：http://lia.aizwys.cn

[G03] 实例属性
来源：http://jfc.birdmap.top

Py:   self.name = "x"
来源：http://xps.hywenlv.cn

PHP:  public string $name = "x";
来源：http://esm.chenzaomai.com

JS:   this.name = "x";
来源：http://dnr.vehdjk.com

TS:   name: string = "x";
来源：http://wrj.dashuyun.cn

Java: private String name;
来源：http://oip.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://apa.jinqigfzy.top

Ruby: @name = "x"
来源：http://prx.cheryme.top

C#:   public string Name { get; set; } = "x";
来源：http://cxk.zhoulong.xyz

[G04] 定义方法
来源：http://qoa.mhx1999.top

Py:   def greet(self): return self.name
来源：http://wpu.sweek.top

PHP:  public function greet(): string { return $this->name; }
来源：http://xnl.dashuyun.cn

JS:   greet() { return this.name; }
来源：http://szj.aibaodan.cn

TS:   greet(): string { return this.name; }
来源：http://pzc.bjfxy.top

Java: String greet() { return name; }
来源：http://baw.zhixingplan.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ghz.gzhubu.top

Ruby: def greet; @name; end
来源：http://nle.shanyushiyangkeji.top

C#:   public string Greet() => Name;
来源：http://oqz.quarkkingdee.top

[G05] 继承
来源：http://kim.dashuyun.cn

Py:   class Admin(User): pass
来源：http://puz.ybcxt.top

PHP:  class Admin extends User {}
来源：http://ofa.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://lie.sxryk.cn

TS:   class Admin extends User {}
来源：http://gsj.iojbl.cn

Java: class Admin extends User {}
来源：http://wfe.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://icd.sxryk.cn

Ruby: class Admin < User; end
来源：http://zwl.hysaishi.cn

C#:   class Admin : User {}
来源：http://ibm.chenjidiqi.icu

[G06] 重写方法
来源：http://qff.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://fep.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://tya.jqgfzy.top

JS:   greet() { return "admin"; }
来源：http://wmv.yj20258888.top

TS:   greet(): string { return "admin"; }
来源：http://ddm.epnwcf.com

Java: @Override String greet() { return "admin"; }
来源：http://glv.hfpthk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://owg.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://rha.cqqwz.cn

C#:   public override string Greet() => "admin";
来源：http://hpe.uphjek.com

[G07] 调用父类方法
来源：http://oao.chenlongwang.top

Py:   super().greet()
来源：http://xxh.zhijiandao.cn

PHP:  parent::greet();
来源：http://ira.sufxvd.cn

JS:   super.greet();
来源：http://nbd.tanke756.top

TS:   super.greet();
来源：http://yqe.tanke756.top

Java: super.greet();
来源：http://jnd.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cet.sjlbkw.cn

Ruby: super
来源：http://csj.zdbjq.cn

C#:   base.Greet();
来源：http://bve.yj202588.top

[G08] 静态方法与属性
来源：http://jfj.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://scf.gotoacloud.top

PHP:  public static function f() {}
来源：http://jfz.dianchejie.cn

JS:   static f() {}
来源：http://doi.zdbjq.cn

TS:   static f(): void {}
来源：http://hap.guowangkeji.top

Java: static void f() {}
来源：http://xsh.jqgufenzy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://rzc.pycfn.com

Ruby: def self.f; end
来源：http://xeo.jianghu66.top

C#:   public static void F() {}
来源：http://kbf.zycfv.cn

[G09] 接口 / 抽象类
来源：http://rlh.cqqwz.cn

Py:   from abc import ABC, abstractmethod
来源：http://hgf.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://dij.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vcb.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://ncj.feifeiyinyue.top

Java: interface Shape { double area(); }
来源：http://qpe.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://ioa.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://btx.cashguo.top

C#:   interface IShape { double Area(); }
来源：http://ioe.sysykeji.top

[G10] 访问控制
来源：http://vms.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://ywr.haohaochexian.top

PHP:  public / protected / private
来源：http://iol.ctjpmb.com

JS:   #private 字段；其余公开
来源：http://wrm.havefunace.top


<!-- 参考信息 -->