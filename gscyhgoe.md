代发 wailian999

Go:   strings.Count(s, "a")
来源：http://vdh.316326.xyz

Ruby: s.count("a")
来源：http://jvm.jqgufenzy.top

C#:   s.Count(c => c == 'a')
来源：http://bjm.xuanzx.com

[E13] 逐字符遍历
来源：http://bsz.zhijiandao.cn

Py:   for ch in s: print(ch)
来源：http://bky.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gtn.bjfxy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ipb.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://hce.jinyuanbaomall.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://viy.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rdf.fengsongda.top

Ruby: s.each_char { |ch| puts ch }
来源：http://vcu.bjfxy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cpi.shanyushiyangtech.top

[E14] URL 编码与 Base64
来源：http://ydu.zdqjudy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dvb.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://abz.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qdd.yj202588.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iid.vehdjk.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tlc.gotoacloud.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ggg.yangfankeji.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yfb.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fsd.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://gcl.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gvf.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qpp.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ixq.jinqigfzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ltk.gzhubu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nuv.hnqzz.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jbl.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hhb.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://how.andypj.xyz

[E16] 数字千分位
来源：http://rus.yongpay.top

Py:   f"{1234567:,}"
来源：http://chd.yj202588.top

PHP:  number_format(1234567);
来源：http://kgk.sweek.top

JS:   (1234567).toLocaleString("en-US")
来源：http://vdf.jinqigufen.top

TS:   (1234567).toLocaleString("en-US")
来源：http://idz.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gqw.c1oappe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qar.jyoumei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nbi.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://umk.haohaochexian.top

[E17] 首字母大写
来源：http://rtl.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vfw.jiagoushi.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://vus.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zhi.fzhhl.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lga.yj20258.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dka.jqgufenzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tki.zhoulong.xyz

Ruby: s.capitalize
来源：http://ama.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lnv.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://cxv.ctjpmb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lhz.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pgd.gzhubu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://egn.yj20258.top

TS:   tpl.replaceAll("{name}", name)
来源：http://dof.fzhhl.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yrd.yvedp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fwv.hnqzz.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kgm.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tli.hammf.cn

[E19] 多行文本按行拆分
来源：http://ubt.xuetiantiany.cn

Py:   s.splitlines()
来源：http://kkq.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rzp.52xcode.cn

JS:   s.split(/\r?\n/)
来源：http://nlx.ctjpmb.com

TS:   s.split(/\r?\n/)
来源：http://yin.tianlin.xyz

Java: s.lines().toList()
来源：http://bbx.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://fvg.epnwcf.com

Ruby: s.lines
来源：http://frd.hammf.cn

C#:   s.Split('\n')
来源：http://dtw.wangdashe.top

[E20] 判断字符串是否为空
来源：http://avg.fzhhl.top

Py:   if not s:
来源：http://slz.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tue.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jhm.tian-w.cn

TS:   if (s === "") {}
来源：http://wqb.ywan-chungtsiang.top

Java: if (s.isEmpty()) {}
来源：http://dsv.mhx1999.top

Go:   if s == "" {}
来源：http://lrj.jinghuilouyu.cn

Ruby: if s.empty?
来源：http://caa.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ujt.0kj1m.cn

[E21] 超长截断加省略号
来源：http://ynh.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nmj.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vnp.gzhubu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dkw.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdt.gzhubu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dzj.52xcode.cn

Go:   // 按 rune 判断长度后截断
来源：http://ohb.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jik.jinghuilouyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ltq.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://odp.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://scb.snrcjt.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pda.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yjf.guowangkeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jjw.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bfj.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tru.nanxinkj.top

Ruby: s.bytesize;  s.length
来源：http://cfe.redwolf501.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ukz.jqgufenzy.top

================================================================================
来源：http://zuq.yuxming.cn

F. 文件与目录
来源：http://zxw.hnqzz.top

================================================================================
来源：http://kqn.fanxiaobao.xyz

[F01] 读取整个文件
来源：http://jre.ctjpmb.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ebf.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://dtx.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dlc.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xnx.feifeiyinyue.top

Java: Files.readString(Path.of("a.txt"))
来源：http://srw.andypj.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sjc.fktsv.cn

Ruby: File.read("a.txt")
来源：http://eyq.haohaochexian.top

C#:   File.ReadAllText("a.txt");
来源：http://whw.cheryme.top

[F02] 逐行读取文件
来源：http://wmx.yangfankeji.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mvk.yangfankeji.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://czc.daxiang520.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qra.ppjwa.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxf.nanxuanxn.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ouu.pengpengdd.cyou

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uyf.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lff.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hcf.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://yue.aizwys.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://afa.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cgd.guowangkeji.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nxb.jinghuilouyu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zeg.chenjidiqi.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://iun.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qhn.yj20258.top

Ruby: File.write("a.txt", "hi")
来源：http://wuv.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aro.guowangkeji.top

