代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gdi.yueranfly.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://chl.chenzaomai.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://icm.gotoacloud.top

[D26] 数组转字符串
来源：http://hsq.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://kgl.gaohongyu789.top

PHP:  implode(", ", $arr);
来源：http://lsm.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://awv.jlsjyb.cn

TS:   arr.join(", ")
来源：http://dmg.zdbjq.cn

Java: String.join(", ", list)
来源：http://hkq.shzxlz.cn

Go:   strings.Join(strs, ", ")
来源：http://wvz.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://mvt.dashuyun.cn

C#:   string.Join(", ", list)
来源：http://psl.nwbrower.top

================================================================================
来源：http://onw.feifeiyinyue.top

E. 字符串处理
来源：http://wlr.ivvv.top

================================================================================
来源：http://gcy.hfpthk.cn

[E01] 拼接字符串
来源：http://imb.shangyingyoupin.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mii.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rcn.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kaj.xuetiantiany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ctl.kuanghao11.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://peo.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ibk.9152youxi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jnq.yonumen.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://juj.daria6918.cn

[E02] 重复字符串
来源：http://lkp.snrcjt.cn

Py:   "ab" * 3
来源：http://ied.xziqi.cn

PHP:  str_repeat("ab", 3);
来源：http://bwa.haohaochexian.top

JS:   "ab".repeat(3)
来源：http://uxx.yj20258.top

TS:   "ab".repeat(3)
来源：http://nph.jinghuilouyu.cn

Java: "ab".repeat(3)
来源：http://ibl.cdnleiting.top

Go:   strings.Repeat("ab", 3)
来源：http://iva.daria6918.cn

Ruby: "ab" * 3
来源：http://fdj.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ess.wangshuangyany.cn

[E03] 截取子串
来源：http://vmu.9152youxi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gxw.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yso.nanxuanxn.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lvf.snrcjt.cn

TS:   s.slice(1, 4)
来源：http://emm.cashguo.top

Java: s.substring(1, 4)
来源：http://kat.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rbr.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mfd.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://zpx.daxiang520.top

[E04] 查找子串位置
来源：http://ctr.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://wzz.vehdjk.com

PHP:  strpos($s, "x");
来源：http://ofd.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fvw.xuanzx.com

TS:   s.indexOf("x")
来源：http://rbz.aibaodan.cn

Java: s.indexOf("x")
来源：http://fmp.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://jxd.hammf.cn

Ruby: s.index("x")
来源：http://mcv.smart0.xyz

C#:   s.IndexOf("x")
来源：http://qqd.hfpthk.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pge.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cvz.zdqjudy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sou.yj202588.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zwu.cqqwz.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://for.nwbrower.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qon.ppjwa.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://rvd.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qtg.sysykeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uah.hywenlv.cn

[E06] 替换子串
来源：http://nae.tian-w.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lpk.hcnkem.com

PHP:  str_replace("a", "b", $s);
来源：http://dzy.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hrq.svipenyu.cn

TS:   s.replaceAll("a", "b")
来源：http://cpj.yj20258888.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tqa.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://byx.fehbvm.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ffl.ehwqpu.com

C#:   s.Replace("a", "b")
来源：http://ggz.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://jfw.zdbjq.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qvt.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zji.ehwqpu.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://lpm.vehdjk.com

TS:   s.split(",")
来源：http://txk.chenzaomai.com

Java: s.split(",");  s.split("\\s+")
来源：http://yfn.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rny.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://aon.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mrt.hammf.cn

[E08] 数组按分隔符合并
来源：http://agb.ctjpmb.com

Py:   ",".join(items)
来源：http://mbv.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://lfz.hnxiangtu.top

JS:   items.join(",")
来源：http://sfs.quarkkingdee.top

TS:   items.join(",")
来源：http://xju.sjlbkw.cn

Java: String.join(",", items)
来源：http://vrg.jiagoushi.top

Go:   strings.Join(items, ",")
来源：http://rwk.hcnkem.com

Ruby: items.join(",")
来源：http://mvc.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://ziw.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://jgh.yuanzhike.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zog.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wue.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://ldd.yuxming.cn

TS:   s.replace(/\s+/g, "")
来源：http://ufv.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://emh.zhongyouzk.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://piy.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://djq.yvedp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ebw.ydzc1.top

[E10] 左侧补零 / 定长填充
来源：http://jbr.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nwg.hammf.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yfl.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://tuy.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://zwd.jinqigufen.top

Java: String.format("%03d", 7)
来源：http://rvw.shzxlz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ydl.cqqwz.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://umo.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bmn.hfpthk.cn

