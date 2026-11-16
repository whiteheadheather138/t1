代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://hrz.andypj.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bfx.daxiang520.top

Ruby: s.gsub(/\s+/, "")
来源：http://iey.redwolf501.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vwu.fanxiaobao.xyz

[E10] 左侧补零 / 定长填充
来源：http://epy.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qxk.yueranfly.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ecf.52xcode.cn

JS:   "7".padStart(3, "0")
来源：http://duf.316326.xyz

TS:   "7".padStart(3, "0")
来源：http://fbi.uphjek.com

Java: String.format("%03d", 7)
来源：http://fyh.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://akf.mhx1999.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gxv.ybcxt.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ghn.hysaishi.cn

[E11] 反转字符串
来源：http://xld.fehbvm.com

Py:   s[::-1]
来源：http://tsl.jqgfzy.top

PHP:  strrev($s);
来源：http://wuo.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://exp.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://jqz.guannengcc.top

Java: new StringBuilder(s).reverse().toString()
来源：http://shj.pengpengdd.cyou

Go:   // 转 []rune 后倒序再转回 string
来源：http://txx.vehdjk.com

Ruby: s.reverse
来源：http://qmg.yueranfly.top

C#:   new string(s.Reverse().ToArray())
来源：http://jif.hnqzz.top

[E12] 统计某字符出现次数
来源：http://qru.jqgfzy.top

Py:   s.count("a")
来源：http://imu.zhoulong.xyz

PHP:  substr_count($s, "a");
来源：http://zrr.dashuyun.cn

JS:   s.split("a").length - 1
来源：http://daq.zdqjudy.top

TS:   s.split("a").length - 1
来源：http://oxp.cheryme.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tok.nwbrower.top

Go:   strings.Count(s, "a")
来源：http://rhd.hnqzz.top

Ruby: s.count("a")
来源：http://jak.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://rfm.andypj.xyz

[E13] 逐字符遍历
来源：http://iqk.cashguo.top

Py:   for ch in s: print(ch)
来源：http://tft.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vpu.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://yox.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jfq.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://crx.tianlin.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://uik.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://duc.yanxiufei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cjc.hywenlv.cn

[E14] URL 编码与 Base64
来源：http://lhr.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ovt.fehbvm.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://rat.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baz.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://htv.zhaomingkeji.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mgl.pengpengdd.cyou

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://khq.yj202588.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mgy.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ouo.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://eno.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fwf.zhixingplan.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://irs.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ozg.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://ovy.jinyuanbaomall.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zrm.gogol.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://axe.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bjz.snrcjt.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iiz.smart0.xyz

[E16] 数字千分位
来源：http://pji.guannengcc.top

Py:   f"{1234567:,}"
来源：http://ybi.svipenyu.cn

PHP:  number_format(1234567);
来源：http://asa.fzhhl.top

JS:   (1234567).toLocaleString("en-US")
来源：http://wmt.hcnkem.com

TS:   (1234567).toLocaleString("en-US")
来源：http://fov.shanyushiyangtech.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://urm.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zgr.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zfm.zycfv.cn

C#:   1234567.ToString("N0")
来源：http://xdu.redwolf501.top

[E17] 首字母大写
来源：http://ydn.guowangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lef.xinyue.icu

PHP:  ucfirst($s);  ucwords($s);
来源：http://nze.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xmj.hnxiangtu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nuj.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tgf.sweek.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kvc.yuanzhike.top

Ruby: s.capitalize
来源：http://jlz.zhiwuduotai.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cvz.jqgufenzy.top

[E18] 模板占位符替换
来源：http://mdj.52xcode.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uah.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gjg.haohaochexian.top

JS:   tpl.replaceAll("{name}", name)
来源：http://pmq.sweek.top

TS:   tpl.replaceAll("{name}", name)
来源：http://crg.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xxw.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://slc.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zpe.cheryme.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vbk.cashguo.top

[E19] 多行文本按行拆分
来源：http://hvw.guowangkeji.top

Py:   s.splitlines()
来源：http://wjw.ydjk.org.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://imi.quarkkingdee.top

JS:   s.split(/\r?\n/)
来源：http://fgq.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://taj.ctjpmb.com

Java: s.lines().toList()
来源：http://zqq.yuanzhike.top

Go:   strings.Split(s, "\n")
来源：http://plw.hywenlv.cn

Ruby: s.lines
来源：http://yza.vehdjk.com

C#:   s.Split('\n')
来源：http://idu.yj20258888.top

[E20] 判断字符串是否为空
来源：http://qju.hesvh.cn

Py:   if not s:
来源：http://zxm.ivvv.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vbq.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tvb.nwbrower.top

TS:   if (s === "") {}
来源：http://vjs.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://tmr.gaohongyu789.top

Go:   if s == "" {}
来源：http://dhw.ybcxt.top

