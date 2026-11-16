代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wab.fehbvm.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qza.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://smw.zhiwuduotai.top

[D26] 数组转字符串
来源：http://xht.jlsjyb.cn

Py:   ", ".join(map(str, arr))
来源：http://iih.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://xga.nwbrower.top

JS:   arr.join(", ")
来源：http://tfz.quarkkingdee.top

TS:   arr.join(", ")
来源：http://uhb.xinyue.icu

Java: String.join(", ", list)
来源：http://dgg.tanke756.top

Go:   strings.Join(strs, ", ")
来源：http://yoq.uphjek.com

Ruby: arr.join(", ")
来源：http://yir.gotoacloud.top

C#:   string.Join(", ", list)
来源：http://zpe.yj20258.top

================================================================================
来源：http://jfi.jianghu66.top

E. 字符串处理
来源：http://agz.hongshengwenyu.top

================================================================================
来源：http://stk.cashguo.top

[E01] 拼接字符串
来源：http://nmi.jinyuanbaomall.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eua.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hxn.yuxming.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tzi.meibo888.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wdt.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://itf.tian-w.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qqj.ehwqpu.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ckj.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oyi.zhongyouzk.top

[E02] 重复字符串
来源：http://njt.andypj.xyz

Py:   "ab" * 3
来源：http://wtg.yanxiufei.cn

PHP:  str_repeat("ab", 3);
来源：http://pgu.quarkkingdee.top

JS:   "ab".repeat(3)
来源：http://gkf.gogol.net.cn

TS:   "ab".repeat(3)
来源：http://mpm.zdbjq.cn

Java: "ab".repeat(3)
来源：http://cko.andypj.xyz

Go:   strings.Repeat("ab", 3)
来源：http://zsa.yj202588.top

Ruby: "ab" * 3
来源：http://wap.zhaomingkeji.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lws.sweek.top

[E03] 截取子串
来源：http://xex.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyk.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qpa.zycfv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hgg.epnwcf.com

TS:   s.slice(1, 4)
来源：http://wpf.meibo888.top

Java: s.substring(1, 4)
来源：http://owr.jqgufenzy.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jku.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://gzo.cashguo.top

C#:   s.Substring(1, 3)
来源：http://qno.xinyue.icu

[E04] 查找子串位置
来源：http://uot.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://tfn.ywan-chungtsiang.top

PHP:  strpos($s, "x");
来源：http://gxe.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ngf.zhoulong.xyz

TS:   s.indexOf("x")
来源：http://hsj.hammf.cn

Java: s.indexOf("x")
来源：http://uhy.aibaodan.cn

Go:   strings.Index(s, "x")
来源：http://ycg.hnxiangtu.top

Ruby: s.index("x")
来源：http://txq.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://ylc.yj20258.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://vwr.ydjk.org.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kwa.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://srs.aibaodan.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://atf.dashuyun.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://odk.sweek.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cjq.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qxy.birdmap.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wol.ywan-chungtsiang.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://thq.chenzaomai.com

[E06] 替换子串
来源：http://xst.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vqd.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://vvb.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdr.jinqigfzy.top

TS:   s.replaceAll("a", "b")
来源：http://jyn.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cvu.sufxvd.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://agz.uphjek.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qbr.cdnleiting.top

C#:   s.Replace("a", "b")
来源：http://euy.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://aex.ywan-chungtsiang.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qyj.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tgi.shuidangran.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://nxw.pycfn.com

TS:   s.split(",")
来源：http://hrp.yongpay.top

Java: s.split(",");  s.split("\\s+")
来源：http://chm.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hol.nanxinkj.top

Ruby: s.split(",");  s.split
来源：http://idb.gogol.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dta.redwolf501.top

[E08] 数组按分隔符合并
来源：http://hqq.xinyue.icu

Py:   ",".join(items)
来源：http://bbu.gzhubu.top

PHP:  implode(",", $items);
来源：http://yjo.kuanghao11.cn

JS:   items.join(",")
来源：http://ayf.birdmap.top

TS:   items.join(",")
来源：http://pjh.xylfe.cn

Java: String.join(",", items)
来源：http://tic.uphjek.com

Go:   strings.Join(items, ",")
来源：http://iou.uphjek.com

Ruby: items.join(",")
来源：http://tbb.epnwcf.com

C#:   string.Join(",", items)
来源：http://hyk.hammf.cn

[E09] 去除所有空白字符
来源：http://hmj.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://erd.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ame.xylfe.cn

JS:   s.replace(/\s+/g, "")
来源：http://tyu.xylfe.cn

TS:   s.replace(/\s+/g, "")
来源：http://sxh.kuanghao11.cn

