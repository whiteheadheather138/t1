代发 wailian999

TS:   "ab".repeat(3)
来源：http://ohg.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://lyh.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://tws.guowangkeji.top

Ruby: "ab" * 3
来源：http://qkz.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oxo.shanyushiyangkeji.top

[E03] 截取子串
来源：http://uwx.ctjpmb.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ovf.feifeiyinyue.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bcm.sxryk.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hcc.fanxiaobao.xyz

TS:   s.slice(1, 4)
来源：http://dnm.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://fov.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vse.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://qsk.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://xbk.nanxuanxn.top

[E04] 查找子串位置
来源：http://efq.yj20258.top

Py:   s.find("x");  s.index("x")
来源：http://uyl.aibaodan.cn

PHP:  strpos($s, "x");
来源：http://ygb.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tjk.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://huu.shanyushiyangkeji.top

Java: s.indexOf("x")
来源：http://lhn.fengsongda.top

Go:   strings.Index(s, "x")
来源：http://zox.vqdsnc.cn

Ruby: s.index("x")
来源：http://hrn.jinqigufen.top

C#:   s.IndexOf("x")
来源：http://fyc.guannengcc.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jga.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sml.vehdjk.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://khj.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xbq.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://rvl.mhx1999.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qer.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rok.ydzc1.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lgc.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ikj.bjfxy.top

[E06] 替换子串
来源：http://jpx.hcnkem.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fnu.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://htr.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://srt.smart0.xyz

TS:   s.replaceAll("a", "b")
来源：http://sii.zycfv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zuz.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dov.yj20258.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ggq.yanxiufei.cn

C#:   s.Replace("a", "b")
来源：http://zft.jqgufenzy.top

[E07] 按分隔符拆分
来源：http://yfu.yongpay.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ruh.daxiang520.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dsy.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nlo.feifeiyinyue.top

TS:   s.split(",")
来源：http://pao.kuanghao11.cn

Java: s.split(",");  s.split("\\s+")
来源：http://obc.fehbvm.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oed.cheryme.top

Ruby: s.split(",");  s.split
来源：http://qzi.yuanzhike.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tvu.nanxuanxn.top

[E08] 数组按分隔符合并
来源：http://olg.smart0.xyz

Py:   ",".join(items)
来源：http://akd.gaohongyu789.top

PHP:  implode(",", $items);
来源：http://juw.xziqi.cn

JS:   items.join(",")
来源：http://zof.cucudq.cn

TS:   items.join(",")
来源：http://ruh.gzhubu.top

Java: String.join(",", items)
来源：http://rgx.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://qgg.fzhhl.top

Ruby: items.join(",")
来源：http://kwb.nanxinkj.top

C#:   string.Join(",", items)
来源：http://igf.fanxiaobao.xyz

[E09] 去除所有空白字符
来源：http://ddf.jyoumei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vlh.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kbr.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://znm.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://ejn.zycfv.cn

Java: s.replaceAll("\\s+", "")
来源：http://mby.xylfe.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lmb.hnqzz.top

Ruby: s.gsub(/\s+/, "")
来源：http://vsj.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cqx.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://ofb.yj20258.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ern.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wzr.ctjpmb.com

JS:   "7".padStart(3, "0")
来源：http://dwt.jinqigfzy.top

TS:   "7".padStart(3, "0")
来源：http://sdl.gogol.net.cn

Java: String.format("%03d", 7)
来源：http://iwz.wangshuangyany.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lbx.tanke756.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://utv.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tmz.pengpengdd.cyou

[E11] 反转字符串
来源：http://kry.xinyue.icu

Py:   s[::-1]
来源：http://jld.guannengcc.top

PHP:  strrev($s);
来源：http://ati.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://mbs.meibo888.top

TS:   [...s].reverse().join("")
来源：http://fxv.daria6918.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://czm.tanke756.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nma.hcnkem.com

Ruby: s.reverse
来源：http://ran.ehwqpu.com

C#:   new string(s.Reverse().ToArray())
来源：http://bug.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://biw.zhengqikj.top

Py:   s.count("a")
来源：http://yay.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://ods.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://mtb.yj202588.top

TS:   s.split("a").length - 1
来源：http://zmg.epnwcf.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fnq.fktsv.cn

Go:   strings.Count(s, "a")
来源：http://zjm.uphjek.com

Ruby: s.count("a")
来源：http://buo.pengpengdd.cyou

C#:   s.Count(c => c == 'a')
来源：http://dfd.nwbrower.top

[E13] 逐字符遍历
来源：http://ftv.vehdjk.com

