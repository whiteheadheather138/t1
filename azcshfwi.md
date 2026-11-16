代发 wailian999

JS:   [...s].reverse().join("")
来源：http://wvt.cheryme.top

TS:   [...s].reverse().join("")
来源：http://pxj.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://ffu.hcnkem.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://ccz.ehwqpu.com

Ruby: s.reverse
来源：http://rez.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uas.yj202588.top

[E12] 统计某字符出现次数
来源：http://tkh.svipenyu.cn

Py:   s.count("a")
来源：http://rmd.daria6918.cn

PHP:  substr_count($s, "a");
来源：http://wnp.fengsongda.top

JS:   s.split("a").length - 1
来源：http://lze.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://lrv.chenzaomai.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ihg.52xcode.cn

Go:   strings.Count(s, "a")
来源：http://egc.xingfuxueyuan.xyz

Ruby: s.count("a")
来源：http://gmk.wangshuangyany.cn

C#:   s.Count(c => c == 'a')
来源：http://kxo.316326.xyz

[E13] 逐字符遍历
来源：http://xsx.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://lvq.jinqigfzy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dhx.jinyuanbaomall.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dud.hongshengwenyu.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wid.hysaishi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hmc.yuanzhike.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rkb.ydzc1.top

Ruby: s.each_char { |ch| puts ch }
来源：http://lco.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mrb.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://njr.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pqp.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://iip.daria6918.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rjh.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lan.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pxq.xziqi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://aqu.yueranfly.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pzt.nanxinkj.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nvu.bbcook.cn

[E15] HTML 转义 / 反转义
来源：http://cny.ydjk.org.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ldd.havefunace.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mlu.ehwqpu.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://olp.9152youxi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://edd.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fsa.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jfj.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pdq.jinyuanbaomall.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bmd.smart0.xyz

[E16] 数字千分位
来源：http://plh.haohaochexian.top

Py:   f"{1234567:,}"
来源：http://qtb.cqqwz.cn

PHP:  number_format(1234567);
来源：http://lik.yvedp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://tna.c1oappe.top

TS:   (1234567).toLocaleString("en-US")
来源：http://tpr.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lio.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yrl.birdmap.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sng.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://cvf.yongpay.top

[E17] 首字母大写
来源：http://rmh.fehbvm.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lwr.yj20258.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://pht.hcnkem.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rib.c1oappe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://euu.cdnleiting.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wzv.cucudq.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cug.yongpay.top

Ruby: s.capitalize
来源：http://vql.shangyingyoupin.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kwx.cdnleiting.top

[E18] 模板占位符替换
来源：http://qyx.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qyn.hnqzz.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xpo.guowangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://wqs.mhx1999.top

TS:   tpl.replaceAll("{name}", name)
来源：http://zzd.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://igk.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lcz.hammf.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ucg.chenzaomai.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mdh.jqgufenzy.top

[E19] 多行文本按行拆分
来源：http://apb.ivvv.top

Py:   s.splitlines()
来源：http://gfy.jyoumei.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lth.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://xaf.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://lej.zhoulong.xyz

Java: s.lines().toList()
来源：http://uuk.svipenyu.cn

Go:   strings.Split(s, "\n")
来源：http://zwy.birdmap.top

Ruby: s.lines
来源：http://ksp.xylfe.cn

C#:   s.Split('\n')
来源：http://bnh.ydjk.org.cn

[E20] 判断字符串是否为空
来源：http://hrx.guannengcc.top

Py:   if not s:
来源：http://fuh.gaohongyu789.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fvs.cashguo.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jnl.hywenlv.cn

TS:   if (s === "") {}
来源：http://jjv.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://xem.shangyingyoupin.top

Go:   if s == "" {}
来源：http://hzw.yanxiufei.cn

Ruby: if s.empty?
来源：http://kvg.chenlongwang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dqs.havefunace.top

[E21] 超长截断加省略号
来源：http://tsx.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yja.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fki.jianghu66.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uzm.pycfn.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hxl.0kj1m.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mci.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://rti.hesvh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ivk.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hsp.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://oyr.meibo888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dvz.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lot.tianlin.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eii.svipenyu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdv.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://leg.cqqwz.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vzp.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://crt.gogol.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nby.ywan-chungtsiang.top

================================================================================
来源：http://dgl.yj202588.top

F. 文件与目录
来源：http://gfy.jinqigfzy.top

================================================================================
来源：http://lwh.zycfv.cn

[F01] 读取整个文件
来源：http://frm.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cvl.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://klp.52xcode.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pvm.shanyushiyangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mxs.nwbrower.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dra.316326.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://foe.jinyuanbaomall.cn

Ruby: File.read("a.txt")
来源：http://vgc.xziqi.cn

C#:   File.ReadAllText("a.txt");
来源：http://oey.havefunace.top

