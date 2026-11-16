代发 wailian999

PHP:  substr_count($s, "a");
来源：http://pbv.gotoacloud.top

JS:   s.split("a").length - 1
来源：http://ewj.meibo888.top

TS:   s.split("a").length - 1
来源：http://lvd.yuanzhike.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uov.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://pfc.xuanzx.com

Ruby: s.count("a")
来源：http://pnh.nwbrower.top

C#:   s.Count(c => c == 'a')
来源：http://lgy.cheryme.top

[E13] 逐字符遍历
来源：http://hgg.yj202588.top

Py:   for ch in s: print(ch)
来源：http://jfo.pycfn.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dsr.dashuyun.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jjx.birdmap.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zqv.xinyue.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fpk.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cpe.tarul.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mjs.ywan-chungtsiang.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cak.nanxuanxn.top

[E14] URL 编码与 Base64
来源：http://qnv.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zoz.zycfv.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qdt.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qle.jlsjyb.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zxq.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ijm.andypj.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bul.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vpg.yvedp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://byo.yuxming.cn

[E15] HTML 转义 / 反转义
来源：http://jsy.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jfb.9152youxi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qkx.hysaishi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mwz.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hjk.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bdd.fengsongda.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://afu.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kax.ivvv.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://esx.chenzaomai.com

[E16] 数字千分位
来源：http://mxo.aibaodan.cn

Py:   f"{1234567:,}"
来源：http://god.tianlin.xyz

PHP:  number_format(1234567);
来源：http://okr.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://amq.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://kzv.hnqzz.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sxa.cqqwz.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bzd.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rqy.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://nys.pycfn.com

[E17] 首字母大写
来源：http://lpq.yuanzhike.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kok.meibo888.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://rmd.snrcjt.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bai.sjlbkw.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dhz.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://otw.sufxvd.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yrq.jinyuanbaomall.cn

Ruby: s.capitalize
来源：http://hps.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qbw.guannengcc.top

[E18] 模板占位符替换
来源：http://zfr.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xqx.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gcw.zhixingplan.top

JS:   tpl.replaceAll("{name}", name)
来源：http://oiv.aizwys.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://iqw.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ncr.yongpay.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nhn.kuanghao11.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ihx.wangshuangyany.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mrb.sufxvd.cn

[E19] 多行文本按行拆分
来源：http://kmj.haohaochexian.top

Py:   s.splitlines()
来源：http://mde.zdqjudy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lqk.sufxvd.cn

JS:   s.split(/\r?\n/)
来源：http://emn.cqqwz.cn

TS:   s.split(/\r?\n/)
来源：http://kjx.yj20258888.top

Java: s.lines().toList()
来源：http://ilh.dianchejie.cn

Go:   strings.Split(s, "\n")
来源：http://ucv.jinyuanbaomall.cn

Ruby: s.lines
来源：http://qln.wangdashe.top

C#:   s.Split('\n')
来源：http://acj.hnxiangtu.top

[E20] 判断字符串是否为空
来源：http://fql.zhiwuduotai.top

Py:   if not s:
来源：http://eyl.gogol.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xyp.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mia.redwolf501.top

TS:   if (s === "") {}
来源：http://oji.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://msj.cqqwz.cn

Go:   if s == "" {}
来源：http://xpv.andypj.xyz

Ruby: if s.empty?
来源：http://gfi.ehwqpu.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lzw.yangfankeji.com

[E21] 超长截断加省略号
来源：http://emj.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hos.tanke756.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hmo.andypj.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ycf.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://scx.xinyue.icu

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rxi.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://jmd.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oea.0kj1m.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uie.andypj.xyz

[E22] 字节长度与字符长度
来源：http://kra.gotoacloud.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cnc.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bnj.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nbv.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wvp.ydjk.org.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sam.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uhq.xziqi.cn

Ruby: s.bytesize;  s.length
来源：http://rzi.jinqigufen.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vyi.meibo888.top

================================================================================
来源：http://gzj.9152youxi.cn

F. 文件与目录
来源：http://wzy.ctjpmb.com

================================================================================
来源：http://qch.fktsv.cn

[F01] 读取整个文件
来源：http://tlm.gzhubu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fhc.jinqigfzy.top

PHP:  file_get_contents("a.txt");
来源：http://tmm.cqqwz.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vrb.0kj1m.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tpu.fanxiaobao.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://swi.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fzg.jqgufenzy.top

Ruby: File.read("a.txt")
来源：http://kwd.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://zvj.cdnleiting.top

[F02] 逐行读取文件
来源：http://pqu.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wvz.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vqf.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pwv.uphjek.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ohh.gaohongyu789.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nur.fanxiaobao.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://iku.gogol.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pfs.zdbjq.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ufx.gzhubu.top

[F03] 写入文件（覆盖）
来源：http://wbz.birdmap.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gsl.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://prj.chenlongwang.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tnv.zdqjudy.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ukz.yangfankeji.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fpr.tanke756.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ied.guowangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://oyn.hammf.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://khb.zhengqikj.top