[F04] 追加写入文件
来源：http://rfi.yangfankeji.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gah.yj20258.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oct.cashguo.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rlj.gotoacloud.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tjn.zhaomingkeji.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dtj.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kyd.aibaodan.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uwe.yfazqb.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kqy.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://awb.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hbm.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://gyt.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://pny.shanyushiyangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://ywf.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://fcp.pengpengdd.cyou

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hop.zhoulong.xyz

Ruby: File.exist?("a.txt")
来源：http://mfl.chenlongwang.top

C#:   File.Exists("a.txt")
来源：http://rhv.zhiwuduotai.top

[F06] 删除文件
来源：http://mpo.guannengcc.top

Py:   os.remove("a.txt")
来源：http://wat.zdbjq.cn

PHP:  unlink("a.txt");
来源：http://mvg.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uft.9152youxi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://czh.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lwp.gotoacloud.top

Go:   os.Remove("a.txt")
来源：http://kvq.52xcode.cn

Ruby: File.delete("a.txt")
来源：http://deo.chenlongwang.top

C#:   File.Delete("a.txt");
来源：http://tho.zhengqikj.top

[F07] 创建目录（含多级）
来源：http://qho.zhoulong.xyz

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dle.vqdsnc.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pse.ehwqpu.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jec.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rqe.xingfuxueyuan.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mxp.daxiang520.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qtq.snrcjt.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dda.tarul.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qos.zycfv.cn

[F08] 遍历目录
来源：http://gfh.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://eyv.gzhubu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ffs.xuanzx.com

JS:   fs.readdirSync("dir")
来源：http://xoq.sweek.top

TS:   fs.readdirSync("dir")
来源：http://vhd.wangdashe.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wyc.bbcook.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://frl.yongpay.top

Ruby: Dir.children("dir")
来源：http://usc.0kj1m.cn

C#:   Directory.GetFiles("dir")
来源：http://pgp.bbcook.cn

[F09] 获取文件大小
来源：http://pog.quarkkingdee.top

Py:   os.path.getsize("a.txt")
来源：http://coh.shanyushiyangkeji.top

PHP:  filesize("a.txt");
来源：http://cli.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://uqd.tianlin.xyz

TS:   fs.statSync("a.txt").size
来源：http://olt.ppjwa.cn

Java: Files.size(Path.of("a.txt"))
来源：http://osf.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oim.jinqigufen.top

Ruby: File.size("a.txt")
来源：http://utr.havefunace.top

C#:   new FileInfo("a.txt").Length
来源：http://vtc.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://gew.yvedp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fum.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rms.xinyue.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kzq.yonumen.top

TS:   path.extname("a.txt")
来源：http://fsc.feifeiyinyue.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fng.daria6918.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://joo.uphjek.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uur.zhongyouzk.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uga.tianlin.xyz

[F11] 复制与移动文件
来源：http://zgm.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://suu.cashguo.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mal.daria6918.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://etq.haohaochexian.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vmi.redwolf501.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ofm.sweek.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bah.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://aht.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cpc.shuidangran.top

[F12] CSV 读写
来源：http://nqe.xingfuxueyuan.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bry.ydzc1.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mxb.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dxk.yj20258888.top

TS:   // 同上
来源：http://xuc.zhiwuduotai.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lkt.fzhhl.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ois.tianlin.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://onz.vehdjk.com

C#:   // 无内置：用 CsvHelper 库
来源：http://lkn.tianlin.xyz

================================================================================
来源：http://max.bbcook.cn

G. 面向对象
来源：http://bxk.gzhubu.top

================================================================================
来源：http://vrg.yonumen.top

[G01] 定义类
来源：http://kta.xylfe.cn

Py:   class User: pass
来源：http://ree.yj20258.top

PHP:  class User {}
来源：http://cvt.wangshuangyany.cn

JS:   class User {}
来源：http://evr.gogol.net.cn

TS:   class User { name: string = ""; }
来源：http://cny.hesvh.cn

Java: class User {}
来源：http://shq.uphjek.com

Go:   type User struct { Name string }
来源：http://oya.yangfankeji.com

Ruby: class User; end
来源：http://ups.ywan-chungtsiang.top

C#:   class User {}
来源：http://gka.kuanghao11.cn

[G02] 构造函数
来源：http://hdk.jyoumei.cn

Py:   def __init__(self, name): self.name = name
来源：http://yht.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://lob.uphjek.com

JS:   constructor(name) { this.name = name; }
来源：http://vrn.snrcjt.cn

TS:   constructor(public name: string) {}
来源：http://ecs.cdnleiting.top

Java: User(String name) { this.name = name; }
来源：http://qrj.fzhhl.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://qkc.316326.xyz

Ruby: def initialize(name); @name = name; end
来源：http://syl.hywenlv.cn

C#:   public User(string name) { Name = name; }
来源：http://vne.fehbvm.com

