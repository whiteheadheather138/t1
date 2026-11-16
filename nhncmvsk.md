代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fra.gotoacloud.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jzj.yfazqb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xuh.chenzaomai.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zfz.ctjpmb.com

[E06] 替换子串
来源：http://zbz.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dbb.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://aer.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nvv.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://cdb.tarul.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://okm.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kgg.jinyuanbaomall.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://uim.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://gjj.fengsongda.top

[E07] 按分隔符拆分
来源：http://ine.feifeiyinyue.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mzr.zhengqikj.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uyw.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ykc.tarul.cn

TS:   s.split(",")
来源：http://bwl.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://xaw.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qqw.hywenlv.cn

Ruby: s.split(",");  s.split
来源：http://lgw.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cai.gzhubu.top

[E08] 数组按分隔符合并
来源：http://gzq.havefunace.top

Py:   ",".join(items)
来源：http://qmv.ivvv.top

PHP:  implode(",", $items);
来源：http://zwp.aizwys.cn

JS:   items.join(",")
来源：http://jlj.cqqwz.cn

TS:   items.join(",")
来源：http://grw.aizwys.cn

Java: String.join(",", items)
来源：http://wei.hongshengwenyu.top

Go:   strings.Join(items, ",")
来源：http://rqo.jqgufenzy.top

Ruby: items.join(",")
来源：http://mrf.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://mtl.redwolf501.top

[E09] 去除所有空白字符
来源：http://jkf.hesvh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sdi.zhaomingkeji.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rgj.yangfankeji.com

JS:   s.replace(/\s+/g, "")
来源：http://eit.hongshengwenyu.top

TS:   s.replace(/\s+/g, "")
来源：http://kmm.tianlin.xyz

Java: s.replaceAll("\\s+", "")
来源：http://awr.zycfv.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hfu.xylfe.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pak.dashuyun.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://slg.tianlin.xyz

[E10] 左侧补零 / 定长填充
来源：http://auc.cucudq.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ubo.smart0.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zbd.fzhhl.top

JS:   "7".padStart(3, "0")
来源：http://gse.jyoumei.cn

TS:   "7".padStart(3, "0")
来源：http://aqq.pycfn.com

Java: String.format("%03d", 7)
来源：http://jca.yonumen.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://djl.hesvh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cbs.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xkd.fktsv.cn

[E11] 反转字符串
来源：http://uxt.kuanghao11.cn

Py:   s[::-1]
来源：http://ldq.ehwqpu.com

PHP:  strrev($s);
来源：http://rcg.zhiwuduotai.top

JS:   [...s].reverse().join("")
来源：http://ikk.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://ezg.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uyz.kuanghao11.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tnk.andypj.xyz

Ruby: s.reverse
来源：http://ynn.daxiang520.top

C#:   new string(s.Reverse().ToArray())
来源：http://lbu.kuanghao11.cn

[E12] 统计某字符出现次数
来源：http://gln.yangfankeji.com

Py:   s.count("a")
来源：http://wto.gzhubu.top

PHP:  substr_count($s, "a");
来源：http://iiv.dianchejie.cn

JS:   s.split("a").length - 1
来源：http://yht.andypj.xyz

TS:   s.split("a").length - 1
来源：http://dle.ppjwa.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pem.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://tel.gzhubu.top

Ruby: s.count("a")
来源：http://tqu.yonumen.top

C#:   s.Count(c => c == 'a')
来源：http://cka.xziqi.cn

[E13] 逐字符遍历
来源：http://pig.zdqjudy.top

Py:   for ch in s: print(ch)
来源：http://pjj.zhengqikj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tdm.ppjwa.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://odr.feifeiyinyue.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wrz.kuanghao11.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vtr.shuidangran.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://azu.zycfv.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vuu.bbcook.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wef.xinyue.icu

[E14] URL 编码与 Base64
来源：http://vdj.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://izj.uphjek.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://xzq.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://knq.tarul.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pva.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ocl.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ppq.zhiwuduotai.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://dpj.aibaodan.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yfn.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://dnn.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://gmm.tanke756.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://txy.yj20258.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://urv.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://roa.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fve.0kj1m.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://efk.52xcode.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://eys.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lsj.yonumen.top

[E16] 数字千分位
来源：http://lrl.c1oappe.top

Py:   f"{1234567:,}"
来源：http://obj.jqgufenzy.top

PHP:  number_format(1234567);
来源：http://wdq.redwolf501.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ktv.hywenlv.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lzf.kuanghao11.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bbv.ppjwa.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gqt.tarul.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xer.yonumen.top

C#:   1234567.ToString("N0")
来源：http://iua.cashguo.top

[E17] 首字母大写
来源：http://fhs.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ich.nanxinkj.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ssb.shanyushiyangkeji.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fcs.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gdt.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kog.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rnx.hnxiangtu.top

