代发 wailian999

Go:   strings.Join(items, ",")
来源：http://umq.bjfxy.top

Ruby: items.join(",")
来源：http://tgb.tanke756.top

C#:   string.Join(",", items)
来源：http://coo.ivvv.top

[E09] 去除所有空白字符
来源：http://iri.gotoacloud.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kpu.yonumen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fej.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://lhw.fengsongda.top

TS:   s.replace(/\s+/g, "")
来源：http://acn.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://uie.uphjek.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://abr.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://emt.9152youxi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hcg.xinyue.icu

[E10] 左侧补零 / 定长填充
来源：http://cvm.zycfv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dhf.52xcode.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kid.havefunace.top

JS:   "7".padStart(3, "0")
来源：http://jsl.sweek.top

TS:   "7".padStart(3, "0")
来源：http://dxo.ydjk.org.cn

Java: String.format("%03d", 7)
来源：http://yhp.c1oappe.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kdw.jqgufenzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nzy.ydjk.org.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gff.cdnleiting.top

[E11] 反转字符串
来源：http://eab.jinghuilouyu.cn

Py:   s[::-1]
来源：http://vkn.xziqi.cn

PHP:  strrev($s);
来源：http://saq.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://cgh.sufxvd.cn

TS:   [...s].reverse().join("")
来源：http://kwo.zhixingplan.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rla.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://eap.9152youxi.cn

Ruby: s.reverse
来源：http://yky.uphjek.com

C#:   new string(s.Reverse().ToArray())
来源：http://ksb.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://fef.chenjidiqi.icu

Py:   s.count("a")
来源：http://cyx.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://swd.fzhhl.top

JS:   s.split("a").length - 1
来源：http://zjt.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://icf.cqqwz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fxn.yonumen.top

Go:   strings.Count(s, "a")
来源：http://nbm.cucudq.cn

Ruby: s.count("a")
来源：http://qjc.mhx1999.top

C#:   s.Count(c => c == 'a')
来源：http://tdq.chenlongwang.top

[E13] 逐字符遍历
来源：http://eon.meibo888.top

Py:   for ch in s: print(ch)
来源：http://pcq.guowangkeji.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iph.jiagoushi.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://kqs.svipenyu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://who.xylfe.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ovm.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mam.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://dat.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vlz.haohaochexian.top

[E14] URL 编码与 Base64
来源：http://nst.cqqwz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ptl.guannengcc.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://arh.zhixingplan.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eds.zdqjudy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kmy.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oga.epnwcf.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oco.tianlin.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jes.gzhubu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cfp.pycfn.com

[E15] HTML 转义 / 反转义
来源：http://xaz.zhoulong.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://itj.birdmap.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dit.shuidangran.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sck.redwolf501.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tge.shanyushiyangkeji.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wvh.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://azw.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bal.bbcook.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rhc.hammf.cn

[E16] 数字千分位
来源：http://lty.jinghuilouyu.cn

Py:   f"{1234567:,}"
来源：http://zvz.yfazqb.com

PHP:  number_format(1234567);
来源：http://qzo.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://asl.xinyue.icu

TS:   (1234567).toLocaleString("en-US")
来源：http://tzf.aibaodan.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nxd.yueranfly.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nby.svipenyu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dxs.chenjidiqi.icu

C#:   1234567.ToString("N0")
来源：http://wdt.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://wmv.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xnq.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://uyb.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lze.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zij.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xub.xingfuxueyuan.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tug.yuanzhike.top

Ruby: s.capitalize
来源：http://eej.jiagoushi.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nkl.meibo888.top

[E18] 模板占位符替换
来源：http://grx.tarul.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fru.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qje.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://enk.shanyushiyangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://xxw.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rqy.yuxming.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rst.jyoumei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gar.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nqf.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://cus.zycfv.cn

Py:   s.splitlines()
来源：http://dep.svipenyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wfh.ehwqpu.com

JS:   s.split(/\r?\n/)
来源：http://fiu.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://ndx.tianlin.xyz

Java: s.lines().toList()
来源：http://ump.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://eno.ybcxt.top

Ruby: s.lines
来源：http://xei.zdbjq.cn

C#:   s.Split('\n')
来源：http://yhr.daxiang520.top

[E20] 判断字符串是否为空
来源：http://lsc.shanyushiyangkeji.top

Py:   if not s:
来源：http://zoh.yuxming.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://flx.nanxuanxn.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://upx.cashguo.top

TS:   if (s === "") {}
来源：http://dxv.sufxvd.cn

Java: if (s.isEmpty()) {}
来源：http://nay.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://frm.yueranfly.top

Ruby: if s.empty?
来源：http://qqx.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://avo.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://cql.quarkkingdee.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ukv.quarkkingdee.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pjz.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jnj.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://axt.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dci.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://jjg.hammf.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mfx.yangfankeji.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tya.fzhhl.top

