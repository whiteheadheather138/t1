代发 wailian999

Ruby: s.reverse
来源：http://eta.epnwcf.com

C#:   new string(s.Reverse().ToArray())
来源：http://coo.sxryk.cn

[E12] 统计某字符出现次数
来源：http://sqd.ctjpmb.com

Py:   s.count("a")
来源：http://lgm.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://rhs.52xcode.cn

JS:   s.split("a").length - 1
来源：http://kjt.wangshuangyany.cn

TS:   s.split("a").length - 1
来源：http://mfj.xziqi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dov.guowangkeji.top

Go:   strings.Count(s, "a")
来源：http://dza.ydjk.org.cn

Ruby: s.count("a")
来源：http://fby.yueranfly.top

C#:   s.Count(c => c == 'a')
来源：http://pvf.daria6918.cn

[E13] 逐字符遍历
来源：http://dtt.jinghuilouyu.cn

Py:   for ch in s: print(ch)
来源：http://kso.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vlg.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uni.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bgy.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kvm.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fty.fktsv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ppg.vehdjk.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qea.aizwys.cn

[E14] URL 编码与 Base64
来源：http://lrw.epnwcf.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pps.sufxvd.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zzh.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zff.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nny.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lca.zhiwuduotai.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zxm.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fdk.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://umj.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://nev.guowangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://osj.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lht.fzhhl.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pfd.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://qxk.yonumen.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yoc.jinqigufen.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mcr.svipenyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://umj.9152youxi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nyp.chenjidiqi.icu

[E16] 数字千分位
来源：http://nqp.zhiwuduotai.top

Py:   f"{1234567:,}"
来源：http://kae.guannengcc.top

PHP:  number_format(1234567);
来源：http://dbe.xylfe.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://elf.guowangkeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://qhn.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uwy.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uja.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qtp.fktsv.cn

C#:   1234567.ToString("N0")
来源：http://ekm.ybcxt.top

[E17] 首字母大写
来源：http://lpk.cdnleiting.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sdb.zhaomingkeji.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://rnn.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mso.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zwv.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gyq.hongshengwenyu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xqe.gzhubu.top

Ruby: s.capitalize
来源：http://mar.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oer.xuanzx.com

[E18] 模板占位符替换
来源：http://mrc.xuanzx.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pai.sxryk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qjk.pengpengdd.cyou

JS:   tpl.replaceAll("{name}", name)
来源：http://fop.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://add.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vkg.tanke756.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zpb.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ver.uphjek.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://khk.jianghu66.top

[E19] 多行文本按行拆分
来源：http://ugl.zdbjq.cn

Py:   s.splitlines()
来源：http://def.tanke756.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nge.mhx1999.top

JS:   s.split(/\r?\n/)
来源：http://xih.ydzc1.top

TS:   s.split(/\r?\n/)
来源：http://lmk.wangshuangyany.cn

Java: s.lines().toList()
来源：http://eom.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://xba.c1oappe.top

Ruby: s.lines
来源：http://spl.0kj1m.cn

C#:   s.Split('\n')
来源：http://stf.cdnleiting.top

[E20] 判断字符串是否为空
来源：http://xqt.xylfe.cn

Py:   if not s:
来源：http://zls.ehwqpu.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hlu.shangyingyoupin.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wdj.fehbvm.com

TS:   if (s === "") {}
来源：http://vrm.yanxiufei.cn

Java: if (s.isEmpty()) {}
来源：http://xxv.guowangkeji.top

Go:   if s == "" {}
来源：http://sut.yongpay.top

Ruby: if s.empty?
来源：http://vos.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dkf.haohaochexian.top

[E21] 超长截断加省略号
来源：http://ops.daxiang520.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hzg.chenzaomai.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iyd.vqdsnc.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://slo.zhoulong.xyz

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pnf.shanyushiyangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wst.cheryme.top

Go:   // 按 rune 判断长度后截断
来源：http://ept.cashguo.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zvm.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rof.fehbvm.com

[E22] 字节长度与字符长度
来源：http://rwg.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mej.cucudq.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rtj.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ihl.xingfuxueyuan.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yow.andypj.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jnv.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yqp.wangshuangyany.cn

Ruby: s.bytesize;  s.length
来源：http://bqt.daria6918.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xjp.zhaomingkeji.xyz

================================================================================
来源：http://cha.c1oappe.top

F. 文件与目录
来源：http://bbr.pengpengdd.cyou

================================================================================
来源：http://vfl.9152youxi.cn

[F01] 读取整个文件
来源：http://jwb.9152youxi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://olp.zhixingplan.top

PHP:  file_get_contents("a.txt");
来源：http://hla.redwolf501.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pib.vqdsnc.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bst.yangfankeji.com

