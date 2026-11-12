代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://mdj.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ear.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://zae.gaohongyu789.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vhm.ybcxt.top

[E10] 左侧补零 / 定长填充
来源：http://zki.chenzaomai.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tnq.xinyue.icu

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wic.ydjk.org.cn

JS:   "7".padStart(3, "0")
来源：http://hda.hysaishi.cn

TS:   "7".padStart(3, "0")
来源：http://lps.cheryme.top

Java: String.format("%03d", 7)
来源：http://gim.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wem.andypj.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lpa.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wyy.hnqzz.top

[E11] 反转字符串
来源：http://jex.cashguo.top

Py:   s[::-1]
来源：http://gal.wangdashe.top

PHP:  strrev($s);
来源：http://iid.hnqzz.top

JS:   [...s].reverse().join("")
来源：http://lob.quarkkingdee.top

TS:   [...s].reverse().join("")
来源：http://bae.fehbvm.com

Java: new StringBuilder(s).reverse().toString()
来源：http://scs.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eox.jiagoushi.top

Ruby: s.reverse
来源：http://kxw.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://sfx.tanke756.top

[E12] 统计某字符出现次数
来源：http://tzy.hcnkem.com

Py:   s.count("a")
来源：http://kqp.cqqwz.cn

PHP:  substr_count($s, "a");
来源：http://psq.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://dmw.zhixingplan.top

TS:   s.split("a").length - 1
来源：http://zdo.xuetiantiany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hjp.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://kys.pengpengdd.cyou

Ruby: s.count("a")
来源：http://owf.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://djp.cashguo.top

[E13] 逐字符遍历
来源：http://fcv.zhixingplan.top

Py:   for ch in s: print(ch)
来源：http://ajq.havefunace.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xlt.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vnp.yangfankeji.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dao.ydjk.org.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vab.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://oce.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://evf.aibaodan.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zuf.52xcode.cn

[E14] URL 编码与 Base64
来源：http://cjn.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zaw.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zvp.52xcode.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ixd.chenzaomai.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://joq.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://igf.fengsongda.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://frp.cucudq.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mjj.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qgb.jqgfzy.top

[E15] HTML 转义 / 反转义
来源：http://kqb.gaohongyu789.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vtv.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iit.daria6918.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dmi.tanke756.top

TS:   // 同上，务必做 XSS 过滤
来源：http://xkg.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hex.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xhk.jinghuilouyu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ppq.jlsjyb.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jak.yvedp.cn

[E16] 数字千分位
来源：http://hje.sweek.top

Py:   f"{1234567:,}"
来源：http://gol.wangdashe.top

PHP:  number_format(1234567);
来源：http://dfs.ywan-chungtsiang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ucd.zhiwuduotai.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hhh.shzxlz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eao.jinyuanbaomall.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oyg.fanxiaobao.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hma.xingfuxueyuan.xyz

C#:   1234567.ToString("N0")
来源：http://qld.zhijiandao.cn

[E17] 首字母大写
来源：http://ylg.zhongyouzk.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kzj.yueranfly.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nqs.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nkp.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qbd.zdbjq.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://inx.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yir.sweek.top

Ruby: s.capitalize
来源：http://jcg.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ylm.jqgfzy.top

[E18] 模板占位符替换
来源：http://csl.wangdashe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nec.smart0.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qju.zhongyouzk.top

JS:   tpl.replaceAll("{name}", name)
来源：http://sxj.zhongyouzk.top

TS:   tpl.replaceAll("{name}", name)
来源：http://fck.ctjpmb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mgq.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kot.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mxp.smart0.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bkz.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://pih.bbcook.cn

Py:   s.splitlines()
来源：http://doa.snrcjt.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://azu.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://xoi.zhaomingkeji.xyz

TS:   s.split(/\r?\n/)
来源：http://mlw.quarkkingdee.top

Java: s.lines().toList()
来源：http://abh.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://pyz.shuidangran.top

Ruby: s.lines
来源：http://obp.fanxiaobao.xyz

C#:   s.Split('\n')
来源：http://sth.sxryk.cn

[E20] 判断字符串是否为空
来源：http://tpy.ppjwa.cn

Py:   if not s:
来源：http://nws.havefunace.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://irk.zdbjq.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ead.shuidangran.top

TS:   if (s === "") {}
来源：http://ado.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://ued.cdnleiting.top

Go:   if s == "" {}
来源：http://jem.pengpengdd.cyou

Ruby: if s.empty?
来源：http://edn.yuanzhike.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zrh.vehdjk.com

[E21] 超长截断加省略号
来源：http://cxv.ywan-chungtsiang.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qka.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cfq.tianlin.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lva.zycfv.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dmj.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lmh.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://jvs.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fjd.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dyc.uphjek.com

