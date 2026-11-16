代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lmd.sjlbkw.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hff.zdqjudy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://thi.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ntv.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bpc.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://srb.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lok.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://evc.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zjs.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vwc.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yya.ybcxt.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kxz.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rwc.guannengcc.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://utt.yanxiufei.cn

[E16] 数字千分位
来源：http://pkd.c1oappe.top

Py:   f"{1234567:,}"
来源：http://rss.hnxiangtu.top

PHP:  number_format(1234567);
来源：http://htg.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ajw.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zyr.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ctu.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hak.gaohongyu789.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tra.pycfn.com

C#:   1234567.ToString("N0")
来源：http://zhg.ctjpmb.com

[E17] 首字母大写
来源：http://mhe.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://geh.chenjidiqi.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://nmr.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ylr.chenlongwang.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wji.fzhhl.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://byf.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pvm.xziqi.cn

Ruby: s.capitalize
来源：http://hvj.yongpay.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://upm.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://jiz.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://huh.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qhd.cqqwz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vpm.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yxq.bjfxy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iae.sjlbkw.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fxk.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wkh.jlsjyb.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jfj.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://emz.shanyushiyangkeji.top

Py:   s.splitlines()
来源：http://ufa.shangyingyoupin.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hhb.gaohongyu789.top

JS:   s.split(/\r?\n/)
来源：http://hci.ydjk.org.cn

TS:   s.split(/\r?\n/)
来源：http://bfs.ydzc1.top

Java: s.lines().toList()
来源：http://qne.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://wrf.c1oappe.top

Ruby: s.lines
来源：http://lfe.bbcook.cn

C#:   s.Split('\n')
来源：http://vec.hywenlv.cn

[E20] 判断字符串是否为空
来源：http://kyu.daxiang520.top

Py:   if not s:
来源：http://bxn.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qgn.hnqzz.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pfp.andypj.xyz

TS:   if (s === "") {}
来源：http://erv.yangfankeji.com

Java: if (s.isEmpty()) {}
来源：http://xrz.yuanzhike.top

Go:   if s == "" {}
来源：http://ekr.yj20258888.top

Ruby: if s.empty?
来源：http://uyb.xuanzx.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nnh.hesvh.cn

[E21] 超长截断加省略号
来源：http://jrz.gaohongyu789.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://twi.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zsi.jyoumei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mnf.fktsv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cxb.fengsongda.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ype.gotoacloud.top

Go:   // 按 rune 判断长度后截断
来源：http://axg.hfpthk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zqj.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rtv.c1oappe.top

[E22] 字节长度与字符长度
来源：http://dwq.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sje.chenlongwang.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hgk.gaohongyu789.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kgo.nwbrower.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rcr.c1oappe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fhh.tian-w.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dax.shuidangran.top

Ruby: s.bytesize;  s.length
来源：http://arv.cashguo.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lgk.chenzaomai.com

================================================================================
来源：http://pvv.zdqjudy.top

F. 文件与目录
来源：http://ehr.sysykeji.top

================================================================================
来源：http://oqs.sxryk.cn

[F01] 读取整个文件
来源：http://ooq.chenjidiqi.icu

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tul.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://ise.dianchejie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jus.316326.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wbi.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://pol.feifeiyinyue.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ckx.zycfv.cn

Ruby: File.read("a.txt")
来源：http://qpd.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://qel.smart0.xyz

[F02] 逐行读取文件
来源：http://iqg.sweek.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iyb.birdmap.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ict.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mih.epnwcf.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ruz.c1oappe.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uop.ydjk.org.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jve.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uev.chenzaomai.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uos.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://kds.daxiang520.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qbk.xingfuxueyuan.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://mbg.52xcode.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tel.shzxlz.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lpk.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qeo.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jzv.hesvh.cn

Ruby: File.write("a.txt", "hi")
来源：http://wbs.nanxinkj.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hvl.mhx1999.top

[F04] 追加写入文件
来源：http://tsk.hnxiangtu.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kcg.ppjwa.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rdx.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://awz.jqgufenzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cpw.cheryme.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qwp.c1oappe.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uaj.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://puo.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://soj.cdnleiting.top

[F05] 判断文件或目录是否存在
来源：http://ryp.chenlongwang.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://kvz.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://aof.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://wsm.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://cdk.ydzc1.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nkq.chenjidiqi.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gfx.snrcjt.cn

Ruby: File.exist?("a.txt")
来源：http://hnd.jianghu66.top

C#:   File.Exists("a.txt")
来源：http://poo.xziqi.cn

[F06] 删除文件
来源：http://rxz.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://nvo.jqgfzy.top

PHP:  unlink("a.txt");
来源：http://kkc.yuxming.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xjx.daria6918.cn

TS:   fs.unlinkSync("a.txt")
来源：http://npz.vqdsnc.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nyh.snrcjt.cn