[G03] 实例属性
来源：http://hhz.gogol.net.cn

Py:   self.name = "x"
来源：http://aku.hnxiangtu.top

PHP:  public string $name = "x";
来源：http://fyl.cdnleiting.top

JS:   this.name = "x";
来源：http://ood.jinqigufen.top

TS:   name: string = "x";
来源：http://twp.xinyue.icu

Java: private String name;
来源：http://dfm.snrcjt.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fet.guowangkeji.top

Ruby: @name = "x"
来源：http://nvb.zhoulong.xyz

C#:   public string Name { get; set; } = "x";
来源：http://tnw.cheryme.top

[G04] 定义方法
来源：http://niy.fengsongda.top

Py:   def greet(self): return self.name
来源：http://naw.wangdashe.top

PHP:  public function greet(): string { return $this->name; }
来源：http://elb.xuanzx.com

JS:   greet() { return this.name; }
来源：http://dyv.ybcxt.top

TS:   greet(): string { return this.name; }
来源：http://gxy.quarkkingdee.top

Java: String greet() { return name; }
来源：http://qar.wangshuangyany.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dwi.zhengqikj.top

Ruby: def greet; @name; end
来源：http://gbu.ppjwa.cn

C#:   public string Greet() => Name;
来源：http://kwr.cqqwz.cn

[G05] 继承
来源：http://huo.jianghu66.top

Py:   class Admin(User): pass
来源：http://dyx.c1oappe.top

PHP:  class Admin extends User {}
来源：http://qti.yueranfly.top

JS:   class Admin extends User {}
来源：http://czl.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://cdz.jianghu66.top

Java: class Admin extends User {}
来源：http://btm.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rxx.vehdjk.com

Ruby: class Admin < User; end
来源：http://gtn.bbcook.cn

C#:   class Admin : User {}
来源：http://hij.ydjk.org.cn

[G06] 重写方法
来源：http://yvj.bbcook.cn

Py:   def greet(self): return "admin"
来源：http://ddg.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gtr.zhaomingkeji.xyz

JS:   greet() { return "admin"; }
来源：http://snj.ydjk.org.cn

TS:   greet(): string { return "admin"; }
来源：http://hab.yfazqb.com

Java: @Override String greet() { return "admin"; }
来源：http://lmu.guannengcc.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yzy.bjfxy.top

Ruby: def greet; "admin"; end
来源：http://ucb.jlsjyb.cn

C#:   public override string Greet() => "admin";
来源：http://xib.hesvh.cn

[G07] 调用父类方法
来源：http://vuc.tianlin.xyz

Py:   super().greet()
来源：http://moy.xuetiantiany.cn

PHP:  parent::greet();
来源：http://tyv.havefunace.top

JS:   super.greet();
来源：http://yfn.tianlin.xyz

TS:   super.greet();
来源：http://kgl.jinqigufen.top

Java: super.greet();
来源：http://lrf.haohaochexian.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xef.ydzc1.top

Ruby: super
来源：http://cfl.jqgufenzy.top

C#:   base.Greet();
来源：http://qpv.nanxuanxn.top

[G08] 静态方法与属性
来源：http://kbk.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vea.yonumen.top

PHP:  public static function f() {}
来源：http://cqs.shzxlz.cn

JS:   static f() {}
来源：http://krq.cashguo.top

TS:   static f(): void {}
来源：http://uzk.shzxlz.cn

Java: static void f() {}
来源：http://dkp.hnxiangtu.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ads.vqdsnc.cn

Ruby: def self.f; end
来源：http://bbq.sjlbkw.cn

C#:   public static void F() {}
来源：http://uga.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://uhu.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://shz.smart0.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://gzj.jqgfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pxu.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://nso.guowangkeji.top

Java: interface Shape { double area(); }
来源：http://lba.birdmap.top

Go:   type Shape interface { Area() float64 }
来源：http://urf.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gyd.chenjidiqi.icu

C#:   interface IShape { double Area(); }
来源：http://gva.zhixingplan.top

[G10] 访问控制
来源：http://vyz.fzhhl.top

Py:   约定 _protected / __private（不强制）
来源：http://atd.ctjpmb.com

PHP:  public / protected / private
来源：http://lck.bjfxy.top

JS:   #private 字段；其余公开
来源：http://mrx.fzhhl.top

TS:   public / protected / private
来源：http://kcu.hnxiangtu.top

Java: public / protected / private / 默认包级
来源：http://kfg.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://mxc.tarul.cn

Ruby: public / protected / private
来源：http://bso.fktsv.cn

C#:   public / protected / private / internal
来源：http://xvp.yanxiufei.cn

[G11] getter / setter
来源：http://jrm.52xcode.cn

Py:   @property 与 @x.setter
来源：http://qfs.andypj.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://gze.zhongyouzk.top


<!-- 参考信息 -->