[E11] 反转字符串
来源：http://cdw.feifeiyinyue.top

Py:   s[::-1]
来源：http://xga.fzhhl.top

PHP:  strrev($s);
来源：http://jjz.jqgfzy.top

JS:   [...s].reverse().join("")
来源：http://enx.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://hzt.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://koe.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://nve.yj20258888.top

Ruby: s.reverse
来源：http://dln.cqqwz.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ary.zycfv.cn

[E12] 统计某字符出现次数
来源：http://cdh.svipenyu.cn

Py:   s.count("a")
来源：http://sfa.birdmap.top

PHP:  substr_count($s, "a");
来源：http://gww.cucudq.cn

JS:   s.split("a").length - 1
来源：http://jsc.hfpthk.cn

TS:   s.split("a").length - 1
来源：http://evw.yuxming.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jrn.xziqi.cn

Go:   strings.Count(s, "a")
来源：http://tij.snrcjt.cn

Ruby: s.count("a")
来源：http://mjx.zdqjudy.top

C#:   s.Count(c => c == 'a')
来源：http://zrb.ywan-chungtsiang.top

[E13] 逐字符遍历
来源：http://dxx.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://azy.pengpengdd.cyou

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://uqp.yuxming.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kjj.tanke756.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://npj.aibaodan.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://edy.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pul.vehdjk.com

Ruby: s.each_char { |ch| puts ch }
来源：http://gky.xuanzx.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bxy.xinyue.icu

[E14] URL 编码与 Base64
来源：http://dbq.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xtf.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://psl.yangfankeji.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tra.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wpb.jqgfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://deh.yj202588.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xga.yj20258888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wmw.zhongyouzk.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fxm.zhaomingkeji.xyz

[E15] HTML 转义 / 反转义
来源：http://kmp.ydzc1.top

Py:   html.escape(s);  html.unescape(s)
来源：http://fea.iojbl.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xeb.ybcxt.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hjq.pengpengdd.cyou

TS:   // 同上，务必做 XSS 过滤
来源：http://ytd.zhijiandao.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ukp.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gev.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mvp.yuxming.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yjy.chenzaomai.com

[E16] 数字千分位
来源：http://gpk.nanxinkj.top

Py:   f"{1234567:,}"
来源：http://pdt.xingfuxueyuan.xyz

PHP:  number_format(1234567);
来源：http://cfo.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://kke.cucudq.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://put.svipenyu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hrg.hesvh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wlq.ydzc1.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://iap.hysaishi.cn

C#:   1234567.ToString("N0")
来源：http://zmw.9152youxi.cn

[E17] 首字母大写
来源：http://eam.zhengqikj.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://djd.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sbd.ydzc1.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zoe.yonumen.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fjs.yueranfly.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gcs.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qfi.ydjk.org.cn

Ruby: s.capitalize
来源：http://mab.sweek.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fhb.jqgfzy.top

[E18] 模板占位符替换
来源：http://oqu.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ore.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aiq.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gzc.daxiang520.top

TS:   tpl.replaceAll("{name}", name)
来源：http://hfd.shanyushiyangtech.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vpj.ydjk.org.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tiz.jqgfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qcr.kuanghao11.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bmc.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://nso.sjlbkw.cn

Py:   s.splitlines()
来源：http://dlf.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nau.ydzc1.top

JS:   s.split(/\r?\n/)
来源：http://how.yj20258.top

TS:   s.split(/\r?\n/)
来源：http://ivj.snrcjt.cn

Java: s.lines().toList()
来源：http://wbk.zdbjq.cn

Go:   strings.Split(s, "\n")
来源：http://mct.ydzc1.top

Ruby: s.lines
来源：http://jpa.daxiang520.top

C#:   s.Split('\n')
来源：http://alv.gotoacloud.top

[E20] 判断字符串是否为空
来源：http://biq.snrcjt.cn

Py:   if not s:
来源：http://zbx.birdmap.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mld.cheryme.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hkb.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://jvq.jinyuanbaomall.cn

Java: if (s.isEmpty()) {}
来源：http://ljn.hysaishi.cn

Go:   if s == "" {}
来源：http://rdn.aibaodan.cn

Ruby: if s.empty?
来源：http://sdk.svipenyu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rnl.havefunace.top

[E21] 超长截断加省略号
来源：http://myt.chenzaomai.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://syx.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ipq.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ann.guowangkeji.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hlj.nanxinkj.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yop.guowangkeji.top

