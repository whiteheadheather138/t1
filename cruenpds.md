代发 wailian999

Go:   strings.Join(items, ",")
来源：http://ldv.hcnkem.com

Ruby: items.join(",")
来源：http://jvq.zhijiandao.cn

C#:   string.Join(",", items)
来源：http://mko.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://wyd.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vdx.yfazqb.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mvx.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://fas.xziqi.cn

TS:   s.replace(/\s+/g, "")
来源：http://nqq.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://mrg.ppjwa.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nhe.c1oappe.top

Ruby: s.gsub(/\s+/, "")
来源：http://dqt.guannengcc.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nut.yueranfly.top

[E10] 左侧补零 / 定长填充
来源：http://rlb.hnxiangtu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kct.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kdh.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://lmx.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://siq.yueranfly.top

Java: String.format("%03d", 7)
来源：http://kwj.sweek.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://jrk.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://deo.fehbvm.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nyc.wangshuangyany.cn

[E11] 反转字符串
来源：http://ozd.guowangkeji.top

Py:   s[::-1]
来源：http://rzq.feifeiyinyue.top

PHP:  strrev($s);
来源：http://iyw.gaohongyu789.top

JS:   [...s].reverse().join("")
来源：http://gxb.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://xht.yongpay.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ncr.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://qbw.wangdashe.top

Ruby: s.reverse
来源：http://xkr.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://vvr.daria6918.cn

[E12] 统计某字符出现次数
来源：http://wky.jyoumei.cn

Py:   s.count("a")
来源：http://sme.jqgfzy.top

PHP:  substr_count($s, "a");
来源：http://syf.meibo888.top

JS:   s.split("a").length - 1
来源：http://vyr.chenzaomai.com

TS:   s.split("a").length - 1
来源：http://wyw.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gbu.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://roo.hywenlv.cn

Ruby: s.count("a")
来源：http://vkc.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://lzp.tarul.cn

[E13] 逐字符遍历
来源：http://ing.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://khy.sweek.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hmk.hnqzz.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nvw.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://xtd.havefunace.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hey.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rif.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ihv.sweek.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bzc.tian-w.cn

[E14] URL 编码与 Base64
来源：http://bfs.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ixq.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ejj.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://oqg.yj20258.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://oqf.hammf.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xje.jinyuanbaomall.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tes.aibaodan.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ubw.vehdjk.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ktb.daria6918.cn

[E15] HTML 转义 / 反转义
来源：http://zuj.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://khw.jinghuilouyu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://owy.meibo888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://plf.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ojl.zycfv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://exz.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ncg.guannengcc.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fsp.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ifq.yanxiufei.cn

[E16] 数字千分位
来源：http://rdp.tian-w.cn

Py:   f"{1234567:,}"
来源：http://aod.epnwcf.com

PHP:  number_format(1234567);
来源：http://juv.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eqh.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://spe.xuetiantiany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://zsi.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oka.gogol.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://egz.xuanzx.com

C#:   1234567.ToString("N0")
来源：http://dyk.316326.xyz

[E17] 首字母大写
来源：http://hwn.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ovx.9152youxi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fsq.nanxinkj.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://khc.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kmc.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pfc.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mig.yj20258.top

Ruby: s.capitalize
来源：http://mzc.sjlbkw.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kxa.cheryme.top

[E18] 模板占位符替换
来源：http://rjg.yonumen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jnz.cashguo.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://giq.zhijiandao.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://crl.zhiwuduotai.top

TS:   tpl.replaceAll("{name}", name)
来源：http://cfx.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jmw.hcnkem.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://slw.daria6918.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pmd.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aui.zdbjq.cn

[E19] 多行文本按行拆分
来源：http://oui.bjfxy.top

Py:   s.splitlines()
来源：http://hfe.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pey.snrcjt.cn

JS:   s.split(/\r?\n/)
来源：http://fry.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://fhd.hywenlv.cn

Java: s.lines().toList()
来源：http://vxg.jyoumei.cn

Go:   strings.Split(s, "\n")
来源：http://pup.yuanzhike.top

Ruby: s.lines
来源：http://cmg.jianghu66.top

C#:   s.Split('\n')
来源：http://var.jiagoushi.top

[E20] 判断字符串是否为空
来源：http://ame.shzxlz.cn

Py:   if not s:
来源：http://mbg.fzhhl.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mlu.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cfx.chenlongwang.top

TS:   if (s === "") {}
来源：http://esg.snrcjt.cn

Java: if (s.isEmpty()) {}
来源：http://poe.tianlin.xyz

Go:   if s == "" {}
来源：http://uiq.shangyingyoupin.top

Ruby: if s.empty?
来源：http://aqg.0kj1m.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://iue.tarul.cn

