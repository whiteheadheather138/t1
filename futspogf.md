代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://ysn.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ydg.cucudq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qmr.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ewv.xingfuxueyuan.xyz

[E10] 左侧补零 / 定长填充
来源：http://wef.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hmt.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aoq.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://swt.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://lxn.yj202588.top

Java: String.format("%03d", 7)
来源：http://vnn.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bvc.nanxuanxn.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wzj.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vuc.jinqigufen.top

[E11] 反转字符串
来源：http://eqm.epnwcf.com

Py:   s[::-1]
来源：http://aaf.fzhhl.top

PHP:  strrev($s);
来源：http://wei.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://sjx.vehdjk.com

TS:   [...s].reverse().join("")
来源：http://dly.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://unm.bbcook.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ofo.shuidangran.top

Ruby: s.reverse
来源：http://hdg.hnqzz.top

C#:   new string(s.Reverse().ToArray())
来源：http://dyu.shanyushiyangkeji.top

[E12] 统计某字符出现次数
来源：http://wzl.xingfuxueyuan.xyz

Py:   s.count("a")
来源：http://dkh.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://ndq.sjlbkw.cn

JS:   s.split("a").length - 1
来源：http://gmw.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://ffe.hfpthk.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cgm.shanyushiyangtech.top

Go:   strings.Count(s, "a")
来源：http://tdk.sweek.top

Ruby: s.count("a")
来源：http://aoa.ydjk.org.cn

C#:   s.Count(c => c == 'a')
来源：http://efy.aizwys.cn

[E13] 逐字符遍历
来源：http://lpi.cashguo.top

Py:   for ch in s: print(ch)
来源：http://snz.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cyq.shangyingyoupin.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mei.zhijiandao.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dpi.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kbe.cheryme.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kgg.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://fmq.birdmap.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wsp.mhx1999.top

[E14] URL 编码与 Base64
来源：http://rsw.pengpengdd.cyou

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nmd.snrcjt.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xqq.dashuyun.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ujt.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lre.aibaodan.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nlo.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://olo.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qnn.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cgc.vehdjk.com

[E15] HTML 转义 / 反转义
来源：http://xjn.hnqzz.top

Py:   html.escape(s);  html.unescape(s)
来源：http://elr.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ewe.gzhubu.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://osa.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ffs.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tmw.dashuyun.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hgp.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pxq.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kmj.ppjwa.cn

[E16] 数字千分位
来源：http://koe.sufxvd.cn

Py:   f"{1234567:,}"
来源：http://vxh.zycfv.cn

PHP:  number_format(1234567);
来源：http://tvv.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rwb.nanxuanxn.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fyx.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oem.yvedp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oqg.gzhubu.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mrf.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://isv.xuanzx.com

[E17] 首字母大写
来源：http://lgu.tianlin.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dob.tianlin.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://gme.shuidangran.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ucp.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ccp.shangyingyoupin.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://spf.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kgi.ydjk.org.cn

Ruby: s.capitalize
来源：http://lfq.hesvh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://egs.ivvv.top

[E18] 模板占位符替换
来源：http://jed.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ruf.hesvh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ecm.cashguo.top

JS:   tpl.replaceAll("{name}", name)
来源：http://lum.havefunace.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xnd.uphjek.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cfi.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gjr.52xcode.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jpq.zhijiandao.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hiy.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://cxi.jqgfzy.top

Py:   s.splitlines()
来源：http://yle.fzhhl.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rax.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://mlz.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://lkd.xuanzx.com

Java: s.lines().toList()
来源：http://ojh.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://llt.yongpay.top

Ruby: s.lines
来源：http://xzq.cheryme.top

C#:   s.Split('\n')
来源：http://vnk.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://lkl.xuetiantiany.cn

Py:   if not s:
来源：http://mve.52xcode.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ikg.fzhhl.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oar.dashuyun.cn

TS:   if (s === "") {}
来源：http://hic.bjfxy.top

Java: if (s.isEmpty()) {}
来源：http://jtb.xziqi.cn

Go:   if s == "" {}
来源：http://yyz.havefunace.top

Ruby: if s.empty?
来源：http://lfn.nwbrower.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://alx.hcnkem.com

[E21] 超长截断加省略号
来源：http://cce.yongpay.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://csh.cqqwz.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ana.yangfankeji.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcx.ctjpmb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fih.ctjpmb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mwi.nanxinkj.top

Go:   // 按 rune 判断长度后截断
来源：http://luw.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://eiu.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qob.c1oappe.top

[E22] 字节长度与字符长度
来源：http://cbo.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sga.jiagoushi.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ksw.c1oappe.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jre.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sgd.iojbl.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ryu.sjlbkw.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hjz.zhixingplan.top

