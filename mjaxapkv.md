代发 wailian999

[E14] URL 编码与 Base64
来源：http://xfw.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dxe.yj202588.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nua.meibo888.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://emq.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xzk.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xky.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://eqg.birdmap.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sgc.mhx1999.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dvz.yangfankeji.com

[E15] HTML 转义 / 反转义
来源：http://qkl.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rht.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wcn.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qey.fanxiaobao.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://yko.wangdashe.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kvf.zhijiandao.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://eqy.9152youxi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lph.nanxinkj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tiv.jianghu66.top

[E16] 数字千分位
来源：http://ewr.daxiang520.top

Py:   f"{1234567:,}"
来源：http://fdn.fanxiaobao.xyz

PHP:  number_format(1234567);
来源：http://pek.hfpthk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jvy.nwbrower.top

TS:   (1234567).toLocaleString("en-US")
来源：http://waq.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wzm.vqdsnc.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nzb.shanyushiyangtech.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cqx.ybcxt.top

C#:   1234567.ToString("N0")
来源：http://lrn.yfazqb.com

[E17] 首字母大写
来源：http://ioo.gotoacloud.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fxu.ctjpmb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://viz.hywenlv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lcs.jyoumei.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tmh.zhongyouzk.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bpp.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jke.pycfn.com

Ruby: s.capitalize
来源：http://exs.gogol.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hhr.cheryme.top

[E18] 模板占位符替换
来源：http://fov.redwolf501.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qwi.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zwz.tianlin.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://nrt.fengsongda.top

TS:   tpl.replaceAll("{name}", name)
来源：http://boe.fengsongda.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ggv.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jbk.sysykeji.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lfh.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://buf.smart0.xyz

[E19] 多行文本按行拆分
来源：http://ypb.daxiang520.top

Py:   s.splitlines()
来源：http://uco.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hfm.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://stg.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://apz.snrcjt.cn

Java: s.lines().toList()
来源：http://qre.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://ezj.yj20258888.top

Ruby: s.lines
来源：http://hrf.zdqjudy.top

C#:   s.Split('\n')
来源：http://avx.redwolf501.top

[E20] 判断字符串是否为空
来源：http://zjs.yuxming.cn

Py:   if not s:
来源：http://jww.shuidangran.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jed.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uwt.yj20258.top

TS:   if (s === "") {}
来源：http://bmw.smart0.xyz

Java: if (s.isEmpty()) {}
来源：http://vqn.shuidangran.top

Go:   if s == "" {}
来源：http://jqt.hammf.cn

Ruby: if s.empty?
来源：http://kcn.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nul.haohaochexian.top

[E21] 超长截断加省略号
来源：http://amy.havefunace.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xzs.svipenyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pvz.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bde.aizwys.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qeg.hammf.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hii.yuanzhike.top

Go:   // 按 rune 判断长度后截断
来源：http://gzf.hysaishi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vlm.tian-w.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qvn.xuetiantiany.cn

[E22] 字节长度与字符长度
来源：http://szx.sxryk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qsy.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wqj.xylfe.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yqy.tarul.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vrm.svipenyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mvw.hywenlv.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://udp.iojbl.cn

Ruby: s.bytesize;  s.length
来源：http://qgv.yj202588.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jdl.yuanzhike.top

================================================================================
来源：http://oed.hcnkem.com

F. 文件与目录
来源：http://nbu.ywan-chungtsiang.top

================================================================================
来源：http://ulp.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://jud.hnqzz.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://izp.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://xtd.ydzc1.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://iri.wangshuangyany.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qqi.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ihn.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gfw.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://qyc.smart0.xyz

C#:   File.ReadAllText("a.txt");
来源：http://cud.cashguo.top

[F02] 逐行读取文件
来源：http://rbo.pycfn.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rhy.zdbjq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vgz.hongshengwenyu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://edy.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zxo.yuanzhike.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rku.chenlongwang.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jsc.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jpt.vqdsnc.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dal.feifeiyinyue.top

[F03] 写入文件（覆盖）
来源：http://edl.meibo888.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wow.gaohongyu789.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ryr.xinyue.icu

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jnw.nanxuanxn.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tdb.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ipj.yj202588.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lbi.wangdashe.top

Ruby: File.write("a.txt", "hi")
来源：http://eej.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sco.aizwys.cn

[F04] 追加写入文件
来源：http://ioa.fehbvm.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gkg.vqdsnc.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qgc.nwbrower.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uxg.gaohongyu789.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nvf.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://evn.shanyushiyangtech.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kmw.316326.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gnr.shanyushiyangtech.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hrt.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://twh.yonumen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://icg.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://sii.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://usp.hongshengwenyu.top

TS:   fs.existsSync("a.txt")
来源：http://snx.c1oappe.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ugr.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jbw.shangyingyoupin.top