Java: Files.readString(Path.of("a.txt"))
来源：http://uhx.sxryk.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tcp.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://djj.yongpay.top

C#:   File.ReadAllText("a.txt");
来源：http://lys.ydzc1.top

[F02] 逐行读取文件
来源：http://dft.gogol.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jds.fktsv.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dik.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://boz.vqdsnc.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jnz.jqgufenzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xov.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kvy.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gjy.guowangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xao.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://miu.jianghu66.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nzx.snrcjt.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ksb.aibaodan.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cyu.sxryk.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iaz.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jrg.tian-w.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ijg.zhongyouzk.top

Ruby: File.write("a.txt", "hi")
来源：http://ozg.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lcz.c1oappe.top

[F04] 追加写入文件
来源：http://gtt.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://egt.kuanghao11.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ouf.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cnn.jqgfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rut.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jhu.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cik.hongshengwenyu.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rnb.hnqzz.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://crt.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://csm.hammf.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://buk.ydzc1.top

PHP:  file_exists("a.txt");
来源：http://uuf.smart0.xyz

JS:   fs.existsSync("a.txt")
来源：http://gwd.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://eja.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://sxu.wangshuangyany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yxw.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://tce.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://dxm.yfazqb.com

[F06] 删除文件
来源：http://ilh.yuxming.cn

Py:   os.remove("a.txt")
来源：http://qth.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://dpg.9152youxi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yih.cheryme.top

TS:   fs.unlinkSync("a.txt")
来源：http://tmt.fanxiaobao.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oav.ydjk.org.cn

Go:   os.Remove("a.txt")
来源：http://kbw.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://mpl.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://tdx.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://qqp.dianchejie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uqo.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rxl.cashguo.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aro.havefunace.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uat.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uqe.0kj1m.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wad.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iss.shanyushiyangtech.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://icm.bbcook.cn

[F08] 遍历目录
来源：http://pom.yj20258.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://zmn.jinqigufen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vkv.316326.xyz

JS:   fs.readdirSync("dir")
来源：http://ean.bbcook.cn

TS:   fs.readdirSync("dir")
来源：http://bid.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://stk.fehbvm.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://uav.cucudq.cn

Ruby: Dir.children("dir")
来源：http://lqp.jianghu66.top

C#:   Directory.GetFiles("dir")
来源：http://uyl.jinghuilouyu.cn

[F09] 获取文件大小
来源：http://phc.tanke756.top

Py:   os.path.getsize("a.txt")
来源：http://msp.zdbjq.cn

PHP:  filesize("a.txt");
来源：http://ufs.bbcook.cn

JS:   fs.statSync("a.txt").size
来源：http://twc.ywan-chungtsiang.top

TS:   fs.statSync("a.txt").size
来源：http://ghk.nwbrower.top

Java: Files.size(Path.of("a.txt"))
来源：http://aaf.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ics.yvedp.cn

Ruby: File.size("a.txt")
来源：http://nth.ydjk.org.cn

C#:   new FileInfo("a.txt").Length
来源：http://njz.ydjk.org.cn

[F10] 取文件扩展名 / 文件名
来源：http://mgm.9152youxi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://okw.jinqigufen.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fgn.zhengqikj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mte.xingfuxueyuan.xyz

TS:   path.extname("a.txt")
来源：http://qbo.jinqigfzy.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cyq.sysykeji.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oys.bbcook.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nni.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xkj.ydzc1.top

[F11] 复制与移动文件
来源：http://quv.jinyuanbaomall.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nuy.jiagoushi.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aex.vehdjk.com

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tyv.jlsjyb.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xty.iojbl.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ous.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zmg.dianchejie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uva.hongshengwenyu.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cjk.guannengcc.top

[F12] CSV 读写
来源：http://nox.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xbm.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ixo.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mhl.aizwys.cn

TS:   // 同上
来源：http://gtr.wangshuangyany.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pdj.nwbrower.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fxw.zdbjq.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ghl.ywan-chungtsiang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://spr.pycfn.com

================================================================================
来源：http://woi.hongshengwenyu.top

G. 面向对象
来源：http://jam.hesvh.cn

================================================================================
来源：http://zom.gotoacloud.top

[G01] 定义类
来源：http://wgp.daria6918.cn

Py:   class User: pass
来源：http://qsa.yangfankeji.com

PHP:  class User {}
来源：http://pfn.tarul.cn

JS:   class User {}
来源：http://dak.dashuyun.cn

TS:   class User { name: string = ""; }
来源：http://odq.guannengcc.top

Java: class User {}
来源：http://wnr.sjlbkw.cn

Go:   type User struct { Name string }
来源：http://peq.jinqigufen.top

