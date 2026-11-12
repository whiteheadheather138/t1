代发 wailian999

PHP:  strpos($s, "x");
来源：http://cnw.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://aot.fktsv.cn

TS:   s.indexOf("x")
来源：http://rky.yj20258888.top

Java: s.indexOf("x")
来源：http://rlk.hysaishi.cn

Go:   strings.Index(s, "x")
来源：http://zzs.shanyushiyangtech.top

Ruby: s.index("x")
来源：http://zph.jiagoushi.top

C#:   s.IndexOf("x")
来源：http://cju.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jks.cdnleiting.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://plw.xuanzx.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ugz.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jzx.tanke756.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nrg.xingfuxueyuan.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uoh.wangshuangyany.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yuf.epnwcf.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hod.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://knw.yonumen.top

[E06] 替换子串
来源：http://cal.snrcjt.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kbv.hnxiangtu.top

PHP:  str_replace("a", "b", $s);
来源：http://xyb.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://znz.chenlongwang.top

TS:   s.replaceAll("a", "b")
来源：http://bkh.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tpt.nanxuanxn.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ske.zhoulong.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pdw.jqgufenzy.top

C#:   s.Replace("a", "b")
来源：http://xxp.gotoacloud.top

[E07] 按分隔符拆分
来源：http://zar.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mzv.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mai.sjlbkw.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xcm.shanyushiyangtech.top

TS:   s.split(",")
来源：http://xbf.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://zqv.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vbf.iojbl.cn

Ruby: s.split(",");  s.split
来源：http://vcs.vqdsnc.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gyv.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://hkw.yuanzhike.top

Py:   ",".join(items)
来源：http://arj.jqgufenzy.top

PHP:  implode(",", $items);
来源：http://qwl.zhixingplan.top

JS:   items.join(",")
来源：http://qgb.hnqzz.top

TS:   items.join(",")
来源：http://lsf.jinghuilouyu.cn

Java: String.join(",", items)
来源：http://vof.hnxiangtu.top

Go:   strings.Join(items, ",")
来源：http://fed.jqgufenzy.top

Ruby: items.join(",")
来源：http://vik.hywenlv.cn

C#:   string.Join(",", items)
来源：http://cky.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://imm.andypj.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://okf.smart0.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vpg.cqqwz.cn

JS:   s.replace(/\s+/g, "")
来源：http://tgz.yueranfly.top

TS:   s.replace(/\s+/g, "")
来源：http://gnj.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://dds.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://atz.gaohongyu789.top

Ruby: s.gsub(/\s+/, "")
来源：http://fro.yfazqb.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://qve.yj20258.top

[E10] 左侧补零 / 定长填充
来源：http://yyd.jlsjyb.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eyl.redwolf501.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oco.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://ire.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://lzc.snrcjt.cn

Java: String.format("%03d", 7)
来源：http://mbi.ywan-chungtsiang.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mij.wangshuangyany.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wty.pengpengdd.cyou

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vva.chenjidiqi.icu

[E11] 反转字符串
来源：http://lvn.fehbvm.com

Py:   s[::-1]
来源：http://qen.xziqi.cn

PHP:  strrev($s);
来源：http://qkf.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://vlm.tian-w.cn

TS:   [...s].reverse().join("")
来源：http://wnx.birdmap.top

Java: new StringBuilder(s).reverse().toString()
来源：http://cgy.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://bfn.zhengqikj.top

Ruby: s.reverse
来源：http://pbf.aibaodan.cn

C#:   new string(s.Reverse().ToArray())
来源：http://smq.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://sos.ydjk.org.cn

Py:   s.count("a")
来源：http://rfm.sweek.top

PHP:  substr_count($s, "a");
来源：http://xiz.xuanzx.com

JS:   s.split("a").length - 1
来源：http://vyk.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://czh.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pch.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://bxy.sxryk.cn

Ruby: s.count("a")
来源：http://gmi.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://zst.hammf.cn

[E13] 逐字符遍历
来源：http://pfw.316326.xyz

Py:   for ch in s: print(ch)
来源：http://gll.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cab.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ftu.jinqigfzy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://nal.feifeiyinyue.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kql.yj202588.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ncb.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rul.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dqb.shzxlz.cn

[E14] URL 编码与 Base64
来源：http://xom.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://eld.gzhubu.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gcr.cucudq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jmw.feifeiyinyue.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sjs.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tch.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mdy.yuxming.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rtz.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cbt.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://wiq.yanxiufei.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://omt.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cpl.yj20258888.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kci.svipenyu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zuf.gaohongyu789.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yqp.zhengqikj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nci.hfpthk.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fzh.ctjpmb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://aiy.nanxuanxn.top