Ruby: File.exist?("a.txt")
来源：http://gpr.hywenlv.cn

C#:   File.Exists("a.txt")
来源：http://gum.jyoumei.cn

[F06] 删除文件
来源：http://ocu.sweek.top

Py:   os.remove("a.txt")
来源：http://mao.ppjwa.cn

PHP:  unlink("a.txt");
来源：http://rpy.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://hyn.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://ean.9152youxi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uvx.chenlongwang.top

Go:   os.Remove("a.txt")
来源：http://jmf.jqgfzy.top

Ruby: File.delete("a.txt")
来源：http://led.sufxvd.cn

C#:   File.Delete("a.txt");
来源：http://eck.iojbl.cn

[F07] 创建目录（含多级）
来源：http://aho.gogol.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fsg.xinyue.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uwp.zhaomingkeji.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vqe.redwolf501.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://anj.gzhubu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://abb.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://yjd.tanke756.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ptq.fanxiaobao.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmq.c1oappe.top

[F08] 遍历目录
来源：http://smv.shzxlz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mtq.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gbc.meibo888.top

JS:   fs.readdirSync("dir")
来源：http://jbj.hnxiangtu.top

TS:   fs.readdirSync("dir")
来源：http://hqx.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://quq.gotoacloud.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://pnv.vehdjk.com

Ruby: Dir.children("dir")
来源：http://syu.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://oyq.shangyingyoupin.top

[F09] 获取文件大小
来源：http://fip.hongshengwenyu.top

Py:   os.path.getsize("a.txt")
来源：http://zkz.nanxinkj.top

PHP:  filesize("a.txt");
来源：http://pie.pengpengdd.cyou

JS:   fs.statSync("a.txt").size
来源：http://ypi.ppjwa.cn

TS:   fs.statSync("a.txt").size
来源：http://ygk.daria6918.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uht.quarkkingdee.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://stp.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://wnt.zhoulong.xyz

C#:   new FileInfo("a.txt").Length
来源：http://rjc.tianlin.xyz

[F10] 取文件扩展名 / 文件名
来源：http://cjj.chenlongwang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mus.dianchejie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ivi.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mzm.zycfv.cn

TS:   path.extname("a.txt")
来源：http://mgm.zhengqikj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fnv.yongpay.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ukv.cucudq.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://icp.gzhubu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rol.hcnkem.com

[F11] 复制与移动文件
来源：http://rpb.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jnf.fanxiaobao.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fms.wangdashe.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lhs.shanyushiyangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sks.hcnkem.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wqg.hcnkem.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xbh.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hnt.tarul.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://osc.xuanzx.com

[F12] CSV 读写
来源：http://oek.sjlbkw.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blc.ehwqpu.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vvd.quarkkingdee.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://awd.yj20258.top

TS:   // 同上
来源：http://lwr.pengpengdd.cyou

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bso.jinghuilouyu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yjf.ivvv.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lkv.andypj.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://tjl.dashuyun.cn

================================================================================
来源：http://jzv.zhiwuduotai.top

G. 面向对象
来源：http://vkd.yanxiufei.cn

================================================================================
来源：http://jcx.pycfn.com

[G01] 定义类
来源：http://fqj.daria6918.cn

Py:   class User: pass
来源：http://pow.iojbl.cn

PHP:  class User {}
来源：http://bob.fengsongda.top

JS:   class User {}
来源：http://lty.zhixingplan.top

TS:   class User { name: string = ""; }
来源：http://olv.feifeiyinyue.top

Java: class User {}
来源：http://mbj.zhongyouzk.top

Go:   type User struct { Name string }
来源：http://jfk.hnqzz.top

Ruby: class User; end
来源：http://fhq.birdmap.top

C#:   class User {}
来源：http://qem.hongshengwenyu.top

[G02] 构造函数
来源：http://vvb.zhiwuduotai.top

Py:   def __init__(self, name): self.name = name
来源：http://kae.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://mfj.gaohongyu789.top

JS:   constructor(name) { this.name = name; }
来源：http://ffr.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://xky.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://riu.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ovn.yj202588.top

Ruby: def initialize(name); @name = name; end
来源：http://tav.fktsv.cn

C#:   public User(string name) { Name = name; }
来源：http://uhq.ydzc1.top

[G03] 实例属性
来源：http://cly.sysykeji.top

Py:   self.name = "x"
来源：http://mpo.sweek.top

PHP:  public string $name = "x";
来源：http://sdu.kuanghao11.cn

JS:   this.name = "x";
来源：http://joa.yuxming.cn

TS:   name: string = "x";
来源：http://obh.wangshuangyany.cn

Java: private String name;
来源：http://aef.chenjidiqi.icu

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tyc.cheryme.top

Ruby: @name = "x"
来源：http://jmq.0kj1m.cn