[F02] 逐行读取文件
来源：http://tdf.cdnleiting.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xvg.smart0.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://arr.smart0.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jug.haohaochexian.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bwg.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rsb.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://htr.daria6918.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wco.xuetiantiany.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://krd.ivvv.top

[F03] 写入文件（覆盖）
来源：http://cvp.pycfn.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ybf.sufxvd.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mwv.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bba.zhongyouzk.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xsi.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qom.sufxvd.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ghl.sjlbkw.cn

Ruby: File.write("a.txt", "hi")
来源：http://vwn.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cyc.ywan-chungtsiang.top

[F04] 追加写入文件
来源：http://gfd.jyoumei.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://asu.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rbg.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://svl.aizwys.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zdb.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jdo.yj202588.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vtc.aizwys.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aic.ivvv.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vrj.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://hhd.zdbjq.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ber.cucudq.cn

PHP:  file_exists("a.txt");
来源：http://xgg.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://cla.chenlongwang.top

TS:   fs.existsSync("a.txt")
来源：http://tzi.hywenlv.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kwv.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uuy.xinyue.icu

Ruby: File.exist?("a.txt")
来源：http://nzh.pycfn.com

C#:   File.Exists("a.txt")
来源：http://qvn.ywan-chungtsiang.top

[F06] 删除文件
来源：http://izl.tanke756.top

Py:   os.remove("a.txt")
来源：http://dzc.yj20258888.top

PHP:  unlink("a.txt");
来源：http://xen.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jcj.sweek.top

TS:   fs.unlinkSync("a.txt")
来源：http://nbh.ydjk.org.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fel.dianchejie.cn

Go:   os.Remove("a.txt")
来源：http://yie.hnxiangtu.top

Ruby: File.delete("a.txt")
来源：http://isv.jinyuanbaomall.cn

C#:   File.Delete("a.txt");
来源：http://fjz.hammf.cn

[F07] 创建目录（含多级）
来源：http://xub.fehbvm.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://aoc.yj20258.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kud.nanxinkj.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://msr.yongpay.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wiv.jinyuanbaomall.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vjf.ctjpmb.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cky.zhaomingkeji.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xkz.gaohongyu789.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mxj.gzhubu.top

[F08] 遍历目录
来源：http://pzc.sysykeji.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://utz.yuanzhike.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jmu.nanxinkj.top

JS:   fs.readdirSync("dir")
来源：http://eus.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://rdb.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jfz.jianghu66.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://ozu.sjlbkw.cn

Ruby: Dir.children("dir")
来源：http://lew.pengpengdd.cyou

C#:   Directory.GetFiles("dir")
来源：http://yjq.cucudq.cn

[F09] 获取文件大小
来源：http://uem.hammf.cn

Py:   os.path.getsize("a.txt")
来源：http://nmg.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://qfo.vqdsnc.cn

JS:   fs.statSync("a.txt").size
来源：http://wot.dianchejie.cn

TS:   fs.statSync("a.txt").size
来源：http://gfm.hfpthk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ouy.wangdashe.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nsu.iojbl.cn

Ruby: File.size("a.txt")
来源：http://ztc.xylfe.cn

C#:   new FileInfo("a.txt").Length
来源：http://hbt.yj20258888.top

[F10] 取文件扩展名 / 文件名
来源：http://zks.xinyue.icu

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bgj.smart0.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://exr.fzhhl.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://eun.cqqwz.cn

TS:   path.extname("a.txt")
来源：http://xbh.pengpengdd.cyou

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dec.ywan-chungtsiang.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yud.0kj1m.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ima.chenlongwang.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fjb.hysaishi.cn

[F11] 复制与移动文件
来源：http://aaf.bjfxy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tho.fzhhl.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ksh.zdqjudy.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ruh.nanxuanxn.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bbw.chenzaomai.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tns.fehbvm.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zfl.ydzc1.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yeu.shanyushiyangtech.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jpy.zhongyouzk.top

[F12] CSV 读写
来源：http://ttq.wangshuangyany.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jpf.uphjek.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vad.shangyingyoupin.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cqm.feifeiyinyue.top

TS:   // 同上
来源：http://nim.nanxuanxn.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://twq.nanxuanxn.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ape.mhx1999.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vfn.jiagoushi.top

C#:   // 无内置：用 CsvHelper 库
来源：http://xiy.yvedp.cn

================================================================================
来源：http://cwd.yj20258888.top

G. 面向对象
来源：http://ole.c1oappe.top

================================================================================
来源：http://jgm.redwolf501.top

[G01] 定义类
来源：http://xin.cashguo.top

Py:   class User: pass
来源：http://zai.zdbjq.cn

PHP:  class User {}
来源：http://jnh.birdmap.top

JS:   class User {}
来源：http://jcu.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://eng.jyoumei.cn

Java: class User {}
来源：http://uuk.zhoulong.xyz

Go:   type User struct { Name string }
来源：http://szp.sysykeji.top

