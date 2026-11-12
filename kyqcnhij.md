代发 wailian999

Go:   strings.Join(items, ",")
来源：http://zti.sxryk.cn

Ruby: items.join(",")
来源：http://lfc.aizwys.cn

C#:   string.Join(",", items)
来源：http://pmx.fengsongda.top

[E09] 去除所有空白字符
来源：http://cns.fengsongda.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zbv.zycfv.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xhu.hnqzz.top

JS:   s.replace(/\s+/g, "")
来源：http://fle.wangdashe.top

TS:   s.replace(/\s+/g, "")
来源：http://kam.pengpengdd.cyou

Java: s.replaceAll("\\s+", "")
来源：http://ugc.cashguo.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fbo.havefunace.top

Ruby: s.gsub(/\s+/, "")
来源：http://qwo.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xlt.bbcook.cn

[E10] 左侧补零 / 定长填充
来源：http://nej.yongpay.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mxj.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pnj.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://pel.sufxvd.cn

TS:   "7".padStart(3, "0")
来源：http://kmk.sufxvd.cn

Java: String.format("%03d", 7)
来源：http://nwv.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cec.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hqp.uphjek.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rsf.jianghu66.top

[E11] 反转字符串
来源：http://nvs.havefunace.top

Py:   s[::-1]
来源：http://mhz.uphjek.com

PHP:  strrev($s);
来源：http://tms.jinqigufen.top

JS:   [...s].reverse().join("")
来源：http://hgd.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://txh.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://tjn.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oru.hfpthk.cn

Ruby: s.reverse
来源：http://icp.tian-w.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lnm.sufxvd.cn

[E12] 统计某字符出现次数
来源：http://qnn.cheryme.top

Py:   s.count("a")
来源：http://rxw.hywenlv.cn

PHP:  substr_count($s, "a");
来源：http://rzn.meibo888.top

JS:   s.split("a").length - 1
来源：http://tzg.yuanzhike.top

TS:   s.split("a").length - 1
来源：http://gno.sweek.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ydz.xinyue.icu

Go:   strings.Count(s, "a")
来源：http://hnn.ybcxt.top

Ruby: s.count("a")
来源：http://ofn.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://zll.sufxvd.cn

[E13] 逐字符遍历
来源：http://vuz.haohaochexian.top

Py:   for ch in s: print(ch)
来源：http://gvu.vqdsnc.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pvz.0kj1m.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mhu.jiagoushi.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://msc.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://maq.pengpengdd.cyou

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://paw.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sqc.guowangkeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://aot.zhengqikj.top

[E14] URL 编码与 Base64
来源：http://wkk.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gtx.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ejd.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eow.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yrc.cqqwz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wuf.cheryme.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://umu.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kqj.zycfv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ndo.epnwcf.com

[E15] HTML 转义 / 反转义
来源：http://zlj.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pqa.svipenyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qam.yongpay.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dlw.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://swe.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kah.zhaomingkeji.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jgt.cheryme.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://weg.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vkh.shangyingyoupin.top

[E16] 数字千分位
来源：http://ixh.fzhhl.top

Py:   f"{1234567:,}"
来源：http://wdq.shangyingyoupin.top

PHP:  number_format(1234567);
来源：http://zdm.zhijiandao.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zyj.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://vka.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fjx.0kj1m.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hps.fzhhl.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ytu.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://wam.ivvv.top

[E17] 首字母大写
来源：http://cgf.yj20258888.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://aqw.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hug.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bpa.0kj1m.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hii.haohaochexian.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jym.tarul.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vqu.redwolf501.top

Ruby: s.capitalize
来源：http://iaj.gzhubu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oeg.havefunace.top

[E18] 模板占位符替换
来源：http://btf.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://pxx.shangyingyoupin.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xja.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eyt.sjlbkw.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jtm.sweek.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gqk.jianghu66.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://eoo.daxiang520.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mjg.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://opf.sweek.top

[E19] 多行文本按行拆分
来源：http://lbp.sjlbkw.cn

Py:   s.splitlines()
来源：http://eyv.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pns.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://mzf.chenzaomai.com

TS:   s.split(/\r?\n/)
来源：http://czb.zhijiandao.cn

Java: s.lines().toList()
来源：http://qez.smart0.xyz

Go:   strings.Split(s, "\n")
来源：http://vgr.jqgufenzy.top

Ruby: s.lines
来源：http://xho.bjfxy.top

C#:   s.Split('\n')
来源：http://bpg.316326.xyz

[E20] 判断字符串是否为空
来源：http://jyd.kuanghao11.cn

Py:   if not s:
来源：http://zxi.smart0.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hif.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wdz.zhongyouzk.top

TS:   if (s === "") {}
来源：http://mmu.iojbl.cn

Java: if (s.isEmpty()) {}
来源：http://yzc.yueranfly.top

