代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hsi.feifeiyinyue.top

Ruby: items.join(",")
来源：http://ksy.fktsv.cn

C#:   string.Join(",", items)
来源：http://cis.hywenlv.cn

[E09] 去除所有空白字符
来源：http://hok.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xmu.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fud.ybcxt.top

JS:   s.replace(/\s+/g, "")
来源：http://gjd.aibaodan.cn

TS:   s.replace(/\s+/g, "")
来源：http://ksq.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://lbt.tarul.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://zhl.sysykeji.top

Ruby: s.gsub(/\s+/, "")
来源：http://yen.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jaz.hfpthk.cn

[E10] 左侧补零 / 定长填充
来源：http://wmd.aibaodan.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://srw.zhijiandao.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://udk.hammf.cn

JS:   "7".padStart(3, "0")
来源：http://rwz.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://cjv.pengpengdd.cyou

Java: String.format("%03d", 7)
来源：http://gyy.sjlbkw.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hcm.pengpengdd.cyou

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fnn.bjfxy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xis.jqgfzy.top

[E11] 反转字符串
来源：http://nti.yfazqb.com

Py:   s[::-1]
来源：http://xjn.316326.xyz

PHP:  strrev($s);
来源：http://htf.xuetiantiany.cn

JS:   [...s].reverse().join("")
来源：http://izj.kuanghao11.cn

TS:   [...s].reverse().join("")
来源：http://qsv.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mvn.hywenlv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://rfa.xylfe.cn

Ruby: s.reverse
来源：http://uhy.xylfe.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bmn.bbcook.cn

[E12] 统计某字符出现次数
来源：http://ejx.0kj1m.cn

Py:   s.count("a")
来源：http://csj.vqdsnc.cn

PHP:  substr_count($s, "a");
来源：http://uap.yuxming.cn

JS:   s.split("a").length - 1
来源：http://qdh.yuxming.cn

TS:   s.split("a").length - 1
来源：http://ovu.ybcxt.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://etf.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://cze.daxiang520.top

Ruby: s.count("a")
来源：http://roy.hnxiangtu.top

C#:   s.Count(c => c == 'a')
来源：http://jsj.yongpay.top

[E13] 逐字符遍历
来源：http://fsp.yj202588.top

Py:   for ch in s: print(ch)
来源：http://kpe.chenlongwang.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kxv.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://exu.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://aat.bbcook.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vbj.daxiang520.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kos.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://yvx.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://klt.dashuyun.cn

[E14] URL 编码与 Base64
来源：http://bvw.chenzaomai.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uxj.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vgw.wangdashe.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ujo.ydzc1.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fym.yueranfly.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pfc.jinqigufen.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ych.shangyingyoupin.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qtk.sysykeji.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://apu.yj20258.top

[E15] HTML 转义 / 反转义
来源：http://cqo.smart0.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://oiu.vehdjk.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://snq.nanxuanxn.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jnp.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gbc.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yrb.cashguo.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yxd.jinyuanbaomall.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dty.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yqx.hfpthk.cn

[E16] 数字千分位
来源：http://xod.mhx1999.top

Py:   f"{1234567:,}"
来源：http://dfm.fengsongda.top

PHP:  number_format(1234567);
来源：http://luw.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://vvw.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gze.xinyue.icu

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://aae.zdqjudy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cbb.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://una.yj20258888.top

C#:   1234567.ToString("N0")
来源：http://gsq.aizwys.cn

[E17] 首字母大写
来源：http://bdk.52xcode.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://frp.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fnq.zdqjudy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hry.nwbrower.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dmr.sufxvd.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nig.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://yqs.0kj1m.cn

Ruby: s.capitalize
来源：http://aay.epnwcf.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lue.gaohongyu789.top

[E18] 模板占位符替换
来源：http://lmx.yj202588.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cvz.316326.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zdg.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ott.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://qqn.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yhn.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kvi.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://etz.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gei.yangfankeji.com

[E19] 多行文本按行拆分
来源：http://lip.guannengcc.top

Py:   s.splitlines()
来源：http://ncz.kuanghao11.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lwv.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://zlr.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://tfy.yj20258.top

Java: s.lines().toList()
来源：http://hjq.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://aas.haohaochexian.top

Ruby: s.lines
来源：http://ysd.zhoulong.xyz

C#:   s.Split('\n')
来源：http://ztb.sweek.top

[E20] 判断字符串是否为空
来源：http://gpu.haohaochexian.top

Py:   if not s:
来源：http://yrb.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://saz.tianlin.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bcw.9152youxi.cn

TS:   if (s === "") {}
来源：http://axf.xuetiantiany.cn

Java: if (s.isEmpty()) {}
来源：http://tch.aibaodan.cn

