代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kne.snrcjt.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pml.ybcxt.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hdb.fzhhl.top

[D26] 数组转字符串
来源：http://ogj.shuidangran.top

Py:   ", ".join(map(str, arr))
来源：http://zje.meibo888.top

PHP:  implode(", ", $arr);
来源：http://mmx.nanxinkj.top

JS:   arr.join(", ")
来源：http://glo.9152youxi.cn

TS:   arr.join(", ")
来源：http://evi.xuanzx.com

Java: String.join(", ", list)
来源：http://yec.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://ycw.sxryk.cn

Ruby: arr.join(", ")
来源：http://kha.52xcode.cn

C#:   string.Join(", ", list)
来源：http://ffb.shuidangran.top

================================================================================
来源：http://ojj.ivvv.top

E. 字符串处理
来源：http://azy.yvedp.cn

================================================================================
来源：http://cjr.sweek.top

[E01] 拼接字符串
来源：http://ojq.hywenlv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pvb.hfpthk.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xkv.shanyushiyangtech.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ehc.cashguo.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://shx.vqdsnc.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vbd.smart0.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hqb.chenjidiqi.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://plw.chenzaomai.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lje.yj202588.top

[E02] 重复字符串
来源：http://gan.jinqigfzy.top

Py:   "ab" * 3
来源：http://uxj.aizwys.cn

PHP:  str_repeat("ab", 3);
来源：http://gff.cashguo.top

JS:   "ab".repeat(3)
来源：http://omf.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://ubb.jinyuanbaomall.cn

Java: "ab".repeat(3)
来源：http://djb.9152youxi.cn

Go:   strings.Repeat("ab", 3)
来源：http://yzc.andypj.xyz

Ruby: "ab" * 3
来源：http://ufz.cdnleiting.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rou.ydjk.org.cn

[E03] 截取子串
来源：http://mwu.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://miy.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kwp.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uno.yfazqb.com

TS:   s.slice(1, 4)
来源：http://ute.c1oappe.top

Java: s.substring(1, 4)
来源：http://uto.yangfankeji.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zdq.ydzc1.top

Ruby: s[1, 3];  s[1..3]
来源：http://zym.hesvh.cn

C#:   s.Substring(1, 3)
来源：http://bhe.yongpay.top

[E04] 查找子串位置
来源：http://drv.meibo888.top

Py:   s.find("x");  s.index("x")
来源：http://yvo.52xcode.cn

PHP:  strpos($s, "x");
来源：http://uys.sufxvd.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qai.dashuyun.cn

TS:   s.indexOf("x")
来源：http://yso.yangfankeji.com

Java: s.indexOf("x")
来源：http://bbf.cqqwz.cn

Go:   strings.Index(s, "x")
来源：http://eva.fehbvm.com

Ruby: s.index("x")
来源：http://bwl.shanyushiyangtech.top

C#:   s.IndexOf("x")
来源：http://nkr.zhengqikj.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qrq.yanxiufei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vnz.cqqwz.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ape.jqgufenzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vbg.wangdashe.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://orc.dianchejie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ltd.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tss.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kmu.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ubh.tian-w.cn

[E06] 替换子串
来源：http://vil.fktsv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://axc.yfazqb.com

PHP:  str_replace("a", "b", $s);
来源：http://kze.havefunace.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yuv.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://fcn.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yka.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uoi.redwolf501.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vpq.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://bny.yj202588.top

[E07] 按分隔符拆分
来源：http://clu.snrcjt.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bky.vehdjk.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tri.sufxvd.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://piq.hammf.cn

TS:   s.split(",")
来源：http://dnl.ybcxt.top

Java: s.split(",");  s.split("\\s+")
来源：http://eaz.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xxn.xziqi.cn

Ruby: s.split(",");  s.split
来源：http://lgl.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ynj.smart0.xyz

[E08] 数组按分隔符合并
来源：http://bsq.yanxiufei.cn

Py:   ",".join(items)
来源：http://jdd.hcnkem.com

PHP:  implode(",", $items);
来源：http://wgb.ydjk.org.cn

JS:   items.join(",")
来源：http://qln.hywenlv.cn

TS:   items.join(",")
来源：http://ptz.zhaomingkeji.xyz

Java: String.join(",", items)
来源：http://ypu.haohaochexian.top

Go:   strings.Join(items, ",")
来源：http://jns.hysaishi.cn

Ruby: items.join(",")
来源：http://rcu.tanke756.top

C#:   string.Join(",", items)
来源：http://ewx.zycfv.cn

[E09] 去除所有空白字符
来源：http://afu.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qks.wangshuangyany.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wij.zhaomingkeji.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ual.hnqzz.top

TS:   s.replace(/\s+/g, "")
来源：http://wxm.shzxlz.cn

Java: s.replaceAll("\\s+", "")
来源：http://emw.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ate.cheryme.top