C#:   public string Name { get; set; } = "x";
来源：http://ngh.xylfe.cn

[G04] 定义方法
来源：http://sne.tarul.cn

Py:   def greet(self): return self.name
来源：http://huf.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ohe.tianlin.xyz

JS:   greet() { return this.name; }
来源：http://xjb.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://lin.jinghuilouyu.cn

Java: String greet() { return name; }
来源：http://gmj.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aoo.nanxuanxn.top

Ruby: def greet; @name; end
来源：http://djb.jianghu66.top

C#:   public string Greet() => Name;
来源：http://kol.zhaomingkeji.xyz

[G05] 继承
来源：http://ywe.haohaochexian.top

Py:   class Admin(User): pass
来源：http://tyz.fengsongda.top

PHP:  class Admin extends User {}
来源：http://ttg.snrcjt.cn

JS:   class Admin extends User {}
来源：http://wob.vehdjk.com

TS:   class Admin extends User {}
来源：http://nzh.0kj1m.cn

Java: class Admin extends User {}
来源：http://gad.tian-w.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sss.jiagoushi.top

Ruby: class Admin < User; end
来源：http://ieb.bjfxy.top

C#:   class Admin : User {}
来源：http://vjv.jianghu66.top

[G06] 重写方法
来源：http://dob.316326.xyz

Py:   def greet(self): return "admin"
来源：http://ufj.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jmz.wangshuangyany.cn

JS:   greet() { return "admin"; }
来源：http://azr.cucudq.cn

TS:   greet(): string { return "admin"; }
来源：http://xmb.ybcxt.top

Java: @Override String greet() { return "admin"; }
来源：http://vbw.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://egh.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://ufe.zhijiandao.cn

C#:   public override string Greet() => "admin";
来源：http://sfc.sysykeji.top

[G07] 调用父类方法
来源：http://get.cucudq.cn

Py:   super().greet()
来源：http://liz.jyoumei.cn

PHP:  parent::greet();
来源：http://cou.hcnkem.com

JS:   super.greet();
来源：http://nvb.hywenlv.cn

TS:   super.greet();
来源：http://xqw.hnqzz.top

Java: super.greet();
来源：http://bmx.xingfuxueyuan.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://niw.chenjidiqi.icu

Ruby: super
来源：http://bmt.ivvv.top

C#:   base.Greet();
来源：http://gqc.jianghu66.top

[G08] 静态方法与属性
来源：http://bwr.ywan-chungtsiang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://axx.uphjek.com

PHP:  public static function f() {}
来源：http://rrn.fktsv.cn

JS:   static f() {}
来源：http://rpi.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://irs.smart0.xyz

Java: static void f() {}
来源：http://zxq.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ppn.nanxuanxn.top

Ruby: def self.f; end
来源：http://ygy.gzhubu.top

C#:   public static void F() {}
来源：http://zit.snrcjt.cn

[G09] 接口 / 抽象类
来源：http://wiz.zdqjudy.top

Py:   from abc import ABC, abstractmethod
来源：http://mqh.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://efk.mhx1999.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ngr.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://aio.52xcode.cn

Java: interface Shape { double area(); }
来源：http://rcm.fanxiaobao.xyz

Go:   type Shape interface { Area() float64 }
来源：http://ygw.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vqk.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://nrm.zdbjq.cn

[G10] 访问控制
来源：http://zyp.shuidangran.top

Py:   约定 _protected / __private（不强制）
来源：http://ymo.snrcjt.cn

PHP:  public / protected / private
来源：http://ddb.smart0.xyz

JS:   #private 字段；其余公开
来源：http://pze.zhaomingkeji.xyz

TS:   public / protected / private
来源：http://vau.316326.xyz

Java: public / protected / private / 默认包级
来源：http://wtd.zdqjudy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://joe.yvedp.cn

Ruby: public / protected / private
来源：http://xch.zhaomingkeji.xyz

C#:   public / protected / private / internal
来源：http://pwu.yj202588.top

[G11] getter / setter
来源：http://tsx.hcnkem.com

Py:   @property 与 @x.setter
来源：http://aqm.yj20258.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ntp.vehdjk.com

JS:   get name() { return this._name; }
来源：http://ahf.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://heu.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://ykn.zdqjudy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bni.cqqwz.cn

Ruby: attr_accessor :name
来源：http://uik.pengpengdd.cyou

C#:   public string Name { get; set; }
来源：http://yhd.jinghuilouyu.cn

[G12] 对象转字符串
来源：http://zhk.svipenyu.cn

Py:   def __str__(self): return self.name
来源：http://yzz.zhiwuduotai.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://del.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://itr.dianchejie.cn

TS:   toString(): string { return this.name; }
来源：http://bfa.shangyingyoupin.top

Java: @Override public String toString() { return name; }
来源：http://xyn.ydjk.org.cn


<!-- 参考信息 -->