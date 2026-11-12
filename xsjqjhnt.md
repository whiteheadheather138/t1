代发 wailian999

PHP:  substr_count($s, "a");
来源：http://mdq.tanke756.top

JS:   s.split("a").length - 1
来源：http://yfp.nwbrower.top

TS:   s.split("a").length - 1
来源：http://gbh.zhongyouzk.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iha.ivvv.top

Go:   strings.Count(s, "a")
来源：http://dya.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://rhm.c1oappe.top

C#:   s.Count(c => c == 'a')
来源：http://ufe.kuanghao11.cn

[E13] 逐字符遍历
来源：http://jrw.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://bfa.jqgfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dvf.guowangkeji.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wqz.kuanghao11.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rzk.vehdjk.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mfj.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gmn.jqgfzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://tyj.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xml.zhiwuduotai.top

[E14] URL 编码与 Base64
来源：http://qyq.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://svk.hfpthk.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://uzt.0kj1m.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rsb.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://efd.gogol.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dqm.tarul.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ome.nanxuanxn.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kaq.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mff.meibo888.top

[E15] HTML 转义 / 反转义
来源：http://hhw.cheryme.top

Py:   html.escape(s);  html.unescape(s)
来源：http://idu.quarkkingdee.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pek.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://eln.nwbrower.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lxh.tanke756.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqk.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yaw.zhaomingkeji.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wwg.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ctb.vehdjk.com

[E16] 数字千分位
来源：http://nct.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://yte.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://ffb.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rkj.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tvt.shangyingyoupin.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ydg.zhixingplan.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rqi.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pwt.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://yum.mhx1999.top

[E17] 首字母大写
来源：http://lrj.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://map.hammf.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vrz.smart0.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bmv.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rhf.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nqi.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dgx.gotoacloud.top

Ruby: s.capitalize
来源：http://hmq.kuanghao11.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eww.aibaodan.cn

[E18] 模板占位符替换
来源：http://cpe.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nyu.hysaishi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mqo.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://jum.c1oappe.top

TS:   tpl.replaceAll("{name}", name)
来源：http://son.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ofe.dianchejie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qlb.zhiwuduotai.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ckz.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yes.nwbrower.top

[E19] 多行文本按行拆分
来源：http://tee.jinqigfzy.top

Py:   s.splitlines()
来源：http://zyd.jqgufenzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fwb.ctjpmb.com

JS:   s.split(/\r?\n/)
来源：http://gcd.andypj.xyz

TS:   s.split(/\r?\n/)
来源：http://qev.gaohongyu789.top

Java: s.lines().toList()
来源：http://puc.jianghu66.top

Go:   strings.Split(s, "\n")
来源：http://zba.cashguo.top

Ruby: s.lines
来源：http://yid.cheryme.top

C#:   s.Split('\n')
来源：http://dyn.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://aiw.jinqigfzy.top

Py:   if not s:
来源：http://nsz.chenlongwang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nce.andypj.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rlt.yj202588.top

TS:   if (s === "") {}
来源：http://cgu.hammf.cn

Java: if (s.isEmpty()) {}
来源：http://dak.havefunace.top

Go:   if s == "" {}
来源：http://yff.nwbrower.top

Ruby: if s.empty?
来源：http://exe.tian-w.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tba.shuidangran.top

[E21] 超长截断加省略号
来源：http://poe.aibaodan.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nmi.redwolf501.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bqg.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://duu.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://srb.meibo888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vzo.daria6918.cn

Go:   // 按 rune 判断长度后截断
来源：http://tgi.snrcjt.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jzv.quarkkingdee.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nii.zhixingplan.top

[E22] 字节长度与字符长度
来源：http://caa.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ciz.yfazqb.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iin.shzxlz.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jmb.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pli.yangfankeji.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wlb.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ooz.jinyuanbaomall.cn

Ruby: s.bytesize;  s.length
来源：http://vtm.nanxuanxn.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ael.chenzaomai.com

================================================================================
来源：http://pmx.c1oappe.top

F. 文件与目录
来源：http://voo.shuidangran.top

================================================================================
来源：http://pub.dashuyun.cn

[F01] 读取整个文件
来源：http://sek.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yba.yj20258.top

PHP:  file_get_contents("a.txt");
来源：http://lxm.jinghuilouyu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fbv.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tyk.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://gmx.xinyue.icu

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xji.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://ckd.nanxuanxn.top

C#:   File.ReadAllText("a.txt");
来源：http://kif.yj20258.top

[F02] 逐行读取文件
来源：http://ckz.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sqv.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://feq.bjfxy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kpa.yueranfly.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sxy.jinqigfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jii.sweek.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rts.aibaodan.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dnh.birdmap.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rde.yongpay.top

