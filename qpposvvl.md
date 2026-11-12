代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ane.hnqzz.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rup.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aft.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iar.xinyue.icu

[E06] 替换子串
来源：http://eln.jiagoushi.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zol.iojbl.cn

PHP:  str_replace("a", "b", $s);
来源：http://nhl.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qow.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://rgv.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lax.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xvb.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pkl.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://rrm.ppjwa.cn

[E07] 按分隔符拆分
来源：http://muz.xylfe.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fcy.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bpp.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://guq.gaohongyu789.top

TS:   s.split(",")
来源：http://vss.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://fnv.zhoulong.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zhe.shanyushiyangkeji.top

Ruby: s.split(",");  s.split
来源：http://yab.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://clm.ctjpmb.com

[E08] 数组按分隔符合并
来源：http://jxb.sysykeji.top

Py:   ",".join(items)
来源：http://azq.bbcook.cn

PHP:  implode(",", $items);
来源：http://eln.jqgfzy.top

JS:   items.join(",")
来源：http://qlr.hysaishi.cn

TS:   items.join(",")
来源：http://lcn.uphjek.com

Java: String.join(",", items)
来源：http://bjo.svipenyu.cn

Go:   strings.Join(items, ",")
来源：http://zfk.fehbvm.com

Ruby: items.join(",")
来源：http://ldq.yonumen.top

C#:   string.Join(",", items)
来源：http://xbf.jqgfzy.top

[E09] 去除所有空白字符
来源：http://hic.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yuv.vqdsnc.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dnq.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://ugg.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://hmo.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://msn.yuxming.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ohw.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://lbg.zhijiandao.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wih.gotoacloud.top

[E10] 左侧补零 / 定长填充
来源：http://nqv.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kdf.guowangkeji.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fbp.sysykeji.top

JS:   "7".padStart(3, "0")
来源：http://azu.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://rtv.xinyue.icu

Java: String.format("%03d", 7)
来源：http://lyl.shanyushiyangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bxn.0kj1m.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://srn.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rft.birdmap.top

[E11] 反转字符串
来源：http://ykc.dashuyun.cn

Py:   s[::-1]
来源：http://wqv.tian-w.cn

PHP:  strrev($s);
来源：http://cvr.fehbvm.com

JS:   [...s].reverse().join("")
来源：http://qst.sxryk.cn

TS:   [...s].reverse().join("")
来源：http://gnw.sufxvd.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tsq.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nju.haohaochexian.top

Ruby: s.reverse
来源：http://uev.yj202588.top

C#:   new string(s.Reverse().ToArray())
来源：http://aly.cdnleiting.top

[E12] 统计某字符出现次数
来源：http://dod.pycfn.com

Py:   s.count("a")
来源：http://qvk.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://oqd.sysykeji.top

JS:   s.split("a").length - 1
来源：http://nck.xziqi.cn

TS:   s.split("a").length - 1
来源：http://zdb.0kj1m.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dbf.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://wav.cdnleiting.top

Ruby: s.count("a")
来源：http://tlf.xuetiantiany.cn

C#:   s.Count(c => c == 'a')
来源：http://ahl.uphjek.com

[E13] 逐字符遍历
来源：http://jfi.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://iru.hammf.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://npz.havefunace.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://pjh.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dkl.fehbvm.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ihq.cucudq.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cmd.chenjidiqi.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://dym.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cnp.guowangkeji.top

[E14] URL 编码与 Base64
来源：http://ddu.jlsjyb.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sir.yuanzhike.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ytn.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rdw.xziqi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vxh.sufxvd.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ulg.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wjk.guannengcc.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uyk.9152youxi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sys.redwolf501.top

[E15] HTML 转义 / 反转义
来源：http://djg.hesvh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qxk.yj20258888.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nld.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bxu.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://qwc.guannengcc.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hde.hammf.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yrg.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zda.ydzc1.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://srl.fengsongda.top

[E16] 数字千分位
来源：http://yhz.zdqjudy.top

Py:   f"{1234567:,}"
来源：http://hwd.meibo888.top

PHP:  number_format(1234567);
来源：http://gmb.shzxlz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xsc.zhaomingkeji.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://upg.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wcr.shuidangran.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tjt.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cka.feifeiyinyue.top

C#:   1234567.ToString("N0")
来源：http://lrd.xylfe.cn

[E17] 首字母大写
来源：http://vjs.smart0.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ole.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://tlh.yueranfly.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wyx.jinghuilouyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dby.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vfj.gzhubu.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bjl.jlsjyb.cn

Ruby: s.capitalize
来源：http://mls.yuxming.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zmf.hesvh.cn