[E21] 超长截断加省略号
来源：http://xlj.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ckq.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hqx.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fbr.svipenyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kmw.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fak.hammf.cn

Go:   // 按 rune 判断长度后截断
来源：http://jjt.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vff.52xcode.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dww.bbcook.cn

[E22] 字节长度与字符长度
来源：http://sak.zhaomingkeji.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://von.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wpa.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://avp.cheryme.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ohd.jinyuanbaomall.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eql.gaohongyu789.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://aab.cashguo.top

Ruby: s.bytesize;  s.length
来源：http://pjp.316326.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xht.haohaochexian.top

================================================================================
来源：http://dol.sufxvd.cn

F. 文件与目录
来源：http://tba.jyoumei.cn

================================================================================
来源：http://aqp.hongshengwenyu.top

[F01] 读取整个文件
来源：http://mdx.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yvc.jianghu66.top

PHP:  file_get_contents("a.txt");
来源：http://zzk.hywenlv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xwn.zhixingplan.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://puc.shzxlz.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xse.meibo888.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ryv.zdbjq.cn

Ruby: File.read("a.txt")
来源：http://rqm.chenlongwang.top

C#:   File.ReadAllText("a.txt");
来源：http://pms.zhongyouzk.top

[F02] 逐行读取文件
来源：http://uia.chenlongwang.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dpd.ywan-chungtsiang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xhu.hcnkem.com

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ixd.hesvh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gwu.xingfuxueyuan.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://dru.yongpay.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bps.zhaomingkeji.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://szx.fzhhl.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cst.dashuyun.cn

[F03] 写入文件（覆盖）
来源：http://kyi.gotoacloud.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uip.fengsongda.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mov.316326.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bil.chenjidiqi.icu

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dzm.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sci.hywenlv.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dnx.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://duq.yuxming.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gqm.jyoumei.cn

[F04] 追加写入文件
来源：http://rmk.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lxd.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fpf.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qga.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hle.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://oci.snrcjt.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wsg.jyoumei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fek.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://udk.gzhubu.top

[F05] 判断文件或目录是否存在
来源：http://qvz.jinghuilouyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sfl.ivvv.top

PHP:  file_exists("a.txt");
来源：http://bkh.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://oci.gaohongyu789.top

TS:   fs.existsSync("a.txt")
来源：http://yli.cheryme.top

Java: Files.exists(Path.of("a.txt"))
来源：http://ehs.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://uix.yfazqb.com

Ruby: File.exist?("a.txt")
来源：http://vas.ydjk.org.cn

C#:   File.Exists("a.txt")
来源：http://vca.jinyuanbaomall.cn

[F06] 删除文件
来源：http://smq.jinghuilouyu.cn

Py:   os.remove("a.txt")
来源：http://hwl.jinqigufen.top

PHP:  unlink("a.txt");
来源：http://mhg.birdmap.top

JS:   fs.unlinkSync("a.txt")
来源：http://zgx.xylfe.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pxe.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nys.zdqjudy.top

Go:   os.Remove("a.txt")
来源：http://puh.shanyushiyangtech.top

Ruby: File.delete("a.txt")
来源：http://bsd.fktsv.cn

C#:   File.Delete("a.txt");
来源：http://eph.zhiwuduotai.top

[F07] 创建目录（含多级）
来源：http://fsl.hnqzz.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://crv.c1oappe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://utq.shzxlz.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bcg.nanxuanxn.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hmz.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://saa.hywenlv.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nle.redwolf501.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vnu.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://moe.jinyuanbaomall.cn

[F08] 遍历目录
来源：http://pwu.birdmap.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://frk.sweek.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fmi.jianghu66.top

JS:   fs.readdirSync("dir")
来源：http://xag.ydzc1.top

TS:   fs.readdirSync("dir")
来源：http://suy.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bnc.shzxlz.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wtk.xziqi.cn

Ruby: Dir.children("dir")
来源：http://nwu.shuidangran.top

C#:   Directory.GetFiles("dir")
来源：http://cvw.cucudq.cn

[F09] 获取文件大小
来源：http://qdm.zdqjudy.top

Py:   os.path.getsize("a.txt")
来源：http://qgl.meibo888.top

PHP:  filesize("a.txt");
来源：http://gvb.tanke756.top

JS:   fs.statSync("a.txt").size
来源：http://yls.yfazqb.com

TS:   fs.statSync("a.txt").size
来源：http://ewa.havefunace.top

Java: Files.size(Path.of("a.txt"))
来源：http://cts.shanyushiyangtech.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zgm.zhiwuduotai.top

Ruby: File.size("a.txt")
来源：http://tfy.yueranfly.top

C#:   new FileInfo("a.txt").Length
来源：http://pwc.sjlbkw.cn