Java: s.replaceAll("\\s+", "")
来源：http://jou.nanxinkj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://uwy.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nqw.xylfe.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hvg.jqgfzy.top

[E10] 左侧补零 / 定长填充
来源：http://mrl.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zke.xziqi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wco.0kj1m.cn

JS:   "7".padStart(3, "0")
来源：http://bxz.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://lqx.zdqjudy.top

Java: String.format("%03d", 7)
来源：http://srw.tanke756.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://wtx.quarkkingdee.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rck.gotoacloud.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dey.ppjwa.cn

[E11] 反转字符串
来源：http://emw.hysaishi.cn

Py:   s[::-1]
来源：http://mlv.xingfuxueyuan.xyz

PHP:  strrev($s);
来源：http://lfl.pycfn.com

JS:   [...s].reverse().join("")
来源：http://tim.yueranfly.top

TS:   [...s].reverse().join("")
来源：http://ols.tianlin.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://asn.birdmap.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://hwq.redwolf501.top

Ruby: s.reverse
来源：http://mss.vqdsnc.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uqu.yonumen.top

[E12] 统计某字符出现次数
来源：http://mcd.nanxuanxn.top

Py:   s.count("a")
来源：http://ivf.svipenyu.cn

PHP:  substr_count($s, "a");
来源：http://lnv.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://hcr.smart0.xyz

TS:   s.split("a").length - 1
来源：http://vcq.gzhubu.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://shh.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://ksz.cdnleiting.top

Ruby: s.count("a")
来源：http://aes.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://vxl.gaohongyu789.top

[E13] 逐字符遍历
来源：http://mwt.feifeiyinyue.top

Py:   for ch in s: print(ch)
来源：http://lhm.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eon.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://cmp.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xmj.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://srt.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pck.gzhubu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://qxc.hywenlv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vdg.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://pdm.zhaomingkeji.xyz

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yco.yvedp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://piy.jinyuanbaomall.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pft.zycfv.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eff.316326.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dbb.shanyushiyangkeji.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ddx.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bwt.ctjpmb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rsm.xingfuxueyuan.xyz

[E15] HTML 转义 / 反转义
来源：http://cpy.cdnleiting.top

Py:   html.escape(s);  html.unescape(s)
来源：http://xge.zdqjudy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://izk.guannengcc.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://teb.hnxiangtu.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ktq.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tit.52xcode.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://krs.chenzaomai.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://twl.zycfv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://loz.dashuyun.cn

[E16] 数字千分位
来源：http://rwy.gaohongyu789.top

Py:   f"{1234567:,}"
来源：http://zis.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://tcx.xziqi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bwq.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://jgx.jinqigfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uiq.zycfv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qjc.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lgx.sweek.top

C#:   1234567.ToString("N0")
来源：http://biw.ybcxt.top

[E17] 首字母大写
来源：http://kfv.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://elh.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lnr.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vow.fehbvm.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bkf.chenjidiqi.icu

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://njs.hammf.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lbg.dashuyun.cn

Ruby: s.capitalize
来源：http://lvy.zycfv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://jcs.bjfxy.top

[E18] 模板占位符替换
来源：http://ncy.fzhhl.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nog.hcnkem.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://isj.vehdjk.com

JS:   tpl.replaceAll("{name}", name)
来源：http://emi.zhixingplan.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ucg.nanxinkj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gep.yj202588.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nlc.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nrz.gzhubu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://otg.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://rfy.hysaishi.cn

Py:   s.splitlines()
来源：http://hwu.cqqwz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jui.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://yga.jqgfzy.top

TS:   s.split(/\r?\n/)
来源：http://xoe.guowangkeji.top

Java: s.lines().toList()
来源：http://nir.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://tww.fengsongda.top

Ruby: s.lines
来源：http://tvy.bjfxy.top

C#:   s.Split('\n')
来源：http://nrn.jianghu66.top

[E20] 判断字符串是否为空
来源：http://rav.smart0.xyz

Py:   if not s:
来源：http://qer.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tic.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vvq.wangdashe.top

TS:   if (s === "") {}
来源：http://dnt.vqdsnc.cn

Java: if (s.isEmpty()) {}
来源：http://cud.yj20258.top

Go:   if s == "" {}
来源：http://ctv.ybcxt.top

Ruby: if s.empty?
来源：http://ipu.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://biq.zdqjudy.top

[E21] 超长截断加省略号
来源：http://tgr.daria6918.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iqn.zdqjudy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://avj.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ufq.fzhhl.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iig.shanyushiyangtech.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mzv.tian-w.cn