Go:   // 按 rune 判断长度后截断
来源：http://ajk.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hoc.uphjek.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bew.xingfuxueyuan.xyz

[E22] 字节长度与字符长度
来源：http://ibd.daxiang520.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://iyx.bjfxy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmc.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://bwn.tanke756.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://znp.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fff.jqgfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tvy.fengsongda.top

Ruby: s.bytesize;  s.length
来源：http://hrk.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hxx.hammf.cn

================================================================================
来源：http://otd.dashuyun.cn

F. 文件与目录
来源：http://cbu.hongshengwenyu.top

================================================================================
来源：http://his.yfazqb.com

[F01] 读取整个文件
来源：http://cap.shanyushiyangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://awa.shanyushiyangtech.top

PHP:  file_get_contents("a.txt");
来源：http://lof.guannengcc.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xfx.cucudq.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xst.sxryk.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xvx.ydzc1.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gee.fengsongda.top

Ruby: File.read("a.txt")
来源：http://uwo.bjfxy.top

C#:   File.ReadAllText("a.txt");
来源：http://dzs.zhixingplan.top

[F02] 逐行读取文件
来源：http://qev.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bcv.zhongyouzk.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dlp.sufxvd.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://imo.cdnleiting.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jwo.vqdsnc.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://akb.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xbc.meibo888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lmt.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xoq.hcnkem.com

[F03] 写入文件（覆盖）
来源：http://nus.zhiwuduotai.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nsm.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://dor.birdmap.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ust.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xcz.nanxinkj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://kyy.jyoumei.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bqy.yvedp.cn

Ruby: File.write("a.txt", "hi")
来源：http://qxq.jinyuanbaomall.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rcm.vqdsnc.cn

[F04] 追加写入文件
来源：http://glt.c1oappe.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ehd.shanyushiyangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uxy.zhoulong.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lqi.fanxiaobao.xyz

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vpr.hnqzz.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qin.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mkv.tanke756.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nek.guannengcc.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xxz.gogol.net.cn

[F05] 判断文件或目录是否存在
来源：http://zlf.316326.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fih.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://wik.mhx1999.top

JS:   fs.existsSync("a.txt")
来源：http://wej.9152youxi.cn

TS:   fs.existsSync("a.txt")
来源：http://oll.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://oky.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hke.xziqi.cn

Ruby: File.exist?("a.txt")
来源：http://vpk.svipenyu.cn

C#:   File.Exists("a.txt")
来源：http://bst.epnwcf.com

[F06] 删除文件
来源：http://fap.zdbjq.cn

Py:   os.remove("a.txt")
来源：http://lyi.chenjidiqi.icu

PHP:  unlink("a.txt");
来源：http://kyw.zycfv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zdw.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://poj.bjfxy.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bik.52xcode.cn

Go:   os.Remove("a.txt")
来源：http://gkm.hongshengwenyu.top

Ruby: File.delete("a.txt")
来源：http://mlz.zhixingplan.top

C#:   File.Delete("a.txt");
来源：http://omt.tianlin.xyz

[F07] 创建目录（含多级）
来源：http://uvz.ivvv.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://awu.chenzaomai.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vfm.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mhj.tianlin.xyz

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ybg.yonumen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://irv.daria6918.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ljx.quarkkingdee.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dmz.havefunace.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ytk.chenzaomai.com

[F08] 遍历目录
来源：http://wft.shanyushiyangtech.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://wnk.sysykeji.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://smx.fanxiaobao.xyz

JS:   fs.readdirSync("dir")
来源：http://ogw.tianlin.xyz

TS:   fs.readdirSync("dir")
来源：http://vsk.hnxiangtu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cww.dashuyun.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rnx.cqqwz.cn

Ruby: Dir.children("dir")
来源：http://deu.daria6918.cn

C#:   Directory.GetFiles("dir")
来源：http://xjn.cdnleiting.top

[F09] 获取文件大小
来源：http://fiw.dianchejie.cn

Py:   os.path.getsize("a.txt")
来源：http://pus.yvedp.cn

PHP:  filesize("a.txt");
来源：http://kmy.fehbvm.com

JS:   fs.statSync("a.txt").size
来源：http://znr.hysaishi.cn

TS:   fs.statSync("a.txt").size
来源：http://icn.shangyingyoupin.top

Java: Files.size(Path.of("a.txt"))
来源：http://csm.jinyuanbaomall.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ncy.hnqzz.top

Ruby: File.size("a.txt")
来源：http://tsm.guowangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://jem.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://het.yuanzhike.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ewi.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qys.sjlbkw.cn


<!-- 参考信息 -->