Ruby: s.bytesize;  s.length
来源：http://jjg.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iat.hcnkem.com

================================================================================
来源：http://qgf.snrcjt.cn

F. 文件与目录
来源：http://nnq.chenzaomai.com

================================================================================
来源：http://dbx.ivvv.top

[F01] 读取整个文件
来源：http://kfm.hongshengwenyu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cpx.jqgfzy.top

PHP:  file_get_contents("a.txt");
来源：http://yrg.chenjidiqi.icu

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zii.nanxinkj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uqt.fehbvm.com

Java: Files.readString(Path.of("a.txt"))
来源：http://rjt.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ofp.fehbvm.com

Ruby: File.read("a.txt")
来源：http://ohb.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://hmz.316326.xyz

[F02] 逐行读取文件
来源：http://ixr.wangdashe.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tvz.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://snf.hywenlv.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jmc.jinqigufen.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nwd.yongpay.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nqp.yanxiufei.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://psg.jiagoushi.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ruq.yfazqb.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bcx.sweek.top

[F03] 写入文件（覆盖）
来源：http://beo.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://fmn.chenjidiqi.icu

PHP:  file_put_contents("a.txt", "hi");
来源：http://jzq.jinyuanbaomall.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ull.havefunace.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jie.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ezt.zhijiandao.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tju.c1oappe.top

Ruby: File.write("a.txt", "hi")
来源：http://gvb.bjfxy.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qri.sysykeji.top

[F04] 追加写入文件
来源：http://gql.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://miz.fzhhl.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pqz.sufxvd.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qbd.yongpay.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nfp.yj20258888.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ula.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ifu.hesvh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://usj.xingfuxueyuan.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gcw.hesvh.cn

[F05] 判断文件或目录是否存在
来源：http://qey.zhongyouzk.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xjq.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://wqd.ydjk.org.cn

JS:   fs.existsSync("a.txt")
来源：http://kbc.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://kqj.fzhhl.top

Java: Files.exists(Path.of("a.txt"))
来源：http://vqb.hysaishi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wth.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://ckb.xingfuxueyuan.xyz

C#:   File.Exists("a.txt")
来源：http://qpl.shangyingyoupin.top

[F06] 删除文件
来源：http://lbf.ydjk.org.cn

Py:   os.remove("a.txt")
来源：http://qgg.cheryme.top

PHP:  unlink("a.txt");
来源：http://jmj.quarkkingdee.top

JS:   fs.unlinkSync("a.txt")
来源：http://fxt.jlsjyb.cn

TS:   fs.unlinkSync("a.txt")
来源：http://too.wangshuangyany.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ias.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://tqn.yuxming.cn

Ruby: File.delete("a.txt")
来源：http://wna.fengsongda.top

C#:   File.Delete("a.txt");
来源：http://xeu.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://yvd.zhijiandao.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sam.jiagoushi.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gqu.fanxiaobao.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qmt.hammf.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nid.jqgfzy.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aet.xziqi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ggb.hammf.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://awt.jinyuanbaomall.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hlm.sxryk.cn

[F08] 遍历目录
来源：http://ekm.tianlin.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://itt.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gcq.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://kra.wangdashe.top

TS:   fs.readdirSync("dir")
来源：http://tyi.vehdjk.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jqk.cqqwz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kks.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://uez.hcnkem.com

C#:   Directory.GetFiles("dir")
来源：http://mwk.haohaochexian.top

[F09] 获取文件大小
来源：http://dry.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://run.yangfankeji.com

PHP:  filesize("a.txt");
来源：http://sat.tarul.cn

JS:   fs.statSync("a.txt").size
来源：http://kbe.fktsv.cn

TS:   fs.statSync("a.txt").size
来源：http://bml.sxryk.cn

Java: Files.size(Path.of("a.txt"))
来源：http://axy.sweek.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://knb.wangdashe.top

Ruby: File.size("a.txt")
来源：http://uqp.hesvh.cn

C#:   new FileInfo("a.txt").Length
来源：http://vtr.ivvv.top

[F10] 取文件扩展名 / 文件名
来源：http://pkh.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pkv.shzxlz.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://olq.hnxiangtu.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xfi.zhiwuduotai.top

TS:   path.extname("a.txt")
来源：http://gyn.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tek.meibo888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://uia.feifeiyinyue.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iva.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mwa.0kj1m.cn

[F11] 复制与移动文件
来源：http://mep.shzxlz.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://aje.yfazqb.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zrs.ppjwa.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fiv.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lrj.aizwys.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zhn.316326.xyz

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://van.jyoumei.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://grh.epnwcf.com

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zlp.birdmap.top