Py:   for ch in s: print(ch)
来源：http://xyh.birdmap.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nat.cheryme.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rvg.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://slm.yfazqb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rvv.hysaishi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fgr.uphjek.com

Ruby: s.each_char { |ch| puts ch }
来源：http://vey.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://djo.sweek.top

[E14] URL 编码与 Base64
来源：http://reo.yonumen.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cwd.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://zid.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://swl.gaohongyu789.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sru.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nvj.sysykeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://upz.ctjpmb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vbn.tarul.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uou.cashguo.top

[E15] HTML 转义 / 反转义
来源：http://xyk.yangfankeji.com

Py:   html.escape(s);  html.unescape(s)
来源：http://dvf.fehbvm.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wuu.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qqh.yangfankeji.com

TS:   // 同上，务必做 XSS 过滤
来源：http://jbw.ybcxt.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://otc.chenlongwang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xrj.shanyushiyangtech.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ito.zhixingplan.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zju.zdbjq.cn

[E16] 数字千分位
来源：http://gdq.ctjpmb.com

Py:   f"{1234567:,}"
来源：http://akj.smart0.xyz

PHP:  number_format(1234567);
来源：http://jjn.jlsjyb.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ayv.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cus.guannengcc.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rxz.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vwl.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gjz.xziqi.cn

C#:   1234567.ToString("N0")
来源：http://mnq.gotoacloud.top

[E17] 首字母大写
来源：http://ejl.fanxiaobao.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jxh.sjlbkw.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nqw.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mll.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mjo.sysykeji.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fnq.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pvb.jyoumei.cn

Ruby: s.capitalize
来源：http://vqm.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://djq.zhoulong.xyz

[E18] 模板占位符替换
来源：http://chy.ybcxt.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://seb.cdnleiting.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jsz.aibaodan.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dlw.shuidangran.top

TS:   tpl.replaceAll("{name}", name)
来源：http://yyp.zhaomingkeji.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ywj.ivvv.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zim.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ptq.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bnb.zhiwuduotai.top

[E19] 多行文本按行拆分
来源：http://ceu.shzxlz.cn

Py:   s.splitlines()
来源：http://cki.yuanzhike.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lwn.smart0.xyz

JS:   s.split(/\r?\n/)
来源：http://jtz.ywan-chungtsiang.top

TS:   s.split(/\r?\n/)
来源：http://apf.pengpengdd.cyou

Java: s.lines().toList()
来源：http://nhc.zhongyouzk.top

Go:   strings.Split(s, "\n")
来源：http://iur.aibaodan.cn

Ruby: s.lines
来源：http://apa.jinghuilouyu.cn

C#:   s.Split('\n')
来源：http://ecx.zycfv.cn

[E20] 判断字符串是否为空
来源：http://zyp.haohaochexian.top

Py:   if not s:
来源：http://mef.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dxz.gaohongyu789.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vbr.dashuyun.cn

TS:   if (s === "") {}
来源：http://jmn.c1oappe.top

Java: if (s.isEmpty()) {}
来源：http://tue.kuanghao11.cn

Go:   if s == "" {}
来源：http://lnj.shanyushiyangtech.top

Ruby: if s.empty?
来源：http://xes.wangdashe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lbk.tianlin.xyz

[E21] 超长截断加省略号
来源：http://uze.xinyue.icu

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cxz.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lnf.svipenyu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xtm.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wtx.jinyuanbaomall.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gzr.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://byo.shanyushiyangtech.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xag.pycfn.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lmw.epnwcf.com

[E22] 字节长度与字符长度
来源：http://lom.cqqwz.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://smc.yuanzhike.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xws.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mag.yueranfly.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://muu.ybcxt.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://foy.yfazqb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://usg.c1oappe.top

Ruby: s.bytesize;  s.length
来源：http://yzh.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nva.cqqwz.cn

================================================================================
来源：http://ocn.xingfuxueyuan.xyz

F. 文件与目录
来源：http://cum.yongpay.top

================================================================================
来源：http://xwg.yj202588.top

[F01] 读取整个文件
来源：http://mkk.shanyushiyangtech.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://inb.fanxiaobao.xyz

PHP:  file_get_contents("a.txt");
来源：http://ttr.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kti.gzhubu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dzk.gaohongyu789.top

Java: Files.readString(Path.of("a.txt"))
来源：http://dxc.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fjt.sxryk.cn

Ruby: File.read("a.txt")
来源：http://vhs.jqgfzy.top

C#:   File.ReadAllText("a.txt");
来源：http://ell.ehwqpu.com

