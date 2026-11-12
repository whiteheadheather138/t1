代发 wailian999

Ruby: s.split(",");  s.split
来源：http://wvs.aibaodan.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ljm.ywan-chungtsiang.top

[E08] 数组按分隔符合并
来源：http://kzt.yvedp.cn

Py:   ",".join(items)
来源：http://ymf.xuetiantiany.cn

PHP:  implode(",", $items);
来源：http://suu.bjfxy.top

JS:   items.join(",")
来源：http://qxw.ywan-chungtsiang.top

TS:   items.join(",")
来源：http://rxt.xinyue.icu

Java: String.join(",", items)
来源：http://kni.yueranfly.top

Go:   strings.Join(items, ",")
来源：http://bsf.cdnleiting.top

Ruby: items.join(",")
来源：http://abo.hysaishi.cn

C#:   string.Join(",", items)
来源：http://asj.daria6918.cn

[E09] 去除所有空白字符
来源：http://phq.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uhn.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://tel.0kj1m.cn

JS:   s.replace(/\s+/g, "")
来源：http://ioy.hysaishi.cn

TS:   s.replace(/\s+/g, "")
来源：http://mqy.chenjidiqi.icu

Java: s.replaceAll("\\s+", "")
来源：http://qbh.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fcg.chenzaomai.com

Ruby: s.gsub(/\s+/, "")
来源：http://owl.nwbrower.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cxo.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://qmo.zdbjq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bzj.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://whg.yonumen.top

JS:   "7".padStart(3, "0")
来源：http://nny.ydjk.org.cn

TS:   "7".padStart(3, "0")
来源：http://fli.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://xor.hnxiangtu.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pvb.zdbjq.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sdk.jinqigfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cgc.vehdjk.com

[E11] 反转字符串
来源：http://gqd.redwolf501.top

Py:   s[::-1]
来源：http://huv.jlsjyb.cn

PHP:  strrev($s);
来源：http://uiv.yj20258888.top

JS:   [...s].reverse().join("")
来源：http://sji.jinyuanbaomall.cn

TS:   [...s].reverse().join("")
来源：http://keo.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://det.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://cye.yongpay.top

Ruby: s.reverse
来源：http://uix.fehbvm.com

C#:   new string(s.Reverse().ToArray())
来源：http://dan.quarkkingdee.top

[E12] 统计某字符出现次数
来源：http://flz.daxiang520.top

Py:   s.count("a")
来源：http://gud.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://nak.hongshengwenyu.top

JS:   s.split("a").length - 1
来源：http://gcp.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://eyv.fengsongda.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rea.chenlongwang.top

Go:   strings.Count(s, "a")
来源：http://kum.yfazqb.com

Ruby: s.count("a")
来源：http://wxe.fanxiaobao.xyz

C#:   s.Count(c => c == 'a')
来源：http://ozm.sxryk.cn

[E13] 逐字符遍历
来源：http://dwb.wangshuangyany.cn

Py:   for ch in s: print(ch)
来源：http://biz.cdnleiting.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tlj.316326.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://tsw.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nrl.nanxinkj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://axj.andypj.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kmt.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ipf.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cjz.cdnleiting.top

[E14] URL 编码与 Base64
来源：http://eof.yuanzhike.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lpy.zhengqikj.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pwu.pengpengdd.cyou

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vgr.wangshuangyany.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qlt.yongpay.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ttp.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rcd.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vhv.zhaomingkeji.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gan.cheryme.top

[E15] HTML 转义 / 反转义
来源：http://wrr.shanyushiyangkeji.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mqg.xziqi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dzj.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jug.tian-w.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pps.jiagoushi.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vvm.sweek.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mqu.yanxiufei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://myt.vehdjk.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zcs.birdmap.top

[E16] 数字千分位
来源：http://gpd.uphjek.com

Py:   f"{1234567:,}"
来源：http://rci.gzhubu.top

PHP:  number_format(1234567);
来源：http://sur.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qge.jyoumei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lfu.guowangkeji.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iiz.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mgv.tian-w.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zed.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://dan.zdqjudy.top

[E17] 首字母大写
来源：http://nfi.sweek.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ens.sxryk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qdx.shanyushiyangtech.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ofc.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bwu.yangfankeji.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vbc.ehwqpu.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qwn.ctjpmb.com

Ruby: s.capitalize
来源：http://eoz.xingfuxueyuan.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tvz.cashguo.top

[E18] 模板占位符替换
来源：http://yvm.yj20258888.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ohi.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hst.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mdw.dianchejie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xgf.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fxs.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yce.yfazqb.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://peq.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://scp.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://ikm.ctjpmb.com

Py:   s.splitlines()
来源：http://csv.52xcode.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qrf.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://jkn.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://tqk.jianghu66.top

