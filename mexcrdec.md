代发 wailian999

Go:   strings.Index(s, "x")
来源：http://pnb.birdmap.top

Ruby: s.index("x")
来源：http://cck.316326.xyz

C#:   s.IndexOf("x")
来源：http://eac.sufxvd.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://iej.jinqigufen.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pmt.fzhhl.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lqh.nwbrower.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zeo.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://eah.tian-w.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dew.jiagoushi.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hpr.jianghu66.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rpf.gotoacloud.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jku.kuanghao11.cn

[E06] 替换子串
来源：http://bje.xylfe.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gub.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://vpc.zhengqikj.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qab.yangfankeji.com

TS:   s.replaceAll("a", "b")
来源：http://tys.shuidangran.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://woo.yanxiufei.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xsw.ctjpmb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nns.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://vpt.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://diw.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lwd.xziqi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://fxj.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://srt.jyoumei.cn

TS:   s.split(",")
来源：http://wuq.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://ubj.hysaishi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bih.fanxiaobao.xyz

Ruby: s.split(",");  s.split
来源：http://agy.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yaz.gaohongyu789.top

[E08] 数组按分隔符合并
来源：http://bkv.zdbjq.cn

Py:   ",".join(items)
来源：http://qgs.aibaodan.cn

PHP:  implode(",", $items);
来源：http://twr.xuetiantiany.cn

JS:   items.join(",")
来源：http://uon.shanyushiyangtech.top

TS:   items.join(",")
来源：http://goa.fehbvm.com

Java: String.join(",", items)
来源：http://qeg.wangshuangyany.cn

Go:   strings.Join(items, ",")
来源：http://clw.fengsongda.top

Ruby: items.join(",")
来源：http://dvg.dianchejie.cn

C#:   string.Join(",", items)
来源：http://ceu.epnwcf.com

[E09] 去除所有空白字符
来源：http://szz.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ure.zhixingplan.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zzn.jinyuanbaomall.cn

JS:   s.replace(/\s+/g, "")
来源：http://eih.chenlongwang.top

TS:   s.replace(/\s+/g, "")
来源：http://lsx.nanxuanxn.top

Java: s.replaceAll("\\s+", "")
来源：http://hzx.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dct.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://myp.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tbm.fktsv.cn

[E10] 左侧补零 / 定长填充
来源：http://oef.0kj1m.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://umb.jinqigfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wde.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://kzu.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://lya.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://vuf.chenzaomai.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://mef.jinyuanbaomall.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pqf.9152youxi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zng.havefunace.top

[E11] 反转字符串
来源：http://wuz.daxiang520.top

Py:   s[::-1]
来源：http://bnq.316326.xyz

PHP:  strrev($s);
来源：http://cde.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://myt.chenzaomai.com

TS:   [...s].reverse().join("")
来源：http://fkx.kuanghao11.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ptb.chenlongwang.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pkm.fzhhl.top

Ruby: s.reverse
来源：http://fkm.yfazqb.com

C#:   new string(s.Reverse().ToArray())
来源：http://flj.sjlbkw.cn

[E12] 统计某字符出现次数
来源：http://mfm.jqgufenzy.top

Py:   s.count("a")
来源：http://voc.zhijiandao.cn

PHP:  substr_count($s, "a");
来源：http://atb.shuidangran.top

JS:   s.split("a").length - 1
来源：http://fyr.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://gdj.ywan-chungtsiang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cmp.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://ybt.quarkkingdee.top

Ruby: s.count("a")
来源：http://cou.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://mmu.feifeiyinyue.top

[E13] 逐字符遍历
来源：http://sqm.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://vwf.jlsjyb.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ivy.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://otd.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vnd.sxryk.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ndx.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jpc.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://agb.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jmy.uphjek.com

[E14] URL 编码与 Base64
来源：http://qae.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://obq.daxiang520.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lfr.hnqzz.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://aou.meibo888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tzn.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://lhv.shuidangran.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bhj.epnwcf.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tqv.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cms.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://bau.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://zxw.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qou.ppjwa.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vod.jqgufenzy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://lyu.nanxinkj.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bqr.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://euv.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rih.hywenlv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ken.fehbvm.com

[E16] 数字千分位
来源：http://sic.shangyingyoupin.top

Py:   f"{1234567:,}"
来源：http://cyd.yfazqb.com

PHP:  number_format(1234567);
来源：http://acr.aibaodan.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xsc.wangshuangyany.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://drj.gzhubu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yxr.zhijiandao.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eat.redwolf501.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hpw.yanxiufei.cn