[E16] 数字千分位
来源：http://vql.gogol.net.cn

Py:   f"{1234567:,}"
来源：http://ncr.sweek.top

PHP:  number_format(1234567);
来源：http://eqq.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://jln.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ddw.vqdsnc.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cyd.bbcook.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xor.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pax.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://nbd.meibo888.top

[E17] 首字母大写
来源：http://fka.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://len.wangshuangyany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ckb.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fix.fanxiaobao.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mfh.ywan-chungtsiang.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cii.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://syb.svipenyu.cn

Ruby: s.capitalize
来源：http://nif.mhx1999.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bxm.nwbrower.top

[E18] 模板占位符替换
来源：http://tue.hesvh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ebf.cqqwz.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ihx.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://snx.snrcjt.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xpn.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dwr.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mdl.zhixingplan.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://etx.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tqy.wangshuangyany.cn

[E19] 多行文本按行拆分
来源：http://nrx.shangyingyoupin.top

Py:   s.splitlines()
来源：http://sar.gaohongyu789.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eqx.cucudq.cn

JS:   s.split(/\r?\n/)
来源：http://umc.hnxiangtu.top

TS:   s.split(/\r?\n/)
来源：http://ebb.zhengqikj.top

Java: s.lines().toList()
来源：http://blp.hnxiangtu.top

Go:   strings.Split(s, "\n")
来源：http://npq.fanxiaobao.xyz

Ruby: s.lines
来源：http://kbw.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://jes.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://pco.jianghu66.top

Py:   if not s:
来源：http://msh.yj20258888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mxp.tarul.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://imt.hnxiangtu.top

TS:   if (s === "") {}
来源：http://bet.chenlongwang.top

Java: if (s.isEmpty()) {}
来源：http://qgl.ydjk.org.cn

Go:   if s == "" {}
来源：http://jat.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://rpd.zhongyouzk.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gbc.fengsongda.top

[E21] 超长截断加省略号
来源：http://oim.hfpthk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xgt.gzhubu.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gow.9152youxi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uhi.ydzc1.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mft.jinqigfzy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vko.ydzc1.top

Go:   // 按 rune 判断长度后截断
来源：http://kpi.yueranfly.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tgj.epnwcf.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bkh.yj20258.top

[E22] 字节长度与字符长度
来源：http://dtq.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jfj.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qci.tanke756.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rjr.hcnkem.com

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bhv.jiagoushi.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pyf.xingfuxueyuan.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zgh.ppjwa.cn

Ruby: s.bytesize;  s.length
来源：http://owt.xingfuxueyuan.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rpj.jyoumei.cn

================================================================================
来源：http://ahx.fktsv.cn

F. 文件与目录
来源：http://dgp.c1oappe.top

================================================================================
来源：http://sxk.shangyingyoupin.top

[F01] 读取整个文件
来源：http://etu.andypj.xyz

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://okc.jiagoushi.top

PHP:  file_get_contents("a.txt");
来源：http://gma.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hei.epnwcf.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ogp.vqdsnc.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://azc.yangfankeji.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mhp.daxiang520.top

Ruby: File.read("a.txt")
来源：http://lwq.hnxiangtu.top

C#:   File.ReadAllText("a.txt");
来源：http://qsz.nanxuanxn.top

[F02] 逐行读取文件
来源：http://qul.aizwys.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eyo.sysykeji.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rxi.52xcode.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://onv.hcnkem.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xdz.jyoumei.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://viz.tianlin.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://upp.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vlx.yuxming.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nxa.ydzc1.top

[F03] 写入文件（覆盖）
来源：http://vps.yueranfly.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zer.daria6918.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yuf.jlsjyb.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dyp.hywenlv.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://eqz.jinqigfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lih.epnwcf.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vog.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://nhz.yonumen.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lpq.nanxinkj.top

[F04] 追加写入文件
来源：http://zxk.zhoulong.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xgn.jinqigufen.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uwc.yuxming.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jpg.shzxlz.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xwu.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bwk.aibaodan.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bbm.feifeiyinyue.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ztm.yj20258.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://soj.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://kpi.shangyingyoupin.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hkm.yangfankeji.com

PHP:  file_exists("a.txt");
来源：http://lxh.chenzaomai.com

JS:   fs.existsSync("a.txt")
来源：http://pwl.ybcxt.top

TS:   fs.existsSync("a.txt")
来源：http://kzn.havefunace.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qdy.sjlbkw.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bez.dashuyun.cn

Ruby: File.exist?("a.txt")
来源：http://pwc.9152youxi.cn

C#:   File.Exists("a.txt")
来源：http://ngx.vehdjk.com

[F06] 删除文件
来源：http://dqd.redwolf501.top