Ruby: class User; end
来源：http://jkw.yj20258.top

C#:   class User {}
来源：http://cww.jianghu66.top

[G02] 构造函数
来源：http://bbu.zhengqikj.top

Py:   def __init__(self, name): self.name = name
来源：http://igr.yonumen.top

PHP:  public function __construct(public string $name) {}
来源：http://eyi.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://bdk.zhijiandao.cn

TS:   constructor(public name: string) {}
来源：http://dln.sxryk.cn

Java: User(String name) { this.name = name; }
来源：http://vcg.daxiang520.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bqy.jiagoushi.top

Ruby: def initialize(name); @name = name; end
来源：http://yoc.chenjidiqi.icu

C#:   public User(string name) { Name = name; }
来源：http://oeg.gzhubu.top

[G03] 实例属性
来源：http://yfc.dianchejie.cn

Py:   self.name = "x"
来源：http://uqc.yangfankeji.com

PHP:  public string $name = "x";
来源：http://qdu.cdnleiting.top

JS:   this.name = "x";
来源：http://zhs.guowangkeji.top

TS:   name: string = "x";
来源：http://xpv.c1oappe.top

Java: private String name;
来源：http://hto.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xed.fehbvm.com

Ruby: @name = "x"
来源：http://vwg.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://lfn.jlsjyb.cn

[G04] 定义方法
来源：http://ozp.yonumen.top

Py:   def greet(self): return self.name
来源：http://mdj.epnwcf.com

PHP:  public function greet(): string { return $this->name; }
来源：http://wvd.aizwys.cn

JS:   greet() { return this.name; }
来源：http://fub.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://muy.hywenlv.cn

Java: String greet() { return name; }
来源：http://rjj.hysaishi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xik.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://kgn.hammf.cn

C#:   public string Greet() => Name;
来源：http://duu.daria6918.cn

[G05] 继承
来源：http://vpq.hywenlv.cn

Py:   class Admin(User): pass
来源：http://wnq.wangdashe.top

PHP:  class Admin extends User {}
来源：http://smv.jinyuanbaomall.cn

JS:   class Admin extends User {}
来源：http://mga.cqqwz.cn

TS:   class Admin extends User {}
来源：http://xcs.epnwcf.com

Java: class Admin extends User {}
来源：http://qmj.jianghu66.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wvu.hesvh.cn

Ruby: class Admin < User; end
来源：http://fmu.jinqigfzy.top

C#:   class Admin : User {}
来源：http://bvw.ppjwa.cn

[G06] 重写方法
来源：http://cvy.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://kzr.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://sfq.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://qqg.jiagoushi.top

TS:   greet(): string { return "admin"; }
来源：http://nva.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://ugl.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iyr.hammf.cn

Ruby: def greet; "admin"; end
来源：http://lvn.hongshengwenyu.top

C#:   public override string Greet() => "admin";
来源：http://hcj.zdqjudy.top

[G07] 调用父类方法
来源：http://dtl.cashguo.top

Py:   super().greet()
来源：http://icq.hfpthk.cn

PHP:  parent::greet();
来源：http://hnh.meibo888.top

JS:   super.greet();
来源：http://glf.jyoumei.cn

TS:   super.greet();
来源：http://aay.hysaishi.cn

Java: super.greet();
来源：http://kfl.cashguo.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bkd.uphjek.com

Ruby: super
来源：http://okf.sysykeji.top

C#:   base.Greet();
来源：http://pnk.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://suh.hammf.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xlo.vehdjk.com

PHP:  public static function f() {}
来源：http://orp.0kj1m.cn

JS:   static f() {}
来源：http://pgm.chenzaomai.com

TS:   static f(): void {}
来源：http://xss.fehbvm.com

Java: static void f() {}
来源：http://wxg.zhijiandao.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://icc.fanxiaobao.xyz

Ruby: def self.f; end
来源：http://yks.ppjwa.cn

C#:   public static void F() {}
来源：http://xan.jinqigfzy.top

[G09] 接口 / 抽象类
来源：http://bqq.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://bbi.hongshengwenyu.top

PHP:  interface Shape { public function area(): float; }
来源：http://gct.xuetiantiany.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dpw.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://jtk.hcnkem.com

Java: interface Shape { double area(); }
来源：http://xmg.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://prp.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mmg.feifeiyinyue.top

C#:   interface IShape { double Area(); }
来源：http://ucz.zhengqikj.top

[G10] 访问控制
来源：http://svt.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://ezg.shanyushiyangtech.top

PHP:  public / protected / private
来源：http://ont.aizwys.cn

JS:   #private 字段；其余公开
来源：http://xih.mhx1999.top


<!-- 参考信息 -->