Ruby: s.gsub(/\s+/, "")
来源：http://hgq.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fip.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://vwz.aizwys.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ugs.jinghuilouyu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aaf.cashguo.top

JS:   "7".padStart(3, "0")
来源：http://ewk.sjlbkw.cn

TS:   "7".padStart(3, "0")
来源：http://ilp.guannengcc.top

Java: String.format("%03d", 7)
来源：http://tyh.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://prs.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://htj.jinghuilouyu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://del.redwolf501.top

[E11] 反转字符串
来源：http://isf.nwbrower.top

Py:   s[::-1]
来源：http://pus.ctjpmb.com

PHP:  strrev($s);
来源：http://bkm.smart0.xyz

JS:   [...s].reverse().join("")
来源：http://skx.shanyushiyangkeji.top

TS:   [...s].reverse().join("")
来源：http://hcb.jinqigfzy.top

Java: new StringBuilder(s).reverse().toString()
来源：http://flg.gogol.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lzf.zhaomingkeji.xyz

Ruby: s.reverse
来源：http://vlf.gogol.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mgk.meibo888.top

[E12] 统计某字符出现次数
来源：http://quo.ehwqpu.com

Py:   s.count("a")
来源：http://klx.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://dpl.xylfe.cn

JS:   s.split("a").length - 1
来源：http://cmx.cashguo.top

TS:   s.split("a").length - 1
来源：http://nzf.zhixingplan.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ber.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://szl.tanke756.top

Ruby: s.count("a")
来源：http://loo.hysaishi.cn

C#:   s.Count(c => c == 'a')
来源：http://csj.yongpay.top

[E13] 逐字符遍历
来源：http://gnw.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://obq.fengsongda.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cdy.zhaomingkeji.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://hqi.shanyushiyangkeji.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://wxj.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qrl.fktsv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pma.gogol.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gno.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ikr.pycfn.com

[E14] URL 编码与 Base64
来源：http://zwb.gaohongyu789.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bqa.yj20258.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://pmw.sxryk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yzb.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ngg.zhixingplan.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tbd.hcnkem.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dcw.cheryme.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mbj.sufxvd.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://top.zhoulong.xyz

[E15] HTML 转义 / 反转义
来源：http://zwf.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://tus.daria6918.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eja.xuanzx.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ype.ctjpmb.com

TS:   // 同上，务必做 XSS 过滤
来源：http://bnm.havefunace.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jce.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lea.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://upm.uphjek.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iap.zhongyouzk.top

[E16] 数字千分位
来源：http://ojb.zhongyouzk.top

Py:   f"{1234567:,}"
来源：http://zgw.guannengcc.top

PHP:  number_format(1234567);
来源：http://uqq.jinghuilouyu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dvn.yangfankeji.com

TS:   (1234567).toLocaleString("en-US")
来源：http://scm.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bmo.nanxuanxn.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wog.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uir.tanke756.top

C#:   1234567.ToString("N0")
来源：http://lue.uphjek.com

[E17] 首字母大写
来源：http://bhk.jinghuilouyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tge.hnxiangtu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lky.yj202588.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gny.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://enc.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://smc.haohaochexian.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xeh.zhengqikj.top

Ruby: s.capitalize
来源：http://qqb.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://prd.sxryk.cn

[E18] 模板占位符替换
来源：http://pcx.ehwqpu.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://igt.gogol.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xmt.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://hfs.jinyuanbaomall.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pdy.ivvv.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hzc.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cnw.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gkx.hongshengwenyu.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://elm.jianghu66.top

[E19] 多行文本按行拆分
来源：http://dgh.ppjwa.cn

Py:   s.splitlines()
来源：http://usx.uphjek.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cin.zhiwuduotai.top

JS:   s.split(/\r?\n/)
来源：http://vou.9152youxi.cn

TS:   s.split(/\r?\n/)
来源：http://vdm.ydjk.org.cn

Java: s.lines().toList()
来源：http://feq.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://btr.hnqzz.top

Ruby: s.lines
来源：http://gsr.ctjpmb.com

C#:   s.Split('\n')
来源：http://jeh.tanke756.top

[E20] 判断字符串是否为空
来源：http://ftw.vqdsnc.cn

Py:   if not s:
来源：http://ixf.uphjek.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hmp.redwolf501.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lnr.quarkkingdee.top

TS:   if (s === "") {}
来源：http://biw.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://dyf.yfazqb.com

Go:   if s == "" {}
来源：http://iav.guowangkeji.top

Ruby: if s.empty?
来源：http://vav.jyoumei.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://enp.epnwcf.com

[E21] 超长截断加省略号
来源：http://ppw.fengsongda.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wyg.zhoulong.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ewe.hcnkem.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://osj.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lfn.guowangkeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zqj.gogol.net.cn