[E22] 字节长度与字符长度
来源：http://mnd.guannengcc.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mlu.zdqjudy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pyt.pycfn.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pbk.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yqq.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://unu.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ygh.zhijiandao.cn

Ruby: s.bytesize;  s.length
来源：http://eic.nwbrower.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wbd.wangdashe.top

================================================================================
来源：http://vwf.xylfe.cn

F. 文件与目录
来源：http://ezb.52xcode.cn

================================================================================
来源：http://enu.xuetiantiany.cn

[F01] 读取整个文件
来源：http://iks.zhijiandao.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://neb.gaohongyu789.top

PHP:  file_get_contents("a.txt");
来源：http://gse.yangfankeji.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://trv.shanyushiyangtech.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sli.sweek.top

Java: Files.readString(Path.of("a.txt"))
来源：http://xyh.sjlbkw.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tic.ywan-chungtsiang.top

Ruby: File.read("a.txt")
来源：http://rdx.ctjpmb.com

C#:   File.ReadAllText("a.txt");
来源：http://vts.tanke756.top

[F02] 逐行读取文件
来源：http://lsk.ydjk.org.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ofd.cucudq.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://npe.xziqi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rvj.bbcook.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hye.meibo888.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hee.nanxinkj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://whv.yfazqb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nfi.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vhz.jinyuanbaomall.cn

[F03] 写入文件（覆盖）
来源：http://xcb.ehwqpu.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ufp.zhiwuduotai.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://czc.chenzaomai.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dzg.chenlongwang.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xmr.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://myt.fzhhl.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eba.jinqigfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://rns.ctjpmb.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bty.jyoumei.cn

[F04] 追加写入文件
来源：http://hrf.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wfy.zhijiandao.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tbw.bbcook.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ieh.zhijiandao.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://djt.yuanzhike.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xhu.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fxm.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xxg.hesvh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nsy.pengpengdd.cyou

[F05] 判断文件或目录是否存在
来源：http://zud.dashuyun.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rxx.feifeiyinyue.top

PHP:  file_exists("a.txt");
来源：http://uhx.sweek.top

JS:   fs.existsSync("a.txt")
来源：http://rqg.yj20258888.top

TS:   fs.existsSync("a.txt")
来源：http://sih.bbcook.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aim.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gjc.ppjwa.cn

Ruby: File.exist?("a.txt")
来源：http://pwf.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://cvt.dianchejie.cn

[F06] 删除文件
来源：http://axc.yuxming.cn

Py:   os.remove("a.txt")
来源：http://sdt.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://bbh.haohaochexian.top

JS:   fs.unlinkSync("a.txt")
来源：http://wrv.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://xyw.yonumen.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iza.hnxiangtu.top

Go:   os.Remove("a.txt")
来源：http://psp.pengpengdd.cyou

Ruby: File.delete("a.txt")
来源：http://mkl.nanxuanxn.top

C#:   File.Delete("a.txt");
来源：http://kpp.andypj.xyz

[F07] 创建目录（含多级）
来源：http://ltk.jinqigufen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jml.xuanzx.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mdx.shangyingyoupin.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ljp.yj20258.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jha.sufxvd.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uai.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hwu.ywan-chungtsiang.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://apt.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cdg.cdnleiting.top

[F08] 遍历目录
来源：http://spl.chenlongwang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yay.ydzc1.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aax.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://jxn.yj20258888.top

TS:   fs.readdirSync("dir")
来源：http://mak.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xxs.feifeiyinyue.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://wku.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://oyd.yj20258.top

C#:   Directory.GetFiles("dir")
来源：http://hfu.haohaochexian.top

[F09] 获取文件大小
来源：http://lri.mhx1999.top

Py:   os.path.getsize("a.txt")
来源：http://jzt.jinqigfzy.top

PHP:  filesize("a.txt");
来源：http://vrf.yonumen.top

JS:   fs.statSync("a.txt").size
来源：http://vzk.jyoumei.cn

TS:   fs.statSync("a.txt").size
来源：http://vrc.fanxiaobao.xyz

Java: Files.size(Path.of("a.txt"))
来源：http://crp.yvedp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xcj.fanxiaobao.xyz

Ruby: File.size("a.txt")
来源：http://ywu.kuanghao11.cn

C#:   new FileInfo("a.txt").Length
来源：http://ttw.aibaodan.cn

[F10] 取文件扩展名 / 文件名
来源：http://oqh.cashguo.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eke.hnqzz.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ygb.9152youxi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pcp.gzhubu.top

TS:   path.extname("a.txt")
来源：http://vgu.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wwp.yonumen.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nwa.sxryk.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://plt.wangdashe.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wql.tian-w.cn