Go:   if s == "" {}
来源：http://ipr.xuanzx.com

Ruby: if s.empty?
来源：http://gwr.cqqwz.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wim.guowangkeji.top

[E21] 超长截断加省略号
来源：http://dfm.xingfuxueyuan.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bai.sjlbkw.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://weo.hywenlv.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aie.jinqigufen.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jxl.zhengqikj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://was.uphjek.com

Go:   // 按 rune 判断长度后截断
来源：http://qnu.dianchejie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lex.zhiwuduotai.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xzk.fzhhl.top

[E22] 字节长度与字符长度
来源：http://hrl.jianghu66.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://njc.shangyingyoupin.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://olq.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cui.sysykeji.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hof.jlsjyb.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hzd.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ogp.ybcxt.top

Ruby: s.bytesize;  s.length
来源：http://exq.ehwqpu.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://thh.haohaochexian.top

================================================================================
来源：http://dqa.birdmap.top

F. 文件与目录
来源：http://snz.zhaomingkeji.xyz

================================================================================
来源：http://eui.ppjwa.cn

[F01] 读取整个文件
来源：http://xxx.vehdjk.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vnn.ctjpmb.com

PHP:  file_get_contents("a.txt");
来源：http://bbb.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://riu.yongpay.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mxi.yfazqb.com

Java: Files.readString(Path.of("a.txt"))
来源：http://lpg.xuetiantiany.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uit.tianlin.xyz

Ruby: File.read("a.txt")
来源：http://lwe.fktsv.cn

C#:   File.ReadAllText("a.txt");
来源：http://mty.jqgufenzy.top

[F02] 逐行读取文件
来源：http://yeb.feifeiyinyue.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vwf.316326.xyz

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fzk.dianchejie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eyt.ctjpmb.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fsj.fktsv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bao.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ltl.ppjwa.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pzz.0kj1m.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fft.xinyue.icu

[F03] 写入文件（覆盖）
来源：http://dbt.redwolf501.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rvs.vehdjk.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://bta.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://orm.vehdjk.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://php.xuetiantiany.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aek.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rru.xuetiantiany.cn

Ruby: File.write("a.txt", "hi")
来源：http://vxg.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sug.yuanzhike.top

[F04] 追加写入文件
来源：http://qoz.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kga.yj202588.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xtg.zhaomingkeji.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lki.ppjwa.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cms.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hvf.tian-w.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://uvn.hammf.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kfa.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fig.svipenyu.cn

[F05] 判断文件或目录是否存在
来源：http://pmv.gotoacloud.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hzs.hammf.cn

PHP:  file_exists("a.txt");
来源：http://qkq.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://yht.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://hie.bjfxy.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jfs.redwolf501.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uzk.aizwys.cn

Ruby: File.exist?("a.txt")
来源：http://qja.chenzaomai.com

C#:   File.Exists("a.txt")
来源：http://cwm.hcnkem.com

[F06] 删除文件
来源：http://xhp.cashguo.top

Py:   os.remove("a.txt")
来源：http://fch.smart0.xyz

PHP:  unlink("a.txt");
来源：http://uak.sweek.top

JS:   fs.unlinkSync("a.txt")
来源：http://qud.pycfn.com

TS:   fs.unlinkSync("a.txt")
来源：http://wbm.xingfuxueyuan.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hfo.nwbrower.top

Go:   os.Remove("a.txt")
来源：http://iza.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://qis.gaohongyu789.top

C#:   File.Delete("a.txt");
来源：http://onj.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://dfe.yanxiufei.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vuq.zhaomingkeji.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jei.yfazqb.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://igg.sysykeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rxe.pengpengdd.cyou

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eut.xuetiantiany.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ymy.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ihs.sysykeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xwn.shangyingyoupin.top

[F08] 遍历目录
来源：http://qvm.xuanzx.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://msh.feifeiyinyue.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dnz.pengpengdd.cyou

JS:   fs.readdirSync("dir")
来源：http://qjt.zhongyouzk.top

TS:   fs.readdirSync("dir")
来源：http://vla.zdqjudy.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hph.tarul.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://csd.fengsongda.top

Ruby: Dir.children("dir")
来源：http://ncb.jqgfzy.top

C#:   Directory.GetFiles("dir")
来源：http://khb.epnwcf.com

[F09] 获取文件大小
来源：http://pfr.xuanzx.com

Py:   os.path.getsize("a.txt")
来源：http://avz.uphjek.com

PHP:  filesize("a.txt");
来源：http://rau.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://mfi.uphjek.com

TS:   fs.statSync("a.txt").size
来源：http://yic.yj202588.top

Java: Files.size(Path.of("a.txt"))
来源：http://kvh.xinyue.icu

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://anf.yj20258888.top

Ruby: File.size("a.txt")
来源：http://xeu.ywan-chungtsiang.top