[F03] 写入文件（覆盖）
来源：http://imm.ppjwa.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ysn.shuidangran.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://asq.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kfb.ivvv.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tsq.hfpthk.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xhn.yuanzhike.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vft.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://cas.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yiq.iojbl.cn

[F04] 追加写入文件
来源：http://zss.ppjwa.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mwf.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ylq.hywenlv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rnt.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hcx.fktsv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qzy.zhijiandao.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ztg.jianghu66.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tmt.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qbg.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://bdm.tanke756.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://juz.cashguo.top

PHP:  file_exists("a.txt");
来源：http://lip.jianghu66.top

JS:   fs.existsSync("a.txt")
来源：http://nlo.sufxvd.cn

TS:   fs.existsSync("a.txt")
来源：http://llb.ehwqpu.com

Java: Files.exists(Path.of("a.txt"))
来源：http://pzl.xuetiantiany.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uwh.fktsv.cn

Ruby: File.exist?("a.txt")
来源：http://qpx.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://yer.yonumen.top

[F06] 删除文件
来源：http://ptm.sysykeji.top

Py:   os.remove("a.txt")
来源：http://eya.quarkkingdee.top

PHP:  unlink("a.txt");
来源：http://zvs.nwbrower.top

JS:   fs.unlinkSync("a.txt")
来源：http://tnq.ehwqpu.com

TS:   fs.unlinkSync("a.txt")
来源：http://kka.chenzaomai.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rmj.gogol.net.cn

Go:   os.Remove("a.txt")
来源：http://iqh.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://bmi.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://hmn.haohaochexian.top

[F07] 创建目录（含多级）
来源：http://gvp.chenlongwang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rdj.haohaochexian.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://smp.feifeiyinyue.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wqz.fktsv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dgh.svipenyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mkl.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gkd.uphjek.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qar.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://onp.havefunace.top

[F08] 遍历目录
来源：http://nzb.vqdsnc.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yrx.jqgfzy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qpp.yongpay.top

JS:   fs.readdirSync("dir")
来源：http://oce.hywenlv.cn

TS:   fs.readdirSync("dir")
来源：http://nvc.chenjidiqi.icu

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yov.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tau.yangfankeji.com

Ruby: Dir.children("dir")
来源：http://bcl.havefunace.top

C#:   Directory.GetFiles("dir")
来源：http://oxn.hnqzz.top

[F09] 获取文件大小
来源：http://abq.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://krf.fehbvm.com

PHP:  filesize("a.txt");
来源：http://uvv.xuanzx.com

JS:   fs.statSync("a.txt").size
来源：http://qsl.tanke756.top

TS:   fs.statSync("a.txt").size
来源：http://tpz.sweek.top

Java: Files.size(Path.of("a.txt"))
来源：http://uho.tarul.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iqh.zhixingplan.top

Ruby: File.size("a.txt")
来源：http://nfg.haohaochexian.top

C#:   new FileInfo("a.txt").Length
来源：http://eix.sysykeji.top

[F10] 取文件扩展名 / 文件名
来源：http://nzt.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gvl.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jau.uphjek.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tuy.guannengcc.top

TS:   path.extname("a.txt")
来源：http://zlg.nwbrower.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmd.fengsongda.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dew.tian-w.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://obu.bbcook.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wsd.uphjek.com

[F11] 复制与移动文件
来源：http://eku.wangdashe.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dwt.bbcook.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wal.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jrt.iojbl.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qiy.svipenyu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://boe.yj202588.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://obf.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lbh.hnqzz.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nsm.hywenlv.cn

[F12] CSV 读写
来源：http://vtp.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://adl.yanxiufei.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vlh.ivvv.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wpj.tanke756.top

TS:   // 同上
来源：http://vao.yj20258.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ioc.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yib.guannengcc.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bwg.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://czq.meibo888.top

================================================================================
来源：http://ivc.fktsv.cn

G. 面向对象
来源：http://rid.gzhubu.top

================================================================================
来源：http://jpb.fanxiaobao.xyz

[G01] 定义类
来源：http://xvj.epnwcf.com

Py:   class User: pass
来源：http://ygv.fktsv.cn

PHP:  class User {}
来源：http://nrf.gaohongyu789.top

JS:   class User {}
来源：http://lon.xingfuxueyuan.xyz

TS:   class User { name: string = ""; }
来源：http://yer.c1oappe.top

Java: class User {}
来源：http://ful.chenlongwang.top

Go:   type User struct { Name string }
来源：http://ofi.cdnleiting.top

Ruby: class User; end
来源：http://edr.dashuyun.cn

C#:   class User {}
来源：http://yrp.xinyue.icu

[G02] 构造函数
来源：http://nlj.vehdjk.com

Py:   def __init__(self, name): self.name = name
来源：http://ojm.0kj1m.cn