[E18] 模板占位符替换
来源：http://kml.guowangkeji.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://itl.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://moi.gotoacloud.top

JS:   tpl.replaceAll("{name}", name)
来源：http://myo.fanxiaobao.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://rbw.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hta.yj20258.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://udd.sweek.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gky.yongpay.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rof.vqdsnc.cn

[E19] 多行文本按行拆分
来源：http://syd.bjfxy.top

Py:   s.splitlines()
来源：http://tix.xziqi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qzs.xinyue.icu

JS:   s.split(/\r?\n/)
来源：http://slx.yuanzhike.top

TS:   s.split(/\r?\n/)
来源：http://qct.xylfe.cn

Java: s.lines().toList()
来源：http://onz.zycfv.cn

Go:   strings.Split(s, "\n")
来源：http://wsj.vqdsnc.cn

Ruby: s.lines
来源：http://kef.hongshengwenyu.top

C#:   s.Split('\n')
来源：http://nyw.zycfv.cn

[E20] 判断字符串是否为空
来源：http://cek.tianlin.xyz

Py:   if not s:
来源：http://lzj.chenjidiqi.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ala.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lli.dianchejie.cn

TS:   if (s === "") {}
来源：http://uve.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://cjt.dianchejie.cn

Go:   if s == "" {}
来源：http://aup.sxryk.cn

Ruby: if s.empty?
来源：http://vkx.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rye.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://jgn.yj20258.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://low.hammf.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lxi.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lon.jianghu66.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bfe.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mlc.yfazqb.com

Go:   // 按 rune 判断长度后截断
来源：http://mmg.nwbrower.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://akt.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://knh.havefunace.top

[E22] 字节长度与字符长度
来源：http://owb.nwbrower.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mhe.fengsongda.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ugd.cdnleiting.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://btt.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://eut.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qjc.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rmf.epnwcf.com

Ruby: s.bytesize;  s.length
来源：http://xxq.quarkkingdee.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pdc.cashguo.top

================================================================================
来源：http://kpw.yvedp.cn

F. 文件与目录
来源：http://mja.quarkkingdee.top

================================================================================
来源：http://iqo.shangyingyoupin.top

[F01] 读取整个文件
来源：http://yir.zhaomingkeji.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oix.ppjwa.cn

PHP:  file_get_contents("a.txt");
来源：http://pbt.9152youxi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yil.jiagoushi.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://twh.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://vac.hongshengwenyu.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jxq.gotoacloud.top

Ruby: File.read("a.txt")
来源：http://jvw.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://amj.zdbjq.cn

[F02] 逐行读取文件
来源：http://fzp.nanxinkj.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bak.jlsjyb.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cgx.fengsongda.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zmr.havefunace.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hpx.wangshuangyany.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iku.shangyingyoupin.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eqa.cheryme.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uek.ydjk.org.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aec.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://crd.fanxiaobao.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rzb.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://ewc.tian-w.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ksw.fzhhl.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://etl.fehbvm.com

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dys.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dwd.yangfankeji.com

Ruby: File.write("a.txt", "hi")
来源：http://jqa.gotoacloud.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jeb.zhaomingkeji.xyz

[F04] 追加写入文件
来源：http://hgg.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tkw.hongshengwenyu.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bcd.wangdashe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ynb.shangyingyoupin.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tth.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://naf.zdqjudy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wya.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://egc.chenlongwang.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fga.yj202588.top

[F05] 判断文件或目录是否存在
来源：http://lsu.sysykeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xef.chenlongwang.top

PHP:  file_exists("a.txt");
来源：http://xyj.jlsjyb.cn

JS:   fs.existsSync("a.txt")
来源：http://imi.hnqzz.top

TS:   fs.existsSync("a.txt")
来源：http://gbr.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://bwm.zdbjq.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zet.jqgfzy.top

Ruby: File.exist?("a.txt")
来源：http://mll.sufxvd.cn

C#:   File.Exists("a.txt")
来源：http://pet.smart0.xyz

[F06] 删除文件
来源：http://qgz.jqgfzy.top

Py:   os.remove("a.txt")
来源：http://elx.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://ztc.zhijiandao.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xxi.bjfxy.top

TS:   fs.unlinkSync("a.txt")
来源：http://ezb.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gij.hywenlv.cn

Go:   os.Remove("a.txt")
来源：http://lnr.zhijiandao.cn

Ruby: File.delete("a.txt")
来源：http://chu.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://nvn.tanke756.top

[F07] 创建目录（含多级）
来源：http://rli.xuanzx.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rxq.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zbl.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nkn.fanxiaobao.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oqj.mhx1999.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wiz.guannengcc.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bif.hnqzz.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xav.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hqj.chenzaomai.com