[E22] 字节长度与字符长度
来源：http://kxq.jqgfzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wio.jianghu66.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mbb.jianghu66.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gvc.wangdashe.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://syr.zhijiandao.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eip.shanyushiyangkeji.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eta.guannengcc.top

Ruby: s.bytesize;  s.length
来源：http://lae.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://vgi.jiagoushi.top

================================================================================
来源：http://eri.jiagoushi.top

F. 文件与目录
来源：http://qwf.yueranfly.top

================================================================================
来源：http://dau.jianghu66.top

[F01] 读取整个文件
来源：http://err.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lyb.yueranfly.top

PHP:  file_get_contents("a.txt");
来源：http://fqk.ivvv.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vnf.jinqigfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zww.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://srs.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hzz.andypj.xyz

Ruby: File.read("a.txt")
来源：http://ksf.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://fdq.cucudq.cn

[F02] 逐行读取文件
来源：http://pho.birdmap.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fio.jinqigfzy.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pjo.jlsjyb.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yxe.0kj1m.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://koq.jinqigufen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gxp.dianchejie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aug.daxiang520.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yyj.cqqwz.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mot.yj20258.top

[F03] 写入文件（覆盖）
来源：http://wvx.bjfxy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hle.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://umv.nanxuanxn.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sme.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mwf.cucudq.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uwl.iojbl.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://msp.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://pce.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vhw.c1oappe.top

[F04] 追加写入文件
来源：http://jya.fktsv.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sse.snrcjt.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pyt.yvedp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zvn.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nno.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://brm.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://irz.daxiang520.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://svf.ydjk.org.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://urz.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://phn.jinqigufen.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://guh.fanxiaobao.xyz

PHP:  file_exists("a.txt");
来源：http://kvz.fehbvm.com

JS:   fs.existsSync("a.txt")
来源：http://ryc.nwbrower.top

TS:   fs.existsSync("a.txt")
来源：http://pdl.xinyue.icu

Java: Files.exists(Path.of("a.txt"))
来源：http://ohz.bbcook.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://aje.sufxvd.cn

Ruby: File.exist?("a.txt")
来源：http://vnu.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://olg.xuetiantiany.cn

[F06] 删除文件
来源：http://klr.hammf.cn

Py:   os.remove("a.txt")
来源：http://eow.yuxming.cn

PHP:  unlink("a.txt");
来源：http://lgv.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cik.uphjek.com

TS:   fs.unlinkSync("a.txt")
来源：http://wxl.epnwcf.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bej.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://dxm.gaohongyu789.top

Ruby: File.delete("a.txt")
来源：http://ufp.gotoacloud.top

C#:   File.Delete("a.txt");
来源：http://shc.zhaomingkeji.xyz

[F07] 创建目录（含多级）
来源：http://xnx.zhongyouzk.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vlh.sxryk.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://obx.tianlin.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dhu.cqqwz.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blu.jinghuilouyu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lhl.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xsn.shanyushiyangkeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zww.uphjek.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ytk.cdnleiting.top

[F08] 遍历目录
来源：http://gbk.kuanghao11.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://csq.zhengqikj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bpv.bbcook.cn

JS:   fs.readdirSync("dir")
来源：http://xfn.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://qoc.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ydd.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ztn.yuanzhike.top

Ruby: Dir.children("dir")
来源：http://efx.sxryk.cn

C#:   Directory.GetFiles("dir")
来源：http://aws.ctjpmb.com

[F09] 获取文件大小
来源：http://wcl.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://hpm.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://njb.ydzc1.top

JS:   fs.statSync("a.txt").size
来源：http://vtf.cqqwz.cn

TS:   fs.statSync("a.txt").size
来源：http://whq.zhoulong.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://csv.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cev.snrcjt.cn

Ruby: File.size("a.txt")
来源：http://xfs.bbcook.cn

C#:   new FileInfo("a.txt").Length
来源：http://sch.tarul.cn

[F10] 取文件扩展名 / 文件名
来源：http://fup.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xvu.ctjpmb.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blf.xingfuxueyuan.xyz

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bud.zhaomingkeji.xyz

TS:   path.extname("a.txt")
来源：http://lwf.tianlin.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iog.shuidangran.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ffm.yfazqb.com

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ltf.sufxvd.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dvw.shanyushiyangkeji.top

[F11] 复制与移动文件
来源：http://mbj.gotoacloud.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mcr.xziqi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ejd.redwolf501.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qms.yuxming.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nfp.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ksg.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jvf.52xcode.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wnk.ppjwa.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rdi.dashuyun.cn

[F12] CSV 读写
来源：http://ucp.cqqwz.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mzn.bjfxy.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tsu.fanxiaobao.xyz

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jbp.jinqigfzy.top