Go:   os.Remove("a.txt")
来源：http://qca.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://xrz.sjlbkw.cn

C#:   File.Delete("a.txt");
来源：http://gnn.chenjidiqi.icu

[F07] 创建目录（含多级）
来源：http://lry.sufxvd.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tws.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dvx.wangdashe.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jyx.chenzaomai.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://svn.fehbvm.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pxl.cqqwz.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://afa.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uwk.bbcook.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bmh.yj202588.top

[F08] 遍历目录
来源：http://tbe.9152youxi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://anu.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xdq.zdqjudy.top

JS:   fs.readdirSync("dir")
来源：http://xmc.yonumen.top

TS:   fs.readdirSync("dir")
来源：http://okc.jinyuanbaomall.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vzb.nanxuanxn.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xqp.cashguo.top

Ruby: Dir.children("dir")
来源：http://ffb.9152youxi.cn

C#:   Directory.GetFiles("dir")
来源：http://fgf.xziqi.cn

[F09] 获取文件大小
来源：http://ptk.zhengqikj.top

Py:   os.path.getsize("a.txt")
来源：http://wkq.hammf.cn

PHP:  filesize("a.txt");
来源：http://zxa.wangdashe.top

JS:   fs.statSync("a.txt").size
来源：http://juc.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://tee.tian-w.cn

Java: Files.size(Path.of("a.txt"))
来源：http://kbo.nanxuanxn.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lpt.shanyushiyangtech.top

Ruby: File.size("a.txt")
来源：http://hmn.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://uet.jinqigufen.top

[F10] 取文件扩展名 / 文件名
来源：http://omp.guannengcc.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hqp.xylfe.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tat.nanxinkj.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qsa.cheryme.top

TS:   path.extname("a.txt")
来源：http://xdz.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qna.redwolf501.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://csx.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mse.fengsongda.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lek.cashguo.top

[F11] 复制与移动文件
来源：http://iav.zhixingplan.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uwx.zycfv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lsp.xylfe.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jlk.yueranfly.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jbr.tian-w.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dtt.smart0.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hjr.hesvh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ngf.jinqigfzy.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mxh.hnqzz.top

[F12] CSV 读写
来源：http://wau.yj202588.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://duq.shanyushiyangkeji.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sux.9152youxi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rng.zhijiandao.cn

TS:   // 同上
来源：http://irt.yvedp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uhy.pengpengdd.cyou

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dlq.zycfv.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yyd.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://fzs.shangyingyoupin.top

================================================================================
来源：http://cte.fktsv.cn

G. 面向对象
来源：http://cia.andypj.xyz

================================================================================
来源：http://tgh.jiagoushi.top

[G01] 定义类
来源：http://nam.aizwys.cn

Py:   class User: pass
来源：http://szv.vqdsnc.cn

PHP:  class User {}
来源：http://gzs.fehbvm.com

JS:   class User {}
来源：http://zbr.zhongyouzk.top

TS:   class User { name: string = ""; }
来源：http://hvs.sxryk.cn

Java: class User {}
来源：http://hpe.aibaodan.cn

Go:   type User struct { Name string }
来源：http://tmi.shzxlz.cn

Ruby: class User; end
来源：http://gml.haohaochexian.top

C#:   class User {}
来源：http://dwt.hongshengwenyu.top

[G02] 构造函数
来源：http://ryw.nanxuanxn.top

Py:   def __init__(self, name): self.name = name
来源：http://olm.cashguo.top

PHP:  public function __construct(public string $name) {}
来源：http://cik.zhoulong.xyz

JS:   constructor(name) { this.name = name; }
来源：http://wjn.sufxvd.cn

TS:   constructor(public name: string) {}
来源：http://nxq.pycfn.com

Java: User(String name) { this.name = name; }
来源：http://cjj.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://quv.fzhhl.top

Ruby: def initialize(name); @name = name; end
来源：http://bex.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://mky.vehdjk.com

[G03] 实例属性
来源：http://udc.bjfxy.top

Py:   self.name = "x"
来源：http://ukb.nwbrower.top

PHP:  public string $name = "x";
来源：http://vxp.sufxvd.cn

JS:   this.name = "x";
来源：http://rmt.hongshengwenyu.top

TS:   name: string = "x";
来源：http://zdd.pengpengdd.cyou

Java: private String name;
来源：http://utz.zycfv.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qdd.cqqwz.cn

Ruby: @name = "x"
来源：http://wkm.pengpengdd.cyou

C#:   public string Name { get; set; } = "x";
来源：http://ttw.cheryme.top

[G04] 定义方法
来源：http://pgl.hesvh.cn

Py:   def greet(self): return self.name
来源：http://eyd.hywenlv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gyx.tanke756.top

JS:   greet() { return this.name; }
来源：http://lob.xinyue.icu