[F02] 逐行读取文件
来源：http://xji.jqgfzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qgf.cqqwz.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tde.zdbjq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kdo.zhixingplan.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hye.bbcook.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zwm.quarkkingdee.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ype.nwbrower.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wrq.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blu.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://epu.jiagoushi.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oed.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://tcx.hywenlv.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fxo.yueranfly.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://und.gaohongyu789.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jqc.ppjwa.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pma.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://bgm.aibaodan.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sfg.hcnkem.com

[F04] 追加写入文件
来源：http://ymk.sweek.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://dey.jyoumei.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ckz.fengsongda.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qyz.jinqigufen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gol.ctjpmb.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vnt.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://skp.yanxiufei.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gts.sufxvd.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kvb.hysaishi.cn

[F05] 判断文件或目录是否存在
来源：http://dux.gogol.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pdy.pengpengdd.cyou

PHP:  file_exists("a.txt");
来源：http://slo.chenjidiqi.icu

JS:   fs.existsSync("a.txt")
来源：http://hoa.daria6918.cn

TS:   fs.existsSync("a.txt")
来源：http://bly.jinghuilouyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hro.kuanghao11.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zpi.yj20258.top

Ruby: File.exist?("a.txt")
来源：http://jvn.gotoacloud.top

C#:   File.Exists("a.txt")
来源：http://fkh.chenlongwang.top

[F06] 删除文件
来源：http://cng.hcnkem.com

Py:   os.remove("a.txt")
来源：http://eyv.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://bza.fengsongda.top

JS:   fs.unlinkSync("a.txt")
来源：http://kvn.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://pyc.tian-w.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yno.zhaomingkeji.xyz

Go:   os.Remove("a.txt")
来源：http://opu.yongpay.top

Ruby: File.delete("a.txt")
来源：http://pjk.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://umg.zdbjq.cn

[F07] 创建目录（含多级）
来源：http://ntt.tarul.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nqq.nanxuanxn.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://whl.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ytv.sweek.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mah.aizwys.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fqz.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://svy.fanxiaobao.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nva.birdmap.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fuc.xuetiantiany.cn

[F08] 遍历目录
来源：http://wbh.zhiwuduotai.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://tai.yangfankeji.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uyg.jlsjyb.cn

JS:   fs.readdirSync("dir")
来源：http://cxf.cdnleiting.top

TS:   fs.readdirSync("dir")
来源：http://rml.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jen.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jxy.yonumen.top

Ruby: Dir.children("dir")
来源：http://cal.hongshengwenyu.top

C#:   Directory.GetFiles("dir")
来源：http://akm.sxryk.cn

[F09] 获取文件大小
来源：http://pgk.feifeiyinyue.top

Py:   os.path.getsize("a.txt")
来源：http://ibg.cqqwz.cn

PHP:  filesize("a.txt");
来源：http://aap.fengsongda.top

JS:   fs.statSync("a.txt").size
来源：http://zkn.zdqjudy.top

TS:   fs.statSync("a.txt").size
来源：http://owp.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://kku.nwbrower.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eee.nwbrower.top

Ruby: File.size("a.txt")
来源：http://igj.52xcode.cn

C#:   new FileInfo("a.txt").Length
来源：http://xek.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://ccf.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://itl.hammf.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dci.sysykeji.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pyv.hongshengwenyu.top

TS:   path.extname("a.txt")
来源：http://mox.fanxiaobao.xyz

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eag.ehwqpu.com

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gly.zhijiandao.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kyv.vehdjk.com

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://moi.hywenlv.cn

[F11] 复制与移动文件
来源：http://yss.yfazqb.com

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pif.9152youxi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://aok.dianchejie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ovt.jqgufenzy.top

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rpz.ydjk.org.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dhi.epnwcf.com

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hle.fzhhl.top

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wjt.nwbrower.top

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qqw.haohaochexian.top

[F12] CSV 读写
来源：http://cwi.meibo888.top

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yhw.xylfe.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xnj.haohaochexian.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lvx.kuanghao11.cn

TS:   // 同上
来源：http://uxx.yanxiufei.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yhg.ehwqpu.com

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://obu.aizwys.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://umt.chenlongwang.top

C#:   // 无内置：用 CsvHelper 库
来源：http://tuf.jinghuilouyu.cn

================================================================================
来源：http://vur.sxryk.cn

G. 面向对象
来源：http://luj.snrcjt.cn

================================================================================
来源：http://duu.zdqjudy.top

[G01] 定义类
来源：http://lqq.jiagoushi.top


<!-- 参考信息 -->