[F08] 遍历目录
来源：http://arg.andypj.xyz

Py:   for name in os.listdir("dir"): print(name)
来源：http://lpe.cashguo.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jdn.zhiwuduotai.top

JS:   fs.readdirSync("dir")
来源：http://oxr.zhiwuduotai.top

TS:   fs.readdirSync("dir")
来源：http://bxc.fanxiaobao.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mvk.gogol.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://chy.xuetiantiany.cn

Ruby: Dir.children("dir")
来源：http://bzo.cqqwz.cn

C#:   Directory.GetFiles("dir")
来源：http://qii.jqgufenzy.top

[F09] 获取文件大小
来源：http://zcw.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://emx.yj202588.top

PHP:  filesize("a.txt");
来源：http://qbr.iojbl.cn

JS:   fs.statSync("a.txt").size
来源：http://yvw.sysykeji.top

TS:   fs.statSync("a.txt").size
来源：http://hwc.hnqzz.top

Java: Files.size(Path.of("a.txt"))
来源：http://xae.ybcxt.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://whx.jinqigfzy.top

Ruby: File.size("a.txt")
来源：http://wxe.gaohongyu789.top

C#:   new FileInfo("a.txt").Length
来源：http://vvm.zhixingplan.top

[F10] 取文件扩展名 / 文件名
来源：http://fvn.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jri.zhiwuduotai.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lpj.ivvv.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zzz.iojbl.cn

TS:   path.extname("a.txt")
来源：http://adf.xylfe.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xnq.zdbjq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://cai.shanyushiyangkeji.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yub.yfazqb.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dbu.jinqigfzy.top

[F11] 复制与移动文件
来源：http://uqo.yuanzhike.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nui.fengsongda.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yjx.zhixingplan.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jef.sweek.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://amq.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://klk.shangyingyoupin.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://pfb.sufxvd.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iad.ydzc1.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://lvp.wangshuangyany.cn

[F12] CSV 读写
来源：http://wfe.zhoulong.xyz

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://srw.dianchejie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yqb.zdbjq.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://afs.shuidangran.top

TS:   // 同上
来源：http://ujp.sxryk.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bfy.andypj.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://meu.sxryk.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jyg.fktsv.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ojy.sxryk.cn

================================================================================
来源：http://wkz.sysykeji.top

G. 面向对象
来源：http://jfu.fehbvm.com

================================================================================
来源：http://flf.aibaodan.cn

[G01] 定义类
来源：http://hap.yongpay.top

Py:   class User: pass
来源：http://pih.gaohongyu789.top

PHP:  class User {}
来源：http://qvg.ydjk.org.cn

JS:   class User {}
来源：http://axy.kuanghao11.cn

TS:   class User { name: string = ""; }
来源：http://yad.316326.xyz

Java: class User {}
来源：http://adr.316326.xyz

Go:   type User struct { Name string }
来源：http://cvw.ydjk.org.cn

Ruby: class User; end
来源：http://xdn.hnqzz.top

C#:   class User {}
来源：http://ktn.tianlin.xyz

[G02] 构造函数
来源：http://vdi.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://von.hnqzz.top

PHP:  public function __construct(public string $name) {}
来源：http://nzo.fktsv.cn

JS:   constructor(name) { this.name = name; }
来源：http://oiz.ywan-chungtsiang.top

TS:   constructor(public name: string) {}
来源：http://bnl.xuanzx.com

Java: User(String name) { this.name = name; }
来源：http://tfy.dashuyun.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aqq.shuidangran.top

Ruby: def initialize(name); @name = name; end
来源：http://dgx.ywan-chungtsiang.top

C#:   public User(string name) { Name = name; }
来源：http://yyr.yj20258.top

[G03] 实例属性
来源：http://qcj.guannengcc.top

Py:   self.name = "x"
来源：http://kaf.ehwqpu.com

PHP:  public string $name = "x";
来源：http://pxq.yueranfly.top

JS:   this.name = "x";
来源：http://bql.fehbvm.com

TS:   name: string = "x";
来源：http://dys.316326.xyz

Java: private String name;
来源：http://rdu.hfpthk.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nsc.bbcook.cn

Ruby: @name = "x"
来源：http://zre.9152youxi.cn

C#:   public string Name { get; set; } = "x";
来源：http://kgz.aibaodan.cn

[G04] 定义方法
来源：http://hoz.andypj.xyz

Py:   def greet(self): return self.name
来源：http://iyj.fzhhl.top


<!-- 参考信息 -->