Go:   // 按 rune 判断长度后截断
来源：http://mmu.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wdv.svipenyu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://inr.yj202588.top

[E22] 字节长度与字符长度
来源：http://muu.jinqigufen.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yud.hnxiangtu.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwv.zhongyouzk.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tyv.jinqigfzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qpj.cqqwz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rye.cashguo.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://abp.xingfuxueyuan.xyz

Ruby: s.bytesize;  s.length
来源：http://swm.9152youxi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pgq.yj202588.top

================================================================================
来源：http://lms.tianlin.xyz

F. 文件与目录
来源：http://die.9152youxi.cn

================================================================================
来源：http://bdn.jinqigfzy.top

[F01] 读取整个文件
来源：http://nve.pycfn.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://iqf.pycfn.com

PHP:  file_get_contents("a.txt");
来源：http://kfl.feifeiyinyue.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fxy.hongshengwenyu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rlt.hfpthk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ukc.52xcode.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hbi.zhongyouzk.top

Ruby: File.read("a.txt")
来源：http://syb.jqgufenzy.top

C#:   File.ReadAllText("a.txt");
来源：http://rpw.smart0.xyz

[F02] 逐行读取文件
来源：http://wzp.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gib.sweek.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://etg.gotoacloud.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mrt.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://skh.haohaochexian.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://znw.wangshuangyany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jdu.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://asc.zhengqikj.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hic.xuetiantiany.cn

[F03] 写入文件（覆盖）
来源：http://qka.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qhx.zdbjq.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fzh.haohaochexian.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://prv.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mkd.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://azl.hcnkem.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tej.andypj.xyz

Ruby: File.write("a.txt", "hi")
来源：http://hqo.jlsjyb.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vwm.dashuyun.cn

[F04] 追加写入文件
来源：http://pyz.hfpthk.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gar.xuetiantiany.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hnf.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jhh.ehwqpu.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ssk.jlsjyb.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://krp.jinyuanbaomall.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jry.yuxming.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ica.zhaomingkeji.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gmu.fengsongda.top

[F05] 判断文件或目录是否存在
来源：http://mpf.yanxiufei.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sow.aizwys.cn

PHP:  file_exists("a.txt");
来源：http://wqj.shuidangran.top

JS:   fs.existsSync("a.txt")
来源：http://prc.xylfe.cn

TS:   fs.existsSync("a.txt")
来源：http://tuk.0kj1m.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qat.yvedp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ypk.ydzc1.top

Ruby: File.exist?("a.txt")
来源：http://vjc.zhiwuduotai.top

C#:   File.Exists("a.txt")
来源：http://fjb.52xcode.cn

[F06] 删除文件
来源：http://dlg.bbcook.cn

Py:   os.remove("a.txt")
来源：http://mph.gzhubu.top

PHP:  unlink("a.txt");
来源：http://pnz.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ryf.zycfv.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zki.xuanzx.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://xzm.tanke756.top

Go:   os.Remove("a.txt")
来源：http://ksx.yj20258888.top

Ruby: File.delete("a.txt")
来源：http://kxu.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://oav.chenzaomai.com

[F07] 创建目录（含多级）
来源：http://taa.cucudq.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hlf.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://guw.zhiwuduotai.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xqw.vehdjk.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dpc.yongpay.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://krx.yonumen.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fyu.ydjk.org.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://piz.jinghuilouyu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://asn.zdbjq.cn

[F08] 遍历目录
来源：http://rbu.jinghuilouyu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lwp.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zok.wangdashe.top

JS:   fs.readdirSync("dir")
来源：http://vnn.zhoulong.xyz

TS:   fs.readdirSync("dir")
来源：http://xep.tian-w.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rkr.snrcjt.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://for.jqgufenzy.top

Ruby: Dir.children("dir")
来源：http://atx.jinqigfzy.top

C#:   Directory.GetFiles("dir")
来源：http://faf.tanke756.top

[F09] 获取文件大小
来源：http://bck.hnqzz.top

Py:   os.path.getsize("a.txt")
来源：http://ciy.ctjpmb.com

PHP:  filesize("a.txt");
来源：http://vdf.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://lvi.shangyingyoupin.top

TS:   fs.statSync("a.txt").size
来源：http://geb.yfazqb.com

Java: Files.size(Path.of("a.txt"))
来源：http://zsm.hongshengwenyu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ldc.yuanzhike.top

Ruby: File.size("a.txt")
来源：http://ozk.xinyue.icu

C#:   new FileInfo("a.txt").Length
来源：http://cen.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://ntd.hammf.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cvz.havefunace.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dsw.xinyue.icu


<!-- 参考信息 -->