[F10] 取文件扩展名 / 文件名
来源：http://mgg.birdmap.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://azo.ivvv.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bos.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wfr.quarkkingdee.top

TS:   path.extname("a.txt")
来源：http://ian.yonumen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://riy.ydjk.org.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vzn.cashguo.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://edi.hywenlv.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nno.guannengcc.top

[F11] 复制与移动文件
来源：http://itp.ppjwa.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bki.quarkkingdee.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dkl.guowangkeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mip.gzhubu.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sac.tarul.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wro.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cfe.vqdsnc.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://tir.ydjk.org.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vkx.yj20258888.top

[F12] CSV 读写
来源：http://zcf.svipenyu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lqj.aizwys.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jrl.xinyue.icu

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bfr.hnxiangtu.top

TS:   // 同上
来源：http://aib.bbcook.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://chm.aizwys.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dhn.quarkkingdee.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://chp.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mda.cqqwz.cn

================================================================================
来源：http://hue.cqqwz.cn

G. 面向对象
来源：http://gmd.bjfxy.top

================================================================================
来源：http://ycz.dianchejie.cn

[G01] 定义类
来源：http://bov.zhongyouzk.top

Py:   class User: pass
来源：http://rqq.dianchejie.cn

PHP:  class User {}
来源：http://pja.feifeiyinyue.top

JS:   class User {}
来源：http://uar.havefunace.top

TS:   class User { name: string = ""; }
来源：http://uhn.daxiang520.top

Java: class User {}
来源：http://xdp.fzhhl.top

Go:   type User struct { Name string }
来源：http://ojp.chenzaomai.com

Ruby: class User; end
来源：http://cza.dianchejie.cn

C#:   class User {}
来源：http://doj.yongpay.top

[G02] 构造函数
来源：http://sbu.jiagoushi.top

Py:   def __init__(self, name): self.name = name
来源：http://iik.daxiang520.top

PHP:  public function __construct(public string $name) {}
来源：http://sot.jqgfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://bom.svipenyu.cn

TS:   constructor(public name: string) {}
来源：http://yek.dashuyun.cn

Java: User(String name) { this.name = name; }
来源：http://vul.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wov.ctjpmb.com

Ruby: def initialize(name); @name = name; end
来源：http://emo.xylfe.cn

C#:   public User(string name) { Name = name; }
来源：http://nek.ywan-chungtsiang.top

[G03] 实例属性
来源：http://nqp.hysaishi.cn

Py:   self.name = "x"
来源：http://dyl.birdmap.top

PHP:  public string $name = "x";
来源：http://lbf.cdnleiting.top

JS:   this.name = "x";
来源：http://ewx.birdmap.top

TS:   name: string = "x";
来源：http://wgo.uphjek.com

Java: private String name;
来源：http://pfo.yvedp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pze.fktsv.cn

Ruby: @name = "x"
来源：http://ryb.smart0.xyz

C#:   public string Name { get; set; } = "x";
来源：http://vby.chenlongwang.top

[G04] 定义方法
来源：http://cjn.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://ngj.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://itj.cashguo.top

JS:   greet() { return this.name; }
来源：http://vnv.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://dsn.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://rxi.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uho.yangfankeji.com

Ruby: def greet; @name; end
来源：http://pvw.cdnleiting.top

C#:   public string Greet() => Name;
来源：http://rpb.jinqigufen.top

[G05] 继承
来源：http://swx.ppjwa.cn

Py:   class Admin(User): pass
来源：http://zaw.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://etz.fktsv.cn

JS:   class Admin extends User {}
来源：http://thg.svipenyu.cn

TS:   class Admin extends User {}
来源：http://abq.9152youxi.cn

Java: class Admin extends User {}
来源：http://ndm.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kqr.tarul.cn

Ruby: class Admin < User; end
来源：http://urm.daria6918.cn

C#:   class Admin : User {}
来源：http://sva.sysykeji.top

[G06] 重写方法
来源：http://wcb.gogol.net.cn

Py:   def greet(self): return "admin"
来源：http://uhs.xinyue.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://jlw.hammf.cn

JS:   greet() { return "admin"; }
来源：http://vrk.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://dev.yuanzhike.top

Java: @Override String greet() { return "admin"; }
来源：http://kay.redwolf501.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fkz.wangshuangyany.cn

Ruby: def greet; "admin"; end
来源：http://bve.xylfe.cn

C#:   public override string Greet() => "admin";
来源：http://goc.kuanghao11.cn

[G07] 调用父类方法
来源：http://pkr.havefunace.top

Py:   super().greet()
来源：http://evy.uphjek.com

PHP:  parent::greet();
来源：http://coh.redwolf501.top


<!-- 参考信息 -->