Ruby: if s.empty?
来源：http://oct.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kna.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://mmc.jqgufenzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qry.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gfl.kuanghao11.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ejf.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xqi.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gvg.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://hbg.9152youxi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lxf.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ogp.daria6918.cn

[E22] 字节长度与字符长度
来源：http://bii.cucudq.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oky.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fhb.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xea.birdmap.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wtz.ctjpmb.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zxt.jinyuanbaomall.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bwg.zdqjudy.top

Ruby: s.bytesize;  s.length
来源：http://ldn.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://zbd.chenlongwang.top

================================================================================
来源：http://lub.yj202588.top

F. 文件与目录
来源：http://ody.meibo888.top

================================================================================
来源：http://qqq.feifeiyinyue.top

[F01] 读取整个文件
来源：http://yhq.yuanzhike.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tcp.hysaishi.cn

PHP:  file_get_contents("a.txt");
来源：http://mxw.c1oappe.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gfd.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://afn.c1oappe.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vuj.aibaodan.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jnr.ydzc1.top

Ruby: File.read("a.txt")
来源：http://rxh.52xcode.cn

C#:   File.ReadAllText("a.txt");
来源：http://pxq.ywan-chungtsiang.top

[F02] 逐行读取文件
来源：http://kbn.fktsv.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ynb.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ptu.ctjpmb.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wwk.hysaishi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://chr.jqgfzy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qym.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vtw.hnqzz.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jtt.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bub.316326.xyz

[F03] 写入文件（覆盖）
来源：http://oib.xylfe.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qvn.fktsv.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xew.vehdjk.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uuf.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dtb.shuidangran.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://imo.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mlg.ehwqpu.com

Ruby: File.write("a.txt", "hi")
来源：http://eaw.iojbl.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lgf.tianlin.xyz

[F04] 追加写入文件
来源：http://awp.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nmn.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vza.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iny.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ntv.wangshuangyany.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://stt.zhengqikj.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ekl.cheryme.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mam.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zcd.jiagoushi.top

[F05] 判断文件或目录是否存在
来源：http://hpl.sxryk.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tdh.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://osz.zhongyouzk.top

JS:   fs.existsSync("a.txt")
来源：http://mxi.zhoulong.xyz

TS:   fs.existsSync("a.txt")
来源：http://evi.andypj.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://jhk.zhiwuduotai.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dyc.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://tgy.pengpengdd.cyou

C#:   File.Exists("a.txt")
来源：http://fmc.sufxvd.cn

[F06] 删除文件
来源：http://zth.meibo888.top

Py:   os.remove("a.txt")
来源：http://iwz.wangshuangyany.cn

PHP:  unlink("a.txt");
来源：http://uix.hysaishi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xpz.yj202588.top

TS:   fs.unlinkSync("a.txt")
来源：http://ufg.cashguo.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bol.aibaodan.cn

Go:   os.Remove("a.txt")
来源：http://ool.hfpthk.cn

Ruby: File.delete("a.txt")
来源：http://dvt.dianchejie.cn

C#:   File.Delete("a.txt");
来源：http://whx.jqgufenzy.top

[F07] 创建目录（含多级）
来源：http://omp.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gvf.xylfe.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rir.yuxming.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fbu.gogol.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bss.zhaomingkeji.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fgu.ybcxt.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hhc.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://caq.cheryme.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gnr.shangyingyoupin.top

[F08] 遍历目录
来源：http://rzt.fehbvm.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://bys.zdqjudy.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rdd.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://lai.snrcjt.cn

TS:   fs.readdirSync("dir")
来源：http://kyj.cashguo.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ekk.chenzaomai.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://gmz.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://jkv.zycfv.cn

C#:   Directory.GetFiles("dir")
来源：http://loh.hnxiangtu.top

[F09] 获取文件大小
来源：http://jic.kuanghao11.cn

Py:   os.path.getsize("a.txt")
来源：http://tlq.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://gde.jinyuanbaomall.cn

JS:   fs.statSync("a.txt").size
来源：http://gty.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://okk.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://vwt.jyoumei.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qea.bjfxy.top

Ruby: File.size("a.txt")
来源：http://cha.gzhubu.top

C#:   new FileInfo("a.txt").Length
来源：http://hqb.nanxuanxn.top

[F10] 取文件扩展名 / 文件名
来源：http://svz.yongpay.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qcs.yj20258888.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bxy.vqdsnc.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://woc.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://slz.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bzc.epnwcf.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sou.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rti.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xqg.jqgfzy.top

[F11] 复制与移动文件
来源：http://neh.zdqjudy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://krn.fktsv.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kta.fktsv.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ifu.zdqjudy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nij.daxiang520.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lwk.nwbrower.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://brb.havefunace.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://kgu.andypj.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fln.shuidangran.top

[F12] CSV 读写
来源：http://iga.gzhubu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gnd.chenzaomai.com

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://tzf.vehdjk.com

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hrq.sysykeji.top