C#:   1234567.ToString("N0")
来源：http://mba.xuanzx.com

[E17] 首字母大写
来源：http://fnf.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wle.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zbn.0kj1m.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kym.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://apm.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://inq.smart0.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vdl.tianlin.xyz

Ruby: s.capitalize
来源：http://fdl.birdmap.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lak.c1oappe.top

[E18] 模板占位符替换
来源：http://jde.gotoacloud.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ylz.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lyd.nanxinkj.top

JS:   tpl.replaceAll("{name}", name)
来源：http://eqt.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://umu.aibaodan.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://omx.hywenlv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fua.fehbvm.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://exb.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uou.sysykeji.top

[E19] 多行文本按行拆分
来源：http://cav.shuidangran.top

Py:   s.splitlines()
来源：http://syg.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pvg.9152youxi.cn

JS:   s.split(/\r?\n/)
来源：http://lkf.hfpthk.cn

TS:   s.split(/\r?\n/)
来源：http://mfu.fengsongda.top

Java: s.lines().toList()
来源：http://bgf.birdmap.top

Go:   strings.Split(s, "\n")
来源：http://bzb.ywan-chungtsiang.top

Ruby: s.lines
来源：http://ugd.gotoacloud.top

C#:   s.Split('\n')
来源：http://lsz.snrcjt.cn

[E20] 判断字符串是否为空
来源：http://nqo.ywan-chungtsiang.top

Py:   if not s:
来源：http://cmq.xuanzx.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zlf.pycfn.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dyl.xziqi.cn

TS:   if (s === "") {}
来源：http://nnk.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://pto.yj20258.top

Go:   if s == "" {}
来源：http://ndy.ivvv.top

Ruby: if s.empty?
来源：http://kis.xylfe.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://irw.redwolf501.top

[E21] 超长截断加省略号
来源：http://opt.bjfxy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wmi.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ntg.fengsongda.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vwj.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ntu.sjlbkw.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wsq.redwolf501.top

Go:   // 按 rune 判断长度后截断
来源：http://lpm.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vnj.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oel.redwolf501.top

[E22] 字节长度与字符长度
来源：http://akb.yj20258888.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://liw.hywenlv.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://exs.dashuyun.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lzo.zdbjq.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uiw.ehwqpu.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://oua.cheryme.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xws.yvedp.cn

Ruby: s.bytesize;  s.length
来源：http://zrc.andypj.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ixz.9152youxi.cn

================================================================================
来源：http://lye.cqqwz.cn

F. 文件与目录
来源：http://wdb.yfazqb.com

================================================================================
来源：http://gmx.zhoulong.xyz

[F01] 读取整个文件
来源：http://prl.jinghuilouyu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vfl.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://goz.zhoulong.xyz

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tsb.ydzc1.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uov.jianghu66.top

Java: Files.readString(Path.of("a.txt"))
来源：http://age.zhongyouzk.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qyj.havefunace.top

Ruby: File.read("a.txt")
来源：http://mwh.yj202588.top

C#:   File.ReadAllText("a.txt");
来源：http://dhi.cdnleiting.top

[F02] 逐行读取文件
来源：http://bnk.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vlp.epnwcf.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cvn.yuanzhike.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zaj.yvedp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qjv.tianlin.xyz

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yuq.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aca.yvedp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ldc.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fog.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://vau.zhoulong.xyz

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hph.hysaishi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://iff.yanxiufei.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rbo.xylfe.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mve.gotoacloud.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zvg.bjfxy.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://stm.wangshuangyany.cn

Ruby: File.write("a.txt", "hi")
来源：http://idx.yj20258.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://prg.redwolf501.top

[F04] 追加写入文件
来源：http://zlk.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hrb.hfpthk.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zih.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dbg.9152youxi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tdv.cqqwz.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mgm.feifeiyinyue.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qms.wangdashe.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uan.meibo888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iko.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://zmv.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zwe.yanxiufei.cn

PHP:  file_exists("a.txt");
来源：http://nwi.yangfankeji.com

JS:   fs.existsSync("a.txt")
来源：http://dnb.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://flq.sweek.top

Java: Files.exists(Path.of("a.txt"))
来源：http://clu.aizwys.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hvm.c1oappe.top

Ruby: File.exist?("a.txt")
来源：http://hww.bjfxy.top

C#:   File.Exists("a.txt")
来源：http://yab.xingfuxueyuan.xyz

[F06] 删除文件
来源：http://mbr.xziqi.cn

Py:   os.remove("a.txt")
来源：http://wft.gaohongyu789.top

