代发 wailian999

JS:   [...s].reverse().join("")
来源：http://obo.daria6918.cn

TS:   [...s].reverse().join("")
来源：http://njp.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://exc.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://wpi.jianghu66.top

Ruby: s.reverse
来源：http://zre.ydjk.org.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jjb.aizwys.cn

[E12] 统计某字符出现次数
来源：http://xqy.fzhhl.top

Py:   s.count("a")
来源：http://uwk.dianchejie.cn

PHP:  substr_count($s, "a");
来源：http://tzy.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://qkn.tarul.cn

TS:   s.split("a").length - 1
来源：http://rtv.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yce.redwolf501.top

Go:   strings.Count(s, "a")
来源：http://adm.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://xxj.aizwys.cn

C#:   s.Count(c => c == 'a')
来源：http://zjw.pycfn.com

[E13] 逐字符遍历
来源：http://ejx.bjfxy.top

Py:   for ch in s: print(ch)
来源：http://aue.xziqi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dcr.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://wbs.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xmj.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fuq.aizwys.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://anq.epnwcf.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ysv.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gqr.zycfv.cn

[E14] URL 编码与 Base64
来源：http://fbk.hongshengwenyu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xwp.cdnleiting.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://mqx.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qsf.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uui.chenlongwang.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ssw.fehbvm.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://enh.shanyushiyangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uxd.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rzk.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://qdf.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bie.shanyushiyangkeji.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kgf.hammf.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cir.zhaomingkeji.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://alf.hysaishi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xjq.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zyz.iojbl.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://guj.mhx1999.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fhs.nanxuanxn.top

[E16] 数字千分位
来源：http://vrb.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://mhz.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://aqv.birdmap.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ccd.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://hgt.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jic.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gcs.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ybo.hesvh.cn

C#:   1234567.ToString("N0")
来源：http://vod.cheryme.top

[E17] 首字母大写
来源：http://ixe.mhx1999.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iec.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://gwy.gotoacloud.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lqn.hywenlv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qku.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vmn.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xui.yuxming.cn

Ruby: s.capitalize
来源：http://cok.zhijiandao.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://isa.xingfuxueyuan.xyz

[E18] 模板占位符替换
来源：http://utc.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://toz.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kmi.pycfn.com

JS:   tpl.replaceAll("{name}", name)
来源：http://vhn.gaohongyu789.top

TS:   tpl.replaceAll("{name}", name)
来源：http://bpi.nwbrower.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://exx.dashuyun.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vpt.bjfxy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qjm.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uaq.gogol.net.cn

[E19] 多行文本按行拆分
来源：http://yir.ehwqpu.com

Py:   s.splitlines()
来源：http://phd.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yau.shangyingyoupin.top

JS:   s.split(/\r?\n/)
来源：http://pru.ybcxt.top

TS:   s.split(/\r?\n/)
来源：http://rhv.jqgufenzy.top

Java: s.lines().toList()
来源：http://oah.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://qsa.ydzc1.top

Ruby: s.lines
来源：http://nru.zhiwuduotai.top

C#:   s.Split('\n')
来源：http://agm.hesvh.cn

[E20] 判断字符串是否为空
来源：http://zfd.pycfn.com

Py:   if not s:
来源：http://tsa.pengpengdd.cyou

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mop.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xoj.daria6918.cn

TS:   if (s === "") {}
来源：http://srw.yvedp.cn

Java: if (s.isEmpty()) {}
来源：http://rxw.shangyingyoupin.top

Go:   if s == "" {}
来源：http://kfr.wangdashe.top

Ruby: if s.empty?
来源：http://wsl.ywan-chungtsiang.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rsr.ctjpmb.com

[E21] 超长截断加省略号
来源：http://fvl.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zao.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qgr.zycfv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yvv.zdbjq.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://peq.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iar.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://ghb.fktsv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hvi.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hwa.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://czt.ppjwa.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pvs.svipenyu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wca.guannengcc.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zyd.shzxlz.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://htg.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oig.xziqi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qeo.snrcjt.cn

Ruby: s.bytesize;  s.length
来源：http://bgt.hnxiangtu.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xag.jqgufenzy.top

================================================================================
来源：http://ggk.cdnleiting.top

F. 文件与目录
来源：http://xke.jinqigfzy.top

================================================================================
来源：http://sku.cashguo.top

[F01] 读取整个文件
来源：http://yko.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ogx.ivvv.top

PHP:  file_get_contents("a.txt");
来源：http://zio.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://epq.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ohf.yj20258.top