TS:   // 同上
来源：http://rgm.yangfankeji.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pjn.sufxvd.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://efl.yj20258888.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xjy.shuidangran.top

C#:   // 无内置：用 CsvHelper 库
来源：http://uwh.epnwcf.com

================================================================================
来源：http://zor.nanxinkj.top

G. 面向对象
来源：http://eoa.sjlbkw.cn

================================================================================
来源：http://rbl.jinqigufen.top

[G01] 定义类
来源：http://ggm.uphjek.com

Py:   class User: pass
来源：http://dli.snrcjt.cn

PHP:  class User {}
来源：http://jjw.shanyushiyangkeji.top

JS:   class User {}
来源：http://vzq.jlsjyb.cn

TS:   class User { name: string = ""; }
来源：http://kgm.yj20258.top

Java: class User {}
来源：http://eou.nanxinkj.top

Go:   type User struct { Name string }
来源：http://ymd.bbcook.cn

Ruby: class User; end
来源：http://uqv.jinghuilouyu.cn

C#:   class User {}
来源：http://dyz.yanxiufei.cn

[G02] 构造函数
来源：http://xjj.yanxiufei.cn

Py:   def __init__(self, name): self.name = name
来源：http://lhs.cdnleiting.top

PHP:  public function __construct(public string $name) {}
来源：http://cap.hnqzz.top

JS:   constructor(name) { this.name = name; }
来源：http://ods.hammf.cn

TS:   constructor(public name: string) {}
来源：http://gzt.hongshengwenyu.top

Java: User(String name) { this.name = name; }
来源：http://syw.ehwqpu.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xcn.chenjidiqi.icu

Ruby: def initialize(name); @name = name; end
来源：http://ifq.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://lnb.sysykeji.top

[G03] 实例属性
来源：http://fjd.ppjwa.cn

Py:   self.name = "x"
来源：http://adw.zdqjudy.top

PHP:  public string $name = "x";
来源：http://gbe.fzhhl.top

JS:   this.name = "x";
来源：http://whl.dianchejie.cn

TS:   name: string = "x";
来源：http://way.jinqigfzy.top

Java: private String name;
来源：http://yxp.birdmap.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pez.shanyushiyangtech.top

Ruby: @name = "x"
来源：http://owr.hfpthk.cn

C#:   public string Name { get; set; } = "x";
来源：http://eam.chenlongwang.top

[G04] 定义方法
来源：http://qxx.dashuyun.cn

Py:   def greet(self): return self.name
来源：http://xpc.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qht.cucudq.cn

JS:   greet() { return this.name; }
来源：http://hhc.gotoacloud.top

TS:   greet(): string { return this.name; }
来源：http://mlq.zhaomingkeji.xyz

Java: String greet() { return name; }
来源：http://bzo.snrcjt.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jew.hesvh.cn

Ruby: def greet; @name; end
来源：http://psr.snrcjt.cn

C#:   public string Greet() => Name;
来源：http://zgg.aizwys.cn

[G05] 继承
来源：http://bih.yfazqb.com

Py:   class Admin(User): pass
来源：http://vqw.vqdsnc.cn

PHP:  class Admin extends User {}
来源：http://hxs.pengpengdd.cyou

JS:   class Admin extends User {}
来源：http://jqv.tanke756.top

TS:   class Admin extends User {}
来源：http://wyh.mhx1999.top

Java: class Admin extends User {}
来源：http://smk.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tqa.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://lit.yj20258.top

C#:   class Admin : User {}
来源：http://aex.cashguo.top

[G06] 重写方法
来源：http://umo.ydzc1.top

Py:   def greet(self): return "admin"
来源：http://yrn.jqgufenzy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zsn.fengsongda.top

JS:   greet() { return "admin"; }
来源：http://aob.0kj1m.cn

TS:   greet(): string { return "admin"; }
来源：http://zfd.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://lwr.jqgfzy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xuh.jinghuilouyu.cn

Ruby: def greet; "admin"; end
来源：http://kky.shangyingyoupin.top

C#:   public override string Greet() => "admin";
来源：http://jue.xylfe.cn

[G07] 调用父类方法
来源：http://wzb.feifeiyinyue.top

Py:   super().greet()
来源：http://egi.jqgfzy.top

PHP:  parent::greet();
来源：http://rbv.redwolf501.top

JS:   super.greet();
来源：http://lhb.daria6918.cn

TS:   super.greet();
来源：http://tba.jlsjyb.cn

Java: super.greet();
来源：http://rwg.hysaishi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tdw.hcnkem.com

Ruby: super
来源：http://jwz.yfazqb.com

C#:   base.Greet();
来源：http://zjx.yonumen.top

[G08] 静态方法与属性
来源：http://iiq.ydjk.org.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jrn.yonumen.top


<!-- 参考信息 -->