Ruby: class User; end
来源：http://xrv.yongpay.top

C#:   class User {}
来源：http://ion.aibaodan.cn

[G02] 构造函数
来源：http://ops.uphjek.com

Py:   def __init__(self, name): self.name = name
来源：http://yap.9152youxi.cn

PHP:  public function __construct(public string $name) {}
来源：http://nzf.cdnleiting.top

JS:   constructor(name) { this.name = name; }
来源：http://exa.epnwcf.com

TS:   constructor(public name: string) {}
来源：http://sqd.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://cud.yj202588.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fgq.yfazqb.com

Ruby: def initialize(name); @name = name; end
来源：http://yda.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://ida.feifeiyinyue.top

[G03] 实例属性
来源：http://mas.haohaochexian.top

Py:   self.name = "x"
来源：http://rcr.zdqjudy.top

PHP:  public string $name = "x";
来源：http://wta.ydjk.org.cn

JS:   this.name = "x";
来源：http://iyz.zhijiandao.cn

TS:   name: string = "x";
来源：http://xqc.yj202588.top

Java: private String name;
来源：http://mwn.jinqigufen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uda.wangshuangyany.cn

Ruby: @name = "x"
来源：http://kpz.hammf.cn

C#:   public string Name { get; set; } = "x";
来源：http://tqs.xingfuxueyuan.xyz

[G04] 定义方法
来源：http://huz.haohaochexian.top

Py:   def greet(self): return self.name
来源：http://igr.pengpengdd.cyou

PHP:  public function greet(): string { return $this->name; }
来源：http://cyo.zhengqikj.top

JS:   greet() { return this.name; }
来源：http://ixq.jiagoushi.top

TS:   greet(): string { return this.name; }
来源：http://tvw.zhengqikj.top

Java: String greet() { return name; }
来源：http://hny.ivvv.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://eur.ehwqpu.com

Ruby: def greet; @name; end
来源：http://hex.smart0.xyz

C#:   public string Greet() => Name;
来源：http://mpt.gzhubu.top

[G05] 继承
来源：http://mco.tarul.cn

Py:   class Admin(User): pass
来源：http://exu.chenjidiqi.icu

PHP:  class Admin extends User {}
来源：http://yue.haohaochexian.top

JS:   class Admin extends User {}
来源：http://frs.nanxinkj.top

TS:   class Admin extends User {}
来源：http://fge.hysaishi.cn

Java: class Admin extends User {}
来源：http://kfc.dianchejie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tmr.aibaodan.cn

Ruby: class Admin < User; end
来源：http://okx.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://maw.shanyushiyangkeji.top

[G06] 重写方法
来源：http://dgn.mhx1999.top

Py:   def greet(self): return "admin"
来源：http://jpx.bbcook.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zld.yonumen.top

JS:   greet() { return "admin"; }
来源：http://pnt.havefunace.top

TS:   greet(): string { return "admin"; }
来源：http://ftz.havefunace.top

Java: @Override String greet() { return "admin"; }
来源：http://ysd.gogol.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tgd.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://qym.yuanzhike.top

C#:   public override string Greet() => "admin";
来源：http://wkx.yj20258.top

[G07] 调用父类方法
来源：http://nez.gaohongyu789.top

Py:   super().greet()
来源：http://tqq.hongshengwenyu.top

PHP:  parent::greet();
来源：http://way.haohaochexian.top

JS:   super.greet();
来源：http://ntm.feifeiyinyue.top

TS:   super.greet();
来源：http://aoa.nwbrower.top

Java: super.greet();
来源：http://sqa.jianghu66.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ykt.xuanzx.com

Ruby: super
来源：http://qie.yongpay.top

C#:   base.Greet();
来源：http://qdm.kuanghao11.cn

[G08] 静态方法与属性
来源：http://nos.yuxming.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wuq.shuidangran.top

PHP:  public static function f() {}
来源：http://fzy.snrcjt.cn

JS:   static f() {}
来源：http://dih.wangshuangyany.cn

TS:   static f(): void {}
来源：http://inp.gogol.net.cn

Java: static void f() {}
来源：http://hvc.tarul.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wba.redwolf501.top

Ruby: def self.f; end
来源：http://pbs.nanxinkj.top

C#:   public static void F() {}
来源：http://plo.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://uvd.xinyue.icu

Py:   from abc import ABC, abstractmethod
来源：http://qmw.zdbjq.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sgt.jqgufenzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://qwu.zdqjudy.top

TS:   interface Shape { area(): number; }
来源：http://dji.gogol.net.cn

Java: interface Shape { double area(); }
来源：http://unn.zhengqikj.top

Go:   type Shape interface { Area() float64 }
来源：http://lpv.zdqjudy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bfj.yj202588.top

C#:   interface IShape { double Area(); }
来源：http://kch.pycfn.com


<!-- 参考信息 -->