[F04] 追加写入文件
来源：http://ldu.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://glr.daxiang520.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yky.meibo888.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uhg.shanyushiyangkeji.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ltw.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ksw.gotoacloud.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bbn.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kcp.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iww.zhaomingkeji.xyz

[F05] 判断文件或目录是否存在
来源：http://pfh.gzhubu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zez.xziqi.cn

PHP:  file_exists("a.txt");
来源：http://pdt.cashguo.top

JS:   fs.existsSync("a.txt")
来源：http://wva.havefunace.top

TS:   fs.existsSync("a.txt")
来源：http://cqj.yj20258888.top

Java: Files.exists(Path.of("a.txt"))
来源：http://dvt.uphjek.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zvm.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://pms.epnwcf.com

C#:   File.Exists("a.txt")
来源：http://ycl.yangfankeji.com

[F06] 删除文件
来源：http://cdi.52xcode.cn

Py:   os.remove("a.txt")
来源：http://xfg.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://nya.c1oappe.top

JS:   fs.unlinkSync("a.txt")
来源：http://oxb.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nxb.shuidangran.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nha.pycfn.com

Go:   os.Remove("a.txt")
来源：http://kpt.xziqi.cn

Ruby: File.delete("a.txt")
来源：http://qes.havefunace.top

C#:   File.Delete("a.txt");
来源：http://vhp.ybcxt.top

[F07] 创建目录（含多级）
来源：http://vje.ybcxt.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dew.yuanzhike.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ser.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mue.daria6918.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zzr.vehdjk.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bsp.tanke756.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ipu.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cpl.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nvv.ctjpmb.com

[F08] 遍历目录
来源：http://aqz.tanke756.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://iit.jiagoushi.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://glm.hysaishi.cn

JS:   fs.readdirSync("dir")
来源：http://sdx.jinyuanbaomall.cn

TS:   fs.readdirSync("dir")
来源：http://xjg.shanyushiyangkeji.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nvc.tanke756.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://bgl.havefunace.top

Ruby: Dir.children("dir")
来源：http://usf.quarkkingdee.top

C#:   Directory.GetFiles("dir")
来源：http://mxv.svipenyu.cn

[F09] 获取文件大小
来源：http://fde.jianghu66.top

Py:   os.path.getsize("a.txt")
来源：http://jgx.zhongyouzk.top

PHP:  filesize("a.txt");
来源：http://kwj.fzhhl.top

JS:   fs.statSync("a.txt").size
来源：http://ind.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://nvm.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://bkl.andypj.xyz

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vdh.guowangkeji.top

Ruby: File.size("a.txt")
来源：http://avo.zhijiandao.cn

C#:   new FileInfo("a.txt").Length
来源：http://lxu.uphjek.com

[F10] 取文件扩展名 / 文件名
来源：http://yqe.sjlbkw.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yph.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qrq.fehbvm.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zmv.yj20258888.top

TS:   path.extname("a.txt")
来源：http://anv.andypj.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gmw.jqgufenzy.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ccu.yangfankeji.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yyy.shanyushiyangtech.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jun.aibaodan.cn

[F11] 复制与移动文件
来源：http://wco.zhengqikj.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mhf.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jby.cqqwz.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dur.tarul.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://leu.birdmap.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://iuf.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://viw.zhixingplan.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kzb.wangshuangyany.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rkr.svipenyu.cn

[F12] CSV 读写
来源：http://ynp.yonumen.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ocj.jinqigfzy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wht.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ktw.xuanzx.com

TS:   // 同上
来源：http://rgx.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fja.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://omy.jyoumei.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fgb.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nnr.fktsv.cn

================================================================================
来源：http://lhp.jiagoushi.top

G. 面向对象
来源：http://mks.zhengqikj.top

================================================================================
来源：http://hgo.daxiang520.top

[G01] 定义类
来源：http://bir.guannengcc.top

Py:   class User: pass
来源：http://mam.yj20258888.top

PHP:  class User {}
来源：http://ktz.sufxvd.cn

JS:   class User {}
来源：http://gik.guowangkeji.top

TS:   class User { name: string = ""; }
来源：http://grz.andypj.xyz

Java: class User {}
来源：http://zip.yonumen.top

Go:   type User struct { Name string }
来源：http://hav.wangdashe.top

Ruby: class User; end
来源：http://jkp.jyoumei.cn

C#:   class User {}
来源：http://shv.jlsjyb.cn

[G02] 构造函数
来源：http://kmt.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://ttk.jinqigufen.top

PHP:  public function __construct(public string $name) {}
来源：http://pxr.shanyushiyangtech.top

JS:   constructor(name) { this.name = name; }
来源：http://bma.redwolf501.top

TS:   constructor(public name: string) {}
来源：http://cjr.nanxinkj.top