Java: Files.readString(Path.of("a.txt"))
来源：http://owy.redwolf501.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kfe.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://yyz.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://bpx.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://dif.nanxuanxn.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rsw.dianchejie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zak.xingfuxueyuan.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pxo.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://anw.yangfankeji.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pbg.tanke756.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wvp.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jha.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mws.nanxuanxn.top

[F03] 写入文件（覆盖）
来源：http://upo.yangfankeji.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ned.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://snh.aizwys.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hwq.aizwys.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bew.bjfxy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wqb.zhaomingkeji.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://twt.pycfn.com

Ruby: File.write("a.txt", "hi")
来源：http://eqr.ywan-chungtsiang.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wzy.cheryme.top

[F04] 追加写入文件
来源：http://nmc.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jfq.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zya.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sjf.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hkn.daxiang520.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mod.316326.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://koo.zhixingplan.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bvh.jinqigufen.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lnk.dashuyun.cn

[F05] 判断文件或目录是否存在
来源：http://kea.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ehw.dianchejie.cn

PHP:  file_exists("a.txt");
来源：http://tfv.pycfn.com

JS:   fs.existsSync("a.txt")
来源：http://ozs.ctjpmb.com

TS:   fs.existsSync("a.txt")
来源：http://url.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://uko.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sli.ywan-chungtsiang.top

Ruby: File.exist?("a.txt")
来源：http://vsw.cdnleiting.top

C#:   File.Exists("a.txt")
来源：http://eyg.dashuyun.cn

[F06] 删除文件
来源：http://ofp.jianghu66.top

Py:   os.remove("a.txt")
来源：http://lwx.zhijiandao.cn

PHP:  unlink("a.txt");
来源：http://nku.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://ovn.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://yyh.tianlin.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wdk.xuetiantiany.cn

Go:   os.Remove("a.txt")
来源：http://oji.ybcxt.top

Ruby: File.delete("a.txt")
来源：http://ijs.wangshuangyany.cn

C#:   File.Delete("a.txt");
来源：http://gyu.mhx1999.top

[F07] 创建目录（含多级）
来源：http://qxu.svipenyu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ycu.nwbrower.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lpz.dianchejie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ulq.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gfl.yvedp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nco.zhijiandao.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ppv.xingfuxueyuan.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lid.fehbvm.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rst.haohaochexian.top

[F08] 遍历目录
来源：http://mqe.jlsjyb.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fxx.fehbvm.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ilp.xuetiantiany.cn

JS:   fs.readdirSync("dir")
来源：http://zdp.jqgufenzy.top

TS:   fs.readdirSync("dir")
来源：http://mbj.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://txg.nanxinkj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://kmc.c1oappe.top

Ruby: Dir.children("dir")
来源：http://dhf.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://xfd.uphjek.com

[F09] 获取文件大小
来源：http://uxj.shangyingyoupin.top

Py:   os.path.getsize("a.txt")
来源：http://yno.vehdjk.com

PHP:  filesize("a.txt");
来源：http://xmc.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://ruo.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://rbf.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://bdp.shanyushiyangkeji.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vzu.daxiang520.top

Ruby: File.size("a.txt")
来源：http://pzg.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://ygl.cqqwz.cn

[F10] 取文件扩展名 / 文件名
来源：http://pjq.yueranfly.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wjt.cqqwz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://erq.zhixingplan.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gzm.iojbl.cn

TS:   path.extname("a.txt")
来源：http://tck.nanxuanxn.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mzl.xylfe.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ljz.sjlbkw.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kxm.ivvv.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zlw.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://pgu.haohaochexian.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://puw.zdqjudy.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://juh.nanxinkj.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aus.redwolf501.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rnw.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bua.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sel.iojbl.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dok.ctjpmb.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kyn.sjlbkw.cn

[F12] CSV 读写
来源：http://zyr.daria6918.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://igx.zycfv.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fww.gotoacloud.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kju.ctjpmb.com

TS:   // 同上
来源：http://ljo.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lls.ctjpmb.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cbs.daria6918.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oiu.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://nyv.pengpengdd.cyou

================================================================================
来源：http://xlo.fehbvm.com

G. 面向对象
来源：http://ckg.jqgufenzy.top

================================================================================
来源：http://kxw.aibaodan.cn

[G01] 定义类
来源：http://grt.c1oappe.top

Py:   class User: pass
来源：http://xtm.haohaochexian.top

PHP:  class User {}
来源：http://wbz.fktsv.cn

JS:   class User {}
来源：http://aqk.hesvh.cn

TS:   class User { name: string = ""; }
来源：http://hhq.shuidangran.top