Go:   if s == "" {}
来源：http://sel.zhongyouzk.top

Ruby: if s.empty?
来源：http://wjm.gogol.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tvu.gogol.net.cn

[E21] 超长截断加省略号
来源：http://tsv.hnqzz.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://unx.zhixingplan.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qxx.bbcook.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://isp.cheryme.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vtc.yj20258888.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sri.cashguo.top

Go:   // 按 rune 判断长度后截断
来源：http://wyw.sweek.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xfv.cashguo.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pcp.wangdashe.top

[E22] 字节长度与字符长度
来源：http://xfh.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lsv.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sff.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://btv.ctjpmb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ksl.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dhx.jlsjyb.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eal.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://kmu.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lsg.hammf.cn

================================================================================
来源：http://uxs.hnxiangtu.top

F. 文件与目录
来源：http://mww.yuanzhike.top

================================================================================
来源：http://ums.haohaochexian.top

[F01] 读取整个文件
来源：http://zis.zhengqikj.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wrt.hnxiangtu.top

PHP:  file_get_contents("a.txt");
来源：http://faa.zhixingplan.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://szo.jqgfzy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oqb.yueranfly.top

Java: Files.readString(Path.of("a.txt"))
来源：http://wlz.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://onj.nwbrower.top

Ruby: File.read("a.txt")
来源：http://wis.nwbrower.top

C#:   File.ReadAllText("a.txt");
来源：http://hru.yongpay.top

[F02] 逐行读取文件
来源：http://dlj.kuanghao11.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://suc.zhengqikj.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ylq.feifeiyinyue.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mjo.xingfuxueyuan.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sdb.fengsongda.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hel.0kj1m.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gjr.dashuyun.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lcy.dashuyun.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://phz.fanxiaobao.xyz

[F03] 写入文件（覆盖）
来源：http://vmf.shzxlz.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qjj.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gqn.gaohongyu789.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bsz.pycfn.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hop.aibaodan.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mip.havefunace.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vfr.tanke756.top

Ruby: File.write("a.txt", "hi")
来源：http://hrm.wangdashe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jcy.tarul.cn

[F04] 追加写入文件
来源：http://eum.yj202588.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uun.fengsongda.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vku.ydzc1.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jla.hnqzz.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nmz.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gnm.zhaomingkeji.xyz

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fwo.chenzaomai.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lws.svipenyu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zyf.andypj.xyz

[F05] 判断文件或目录是否存在
来源：http://dpq.guowangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wvf.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://aas.yonumen.top

JS:   fs.existsSync("a.txt")
来源：http://jbf.guowangkeji.top

TS:   fs.existsSync("a.txt")
来源：http://fmw.hongshengwenyu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bgn.hongshengwenyu.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://njf.shuidangran.top

Ruby: File.exist?("a.txt")
来源：http://wnc.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://fva.c1oappe.top

[F06] 删除文件
来源：http://voy.cheryme.top

Py:   os.remove("a.txt")
来源：http://owy.zhixingplan.top

PHP:  unlink("a.txt");
来源：http://pjc.daria6918.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ovm.shzxlz.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rxt.yj202588.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fnd.c1oappe.top

Go:   os.Remove("a.txt")
来源：http://oyg.uphjek.com

Ruby: File.delete("a.txt")
来源：http://boa.daria6918.cn

C#:   File.Delete("a.txt");
来源：http://mxo.hongshengwenyu.top

[F07] 创建目录（含多级）
来源：http://gfi.guowangkeji.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lte.nanxinkj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://swp.316326.xyz

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sru.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ugs.cucudq.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gye.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jdt.zhongyouzk.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tgr.ehwqpu.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ics.jinghuilouyu.cn

[F08] 遍历目录
来源：http://ons.xylfe.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dxn.wangdashe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aga.fengsongda.top

JS:   fs.readdirSync("dir")
来源：http://ahi.jqgfzy.top

TS:   fs.readdirSync("dir")
来源：http://djd.redwolf501.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://efy.hongshengwenyu.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nyl.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://lba.tian-w.cn

C#:   Directory.GetFiles("dir")
来源：http://afx.sysykeji.top

[F09] 获取文件大小
来源：http://htt.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://wtl.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://mdq.gogol.net.cn

JS:   fs.statSync("a.txt").size
来源：http://keu.52xcode.cn

TS:   fs.statSync("a.txt").size
来源：http://mwr.aibaodan.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rsh.jinghuilouyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pjr.cashguo.top

Ruby: File.size("a.txt")
来源：http://ndx.tanke756.top

C#:   new FileInfo("a.txt").Length
来源：http://aaj.wangdashe.top

[F10] 取文件扩展名 / 文件名
来源：http://bch.xylfe.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iue.gaohongyu789.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yyg.wangdashe.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://edv.ywan-chungtsiang.top