PHP:  public function __construct(public string $name) {}
来源：http://aoo.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://vtm.daria6918.cn

TS:   constructor(public name: string) {}
来源：http://twa.vqdsnc.cn

Java: User(String name) { this.name = name; }
来源：http://htc.tanke756.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pjd.epnwcf.com

Ruby: def initialize(name); @name = name; end
来源：http://hwc.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://tqn.xinyue.icu

[G03] 实例属性
来源：http://ytg.jinqigufen.top

Py:   self.name = "x"
来源：http://zyr.birdmap.top

PHP:  public string $name = "x";
来源：http://ckf.pycfn.com

JS:   this.name = "x";
来源：http://jlm.smart0.xyz

TS:   name: string = "x";
来源：http://wio.xuetiantiany.cn

Java: private String name;
来源：http://fkj.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://inc.zhengqikj.top

Ruby: @name = "x"
来源：http://mse.zdqjudy.top

C#:   public string Name { get; set; } = "x";
来源：http://sca.epnwcf.com

[G04] 定义方法
来源：http://vus.fengsongda.top

Py:   def greet(self): return self.name
来源：http://vwt.iojbl.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jdd.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://yln.hesvh.cn

TS:   greet(): string { return this.name; }
来源：http://eax.yongpay.top

Java: String greet() { return name; }
来源：http://emu.jqgfzy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nue.meibo888.top

Ruby: def greet; @name; end
来源：http://myw.daxiang520.top

C#:   public string Greet() => Name;
来源：http://zpx.zhoulong.xyz

[G05] 继承
来源：http://eqb.iojbl.cn

Py:   class Admin(User): pass
来源：http://lbk.sufxvd.cn

PHP:  class Admin extends User {}
来源：http://gkc.316326.xyz

JS:   class Admin extends User {}
来源：http://jpn.nanxinkj.top

TS:   class Admin extends User {}
来源：http://bhj.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://ble.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pxc.haohaochexian.top

Ruby: class Admin < User; end
来源：http://riy.zdbjq.cn

C#:   class Admin : User {}
来源：http://cgr.hammf.cn

[G06] 重写方法
来源：http://dlh.shanyushiyangtech.top

Py:   def greet(self): return "admin"
来源：http://ahy.cheryme.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vod.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://hgi.zhoulong.xyz

TS:   greet(): string { return "admin"; }
来源：http://jey.daria6918.cn

Java: @Override String greet() { return "admin"; }
来源：http://ynu.hcnkem.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vhs.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://nzq.tian-w.cn

C#:   public override string Greet() => "admin";
来源：http://bvb.tianlin.xyz

[G07] 调用父类方法
来源：http://nih.dianchejie.cn

Py:   super().greet()
来源：http://yzh.bbcook.cn

PHP:  parent::greet();
来源：http://laz.zhengqikj.top

JS:   super.greet();
来源：http://okt.ydjk.org.cn

TS:   super.greet();
来源：http://inb.shuidangran.top

Java: super.greet();
来源：http://bfx.ydjk.org.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dbs.cucudq.cn

Ruby: super
来源：http://abe.yuanzhike.top

C#:   base.Greet();
来源：http://dyr.dianchejie.cn

[G08] 静态方法与属性
来源：http://ohu.zdqjudy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oog.cdnleiting.top

PHP:  public static function f() {}
来源：http://roe.haohaochexian.top

JS:   static f() {}
来源：http://oxz.smart0.xyz

TS:   static f(): void {}
来源：http://xfd.nanxuanxn.top

Java: static void f() {}
来源：http://kwy.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ape.cdnleiting.top

Ruby: def self.f; end
来源：http://sci.zhongyouzk.top

C#:   public static void F() {}
来源：http://ihm.meibo888.top

[G09] 接口 / 抽象类
来源：http://zlg.havefunace.top

Py:   from abc import ABC, abstractmethod
来源：http://cin.guowangkeji.top

PHP:  interface Shape { public function area(): float; }
来源：http://axn.hfpthk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rnr.bbcook.cn

TS:   interface Shape { area(): number; }
来源：http://pcl.aibaodan.cn

Java: interface Shape { double area(); }
来源：http://rzm.yueranfly.top

Go:   type Shape interface { Area() float64 }
来源：http://rea.tian-w.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://plr.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://awb.sufxvd.cn

[G10] 访问控制
来源：http://fpd.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://sfw.smart0.xyz

PHP:  public / protected / private
来源：http://ape.fengsongda.top

JS:   #private 字段；其余公开
来源：http://hdn.yj202588.top

TS:   public / protected / private
来源：http://oqc.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://kte.yangfankeji.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://ynb.yj20258888.top

Ruby: public / protected / private
来源：http://mmy.smart0.xyz


<!-- 参考信息 -->