Ruby: s.capitalize
来源：http://hnc.hnxiangtu.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dmd.yongpay.top

[E18] 模板占位符替换
来源：http://php.kuanghao11.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xgs.yuanzhike.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xay.c1oappe.top

JS:   tpl.replaceAll("{name}", name)
来源：http://elf.jqgufenzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kuf.zhixingplan.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lbf.andypj.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nkg.tarul.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://iye.zhaomingkeji.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://boi.zhongyouzk.top

[E19] 多行文本按行拆分
来源：http://djw.zhongyouzk.top

Py:   s.splitlines()
来源：http://mgi.hongshengwenyu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iyr.aizwys.cn

JS:   s.split(/\r?\n/)
来源：http://xzx.gogol.net.cn

TS:   s.split(/\r?\n/)
来源：http://nks.yonumen.top

Java: s.lines().toList()
来源：http://byd.gaohongyu789.top

Go:   strings.Split(s, "\n")
来源：http://yfi.meibo888.top

Ruby: s.lines
来源：http://slw.pycfn.com

C#:   s.Split('\n')
来源：http://jrh.chenjidiqi.icu

[E20] 判断字符串是否为空
来源：http://mos.birdmap.top

Py:   if not s:
来源：http://ypt.jqgfzy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://che.c1oappe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://spj.cdnleiting.top

TS:   if (s === "") {}
来源：http://xoh.pengpengdd.cyou

Java: if (s.isEmpty()) {}
来源：http://ttm.xylfe.cn

Go:   if s == "" {}
来源：http://okf.xinyue.icu

Ruby: if s.empty?
来源：http://myw.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pze.hfpthk.cn

[E21] 超长截断加省略号
来源：http://las.9152youxi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ajc.havefunace.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yvw.jinyuanbaomall.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vou.chenjidiqi.icu

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://inf.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://atg.xuetiantiany.cn

Go:   // 按 rune 判断长度后截断
来源：http://omk.birdmap.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qoe.zdbjq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ssm.sysykeji.top

[E22] 字节长度与字符长度
来源：http://mnd.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vtd.shzxlz.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vye.andypj.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bdm.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rub.shanyushiyangkeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hle.bjfxy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pje.jiagoushi.top

Ruby: s.bytesize;  s.length
来源：http://ijz.hammf.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pci.yj20258.top

================================================================================
来源：http://gzf.ctjpmb.com

F. 文件与目录
来源：http://xpf.ppjwa.cn

================================================================================
来源：http://gyq.chenzaomai.com

[F01] 读取整个文件
来源：http://wkx.hnxiangtu.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iyh.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://sjo.xingfuxueyuan.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xju.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tlq.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://zuz.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://osw.vehdjk.com

Ruby: File.read("a.txt")
来源：http://bol.shangyingyoupin.top

C#:   File.ReadAllText("a.txt");
来源：http://njg.gogol.net.cn

[F02] 逐行读取文件
来源：http://skm.hammf.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pzr.havefunace.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://doo.nanxuanxn.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dmc.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hcd.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://biz.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aiq.yuanzhike.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fbs.shanyushiyangkeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cmz.jyoumei.cn

[F03] 写入文件（覆盖）
来源：http://sek.hesvh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://txw.daxiang520.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://oww.hysaishi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://adx.kuanghao11.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zzo.nanxuanxn.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blm.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nic.nanxuanxn.top

Ruby: File.write("a.txt", "hi")
来源：http://omy.fktsv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cms.shanyushiyangtech.top

[F04] 追加写入文件
来源：http://foq.gogol.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xbe.mhx1999.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kvn.quarkkingdee.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zni.jinqigfzy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zxy.feifeiyinyue.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yjl.vqdsnc.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vip.vehdjk.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gvq.uphjek.com

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jjn.jyoumei.cn

[F05] 判断文件或目录是否存在
来源：http://vpq.birdmap.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nup.hongshengwenyu.top

PHP:  file_exists("a.txt");
来源：http://xee.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://gsm.gotoacloud.top

TS:   fs.existsSync("a.txt")
来源：http://hyo.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://jak.daria6918.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mkr.jinqigufen.top

Ruby: File.exist?("a.txt")
来源：http://ffh.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://kqy.xuanzx.com

[F06] 删除文件
来源：http://xhs.guowangkeji.top

Py:   os.remove("a.txt")
来源：http://jnl.ydjk.org.cn

PHP:  unlink("a.txt");
来源：http://xsq.shanyushiyangtech.top

JS:   fs.unlinkSync("a.txt")
来源：http://zrl.zhijiandao.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zqz.nanxinkj.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kct.fehbvm.com

Go:   os.Remove("a.txt")
来源：http://jfx.yonumen.top

Ruby: File.delete("a.txt")
来源：http://wry.9152youxi.cn

