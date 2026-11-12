代发 wailian999

Go:   strings.Join(items, ",")
来源：http://lrx.ehwqpu.com

Ruby: items.join(",")
来源：http://yff.shuidangran.top

C#:   string.Join(",", items)
来源：http://irp.zhongyouzk.top

[E09] 去除所有空白字符
来源：http://mkk.0kj1m.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pvz.cdnleiting.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vdl.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://zhe.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://lly.wangdashe.top

Java: s.replaceAll("\\s+", "")
来源：http://ovv.aizwys.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ybj.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://mcx.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ijn.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://jqe.smart0.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ymk.epnwcf.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://dws.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://xff.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://uht.xinyue.icu

Java: String.format("%03d", 7)
来源：http://fop.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://edd.hongshengwenyu.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hgw.chenzaomai.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sjq.kuanghao11.cn

[E11] 反转字符串
来源：http://pzg.tanke756.top

Py:   s[::-1]
来源：http://pko.ydzc1.top

PHP:  strrev($s);
来源：http://zli.zhengqikj.top

JS:   [...s].reverse().join("")
来源：http://smj.cheryme.top

TS:   [...s].reverse().join("")
来源：http://ade.fktsv.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aav.316326.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://pbg.chenzaomai.com

Ruby: s.reverse
来源：http://poh.tarul.cn

C#:   new string(s.Reverse().ToArray())
来源：http://eka.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://sno.zdbjq.cn

Py:   s.count("a")
来源：http://dak.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://mcc.pycfn.com

JS:   s.split("a").length - 1
来源：http://kpu.sweek.top

TS:   s.split("a").length - 1
来源：http://dzw.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kot.dashuyun.cn

Go:   strings.Count(s, "a")
来源：http://wzb.tarul.cn

Ruby: s.count("a")
来源：http://csp.jqgfzy.top

C#:   s.Count(c => c == 'a')
来源：http://hyr.guowangkeji.top

[E13] 逐字符遍历
来源：http://znv.zycfv.cn

Py:   for ch in s: print(ch)
来源：http://qpw.snrcjt.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mru.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uou.yfazqb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://oot.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ush.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tbt.pycfn.com

Ruby: s.each_char { |ch| puts ch }
来源：http://mrq.hnxiangtu.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ysc.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://zun.ydzc1.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zsc.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zuf.shzxlz.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ozo.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kwu.yanxiufei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ppf.cashguo.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bsh.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wkt.shanyushiyangkeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zoc.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://uxu.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xci.haohaochexian.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ywr.iojbl.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qeb.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://iym.chenzaomai.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cmy.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ymd.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xza.cashguo.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nbn.andypj.xyz

[E16] 数字千分位
来源：http://wcj.cucudq.cn

Py:   f"{1234567:,}"
来源：http://uhm.ybcxt.top

PHP:  number_format(1234567);
来源：http://qnx.zdqjudy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://bxv.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nkf.nwbrower.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://plo.52xcode.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ogk.yueranfly.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dgx.sjlbkw.cn

C#:   1234567.ToString("N0")
来源：http://emz.svipenyu.cn

[E17] 首字母大写
来源：http://faz.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cbz.cashguo.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://cjb.zhiwuduotai.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ali.ivvv.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jis.fktsv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ple.jqgfzy.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yqu.meibo888.top

Ruby: s.capitalize
来源：http://sdm.nanxuanxn.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vde.zhoulong.xyz

[E18] 模板占位符替换
来源：http://ohv.jinqigufen.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qsa.shuidangran.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cho.fzhhl.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xsd.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nkh.cashguo.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ftc.meibo888.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nhp.fktsv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jlm.epnwcf.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jrk.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://iip.ydzc1.top

Py:   s.splitlines()
来源：http://zfi.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kbg.yueranfly.top

JS:   s.split(/\r?\n/)
来源：http://zji.tianlin.xyz

TS:   s.split(/\r?\n/)
来源：http://aya.daria6918.cn

Java: s.lines().toList()
来源：http://bbr.jinqigufen.top

Go:   strings.Split(s, "\n")
来源：http://vrs.jyoumei.cn

Ruby: s.lines
来源：http://yvz.sweek.top

C#:   s.Split('\n')
来源：http://yjb.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://vjg.andypj.xyz

Py:   if not s:
来源：http://nvq.jinqigfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ndj.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bzq.jinghuilouyu.cn

TS:   if (s === "") {}
来源：http://own.jinqigfzy.top

Java: if (s.isEmpty()) {}
来源：http://pri.zhiwuduotai.top

Go:   if s == "" {}
来源：http://llz.yj20258888.top

Ruby: if s.empty?
来源：http://wsz.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wkv.fengsongda.top

