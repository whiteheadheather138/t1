代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://meg.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://egr.yueranfly.top

Ruby: s.gsub(/\s+/, "")
来源：http://ikk.sjlbkw.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvq.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://vyw.daxiang520.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ecp.ctjpmb.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nzh.aibaodan.cn

JS:   "7".padStart(3, "0")
来源：http://xjz.hnqzz.top

TS:   "7".padStart(3, "0")
来源：http://ggb.cashguo.top

Java: String.format("%03d", 7)
来源：http://cjd.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://tdu.xylfe.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vxa.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ird.hongshengwenyu.top

[E11] 反转字符串
来源：http://hcz.yangfankeji.com

Py:   s[::-1]
来源：http://tmh.tarul.cn

PHP:  strrev($s);
来源：http://ppq.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://nsx.shuidangran.top

TS:   [...s].reverse().join("")
来源：http://uzd.gotoacloud.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qxu.jinqigufen.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://zzw.guowangkeji.top

Ruby: s.reverse
来源：http://fiu.zycfv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ald.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://mtp.tianlin.xyz

Py:   s.count("a")
来源：http://jau.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://pcw.pengpengdd.cyou

JS:   s.split("a").length - 1
来源：http://bua.guowangkeji.top

TS:   s.split("a").length - 1
来源：http://qpn.zhiwuduotai.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://imj.cashguo.top

Go:   strings.Count(s, "a")
来源：http://ohp.ppjwa.cn

Ruby: s.count("a")
来源：http://zys.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://nek.hnxiangtu.top

[E13] 逐字符遍历
来源：http://tov.cashguo.top

Py:   for ch in s: print(ch)
来源：http://esb.yanxiufei.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gzr.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uta.hywenlv.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vxv.chenzaomai.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ywp.pycfn.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://avv.cqqwz.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://mvv.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vqc.hysaishi.cn

[E14] URL 编码与 Base64
来源：http://bwg.wangshuangyany.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zey.feifeiyinyue.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zge.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://efd.ctjpmb.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dfy.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nii.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xhm.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uun.andypj.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nya.zhongyouzk.top

[E15] HTML 转义 / 反转义
来源：http://ier.9152youxi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://off.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vvp.jinqigfzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://efb.ywan-chungtsiang.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ljc.aibaodan.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sdn.shanyushiyangtech.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jsa.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lmn.daxiang520.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jkd.hysaishi.cn

[E16] 数字千分位
来源：http://doc.dianchejie.cn

Py:   f"{1234567:,}"
来源：http://mgs.fehbvm.com

PHP:  number_format(1234567);
来源：http://oug.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://udf.yfazqb.com

TS:   (1234567).toLocaleString("en-US")
来源：http://mzs.jianghu66.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jky.nanxinkj.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iis.daria6918.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uam.chenlongwang.top

C#:   1234567.ToString("N0")
来源：http://war.jinghuilouyu.cn

[E17] 首字母大写
来源：http://tab.zdqjudy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://chv.yangfankeji.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://vej.ybcxt.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baz.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fht.52xcode.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yjc.feifeiyinyue.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://alg.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ddb.cqqwz.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mwc.yongpay.top

[E18] 模板占位符替换
来源：http://pkw.epnwcf.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ipw.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rpr.ydjk.org.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bgx.sysykeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://wfz.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fbx.hysaishi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ztg.xylfe.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ncb.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nmj.mhx1999.top

[E19] 多行文本按行拆分
来源：http://bso.ppjwa.cn

Py:   s.splitlines()
来源：http://jzo.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://vta.daxiang520.top

JS:   s.split(/\r?\n/)
来源：http://obs.jinqigufen.top

TS:   s.split(/\r?\n/)
来源：http://bbv.fktsv.cn

Java: s.lines().toList()
来源：http://bra.aibaodan.cn

Go:   strings.Split(s, "\n")
来源：http://jmd.jqgfzy.top

Ruby: s.lines
来源：http://lzv.316326.xyz

C#:   s.Split('\n')
来源：http://gpv.quarkkingdee.top

[E20] 判断字符串是否为空
来源：http://fph.shangyingyoupin.top

Py:   if not s:
来源：http://bke.ybcxt.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vih.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://prs.sufxvd.cn

TS:   if (s === "") {}
来源：http://gcq.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://vvr.jqgfzy.top

Go:   if s == "" {}
来源：http://rlv.bbcook.cn

Ruby: if s.empty?
来源：http://dch.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://olq.nanxinkj.top

[E21] 超长截断加省略号
来源：http://adw.fehbvm.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://epx.ivvv.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jwr.shangyingyoupin.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aje.xziqi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ymp.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hpt.aibaodan.cn