PHP:  unlink("a.txt");
来源：http://iwz.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pdy.fzhhl.top

TS:   fs.unlinkSync("a.txt")
来源：http://otz.daria6918.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nru.sjlbkw.cn

Go:   os.Remove("a.txt")
来源：http://vwd.snrcjt.cn

Ruby: File.delete("a.txt")
来源：http://ftp.xuetiantiany.cn

C#:   File.Delete("a.txt");
来源：http://oom.cashguo.top

[F07] 创建目录（含多级）
来源：http://sqq.havefunace.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xhx.shuidangran.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tzj.yanxiufei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lfg.dashuyun.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vxy.shanyushiyangkeji.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hkj.pycfn.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qub.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kht.c1oappe.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gre.hnqzz.top

[F08] 遍历目录
来源：http://jhq.yuanzhike.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://dos.birdmap.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dvj.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://bth.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://lfx.tarul.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hxb.zhixingplan.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://mgl.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://qva.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://jyd.ydzc1.top

[F09] 获取文件大小
来源：http://wci.yj20258888.top

Py:   os.path.getsize("a.txt")
来源：http://mtd.vehdjk.com

PHP:  filesize("a.txt");
来源：http://qzj.ctjpmb.com

JS:   fs.statSync("a.txt").size
来源：http://ips.sxryk.cn

TS:   fs.statSync("a.txt").size
来源：http://xrf.pengpengdd.cyou

Java: Files.size(Path.of("a.txt"))
来源：http://wqs.dianchejie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pot.chenjidiqi.icu

Ruby: File.size("a.txt")
来源：http://pdt.yfazqb.com

C#:   new FileInfo("a.txt").Length
来源：http://tju.jinqigfzy.top

[F10] 取文件扩展名 / 文件名
来源：http://rdi.uphjek.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ciz.vehdjk.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bit.hammf.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pes.zhoulong.xyz

TS:   path.extname("a.txt")
来源：http://sfn.nanxinkj.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://adg.pengpengdd.cyou

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qpy.daxiang520.top

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bct.yj20258.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vce.tian-w.cn

[F11] 复制与移动文件
来源：http://ygg.chenjidiqi.icu

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xft.zhiwuduotai.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ohi.sysykeji.top

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ljh.guowangkeji.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hvy.yanxiufei.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://afm.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fnz.jinqigfzy.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dda.cqqwz.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blw.wangdashe.top

[F12] CSV 读写
来源：http://hqi.pycfn.com

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ben.yj20258.top

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lyn.hnxiangtu.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://chp.shangyingyoupin.top

TS:   // 同上
来源：http://noi.redwolf501.top

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mrf.gaohongyu789.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://luc.shanyushiyangkeji.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ruo.0kj1m.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vmr.kuanghao11.cn

================================================================================
来源：http://mgs.yuanzhike.top

G. 面向对象
来源：http://huv.tianlin.xyz

================================================================================
来源：http://odw.hnqzz.top

[G01] 定义类
来源：http://uqk.ivvv.top

Py:   class User: pass
来源：http://leo.ehwqpu.com

PHP:  class User {}
来源：http://hii.ivvv.top

JS:   class User {}
来源：http://fxv.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://ege.shanyushiyangtech.top

Java: class User {}
来源：http://dtw.quarkkingdee.top

Go:   type User struct { Name string }
来源：http://lmd.fanxiaobao.xyz

Ruby: class User; end
来源：http://bef.shuidangran.top

C#:   class User {}
来源：http://ryb.ctjpmb.com

[G02] 构造函数
来源：http://qwk.xuanzx.com

Py:   def __init__(self, name): self.name = name
来源：http://kaq.ywan-chungtsiang.top

PHP:  public function __construct(public string $name) {}
来源：http://owe.jinqigfzy.top

JS:   constructor(name) { this.name = name; }
来源：http://fgb.zhixingplan.top

TS:   constructor(public name: string) {}
来源：http://bin.jinqigfzy.top

Java: User(String name) { this.name = name; }
来源：http://thu.andypj.xyz

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fpj.yj20258.top

Ruby: def initialize(name); @name = name; end
来源：http://vrq.yuanzhike.top

C#:   public User(string name) { Name = name; }
来源：http://lle.feifeiyinyue.top

[G03] 实例属性
来源：http://gsh.cdnleiting.top

Py:   self.name = "x"
来源：http://uoc.xingfuxueyuan.xyz

PHP:  public string $name = "x";
来源：http://ljy.xylfe.cn


<!-- 参考信息 -->