C#:   File.Delete("a.txt");
来源：http://elx.xingfuxueyuan.xyz

[F07] 创建目录（含多级）
来源：http://kqe.zhengqikj.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tgr.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cug.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fpn.aibaodan.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tnd.sysykeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rqs.uphjek.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vit.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wao.guowangkeji.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://aos.yj20258.top

[F08] 遍历目录
来源：http://krz.cdnleiting.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://fio.yongpay.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jav.epnwcf.com

JS:   fs.readdirSync("dir")
来源：http://fqs.nwbrower.top

TS:   fs.readdirSync("dir")
来源：http://cak.yonumen.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ooh.zhengqikj.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nnx.sxryk.cn

Ruby: Dir.children("dir")
来源：http://sfx.tanke756.top

C#:   Directory.GetFiles("dir")
来源：http://yyx.hcnkem.com

[F09] 获取文件大小
来源：http://nly.fktsv.cn

Py:   os.path.getsize("a.txt")
来源：http://mcg.chenjidiqi.icu

PHP:  filesize("a.txt");
来源：http://kkh.sufxvd.cn

JS:   fs.statSync("a.txt").size
来源：http://axl.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://qqr.fehbvm.com

Java: Files.size(Path.of("a.txt"))
来源：http://eoh.wangshuangyany.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bgb.yj20258888.top

Ruby: File.size("a.txt")
来源：http://cxz.wangshuangyany.cn

C#:   new FileInfo("a.txt").Length
来源：http://pcj.cheryme.top

[F10] 取文件扩展名 / 文件名
来源：http://avl.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fwd.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ugl.yj20258888.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ect.ctjpmb.com

TS:   path.extname("a.txt")
来源：http://gau.jinqigufen.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kro.dashuyun.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://tvk.ppjwa.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zhj.ybcxt.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xbz.cdnleiting.top

[F11] 复制与移动文件
来源：http://rjs.jqgufenzy.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ngk.zhijiandao.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rzb.xuetiantiany.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yvc.shangyingyoupin.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zce.ctjpmb.com

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fmp.haohaochexian.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uhf.kuanghao11.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zpj.fzhhl.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ijt.yj20258888.top

[F12] CSV 读写
来源：http://nph.cdnleiting.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://afg.fengsongda.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bso.sufxvd.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bdj.sysykeji.top

TS:   // 同上
来源：http://lae.gogol.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pmh.daria6918.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xgv.uphjek.com

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bij.shangyingyoupin.top

C#:   // 无内置：用 CsvHelper 库
来源：http://zfx.pycfn.com

================================================================================
来源：http://qon.0kj1m.cn

G. 面向对象
来源：http://myz.meibo888.top

================================================================================
来源：http://zai.cheryme.top

[G01] 定义类
来源：http://lwu.pengpengdd.cyou

Py:   class User: pass
来源：http://wox.fehbvm.com

PHP:  class User {}
来源：http://ont.dianchejie.cn

JS:   class User {}
来源：http://vxl.jinqigfzy.top

TS:   class User { name: string = ""; }
来源：http://hog.fengsongda.top

Java: class User {}
来源：http://olb.shangyingyoupin.top

Go:   type User struct { Name string }
来源：http://ycm.bjfxy.top

Ruby: class User; end
来源：http://jty.fzhhl.top

C#:   class User {}
来源：http://bhn.jinyuanbaomall.cn

[G02] 构造函数
来源：http://gta.sysykeji.top

Py:   def __init__(self, name): self.name = name
来源：http://trw.hammf.cn

PHP:  public function __construct(public string $name) {}
来源：http://hqp.kuanghao11.cn

JS:   constructor(name) { this.name = name; }
来源：http://grd.ybcxt.top

TS:   constructor(public name: string) {}
来源：http://nuz.xziqi.cn

Java: User(String name) { this.name = name; }
来源：http://ppd.havefunace.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pyx.tanke756.top

Ruby: def initialize(name); @name = name; end
来源：http://ibd.yj20258.top

C#:   public User(string name) { Name = name; }
来源：http://wlv.jyoumei.cn

[G03] 实例属性
来源：http://kas.birdmap.top

Py:   self.name = "x"
来源：http://yww.yonumen.top

PHP:  public string $name = "x";
来源：http://qml.zhixingplan.top

JS:   this.name = "x";
来源：http://pke.sweek.top

TS:   name: string = "x";
来源：http://trw.jinyuanbaomall.cn

Java: private String name;
来源：http://isa.hnxiangtu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pqb.zdqjudy.top

Ruby: @name = "x"
来源：http://lrp.svipenyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://uss.gaohongyu789.top

[G04] 定义方法
来源：http://tfb.hysaishi.cn

Py:   def greet(self): return self.name
来源：http://ioz.iojbl.cn


<!-- 参考信息 -->