Go:   // 按 rune 判断长度后截断
来源：http://pmk.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lwe.cqqwz.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jix.sysykeji.top

[E22] 字节长度与字符长度
来源：http://ths.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ggg.shuidangran.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sxi.vehdjk.com

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://crs.ppjwa.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nif.zhoulong.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eox.ctjpmb.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://juz.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://mcc.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gwa.wangdashe.top

================================================================================
来源：http://tou.dianchejie.cn

F. 文件与目录
来源：http://zvv.dianchejie.cn

================================================================================
来源：http://oof.quarkkingdee.top

[F01] 读取整个文件
来源：http://rtk.tian-w.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gyv.yfazqb.com

PHP:  file_get_contents("a.txt");
来源：http://fnk.cucudq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gqb.zhengqikj.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://juh.xylfe.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jon.birdmap.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yyg.ybcxt.top

Ruby: File.read("a.txt")
来源：http://opu.hysaishi.cn

C#:   File.ReadAllText("a.txt");
来源：http://fwh.daria6918.cn

[F02] 逐行读取文件
来源：http://rxb.zhongyouzk.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gep.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qzw.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pag.hfpthk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ekh.shanyushiyangtech.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uwi.jianghu66.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zzn.wangshuangyany.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lhj.gotoacloud.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ryo.shuidangran.top

[F03] 写入文件（覆盖）
来源：http://hny.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ene.jlsjyb.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ulh.hcnkem.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qmj.jinqigufen.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zjc.yueranfly.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tdh.meibo888.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jsi.jlsjyb.cn

Ruby: File.write("a.txt", "hi")
来源：http://fql.uphjek.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rkb.shanyushiyangkeji.top

[F04] 追加写入文件
来源：http://cka.jianghu66.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sjg.ydzc1.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pbg.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ljs.yonumen.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kpf.pengpengdd.cyou

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pkq.shangyingyoupin.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://osc.fktsv.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yud.c1oappe.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hwb.ctjpmb.com

[F05] 判断文件或目录是否存在
来源：http://hzj.xingfuxueyuan.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jos.52xcode.cn

PHP:  file_exists("a.txt");
来源：http://pym.jqgfzy.top

JS:   fs.existsSync("a.txt")
来源：http://nnn.andypj.xyz

TS:   fs.existsSync("a.txt")
来源：http://wtt.shanyushiyangtech.top

Java: Files.exists(Path.of("a.txt"))
来源：http://juh.iojbl.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yzz.yanxiufei.cn

Ruby: File.exist?("a.txt")
来源：http://vnm.chenjidiqi.icu

C#:   File.Exists("a.txt")
来源：http://vya.zhoulong.xyz

[F06] 删除文件
来源：http://bjo.hcnkem.com

Py:   os.remove("a.txt")
来源：http://mow.cqqwz.cn

PHP:  unlink("a.txt");
来源：http://gzs.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://isd.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ogw.quarkkingdee.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eec.hammf.cn

Go:   os.Remove("a.txt")
来源：http://vee.fktsv.cn

Ruby: File.delete("a.txt")
来源：http://ozr.cdnleiting.top

C#:   File.Delete("a.txt");
来源：http://hoe.kuanghao11.cn

[F07] 创建目录（含多级）
来源：http://bbq.zhixingplan.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ujz.jinqigfzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fnl.zycfv.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gbr.0kj1m.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xhy.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zsz.yongpay.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://okm.zycfv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://okm.zdbjq.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://grt.sysykeji.top

[F08] 遍历目录
来源：http://wht.jiagoushi.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mte.zhixingplan.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eya.yuanzhike.top

JS:   fs.readdirSync("dir")
来源：http://bac.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://rqg.yongpay.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://csr.vqdsnc.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yms.nwbrower.top

Ruby: Dir.children("dir")
来源：http://uqj.wangdashe.top

C#:   Directory.GetFiles("dir")
来源：http://xyw.yanxiufei.cn

[F09] 获取文件大小
来源：http://iiy.zhixingplan.top

Py:   os.path.getsize("a.txt")
来源：http://ymm.jqgufenzy.top

PHP:  filesize("a.txt");
来源：http://lqf.hnqzz.top

JS:   fs.statSync("a.txt").size
来源：http://pfl.xziqi.cn

TS:   fs.statSync("a.txt").size
来源：http://thc.ctjpmb.com

Java: Files.size(Path.of("a.txt"))
来源：http://gel.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ovr.xuanzx.com

Ruby: File.size("a.txt")
来源：http://orl.zdbjq.cn

C#:   new FileInfo("a.txt").Length
来源：http://taf.tanke756.top

[F10] 取文件扩展名 / 文件名
来源：http://fnl.0kj1m.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rjk.hywenlv.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bfq.hnxiangtu.top


<!-- 参考信息 -->