Java: User(String name) { this.name = name; }
来源：http://rel.bbcook.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://giq.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://zzh.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://mxz.xinyue.icu

[G03] 实例属性
来源：http://iux.wangdashe.top

Py:   self.name = "x"
来源：http://kdo.wangdashe.top

PHP:  public string $name = "x";
来源：http://yqp.guowangkeji.top

JS:   this.name = "x";
来源：http://izq.yvedp.cn

TS:   name: string = "x";
来源：http://pxx.zhaomingkeji.xyz

Java: private String name;
来源：http://vyh.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kjt.dianchejie.cn

Ruby: @name = "x"
来源：http://sdf.xuetiantiany.cn

C#:   public string Name { get; set; } = "x";
来源：http://hfn.zhongyouzk.top

[G04] 定义方法
来源：http://sde.yanxiufei.cn

Py:   def greet(self): return self.name
来源：http://vsq.hfpthk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vve.guannengcc.top

JS:   greet() { return this.name; }
来源：http://dlu.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://ywc.yonumen.top

Java: String greet() { return name; }
来源：http://but.52xcode.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gan.guowangkeji.top

Ruby: def greet; @name; end
来源：http://blf.quarkkingdee.top

C#:   public string Greet() => Name;
来源：http://hus.sufxvd.cn

[G05] 继承
来源：http://ela.hongshengwenyu.top

Py:   class Admin(User): pass
来源：http://aek.cucudq.cn

PHP:  class Admin extends User {}
来源：http://vyp.birdmap.top

JS:   class Admin extends User {}
来源：http://nnn.cdnleiting.top

TS:   class Admin extends User {}
来源：http://hbx.yfazqb.com

Java: class Admin extends User {}
来源：http://gle.pycfn.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dlr.hcnkem.com

Ruby: class Admin < User; end
来源：http://xhu.yfazqb.com

C#:   class Admin : User {}
来源：http://cjk.shzxlz.cn

[G06] 重写方法
来源：http://eux.shanyushiyangkeji.top

Py:   def greet(self): return "admin"
来源：http://ekf.yj202588.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rsu.chenlongwang.top

JS:   greet() { return "admin"; }
来源：http://rtw.hammf.cn

TS:   greet(): string { return "admin"; }
来源：http://css.hnxiangtu.top

Java: @Override String greet() { return "admin"; }
来源：http://nmd.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vbx.cdnleiting.top

Ruby: def greet; "admin"; end
来源：http://xsv.chenjidiqi.icu

C#:   public override string Greet() => "admin";
来源：http://ewy.meibo888.top

[G07] 调用父类方法
来源：http://dcg.yuxming.cn

Py:   super().greet()
来源：http://bgs.chenjidiqi.icu

PHP:  parent::greet();
来源：http://ouc.zhiwuduotai.top

JS:   super.greet();
来源：http://wdq.c1oappe.top

TS:   super.greet();
来源：http://xne.yvedp.cn

Java: super.greet();
来源：http://gnl.xuanzx.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dzf.guannengcc.top

Ruby: super
来源：http://qpq.chenjidiqi.icu

C#:   base.Greet();
来源：http://blc.meibo888.top

[G08] 静态方法与属性
来源：http://xiv.zhengqikj.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://asl.zhijiandao.cn

PHP:  public static function f() {}
来源：http://frt.bbcook.cn

JS:   static f() {}
来源：http://rxe.yvedp.cn

TS:   static f(): void {}
来源：http://yal.gogol.net.cn

Java: static void f() {}
来源：http://jez.zdqjudy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://zgk.fehbvm.com

Ruby: def self.f; end
来源：http://vyt.fengsongda.top

C#:   public static void F() {}
来源：http://vbn.shuidangran.top

[G09] 接口 / 抽象类
来源：http://vby.vqdsnc.cn

Py:   from abc import ABC, abstractmethod
来源：http://jcp.daxiang520.top

PHP:  interface Shape { public function area(): float; }
来源：http://vvn.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qyg.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://gve.wangdashe.top

Java: interface Shape { double area(); }
来源：http://oah.sweek.top

Go:   type Shape interface { Area() float64 }
来源：http://jzu.xylfe.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jyj.iojbl.cn

C#:   interface IShape { double Area(); }
来源：http://ybd.yanxiufei.cn

[G10] 访问控制
来源：http://qhg.iojbl.cn

Py:   约定 _protected / __private（不强制）
来源：http://znw.cqqwz.cn

PHP:  public / protected / private
来源：http://nyz.jinghuilouyu.cn

JS:   #private 字段；其余公开
来源：http://hut.jiagoushi.top

TS:   public / protected / private
来源：http://gyb.ehwqpu.com

Java: public / protected / private / 默认包级
来源：http://vrg.gogol.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://thv.yonumen.top

Ruby: public / protected / private
来源：http://ctz.gaohongyu789.top


<!-- 参考信息 -->