Java: s.lines().toList()
来源：http://sbg.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://lud.hnxiangtu.top

Ruby: s.lines
来源：http://myr.sysykeji.top

C#:   s.Split('\n')
来源：http://kbv.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://omx.tanke756.top

Py:   if not s:
来源：http://ufh.dianchejie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jrl.hysaishi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jmg.ybcxt.top

TS:   if (s === "") {}
来源：http://qef.hfpthk.cn

Java: if (s.isEmpty()) {}
来源：http://wfc.daria6918.cn

Go:   if s == "" {}
来源：http://qdw.uphjek.com

Ruby: if s.empty?
来源：http://pdo.meibo888.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bde.fehbvm.com

[E21] 超长截断加省略号
来源：http://vpv.hysaishi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://agz.hfpthk.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mxz.nwbrower.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vlu.hammf.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://czi.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://frs.ctjpmb.com

Go:   // 按 rune 判断长度后截断
来源：http://dcy.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cwo.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fkf.bjfxy.top

[E22] 字节长度与字符长度
来源：http://nco.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ikb.fzhhl.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vqb.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://daq.yfazqb.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bkt.hfpthk.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://otu.pengpengdd.cyou

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hea.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://pax.pengpengdd.cyou

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://clx.0kj1m.cn

================================================================================
来源：http://xmd.jinghuilouyu.cn

F. 文件与目录
来源：http://trf.yvedp.cn

================================================================================
来源：http://hgv.xuetiantiany.cn

[F01] 读取整个文件
来源：http://xul.fzhhl.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tef.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://jds.chenlongwang.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dlv.yangfankeji.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mhx.shangyingyoupin.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dmt.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sqh.zhixingplan.top

Ruby: File.read("a.txt")
来源：http://alk.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://igd.hfpthk.cn

[F02] 逐行读取文件
来源：http://arw.yfazqb.com

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qky.daria6918.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bbz.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://glu.hongshengwenyu.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ppd.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yrp.yj20258888.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://odl.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xlz.zhongyouzk.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://leo.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://edl.guannengcc.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bws.yj202588.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://mix.zycfv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ttl.zhiwuduotai.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hro.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lbv.feifeiyinyue.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sqn.shanyushiyangkeji.top

Ruby: File.write("a.txt", "hi")
来源：http://uco.dashuyun.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sip.jinyuanbaomall.cn

[F04] 追加写入文件
来源：http://tvm.xingfuxueyuan.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://uej.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ydw.mhx1999.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pun.xylfe.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xog.pycfn.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://giq.sysykeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://olq.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ppp.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tpl.9152youxi.cn

[F05] 判断文件或目录是否存在
来源：http://yxl.cheryme.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fxh.jlsjyb.cn

PHP:  file_exists("a.txt");
来源：http://gcf.wangshuangyany.cn

JS:   fs.existsSync("a.txt")
来源：http://jsp.hnxiangtu.top

TS:   fs.existsSync("a.txt")
来源：http://wns.chenlongwang.top

Java: Files.exists(Path.of("a.txt"))
来源：http://afi.pycfn.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ruy.feifeiyinyue.top

Ruby: File.exist?("a.txt")
来源：http://elc.tarul.cn

C#:   File.Exists("a.txt")
来源：http://aws.zhiwuduotai.top

[F06] 删除文件
来源：http://hnz.yuxming.cn

Py:   os.remove("a.txt")
来源：http://utb.andypj.xyz

PHP:  unlink("a.txt");
来源：http://zqb.bbcook.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lmr.yvedp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gnn.shanyushiyangkeji.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aet.vehdjk.com

Go:   os.Remove("a.txt")
来源：http://mum.xinyue.icu

Ruby: File.delete("a.txt")
来源：http://srm.yvedp.cn

C#:   File.Delete("a.txt");
来源：http://jyi.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://hdd.guannengcc.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mvs.dashuyun.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kfo.yangfankeji.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eum.sufxvd.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://olq.nanxuanxn.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ydr.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gng.zhengqikj.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gjl.dashuyun.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uct.ybcxt.top

[F08] 遍历目录
来源：http://fkf.xinyue.icu

Py:   for name in os.listdir("dir"): print(name)
来源：http://twx.hnxiangtu.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pac.nwbrower.top

JS:   fs.readdirSync("dir")
来源：http://yie.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://usj.9152youxi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://agm.hammf.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tcc.hywenlv.cn

Ruby: Dir.children("dir")
来源：http://ewo.cheryme.top

C#:   Directory.GetFiles("dir")
来源：http://ked.fzhhl.top

[F09] 获取文件大小
来源：http://soq.haohaochexian.top

Py:   os.path.getsize("a.txt")
来源：http://thx.cdnleiting.top

PHP:  filesize("a.txt");
来源：http://jak.chenlongwang.top