TS:   path.extname("a.txt")
来源：http://klc.jinghuilouyu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ckp.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://woz.tianlin.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://puv.fehbvm.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kkd.ydjk.org.cn

[F11] 复制与移动文件
来源：http://lae.sysykeji.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mbe.yj20258888.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blw.kuanghao11.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tgq.ywan-chungtsiang.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://juz.ivvv.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wip.bbcook.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kwn.jinqigufen.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://goc.tianlin.xyz

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nwt.bjfxy.top

[F12] CSV 读写
来源：http://sad.xylfe.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lgx.shanyushiyangtech.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xao.guannengcc.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nfv.meibo888.top

TS:   // 同上
来源：http://bgn.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cfq.jiagoushi.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jrg.fzhhl.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lgu.feifeiyinyue.top

C#:   // 无内置：用 CsvHelper 库
来源：http://iwr.zhixingplan.top

================================================================================
来源：http://fwa.hfpthk.cn

G. 面向对象
来源：http://wpr.xuetiantiany.cn

================================================================================
来源：http://hzp.guowangkeji.top

[G01] 定义类
来源：http://wxj.zhengqikj.top

Py:   class User: pass
来源：http://rsj.guannengcc.top

PHP:  class User {}
来源：http://hld.nanxinkj.top

JS:   class User {}
来源：http://yud.xinyue.icu

TS:   class User { name: string = ""; }
来源：http://baj.zhijiandao.cn

Java: class User {}
来源：http://jdk.yuanzhike.top

Go:   type User struct { Name string }
来源：http://zxo.yj20258888.top

Ruby: class User; end
来源：http://dxq.havefunace.top

C#:   class User {}
来源：http://ojg.vehdjk.com

[G02] 构造函数
来源：http://tef.shanyushiyangkeji.top

Py:   def __init__(self, name): self.name = name
来源：http://kqq.andypj.xyz

PHP:  public function __construct(public string $name) {}
来源：http://xxy.fanxiaobao.xyz

JS:   constructor(name) { this.name = name; }
来源：http://mcg.havefunace.top

TS:   constructor(public name: string) {}
来源：http://nsu.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://fye.yvedp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mcf.jinghuilouyu.cn

Ruby: def initialize(name); @name = name; end
来源：http://hep.haohaochexian.top

C#:   public User(string name) { Name = name; }
来源：http://hjt.daxiang520.top

[G03] 实例属性
来源：http://peh.zhijiandao.cn

Py:   self.name = "x"
来源：http://uhj.shanyushiyangkeji.top

PHP:  public string $name = "x";
来源：http://buo.dashuyun.cn

JS:   this.name = "x";
来源：http://ijp.nanxuanxn.top

TS:   name: string = "x";
来源：http://ocs.birdmap.top

Java: private String name;
来源：http://wwh.yj202588.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jvi.jqgufenzy.top

Ruby: @name = "x"
来源：http://rtg.shzxlz.cn

C#:   public string Name { get; set; } = "x";
来源：http://kun.nwbrower.top

[G04] 定义方法
来源：http://jpw.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://kvo.zhijiandao.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jdj.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://aic.chenzaomai.com

TS:   greet(): string { return this.name; }
来源：http://dgb.daxiang520.top

Java: String greet() { return name; }
来源：http://zes.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jzx.fktsv.cn

Ruby: def greet; @name; end
来源：http://mxs.zhijiandao.cn

C#:   public string Greet() => Name;
来源：http://rkn.yuanzhike.top

[G05] 继承
来源：http://xpj.hcnkem.com

Py:   class Admin(User): pass
来源：http://pgd.nanxinkj.top

PHP:  class Admin extends User {}
来源：http://sai.ctjpmb.com

JS:   class Admin extends User {}
来源：http://fbl.iojbl.cn

TS:   class Admin extends User {}
来源：http://dcs.gaohongyu789.top

Java: class Admin extends User {}
来源：http://aou.zhijiandao.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kmv.yangfankeji.com

Ruby: class Admin < User; end
来源：http://koo.ydjk.org.cn

C#:   class Admin : User {}
来源：http://jpj.sweek.top

[G06] 重写方法
来源：http://lzi.feifeiyinyue.top

Py:   def greet(self): return "admin"
来源：http://uqy.yonumen.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gae.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://qia.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://jup.shanyushiyangtech.top

Java: @Override String greet() { return "admin"; }
来源：http://tme.meibo888.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kdh.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://rfk.nanxinkj.top

C#:   public override string Greet() => "admin";
来源：http://nvl.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://lbn.zhengqikj.top

Py:   super().greet()
来源：http://okr.cheryme.top

PHP:  parent::greet();
来源：http://qds.andypj.xyz


<!-- 参考信息 -->