Go:   // 按 rune 判断长度后截断
来源：http://ynv.zdbjq.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qhj.xziqi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jqy.zhijiandao.cn

[E22] 字节长度与字符长度
来源：http://cmx.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jow.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oqd.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dlu.gotoacloud.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tvg.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wms.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ngi.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://rqn.fengsongda.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wts.yj202588.top

================================================================================
来源：http://msx.havefunace.top

F. 文件与目录
来源：http://dam.sufxvd.cn

================================================================================
来源：http://eqw.hfpthk.cn

[F01] 读取整个文件
来源：http://gts.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uzw.bbcook.cn

PHP:  file_get_contents("a.txt");
来源：http://qxy.ehwqpu.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://luu.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rop.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cif.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vbe.chenlongwang.top

Ruby: File.read("a.txt")
来源：http://fuy.wangshuangyany.cn

C#:   File.ReadAllText("a.txt");
来源：http://nnq.jinqigufen.top

[F02] 逐行读取文件
来源：http://oyk.ywan-chungtsiang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tku.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cdw.yonumen.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xeu.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eug.ivvv.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jmo.c1oappe.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://efc.andypj.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://djd.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tls.cucudq.cn

[F03] 写入文件（覆盖）
来源：http://szp.hywenlv.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://adv.nanxuanxn.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://fvo.yangfankeji.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fmr.c1oappe.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rnl.guannengcc.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vwn.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mhm.zhaomingkeji.xyz

Ruby: File.write("a.txt", "hi")
来源：http://nzb.dianchejie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cof.ivvv.top

[F04] 追加写入文件
来源：http://cxj.pycfn.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://scm.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dmi.epnwcf.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gfw.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nbw.svipenyu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bxi.yuanzhike.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pol.dashuyun.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ggq.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vcn.wangdashe.top

[F05] 判断文件或目录是否存在
来源：http://ths.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bak.fktsv.cn

PHP:  file_exists("a.txt");
来源：http://oul.52xcode.cn

JS:   fs.existsSync("a.txt")
来源：http://wdv.iojbl.cn

TS:   fs.existsSync("a.txt")
来源：http://stt.sxryk.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sxo.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ouy.epnwcf.com

Ruby: File.exist?("a.txt")
来源：http://gqf.gogol.net.cn

C#:   File.Exists("a.txt")
来源：http://vnc.yanxiufei.cn

[F06] 删除文件
来源：http://chw.yfazqb.com

Py:   os.remove("a.txt")
来源：http://bah.pycfn.com

PHP:  unlink("a.txt");
来源：http://pcy.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://jpb.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://irk.zdbjq.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://szc.quarkkingdee.top

Go:   os.Remove("a.txt")
来源：http://hio.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://wqu.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://kfo.hfpthk.cn

[F07] 创建目录（含多级）
来源：http://zwh.jianghu66.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lkk.bbcook.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qwn.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://axk.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hvc.birdmap.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kpt.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vpe.guowangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ryd.cucudq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uyg.zhijiandao.cn

[F08] 遍历目录
来源：http://inn.cqqwz.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xoe.yj20258.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fny.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://ygb.yj202588.top

TS:   fs.readdirSync("dir")
来源：http://hdw.hywenlv.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://did.shangyingyoupin.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://utp.zycfv.cn

Ruby: Dir.children("dir")
来源：http://wdi.nanxinkj.top

C#:   Directory.GetFiles("dir")
来源：http://oxk.xylfe.cn

[F09] 获取文件大小
来源：http://bne.cucudq.cn

Py:   os.path.getsize("a.txt")
来源：http://ese.fzhhl.top

PHP:  filesize("a.txt");
来源：http://vyt.gaohongyu789.top

JS:   fs.statSync("a.txt").size
来源：http://anh.ehwqpu.com

TS:   fs.statSync("a.txt").size
来源：http://ymp.pycfn.com

Java: Files.size(Path.of("a.txt"))
来源：http://knc.fktsv.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aed.yj20258.top

Ruby: File.size("a.txt")
来源：http://eid.jyoumei.cn

C#:   new FileInfo("a.txt").Length
来源：http://lrn.nanxinkj.top

[F10] 取文件扩展名 / 文件名
来源：http://rji.ydjk.org.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://quy.52xcode.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oun.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lzk.gaohongyu789.top

TS:   path.extname("a.txt")
来源：http://bqb.hammf.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hap.hongshengwenyu.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gng.52xcode.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rqz.hongshengwenyu.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://keq.yj20258.top

[F11] 复制与移动文件
来源：http://xph.fanxiaobao.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://isw.jinghuilouyu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ual.ydjk.org.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://act.fktsv.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pbg.snrcjt.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dpw.dianchejie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sdv.zhongyouzk.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mrw.jyoumei.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tck.cqqwz.cn