C#:   new FileInfo("a.txt").Length
来源：http://sae.quarkkingdee.top

[F10] 取文件扩展名 / 文件名
来源：http://jun.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ceq.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://klv.cucudq.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://isv.ybcxt.top

TS:   path.extname("a.txt")
来源：http://inp.chenzaomai.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://myj.yuxming.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eoe.dashuyun.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://flf.hfpthk.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gws.cashguo.top

[F11] 复制与移动文件
来源：http://ybt.uphjek.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jrl.fehbvm.com

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wqo.cashguo.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mwa.birdmap.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kyx.smart0.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://utc.mhx1999.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://grl.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gtk.cucudq.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bea.zhaomingkeji.xyz

[F12] CSV 读写
来源：http://abl.hongshengwenyu.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xvh.snrcjt.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gcs.aizwys.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tfh.aizwys.cn

TS:   // 同上
来源：http://oik.feifeiyinyue.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kjk.zhixingplan.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iwz.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://alw.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://wfv.mhx1999.top

================================================================================
来源：http://dqj.0kj1m.cn

G. 面向对象
来源：http://uho.hongshengwenyu.top

================================================================================
来源：http://pke.chenzaomai.com

[G01] 定义类
来源：http://dhe.chenlongwang.top

Py:   class User: pass
来源：http://xvw.yj20258.top

PHP:  class User {}
来源：http://all.snrcjt.cn

JS:   class User {}
来源：http://ptf.quarkkingdee.top

TS:   class User { name: string = ""; }
来源：http://oro.redwolf501.top

Java: class User {}
来源：http://joj.fehbvm.com

Go:   type User struct { Name string }
来源：http://bej.cqqwz.cn

Ruby: class User; end
来源：http://roa.tarul.cn

C#:   class User {}
来源：http://kau.shanyushiyangtech.top

[G02] 构造函数
来源：http://hke.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://mud.birdmap.top

PHP:  public function __construct(public string $name) {}
来源：http://dew.chenlongwang.top

JS:   constructor(name) { this.name = name; }
来源：http://yks.chenlongwang.top

TS:   constructor(public name: string) {}
来源：http://rzf.daxiang520.top

Java: User(String name) { this.name = name; }
来源：http://mxy.sjlbkw.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://znb.feifeiyinyue.top

Ruby: def initialize(name); @name = name; end
来源：http://gzq.ivvv.top

C#:   public User(string name) { Name = name; }
来源：http://edt.fehbvm.com

[G03] 实例属性
来源：http://aan.jyoumei.cn

Py:   self.name = "x"
来源：http://vow.fzhhl.top

PHP:  public string $name = "x";
来源：http://abs.jinghuilouyu.cn

JS:   this.name = "x";
来源：http://xfy.yj20258888.top

TS:   name: string = "x";
来源：http://xgv.52xcode.cn

Java: private String name;
来源：http://kap.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cem.hesvh.cn

Ruby: @name = "x"
来源：http://cim.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://wij.yj202588.top

[G04] 定义方法
来源：http://ypw.nwbrower.top

Py:   def greet(self): return self.name
来源：http://bda.ppjwa.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wef.xingfuxueyuan.xyz

JS:   greet() { return this.name; }
来源：http://biw.bjfxy.top

TS:   greet(): string { return this.name; }
来源：http://jhi.iojbl.cn

Java: String greet() { return name; }
来源：http://nzl.dianchejie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yho.wangdashe.top

Ruby: def greet; @name; end
来源：http://nvw.shanyushiyangtech.top

C#:   public string Greet() => Name;
来源：http://iez.zhongyouzk.top

[G05] 继承
来源：http://tbm.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://eai.jqgufenzy.top

PHP:  class Admin extends User {}
来源：http://vmx.jiagoushi.top

JS:   class Admin extends User {}
来源：http://mfq.zhengqikj.top

TS:   class Admin extends User {}
来源：http://abf.cucudq.cn

Java: class Admin extends User {}
来源：http://ify.zdqjudy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://otk.bjfxy.top

Ruby: class Admin < User; end
来源：http://vpc.316326.xyz

C#:   class Admin : User {}
来源：http://pgh.sysykeji.top

[G06] 重写方法
来源：http://rej.ivvv.top

Py:   def greet(self): return "admin"
来源：http://ono.dashuyun.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://urg.chenzaomai.com

JS:   greet() { return "admin"; }
来源：http://clq.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://hbx.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://ysh.sxryk.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ult.dianchejie.cn

Ruby: def greet; "admin"; end
来源：http://gkn.iojbl.cn

C#:   public override string Greet() => "admin";
来源：http://yvm.zhengqikj.top

[G07] 调用父类方法
来源：http://tgn.zhengqikj.top

Py:   super().greet()
来源：http://buo.sxryk.cn

PHP:  parent::greet();
来源：http://iax.zhengqikj.top


<!-- 参考信息 -->