[E21] 超长截断加省略号
来源：http://cfc.sufxvd.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dvz.jinghuilouyu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jns.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gnl.iojbl.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://urr.epnwcf.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zch.zhijiandao.cn

Go:   // 按 rune 判断长度后截断
来源：http://bpx.ehwqpu.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yxj.sjlbkw.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bzy.sweek.top

[E22] 字节长度与字符长度
来源：http://fkv.jqgufenzy.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mmr.yangfankeji.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qlg.cheryme.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oku.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ufe.quarkkingdee.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://erf.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yvr.dashuyun.cn

Ruby: s.bytesize;  s.length
来源：http://hyr.sweek.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://izg.zhengqikj.top

================================================================================
来源：http://kpd.snrcjt.cn

F. 文件与目录
来源：http://ztx.zhixingplan.top

================================================================================
来源：http://nyt.jyoumei.cn

[F01] 读取整个文件
来源：http://eyh.jiagoushi.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ljk.c1oappe.top

PHP:  file_get_contents("a.txt");
来源：http://ckp.yonumen.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ami.yj20258.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://kyg.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tct.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://six.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://beg.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://ipk.hammf.cn

[F02] 逐行读取文件
来源：http://ulm.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hau.chenzaomai.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sez.cdnleiting.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gxc.gotoacloud.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tzg.hnxiangtu.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bjb.chenzaomai.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bfe.kuanghao11.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zjv.yj20258888.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://did.sweek.top

[F03] 写入文件（覆盖）
来源：http://vle.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://owt.ctjpmb.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://erx.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ucp.snrcjt.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksk.haohaochexian.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rol.jinyuanbaomall.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dlp.aibaodan.cn

Ruby: File.write("a.txt", "hi")
来源：http://yhw.xuanzx.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://koz.nanxinkj.top

[F04] 追加写入文件
来源：http://bth.kuanghao11.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qdt.jlsjyb.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cei.dianchejie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dvu.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rpx.tian-w.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nkj.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ncu.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ygv.tarul.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://klv.fehbvm.com

[F05] 判断文件或目录是否存在
来源：http://fsw.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nej.aibaodan.cn

PHP:  file_exists("a.txt");
来源：http://vud.zdbjq.cn

JS:   fs.existsSync("a.txt")
来源：http://jes.cashguo.top

TS:   fs.existsSync("a.txt")
来源：http://mdn.zhengqikj.top

Java: Files.exists(Path.of("a.txt"))
来源：http://iou.jqgfzy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tty.ctjpmb.com

Ruby: File.exist?("a.txt")
来源：http://lot.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://ygp.chenjidiqi.icu

[F06] 删除文件
来源：http://sbp.shangyingyoupin.top

Py:   os.remove("a.txt")
来源：http://jnl.daxiang520.top

PHP:  unlink("a.txt");
来源：http://fkp.xuanzx.com

JS:   fs.unlinkSync("a.txt")
来源：http://shh.vehdjk.com

TS:   fs.unlinkSync("a.txt")
来源：http://bwq.iojbl.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://huw.316326.xyz

Go:   os.Remove("a.txt")
来源：http://qpg.ydzc1.top

Ruby: File.delete("a.txt")
来源：http://tec.bbcook.cn

C#:   File.Delete("a.txt");
来源：http://qcc.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://wwq.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sdv.fzhhl.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xxg.guannengcc.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ofa.pycfn.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://czu.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://diq.fzhhl.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oyx.yuxming.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vjn.smart0.xyz

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gnk.daxiang520.top

[F08] 遍历目录
来源：http://pmg.nanxinkj.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eyj.yonumen.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jfh.aizwys.cn

JS:   fs.readdirSync("dir")
来源：http://pny.gaohongyu789.top

TS:   fs.readdirSync("dir")
来源：http://rxx.jinqigufen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wea.daxiang520.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nrm.cdnleiting.top

Ruby: Dir.children("dir")
来源：http://aii.cdnleiting.top

C#:   Directory.GetFiles("dir")
来源：http://mta.jianghu66.top

[F09] 获取文件大小
来源：http://bze.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://gif.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://txc.hesvh.cn

JS:   fs.statSync("a.txt").size
来源：http://uii.shanyushiyangtech.top

TS:   fs.statSync("a.txt").size
来源：http://ltj.yonumen.top

Java: Files.size(Path.of("a.txt"))
来源：http://bxe.cheryme.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ykj.yuxming.cn

Ruby: File.size("a.txt")
来源：http://xaq.chenzaomai.com

C#:   new FileInfo("a.txt").Length
来源：http://drq.snrcjt.cn

[F10] 取文件扩展名 / 文件名
来源：http://xnu.jqgufenzy.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zep.chenlongwang.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jxg.sweek.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sns.daxiang520.top