Java: class User {}
来源：http://kgs.shanyushiyangkeji.top

Go:   type User struct { Name string }
来源：http://kzz.xylfe.cn

Ruby: class User; end
来源：http://mek.nanxinkj.top

C#:   class User {}
来源：http://vue.c1oappe.top

[G02] 构造函数
来源：http://lap.c1oappe.top

Py:   def __init__(self, name): self.name = name
来源：http://xij.daria6918.cn

PHP:  public function __construct(public string $name) {}
来源：http://kuj.yfazqb.com

JS:   constructor(name) { this.name = name; }
来源：http://mst.fengsongda.top

TS:   constructor(public name: string) {}
来源：http://ena.jinghuilouyu.cn

Java: User(String name) { this.name = name; }
来源：http://grf.shzxlz.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nqj.jqgfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://aox.snrcjt.cn

C#:   public User(string name) { Name = name; }
来源：http://ebj.zdqjudy.top

[G03] 实例属性
来源：http://rwm.tarul.cn

Py:   self.name = "x"
来源：http://goy.shuidangran.top

PHP:  public string $name = "x";
来源：http://fkv.fengsongda.top

JS:   this.name = "x";
来源：http://jdu.zycfv.cn

TS:   name: string = "x";
来源：http://uaj.shangyingyoupin.top

Java: private String name;
来源：http://meo.cheryme.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gzs.hcnkem.com

Ruby: @name = "x"
来源：http://xxn.dashuyun.cn

C#:   public string Name { get; set; } = "x";
来源：http://suq.bjfxy.top

[G04] 定义方法
来源：http://zbr.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://lda.havefunace.top

PHP:  public function greet(): string { return $this->name; }
来源：http://uay.yj20258.top

JS:   greet() { return this.name; }
来源：http://xyt.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://amy.zhiwuduotai.top

Java: String greet() { return name; }
来源：http://zcu.xylfe.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tje.sweek.top

Ruby: def greet; @name; end
来源：http://enw.ydzc1.top

C#:   public string Greet() => Name;
来源：http://hgo.bjfxy.top

[G05] 继承
来源：http://mxx.gotoacloud.top

Py:   class Admin(User): pass
来源：http://rbr.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://wbm.nanxinkj.top

JS:   class Admin extends User {}
来源：http://ugj.316326.xyz

TS:   class Admin extends User {}
来源：http://adz.tarul.cn

Java: class Admin extends User {}
来源：http://czw.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tnt.c1oappe.top

Ruby: class Admin < User; end
来源：http://ysp.vehdjk.com

C#:   class Admin : User {}
来源：http://btg.yanxiufei.cn

[G06] 重写方法
来源：http://fnf.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://alb.hnqzz.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gqi.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://bqm.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://dhw.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://ijh.hywenlv.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tze.zycfv.cn

Ruby: def greet; "admin"; end
来源：http://wso.vehdjk.com

C#:   public override string Greet() => "admin";
来源：http://yej.c1oappe.top

[G07] 调用父类方法
来源：http://vlr.shanyushiyangtech.top

Py:   super().greet()
来源：http://wap.daria6918.cn

PHP:  parent::greet();
来源：http://ssp.nanxinkj.top

JS:   super.greet();
来源：http://rvl.316326.xyz

TS:   super.greet();
来源：http://kbz.fengsongda.top

Java: super.greet();
来源：http://ggc.jlsjyb.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lnw.wangshuangyany.cn

Ruby: super
来源：http://kqf.jinqigufen.top

C#:   base.Greet();
来源：http://yfx.c1oappe.top

[G08] 静态方法与属性
来源：http://jxk.c1oappe.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gpk.shzxlz.cn

PHP:  public static function f() {}
来源：http://kts.ppjwa.cn

JS:   static f() {}
来源：http://sfh.zhaomingkeji.xyz

TS:   static f(): void {}
来源：http://jbt.xuetiantiany.cn

Java: static void f() {}
来源：http://zcs.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nqm.gaohongyu789.top

Ruby: def self.f; end
来源：http://uig.chenlongwang.top

C#:   public static void F() {}
来源：http://krd.jqgfzy.top

[G09] 接口 / 抽象类
来源：http://xni.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://fjh.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://mcm.haohaochexian.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ssl.gogol.net.cn

TS:   interface Shape { area(): number; }
来源：http://hvp.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://yyb.fzhhl.top

Go:   type Shape interface { Area() float64 }
来源：http://guc.kuanghao11.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mcd.52xcode.cn

C#:   interface IShape { double Area(); }
来源：http://yxk.jyoumei.cn


<!-- 参考信息 -->