[F12] CSV 读写
来源：http://qwh.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hus.zhoulong.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pxr.jyoumei.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oum.quarkkingdee.top

TS:   // 同上
来源：http://cbj.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mhb.iojbl.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vwt.nanxinkj.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ahj.jqgfzy.top

C#:   // 无内置：用 CsvHelper 库
来源：http://cff.sysykeji.top

================================================================================
来源：http://rii.ywan-chungtsiang.top

G. 面向对象
来源：http://fux.sufxvd.cn

================================================================================
来源：http://pof.hammf.cn

[G01] 定义类
来源：http://rrj.hnxiangtu.top

Py:   class User: pass
来源：http://ppw.zdbjq.cn

PHP:  class User {}
来源：http://gnb.yonumen.top

JS:   class User {}
来源：http://kzi.gaohongyu789.top

TS:   class User { name: string = ""; }
来源：http://clk.mhx1999.top

Java: class User {}
来源：http://mxj.wangshuangyany.cn

Go:   type User struct { Name string }
来源：http://ftl.316326.xyz

Ruby: class User; end
来源：http://vtk.aizwys.cn

C#:   class User {}
来源：http://muq.fzhhl.top

[G02] 构造函数
来源：http://uww.tian-w.cn

Py:   def __init__(self, name): self.name = name
来源：http://juq.yanxiufei.cn

PHP:  public function __construct(public string $name) {}
来源：http://arx.zycfv.cn

JS:   constructor(name) { this.name = name; }
来源：http://jvp.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://zxz.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://osd.ppjwa.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ljm.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://oey.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://rox.yuxming.cn

[G03] 实例属性
来源：http://lwz.fengsongda.top

Py:   self.name = "x"
来源：http://mzb.cashguo.top

PHP:  public string $name = "x";
来源：http://hvv.jinyuanbaomall.cn

JS:   this.name = "x";
来源：http://qsd.hnxiangtu.top

TS:   name: string = "x";
来源：http://ymm.xinyue.icu

Java: private String name;
来源：http://ezg.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sxj.ctjpmb.com

Ruby: @name = "x"
来源：http://iya.havefunace.top

C#:   public string Name { get; set; } = "x";
来源：http://fnm.guannengcc.top

[G04] 定义方法
来源：http://rlq.tarul.cn

Py:   def greet(self): return self.name
来源：http://dks.tanke756.top

PHP:  public function greet(): string { return $this->name; }
来源：http://nuq.316326.xyz

JS:   greet() { return this.name; }
来源：http://uhx.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://fyy.hfpthk.cn

Java: String greet() { return name; }
来源：http://hpj.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://xew.yuanzhike.top

Ruby: def greet; @name; end
来源：http://pyi.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://fls.yongpay.top

[G05] 继承
来源：http://cgs.zhengqikj.top

Py:   class Admin(User): pass
来源：http://xyc.zdqjudy.top

PHP:  class Admin extends User {}
来源：http://mrn.yueranfly.top

JS:   class Admin extends User {}
来源：http://nuq.hfpthk.cn

TS:   class Admin extends User {}
来源：http://zmt.jlsjyb.cn

Java: class Admin extends User {}
来源：http://ywf.aibaodan.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jli.cheryme.top

Ruby: class Admin < User; end
来源：http://qow.zdqjudy.top

C#:   class Admin : User {}
来源：http://aly.jinghuilouyu.cn

[G06] 重写方法
来源：http://dar.daxiang520.top

Py:   def greet(self): return "admin"
来源：http://kup.shzxlz.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qzu.tian-w.cn

JS:   greet() { return "admin"; }
来源：http://ugc.yuxming.cn

TS:   greet(): string { return "admin"; }
来源：http://eex.xuetiantiany.cn

Java: @Override String greet() { return "admin"; }
来源：http://srf.316326.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vos.yfazqb.com

Ruby: def greet; "admin"; end
来源：http://iue.xziqi.cn

C#:   public override string Greet() => "admin";
来源：http://fzg.zhijiandao.cn

[G07] 调用父类方法
来源：http://ecd.yj20258888.top

Py:   super().greet()
来源：http://coq.yueranfly.top

PHP:  parent::greet();
来源：http://stf.jinghuilouyu.cn

JS:   super.greet();
来源：http://swo.haohaochexian.top

TS:   super.greet();
来源：http://hzj.chenzaomai.com

Java: super.greet();
来源：http://afv.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jwm.yuxming.cn

Ruby: super
来源：http://icr.pycfn.com

C#:   base.Greet();
来源：http://bng.yanxiufei.cn

[G08] 静态方法与属性
来源：http://jyr.hywenlv.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gyh.snrcjt.cn


<!-- 参考信息 -->