JS:   fs.statSync("a.txt").size
来源：http://pgs.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://dgm.0kj1m.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qft.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lcf.jyoumei.cn

Ruby: File.size("a.txt")
来源：http://vxu.pengpengdd.cyou

C#:   new FileInfo("a.txt").Length
来源：http://daj.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://itn.kuanghao11.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iyk.sjlbkw.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://myl.jlsjyb.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wlb.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://ahy.jyoumei.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lrv.9152youxi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aqd.nanxinkj.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tkb.epnwcf.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://eqa.jinqigufen.top

[F11] 复制与移动文件
来源：http://clh.ywan-chungtsiang.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://syc.shanyushiyangtech.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hbk.meibo888.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://alt.hysaishi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rgh.zhaomingkeji.xyz

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://edv.zhixingplan.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tgj.xuanzx.com

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zlu.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://azg.ydjk.org.cn

[F12] CSV 读写
来源：http://pts.mhx1999.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bvk.shuidangran.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ddb.gzhubu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ihq.cheryme.top

TS:   // 同上
来源：http://ivu.xylfe.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://iqt.yonumen.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wfr.yangfankeji.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mwn.uphjek.com

C#:   // 无内置：用 CsvHelper 库
来源：http://oad.gogol.net.cn

================================================================================
来源：http://kct.nanxinkj.top

G. 面向对象
来源：http://ggf.svipenyu.cn

================================================================================
来源：http://qht.guannengcc.top

[G01] 定义类
来源：http://gyo.hnqzz.top

Py:   class User: pass
来源：http://lyz.xinyue.icu

PHP:  class User {}
来源：http://lch.yj20258.top

JS:   class User {}
来源：http://mss.yongpay.top

TS:   class User { name: string = ""; }
来源：http://rae.zhengqikj.top

Java: class User {}
来源：http://xmf.jyoumei.cn

Go:   type User struct { Name string }
来源：http://rdo.nanxinkj.top

Ruby: class User; end
来源：http://zzo.yvedp.cn

C#:   class User {}
来源：http://keu.hysaishi.cn

[G02] 构造函数
来源：http://tuz.gaohongyu789.top

Py:   def __init__(self, name): self.name = name
来源：http://qsd.zhongyouzk.top

PHP:  public function __construct(public string $name) {}
来源：http://znc.jinghuilouyu.cn

JS:   constructor(name) { this.name = name; }
来源：http://uhu.wangdashe.top

TS:   constructor(public name: string) {}
来源：http://pdq.hysaishi.cn

Java: User(String name) { this.name = name; }
来源：http://eae.gogol.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bym.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://aqp.feifeiyinyue.top

C#:   public User(string name) { Name = name; }
来源：http://klo.ydjk.org.cn

[G03] 实例属性
来源：http://lgi.hysaishi.cn

Py:   self.name = "x"
来源：http://yym.nanxinkj.top

PHP:  public string $name = "x";
来源：http://kib.dianchejie.cn

JS:   this.name = "x";
来源：http://bvj.guannengcc.top

TS:   name: string = "x";
来源：http://kao.jiagoushi.top

Java: private String name;
来源：http://xrz.hongshengwenyu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bgm.aibaodan.cn

Ruby: @name = "x"
来源：http://enx.hnxiangtu.top

C#:   public string Name { get; set; } = "x";
来源：http://tat.shangyingyoupin.top

[G04] 定义方法
来源：http://ref.ehwqpu.com

Py:   def greet(self): return self.name
来源：http://fnb.yangfankeji.com

PHP:  public function greet(): string { return $this->name; }
来源：http://ocg.shanyushiyangtech.top

JS:   greet() { return this.name; }
来源：http://ein.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://eza.fengsongda.top

Java: String greet() { return name; }
来源：http://brh.zhaomingkeji.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://jsa.aizwys.cn

Ruby: def greet; @name; end
来源：http://cwy.cucudq.cn

C#:   public string Greet() => Name;
来源：http://gcc.xinyue.icu

[G05] 继承
来源：http://agx.hammf.cn

Py:   class Admin(User): pass
来源：http://hcv.ybcxt.top

PHP:  class Admin extends User {}
来源：http://uha.yfazqb.com

JS:   class Admin extends User {}
来源：http://kif.sufxvd.cn

TS:   class Admin extends User {}
来源：http://gcq.nwbrower.top

Java: class Admin extends User {}
来源：http://ggr.yongpay.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qpr.shanyushiyangtech.top

Ruby: class Admin < User; end
来源：http://uga.yj20258.top

C#:   class Admin : User {}
来源：http://wvj.ehwqpu.com

[G06] 重写方法
来源：http://rgg.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://ssl.zdqjudy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hmy.haohaochexian.top

JS:   greet() { return "admin"; }
来源：http://tpn.zhixingplan.top


<!-- 参考信息 -->