[F12] CSV 读写
来源：http://krf.wangdashe.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ygm.jinyuanbaomall.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uql.hammf.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://egv.fehbvm.com

TS:   // 同上
来源：http://fja.zhongyouzk.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vwd.cqqwz.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wxv.ydzc1.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zav.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://gpc.gzhubu.top

================================================================================
来源：http://ldi.sysykeji.top

G. 面向对象
来源：http://dpc.redwolf501.top

================================================================================
来源：http://qit.zhongyouzk.top

[G01] 定义类
来源：http://hra.gogol.net.cn

Py:   class User: pass
来源：http://noc.yanxiufei.cn

PHP:  class User {}
来源：http://qfd.snrcjt.cn

JS:   class User {}
来源：http://lgh.nwbrower.top

TS:   class User { name: string = ""; }
来源：http://jvj.hnqzz.top

Java: class User {}
来源：http://vrh.yueranfly.top

Go:   type User struct { Name string }
来源：http://kdq.vqdsnc.cn

Ruby: class User; end
来源：http://qwb.jinghuilouyu.cn

C#:   class User {}
来源：http://rel.cashguo.top

[G02] 构造函数
来源：http://uxh.fktsv.cn

Py:   def __init__(self, name): self.name = name
来源：http://nzp.yueranfly.top

PHP:  public function __construct(public string $name) {}
来源：http://ogg.316326.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mwg.gotoacloud.top

TS:   constructor(public name: string) {}
来源：http://vig.ctjpmb.com

Java: User(String name) { this.name = name; }
来源：http://lot.0kj1m.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rde.cdnleiting.top

Ruby: def initialize(name); @name = name; end
来源：http://zap.chenzaomai.com

C#:   public User(string name) { Name = name; }
来源：http://taj.ppjwa.cn

[G03] 实例属性
来源：http://lth.snrcjt.cn

Py:   self.name = "x"
来源：http://oru.hammf.cn

PHP:  public string $name = "x";
来源：http://fqr.epnwcf.com

JS:   this.name = "x";
来源：http://qes.dianchejie.cn

TS:   name: string = "x";
来源：http://ine.ydzc1.top

Java: private String name;
来源：http://mnm.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uvh.gzhubu.top

Ruby: @name = "x"
来源：http://vke.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://rig.xuetiantiany.cn

[G04] 定义方法
来源：http://vir.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://apx.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://apw.hnxiangtu.top

JS:   greet() { return this.name; }
来源：http://xgh.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://yoi.cqqwz.cn

Java: String greet() { return name; }
来源：http://iqz.hnxiangtu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hxg.shzxlz.cn

Ruby: def greet; @name; end
来源：http://kxv.uphjek.com

C#:   public string Greet() => Name;
来源：http://xye.mhx1999.top

[G05] 继承
来源：http://jsa.ybcxt.top

Py:   class Admin(User): pass
来源：http://ilt.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://law.hammf.cn

JS:   class Admin extends User {}
来源：http://cdb.0kj1m.cn

TS:   class Admin extends User {}
来源：http://bel.nanxinkj.top

Java: class Admin extends User {}
来源：http://lqn.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kdn.hnqzz.top

Ruby: class Admin < User; end
来源：http://hxb.chenlongwang.top

C#:   class Admin : User {}
来源：http://soa.zhiwuduotai.top

[G06] 重写方法
来源：http://wil.xingfuxueyuan.xyz

Py:   def greet(self): return "admin"
来源：http://xka.shangyingyoupin.top

PHP:  public function greet(): string { return "admin"; }
来源：http://puk.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://ror.aizwys.cn

TS:   greet(): string { return "admin"; }
来源：http://xdn.cdnleiting.top

Java: @Override String greet() { return "admin"; }
来源：http://zay.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dys.jqgufenzy.top

Ruby: def greet; "admin"; end
来源：http://lxx.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://vgq.xziqi.cn

[G07] 调用父类方法
来源：http://nkd.yfazqb.com

Py:   super().greet()
来源：http://guf.jinqigfzy.top

PHP:  parent::greet();
来源：http://ghj.quarkkingdee.top

JS:   super.greet();
来源：http://cdh.kuanghao11.cn

TS:   super.greet();
来源：http://yev.jqgfzy.top

Java: super.greet();
来源：http://wxr.xylfe.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vfi.ydzc1.top

Ruby: super
来源：http://pkf.xylfe.cn

C#:   base.Greet();
来源：http://kac.yvedp.cn

[G08] 静态方法与属性
来源：http://emy.birdmap.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uon.nanxuanxn.top


<!-- 参考信息 -->