TS:   path.extname("a.txt")
来源：http://act.redwolf501.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xvs.yj20258888.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wnm.jinqigfzy.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://phg.vqdsnc.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yfh.feifeiyinyue.top

[F11] 复制与移动文件
来源：http://lxo.dianchejie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://joj.andypj.xyz

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tfv.ybcxt.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://due.gotoacloud.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fap.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://etn.jqgfzy.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rzz.bbcook.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mje.gaohongyu789.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zjo.52xcode.cn

[F12] CSV 读写
来源：http://dbq.zhixingplan.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://brx.tianlin.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wrq.vqdsnc.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://htr.aizwys.cn

TS:   // 同上
来源：http://kjv.yuxming.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bjx.gotoacloud.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bsm.ybcxt.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://imq.xylfe.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nyv.aizwys.cn

================================================================================
来源：http://lng.sjlbkw.cn

G. 面向对象
来源：http://uhl.hcnkem.com

================================================================================
来源：http://rif.redwolf501.top

[G01] 定义类
来源：http://drv.wangdashe.top

Py:   class User: pass
来源：http://das.yonumen.top

PHP:  class User {}
来源：http://kic.snrcjt.cn

JS:   class User {}
来源：http://wos.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://osh.hammf.cn

Java: class User {}
来源：http://ovj.vqdsnc.cn

Go:   type User struct { Name string }
来源：http://dav.ywan-chungtsiang.top

Ruby: class User; end
来源：http://lry.daria6918.cn

C#:   class User {}
来源：http://qni.fanxiaobao.xyz

[G02] 构造函数
来源：http://qgg.yfazqb.com

Py:   def __init__(self, name): self.name = name
来源：http://vze.chenzaomai.com

PHP:  public function __construct(public string $name) {}
来源：http://bqz.guowangkeji.top

JS:   constructor(name) { this.name = name; }
来源：http://qqz.nanxuanxn.top

TS:   constructor(public name: string) {}
来源：http://vfb.cheryme.top

Java: User(String name) { this.name = name; }
来源：http://lgm.quarkkingdee.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://myk.xylfe.cn

Ruby: def initialize(name); @name = name; end
来源：http://vxr.gzhubu.top

C#:   public User(string name) { Name = name; }
来源：http://fwp.cucudq.cn

[G03] 实例属性
来源：http://yiv.fzhhl.top

Py:   self.name = "x"
来源：http://zow.yj20258.top

PHP:  public string $name = "x";
来源：http://suv.sysykeji.top

JS:   this.name = "x";
来源：http://qsd.tian-w.cn

TS:   name: string = "x";
来源：http://toc.svipenyu.cn

Java: private String name;
来源：http://fla.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qta.xylfe.cn

Ruby: @name = "x"
来源：http://egk.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://gzz.shzxlz.cn

[G04] 定义方法
来源：http://nvl.zhongyouzk.top

Py:   def greet(self): return self.name
来源：http://qut.sxryk.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://krh.vehdjk.com

JS:   greet() { return this.name; }
来源：http://jfj.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://jfv.mhx1999.top

Java: String greet() { return name; }
来源：http://ypz.nanxinkj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://dah.c1oappe.top

Ruby: def greet; @name; end
来源：http://arv.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://bgs.sweek.top

[G05] 继承
来源：http://rzc.aibaodan.cn

Py:   class Admin(User): pass
来源：http://pmr.meibo888.top

PHP:  class Admin extends User {}
来源：http://lyq.gzhubu.top

JS:   class Admin extends User {}
来源：http://znx.dianchejie.cn

TS:   class Admin extends User {}
来源：http://iub.chenjidiqi.icu

Java: class Admin extends User {}
来源：http://auw.jqgfzy.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nal.zhongyouzk.top

Ruby: class Admin < User; end
来源：http://erk.guannengcc.top

C#:   class Admin : User {}
来源：http://rbd.uphjek.com

[G06] 重写方法
来源：http://kmj.jqgufenzy.top

Py:   def greet(self): return "admin"
来源：http://rtb.xziqi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://spp.cqqwz.cn

JS:   greet() { return "admin"; }
来源：http://zil.mhx1999.top

TS:   greet(): string { return "admin"; }
来源：http://qpv.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://lva.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hll.shanyushiyangtech.top

Ruby: def greet; "admin"; end
来源：http://cmt.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://gqc.epnwcf.com

[G07] 调用父类方法
来源：http://hym.zhixingplan.top

Py:   super().greet()
来源：http://rys.hysaishi.cn

PHP:  parent::greet();
来源：http://awp.hysaishi.cn


<!-- 参考信息 -->