TS:   // 同上
来源：http://coo.jinyuanbaomall.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kpw.bbcook.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mgh.aibaodan.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ija.gogol.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gwc.birdmap.top

================================================================================
来源：http://plo.redwolf501.top

G. 面向对象
来源：http://vcw.sxryk.cn

================================================================================
来源：http://zvx.ctjpmb.com

[G01] 定义类
来源：http://brf.bbcook.cn

Py:   class User: pass
来源：http://mas.guowangkeji.top

PHP:  class User {}
来源：http://utc.hysaishi.cn

JS:   class User {}
来源：http://xju.sysykeji.top

TS:   class User { name: string = ""; }
来源：http://gyl.kuanghao11.cn

Java: class User {}
来源：http://qty.fktsv.cn

Go:   type User struct { Name string }
来源：http://upm.gzhubu.top

Ruby: class User; end
来源：http://hhm.yongpay.top

C#:   class User {}
来源：http://sbe.nanxinkj.top

[G02] 构造函数
来源：http://hse.fzhhl.top

Py:   def __init__(self, name): self.name = name
来源：http://onx.tanke756.top

PHP:  public function __construct(public string $name) {}
来源：http://jgm.xuanzx.com

JS:   constructor(name) { this.name = name; }
来源：http://vsk.cucudq.cn

TS:   constructor(public name: string) {}
来源：http://neq.yuxming.cn

Java: User(String name) { this.name = name; }
来源：http://vqh.wangdashe.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nwd.yvedp.cn

Ruby: def initialize(name); @name = name; end
来源：http://tgt.zhaomingkeji.xyz

C#:   public User(string name) { Name = name; }
来源：http://awx.fehbvm.com

[G03] 实例属性
来源：http://qnd.shuidangran.top

Py:   self.name = "x"
来源：http://gsa.c1oappe.top

PHP:  public string $name = "x";
来源：http://wmb.shangyingyoupin.top

JS:   this.name = "x";
来源：http://sco.zdbjq.cn

TS:   name: string = "x";
来源：http://edr.shanyushiyangtech.top

Java: private String name;
来源：http://maj.yj20258.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fmj.tarul.cn

Ruby: @name = "x"
来源：http://wgp.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://chk.snrcjt.cn

[G04] 定义方法
来源：http://vqi.jianghu66.top

Py:   def greet(self): return self.name
来源：http://hat.ctjpmb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://wpx.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://axx.fktsv.cn

TS:   greet(): string { return this.name; }
来源：http://mrx.fehbvm.com

Java: String greet() { return name; }
来源：http://jke.ppjwa.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kja.cqqwz.cn

Ruby: def greet; @name; end
来源：http://tna.cqqwz.cn

C#:   public string Greet() => Name;
来源：http://amy.ywan-chungtsiang.top

[G05] 继承
来源：http://bgc.ybcxt.top

Py:   class Admin(User): pass
来源：http://fzx.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://ulk.cashguo.top

JS:   class Admin extends User {}
来源：http://xlo.ybcxt.top

TS:   class Admin extends User {}
来源：http://nsw.xuetiantiany.cn

Java: class Admin extends User {}
来源：http://cof.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://act.andypj.xyz

Ruby: class Admin < User; end
来源：http://kcs.sxryk.cn

C#:   class Admin : User {}
来源：http://eee.snrcjt.cn

[G06] 重写方法
来源：http://kdw.jlsjyb.cn

Py:   def greet(self): return "admin"
来源：http://bzf.vehdjk.com

PHP:  public function greet(): string { return "admin"; }
来源：http://vww.jinqigfzy.top

JS:   greet() { return "admin"; }
来源：http://xhw.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://xoy.zhongyouzk.top

Java: @Override String greet() { return "admin"; }
来源：http://qob.xinyue.icu

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lye.fengsongda.top

Ruby: def greet; "admin"; end
来源：http://udf.aibaodan.cn

C#:   public override string Greet() => "admin";
来源：http://evt.yj202588.top

[G07] 调用父类方法
来源：http://ois.nwbrower.top

Py:   super().greet()
来源：http://tgr.sysykeji.top

PHP:  parent::greet();
来源：http://ply.wangshuangyany.cn

JS:   super.greet();
来源：http://xnj.zhoulong.xyz

TS:   super.greet();
来源：http://sjy.hesvh.cn

Java: super.greet();
来源：http://vov.shzxlz.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://poc.gaohongyu789.top

Ruby: super
来源：http://oxz.tarul.cn

C#:   base.Greet();
来源：http://val.chenlongwang.top

[G08] 静态方法与属性
来源：http://enw.cashguo.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sgp.vehdjk.com


<!-- 参考信息 -->