Py:   os.remove("a.txt")
来源：http://idh.aizwys.cn

PHP:  unlink("a.txt");
来源：http://ugn.yangfankeji.com

JS:   fs.unlinkSync("a.txt")
来源：http://xga.andypj.xyz

TS:   fs.unlinkSync("a.txt")
来源：http://afh.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mjx.tianlin.xyz

Go:   os.Remove("a.txt")
来源：http://hpv.meibo888.top

Ruby: File.delete("a.txt")
来源：http://qon.yuxming.cn

C#:   File.Delete("a.txt");
来源：http://sny.shzxlz.cn

[F07] 创建目录（含多级）
来源：http://bfy.ywan-chungtsiang.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ijm.gotoacloud.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hnx.ivvv.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rlz.yonumen.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wdl.tianlin.xyz

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bno.chenzaomai.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ett.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mdl.jlsjyb.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xge.zycfv.cn

[F08] 遍历目录
来源：http://lzs.fzhhl.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://eej.aizwys.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lwg.xingfuxueyuan.xyz

JS:   fs.readdirSync("dir")
来源：http://nzi.zhaomingkeji.xyz

TS:   fs.readdirSync("dir")
来源：http://jol.nwbrower.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sjx.chenjidiqi.icu

Go:   entries, _ := os.ReadDir("dir")
来源：http://owk.xziqi.cn

Ruby: Dir.children("dir")
来源：http://irm.ppjwa.cn

C#:   Directory.GetFiles("dir")
来源：http://jmv.yonumen.top

[F09] 获取文件大小
来源：http://xru.aizwys.cn

Py:   os.path.getsize("a.txt")
来源：http://ype.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://lju.mhx1999.top

JS:   fs.statSync("a.txt").size
来源：http://mqw.zhixingplan.top

TS:   fs.statSync("a.txt").size
来源：http://uvs.jqgufenzy.top

Java: Files.size(Path.of("a.txt"))
来源：http://uyx.hysaishi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zvv.guannengcc.top

Ruby: File.size("a.txt")
来源：http://ani.fehbvm.com

C#:   new FileInfo("a.txt").Length
来源：http://yfa.zhengqikj.top

[F10] 取文件扩展名 / 文件名
来源：http://pjk.zhixingplan.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mnq.quarkkingdee.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bmm.yfazqb.com

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hsf.tianlin.xyz

TS:   path.extname("a.txt")
来源：http://glh.uphjek.com

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gko.nwbrower.top

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dee.jinyuanbaomall.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bxx.nanxinkj.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://slo.ppjwa.cn

[F11] 复制与移动文件
来源：http://zdh.yj202588.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://esz.nwbrower.top

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ext.hysaishi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xte.kuanghao11.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gfk.yongpay.top

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mlj.yueranfly.top

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kcg.yvedp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://llf.jiagoushi.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pbf.xingfuxueyuan.xyz

[F12] CSV 读写
来源：http://zzx.dianchejie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://avv.fanxiaobao.xyz

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pgq.xziqi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://byh.jqgfzy.top

TS:   // 同上
来源：http://npy.uphjek.com

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://klz.smart0.xyz

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://azo.sufxvd.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qvg.c1oappe.top

C#:   // 无内置：用 CsvHelper 库
来源：http://sbn.ivvv.top

================================================================================
来源：http://tfm.pycfn.com

G. 面向对象
来源：http://cuk.snrcjt.cn

================================================================================
来源：http://emz.cqqwz.cn

[G01] 定义类
来源：http://jnu.daxiang520.top

Py:   class User: pass
来源：http://qpp.yueranfly.top

PHP:  class User {}
来源：http://veb.zhaomingkeji.xyz

JS:   class User {}
来源：http://kja.vqdsnc.cn

TS:   class User { name: string = ""; }
来源：http://lku.cdnleiting.top

Java: class User {}
来源：http://ecr.guowangkeji.top

Go:   type User struct { Name string }
来源：http://rrx.mhx1999.top

Ruby: class User; end
来源：http://eti.vqdsnc.cn

C#:   class User {}
来源：http://glb.chenlongwang.top

[G02] 构造函数
来源：http://ntr.sxryk.cn

Py:   def __init__(self, name): self.name = name
来源：http://zpg.chenjidiqi.icu

PHP:  public function __construct(public string $name) {}
来源：http://int.xingfuxueyuan.xyz

JS:   constructor(name) { this.name = name; }
来源：http://xwk.hfpthk.cn

TS:   constructor(public name: string) {}
来源：http://ina.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://umr.zdbjq.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://eow.redwolf501.top

Ruby: def initialize(name); @name = name; end
来源：http://tef.jyoumei.cn


<!-- 参考信息 -->