[F11] 复制与移动文件
来源：http://wxp.tianlin.xyz

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cax.cqqwz.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kmp.tian-w.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cmx.xylfe.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://thm.xuetiantiany.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tou.yj20258888.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nlk.pengpengdd.cyou

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wvs.mhx1999.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jbm.zdqjudy.top

[F12] CSV 读写
来源：http://wap.yueranfly.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zui.yj20258888.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vrj.mhx1999.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://odm.sysykeji.top

TS:   // 同上
来源：http://nsh.kuanghao11.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rag.jianghu66.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vgq.andypj.xyz

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cwf.zhoulong.xyz

C#:   // 无内置：用 CsvHelper 库
来源：http://gcy.0kj1m.cn

================================================================================
来源：http://rao.tarul.cn

G. 面向对象
来源：http://rtf.fengsongda.top

================================================================================
来源：http://ygw.nanxinkj.top

[G01] 定义类
来源：http://tzy.xylfe.cn

Py:   class User: pass
来源：http://rzq.ydjk.org.cn

PHP:  class User {}
来源：http://slh.xinyue.icu

JS:   class User {}
来源：http://kgb.xuetiantiany.cn

TS:   class User { name: string = ""; }
来源：http://ogz.zhongyouzk.top

Java: class User {}
来源：http://yqf.gogol.net.cn

Go:   type User struct { Name string }
来源：http://tja.pycfn.com

Ruby: class User; end
来源：http://upw.hfpthk.cn

C#:   class User {}
来源：http://vnm.yfazqb.com

[G02] 构造函数
来源：http://mbs.birdmap.top

Py:   def __init__(self, name): self.name = name
来源：http://psf.ppjwa.cn

PHP:  public function __construct(public string $name) {}
来源：http://ztk.pycfn.com

JS:   constructor(name) { this.name = name; }
来源：http://xii.c1oappe.top

TS:   constructor(public name: string) {}
来源：http://xxy.redwolf501.top

Java: User(String name) { this.name = name; }
来源：http://sum.tarul.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pul.sysykeji.top

Ruby: def initialize(name); @name = name; end
来源：http://vzw.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://hpf.jiagoushi.top

[G03] 实例属性
来源：http://buv.zhengqikj.top

Py:   self.name = "x"
来源：http://pzy.yj20258888.top

PHP:  public string $name = "x";
来源：http://sch.shangyingyoupin.top

JS:   this.name = "x";
来源：http://oth.zdbjq.cn

TS:   name: string = "x";
来源：http://pem.shanyushiyangkeji.top

Java: private String name;
来源：http://eku.sufxvd.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ioh.xuetiantiany.cn

Ruby: @name = "x"
来源：http://dtl.yj20258.top

C#:   public string Name { get; set; } = "x";
来源：http://rot.vehdjk.com

[G04] 定义方法
来源：http://adx.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://yot.zhongyouzk.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tof.cucudq.cn

JS:   greet() { return this.name; }
来源：http://npa.cucudq.cn

TS:   greet(): string { return this.name; }
来源：http://amo.yangfankeji.com

Java: String greet() { return name; }
来源：http://iin.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://sjl.fzhhl.top

Ruby: def greet; @name; end
来源：http://vpm.jinyuanbaomall.cn

C#:   public string Greet() => Name;
来源：http://qfy.cashguo.top

[G05] 继承
来源：http://clm.snrcjt.cn

Py:   class Admin(User): pass
来源：http://ode.hfpthk.cn

PHP:  class Admin extends User {}
来源：http://qoc.zycfv.cn

JS:   class Admin extends User {}
来源：http://sgz.pycfn.com

TS:   class Admin extends User {}
来源：http://qwr.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://gwc.cqqwz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cfz.sysykeji.top

Ruby: class Admin < User; end
来源：http://tik.vqdsnc.cn

C#:   class Admin : User {}
来源：http://hya.zhijiandao.cn

[G06] 重写方法
来源：http://oob.jyoumei.cn

Py:   def greet(self): return "admin"
来源：http://lit.yongpay.top

PHP:  public function greet(): string { return "admin"; }
来源：http://iev.aibaodan.cn

JS:   greet() { return "admin"; }
来源：http://fkv.9152youxi.cn

TS:   greet(): string { return "admin"; }
来源：http://yrp.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://tca.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qau.uphjek.com

Ruby: def greet; "admin"; end
来源：http://riu.zhengqikj.top

C#:   public override string Greet() => "admin";
来源：http://whz.sxryk.cn

[G07] 调用父类方法
来源：http://zyp.uphjek.com

Py:   super().greet()
来源：http://ahx.shzxlz.cn

PHP:  parent::greet();
来源：http://ift.kuanghao11.cn


<!-- 参考信息 -->