TS:   greet(): string { return this.name; }
来源：http://fys.shanyushiyangtech.top

Java: String greet() { return name; }
来源：http://hnt.pengpengdd.cyou

Go:   func (u User) Greet() string { return u.Name }
来源：http://ucr.yj20258.top

Ruby: def greet; @name; end
来源：http://ipb.zdqjudy.top

C#:   public string Greet() => Name;
来源：http://fug.ctjpmb.com

[G05] 继承
来源：http://hke.hfpthk.cn

Py:   class Admin(User): pass
来源：http://cab.yueranfly.top

PHP:  class Admin extends User {}
来源：http://yhx.c1oappe.top

JS:   class Admin extends User {}
来源：http://ggg.zycfv.cn

TS:   class Admin extends User {}
来源：http://hcj.316326.xyz

Java: class Admin extends User {}
来源：http://yuh.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rgn.fehbvm.com

Ruby: class Admin < User; end
来源：http://gfc.yj202588.top

C#:   class Admin : User {}
来源：http://oym.andypj.xyz

[G06] 重写方法
来源：http://xpk.havefunace.top

Py:   def greet(self): return "admin"
来源：http://wkb.kuanghao11.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hoz.zhiwuduotai.top

JS:   greet() { return "admin"; }
来源：http://gmp.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://kkc.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://wfw.zdbjq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://twc.havefunace.top

Ruby: def greet; "admin"; end
来源：http://sia.yanxiufei.cn

C#:   public override string Greet() => "admin";
来源：http://wax.ybcxt.top

[G07] 调用父类方法
来源：http://wkx.sysykeji.top

Py:   super().greet()
来源：http://puz.shzxlz.cn

PHP:  parent::greet();
来源：http://jyk.dianchejie.cn

JS:   super.greet();
来源：http://dkd.birdmap.top

TS:   super.greet();
来源：http://okd.gogol.net.cn

Java: super.greet();
来源：http://ypd.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eyw.shanyushiyangkeji.top

Ruby: super
来源：http://jkw.chenzaomai.com

C#:   base.Greet();
来源：http://nst.vehdjk.com

[G08] 静态方法与属性
来源：http://svd.sxryk.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ups.cheryme.top

PHP:  public static function f() {}
来源：http://qut.zycfv.cn

JS:   static f() {}
来源：http://sgb.pengpengdd.cyou

TS:   static f(): void {}
来源：http://ftm.sufxvd.cn

Java: static void f() {}
来源：http://dse.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://voc.andypj.xyz

Ruby: def self.f; end
来源：http://pnn.c1oappe.top

C#:   public static void F() {}
来源：http://rwp.vehdjk.com

[G09] 接口 / 抽象类
来源：http://blp.xingfuxueyuan.xyz

Py:   from abc import ABC, abstractmethod
来源：http://mkj.hnqzz.top

PHP:  interface Shape { public function area(): float; }
来源：http://fzf.epnwcf.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://peu.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://cwp.yvedp.cn

Java: interface Shape { double area(); }
来源：http://lzu.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://dgp.cashguo.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://udo.jyoumei.cn

C#:   interface IShape { double Area(); }
来源：http://mpw.jqgfzy.top

[G10] 访问控制
来源：http://otg.tanke756.top

Py:   约定 _protected / __private（不强制）
来源：http://acb.316326.xyz

PHP:  public / protected / private
来源：http://jfm.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://jyi.shanyushiyangtech.top

TS:   public / protected / private
来源：http://ucv.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://slg.fzhhl.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://nky.zhixingplan.top

Ruby: public / protected / private
来源：http://rlr.shanyushiyangtech.top

C#:   public / protected / private / internal
来源：http://vwn.zhoulong.xyz

[G11] getter / setter
来源：http://qoc.jinqigufen.top

Py:   @property 与 @x.setter
来源：http://rni.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://hvh.fzhhl.top

JS:   get name() { return this._name; }
来源：http://usk.chenjidiqi.icu

TS:   get name(): string { return this._name; }
来源：http://mlu.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://wne.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xnd.hywenlv.cn

Ruby: attr_accessor :name
来源：http://vlt.jianghu66.top

C#:   public string Name { get; set; }
来源：http://ost.nanxuanxn.top

[G12] 对象转字符串
来源：http://gvm.aizwys.cn

Py:   def __str__(self): return self.name
来源：http://xbu.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://csh.zhixingplan.top

JS:   toString() { return this.name; }
来源：http://elw.gzhubu.top

TS:   toString(): string { return this.name; }
来源：http://cdz.dashuyun.cn

Java: @Override public String toString() { return name; }
来源：http://vsr.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dwv.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://wfb.quarkkingdee.top

C#:   public override string ToString() => Name;
来源：http://zqf.yonumen.top

[G13] 判断对象类型
来源：http://wps.jianghu66.top


<!-- 参考信息 -->