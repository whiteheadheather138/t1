代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://icu.birdmap.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rvk.fktsv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gqv.sxryk.cn

[D26] 数组转字符串
来源：http://xfe.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://rlp.fengsongda.top

PHP:  implode(", ", $arr);
来源：http://ghs.smart0.xyz

JS:   arr.join(", ")
来源：http://oum.yongpay.top

TS:   arr.join(", ")
来源：http://nti.hcnkem.com

Java: String.join(", ", list)
来源：http://yoy.pycfn.com

Go:   strings.Join(strs, ", ")
来源：http://bqi.xinyue.icu

Ruby: arr.join(", ")
来源：http://vov.nanxinkj.top

C#:   string.Join(", ", list)
来源：http://tbp.dianchejie.cn

================================================================================
来源：http://nxj.yvedp.cn

E. 字符串处理
来源：http://vsi.zhengqikj.top

================================================================================
来源：http://hre.jiagoushi.top

[E01] 拼接字符串
来源：http://puc.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://owu.sweek.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qpp.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://crd.hysaishi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gco.svipenyu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://kmd.shanyushiyangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kfb.jlsjyb.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://eec.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ltm.yvedp.cn

[E02] 重复字符串
来源：http://kmp.iojbl.cn

Py:   "ab" * 3
来源：http://kmm.ydzc1.top

PHP:  str_repeat("ab", 3);
来源：http://fgj.smart0.xyz

JS:   "ab".repeat(3)
来源：http://wow.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://wvv.yfazqb.com

Java: "ab".repeat(3)
来源：http://ato.xylfe.cn

Go:   strings.Repeat("ab", 3)
来源：http://adj.nwbrower.top

Ruby: "ab" * 3
来源：http://fba.52xcode.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rwz.jqgufenzy.top

[E03] 截取子串
来源：http://tpn.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pwi.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jve.kuanghao11.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dlu.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://yzh.cheryme.top

Java: s.substring(1, 4)
来源：http://efp.sjlbkw.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://izd.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lac.jinqigufen.top

C#:   s.Substring(1, 3)
来源：http://zlu.yuanzhike.top

[E04] 查找子串位置
来源：http://kxb.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://mzl.yfazqb.com

PHP:  strpos($s, "x");
来源：http://yux.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bte.ehwqpu.com

TS:   s.indexOf("x")
来源：http://ygw.yfazqb.com

Java: s.indexOf("x")
来源：http://qdt.jinqigufen.top

Go:   strings.Index(s, "x")
来源：http://gia.haohaochexian.top

Ruby: s.index("x")
来源：http://zsd.smart0.xyz

C#:   s.IndexOf("x")
来源：http://kef.redwolf501.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rbv.shuidangran.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wwp.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kuc.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kcy.gotoacloud.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://oha.0kj1m.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rug.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ydt.redwolf501.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zmw.316326.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://idn.jlsjyb.cn

[E06] 替换子串
来源：http://lhq.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wby.sysykeji.top

PHP:  str_replace("a", "b", $s);
来源：http://lrj.birdmap.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xzc.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://wud.wangshuangyany.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cdk.wangdashe.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sfr.sxryk.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://iox.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://mfk.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://uvr.yueranfly.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://eui.tanke756.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zwl.cheryme.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vfe.52xcode.cn

TS:   s.split(",")
来源：http://tad.yj202588.top

Java: s.split(",");  s.split("\\s+")
来源：http://hoq.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hkc.yonumen.top

Ruby: s.split(",");  s.split
来源：http://oea.daxiang520.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yqn.chenzaomai.com

[E08] 数组按分隔符合并
来源：http://osu.gzhubu.top

Py:   ",".join(items)
来源：http://kvv.tianlin.xyz

PHP:  implode(",", $items);
来源：http://jss.quarkkingdee.top

JS:   items.join(",")
来源：http://tju.jinqigfzy.top

TS:   items.join(",")
来源：http://ikj.shzxlz.cn

Java: String.join(",", items)
来源：http://dzp.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://iyk.tarul.cn

Ruby: items.join(",")
来源：http://qda.bjfxy.top

C#:   string.Join(",", items)
来源：http://gev.hfpthk.cn

[E09] 去除所有空白字符
来源：http://hsd.fanxiaobao.xyz

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tor.zdqjudy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vun.nanxinkj.top

JS:   s.replace(/\s+/g, "")
来源：http://dls.zhongyouzk.top

TS:   s.replace(/\s+/g, "")
来源：http://klo.bbcook.cn

Java: s.replaceAll("\\s+", "")
来源：http://csr.hysaishi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lpb.fzhhl.top

Ruby: s.gsub(/\s+/, "")
来源：http://ovb.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gmv.fehbvm.com

[E10] 左侧补零 / 定长填充
来源：http://klr.wangdashe.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qno.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://foj.snrcjt.cn

JS:   "7".padStart(3, "0")
来源：http://inv.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://tal.yanxiufei.cn

Java: String.format("%03d", 7)
来源：http://krm.zhijiandao.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pxi.yuxming.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rla.c1oappe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uyh.zhaomingkeji.xyz

[E11] 反转字符串
来源：http://knn.redwolf501.top

Py:   s[::-1]
来源：http://kgd.316326.xyz

PHP:  strrev($s);
来源：http://hig.yj202588.top

JS:   [...s].reverse().join("")
来源：http://ibd.hfpthk.cn

TS:   [...s].reverse().join("")
来源：http://ohv.chenlongwang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jfd.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qdi.dianchejie.cn

Ruby: s.reverse
来源：http://wnp.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://foc.zhoulong.xyz

[E12] 统计某字符出现次数
来源：http://xmq.c1oappe.top

Py:   s.count("a")
来源：http://rbo.nanxuanxn.top

PHP:  substr_count($s, "a");
来源：http://rxi.guannengcc.top

JS:   s.split("a").length - 1
来源：http://mwj.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://cpf.cucudq.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hna.tarul.cn

Go:   strings.Count(s, "a")
来源：http://cgv.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://ddt.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://gvu.iojbl.cn

[E13] 逐字符遍历
来源：http://yfr.hesvh.cn

Py:   for ch in s: print(ch)
来源：http://jwc.wangshuangyany.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://npr.yueranfly.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://dzv.uphjek.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://iqg.gzhubu.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://giv.fzhhl.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eos.tanke756.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bwi.cqqwz.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hza.sxryk.cn

[E14] URL 编码与 Base64
来源：http://bat.cdnleiting.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ddt.c1oappe.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ars.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dhy.zhijiandao.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kvb.shzxlz.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vfw.iojbl.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xpd.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nqa.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsd.xuetiantiany.cn

[E15] HTML 转义 / 反转义
来源：http://bmf.shangyingyoupin.top

Py:   html.escape(s);  html.unescape(s)
来源：http://vaq.jqgufenzy.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqf.vehdjk.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tee.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://los.ppjwa.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bmh.hfpthk.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjv.yangfankeji.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hxi.yfazqb.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vil.hnqzz.top

[E16] 数字千分位
来源：http://hjh.hammf.cn

Py:   f"{1234567:,}"
来源：http://vjt.fktsv.cn

PHP:  number_format(1234567);
来源：http://uuc.tian-w.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://flk.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://cpl.hnxiangtu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qbv.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pti.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qoe.xylfe.cn

C#:   1234567.ToString("N0")
来源：http://toz.dianchejie.cn

[E17] 首字母大写
来源：http://ccf.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://juu.bbcook.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uxb.cheryme.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xbk.quarkkingdee.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iym.jiagoushi.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tfe.xuanzx.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://alp.hongshengwenyu.top

Ruby: s.capitalize
来源：http://ppu.svipenyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wxs.wangdashe.top

[E18] 模板占位符替换
来源：http://qab.yangfankeji.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hay.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ixl.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://anh.tarul.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tgc.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nyz.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zmm.yuanzhike.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://plt.yueranfly.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uss.yvedp.cn

[E19] 多行文本按行拆分
来源：http://req.mhx1999.top

Py:   s.splitlines()
来源：http://arv.zhaomingkeji.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xvq.cheryme.top

JS:   s.split(/\r?\n/)
来源：http://whq.xinyue.icu

TS:   s.split(/\r?\n/)
来源：http://yfq.yj20258.top

Java: s.lines().toList()
来源：http://nul.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://mwi.fzhhl.top

Ruby: s.lines
来源：http://hvw.vehdjk.com

C#:   s.Split('\n')
来源：http://ggb.jinghuilouyu.cn

[E20] 判断字符串是否为空
来源：http://zvf.52xcode.cn

Py:   if not s:
来源：http://hyf.bjfxy.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mrx.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://owf.shzxlz.cn

TS:   if (s === "") {}
来源：http://apj.cheryme.top

Java: if (s.isEmpty()) {}
来源：http://cgn.haohaochexian.top

Go:   if s == "" {}
来源：http://hvb.316326.xyz

Ruby: if s.empty?
来源：http://oyz.ydjk.org.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bod.nwbrower.top

[E21] 超长截断加省略号
来源：http://qep.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://djn.zhengqikj.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jbu.dianchejie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yze.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rsp.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mcg.jinghuilouyu.cn

Go:   // 按 rune 判断长度后截断
来源：http://kzj.vqdsnc.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebq.xuanzx.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gpi.yongpay.top

[E22] 字节长度与字符长度
来源：http://tzr.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yhn.tianlin.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pha.zhengqikj.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tkg.shanyushiyangtech.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://pvu.pycfn.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vij.jinqigfzy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xfw.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://pkk.tanke756.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://npx.redwolf501.top

================================================================================
来源：http://ylh.aizwys.cn

F. 文件与目录
来源：http://kgr.fzhhl.top

================================================================================
来源：http://ozh.cqqwz.cn

[F01] 读取整个文件
来源：http://pze.ydjk.org.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nkt.zhiwuduotai.top

PHP:  file_get_contents("a.txt");
来源：http://ggd.zdbjq.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qdr.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cne.chenzaomai.com

Java: Files.readString(Path.of("a.txt"))
来源：http://kso.cashguo.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://idi.vehdjk.com

Ruby: File.read("a.txt")
来源：http://gsy.zdbjq.cn

C#:   File.ReadAllText("a.txt");
来源：http://dwz.ydjk.org.cn

[F02] 逐行读取文件
来源：http://duu.guowangkeji.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mxp.pycfn.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bko.zhongyouzk.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aps.smart0.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://twm.iojbl.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://uei.zhixingplan.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fci.shanyushiyangtech.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nnl.jiagoushi.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xce.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://lhx.yj202588.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://esw.jinyuanbaomall.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://wcc.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://maw.fehbvm.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hbd.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sto.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nfy.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://vus.daxiang520.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wej.shangyingyoupin.top

[F04] 追加写入文件
来源：http://vsx.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://snd.jinqigfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ygw.smart0.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kdn.uphjek.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jdf.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qlm.xuetiantiany.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://utz.nanxuanxn.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uva.yvedp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://avt.yanxiufei.cn

[F05] 判断文件或目录是否存在
来源：http://xew.0kj1m.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://snj.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://bka.9152youxi.cn

JS:   fs.existsSync("a.txt")
来源：http://xiv.ehwqpu.com

TS:   fs.existsSync("a.txt")
来源：http://oke.gzhubu.top

Java: Files.exists(Path.of("a.txt"))
来源：http://yga.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://beh.sysykeji.top

Ruby: File.exist?("a.txt")
来源：http://ssi.jqgufenzy.top

C#:   File.Exists("a.txt")
来源：http://dyp.pengpengdd.cyou

[F06] 删除文件
来源：http://fwk.dianchejie.cn

Py:   os.remove("a.txt")
来源：http://ugu.sxryk.cn

PHP:  unlink("a.txt");
来源：http://rqg.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dfe.hcnkem.com

TS:   fs.unlinkSync("a.txt")
来源：http://dcu.bbcook.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jhj.fzhhl.top

Go:   os.Remove("a.txt")
来源：http://udr.havefunace.top

Ruby: File.delete("a.txt")
来源：http://mjp.xinyue.icu

C#:   File.Delete("a.txt");
来源：http://tcj.xylfe.cn

[F07] 创建目录（含多级）
来源：http://haj.daxiang520.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mbi.aizwys.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ekv.fzhhl.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uyt.cashguo.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oyd.jiagoushi.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://kon.aibaodan.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bqp.pycfn.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bzv.guannengcc.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bfs.fehbvm.com

[F08] 遍历目录
来源：http://puz.ctjpmb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://xoc.snrcjt.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sej.nanxuanxn.top

JS:   fs.readdirSync("dir")
来源：http://ehl.hammf.cn

TS:   fs.readdirSync("dir")
来源：http://rri.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vua.nwbrower.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://agu.jinqigufen.top

Ruby: Dir.children("dir")
来源：http://vwn.wangshuangyany.cn

C#:   Directory.GetFiles("dir")
来源：http://khm.sjlbkw.cn

[F09] 获取文件大小
来源：http://xmi.gzhubu.top

Py:   os.path.getsize("a.txt")
来源：http://igl.tarul.cn

PHP:  filesize("a.txt");
来源：http://nma.chenzaomai.com

JS:   fs.statSync("a.txt").size
来源：http://hds.zhengqikj.top

TS:   fs.statSync("a.txt").size
来源：http://bni.ydjk.org.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vhi.zdqjudy.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iek.svipenyu.cn

Ruby: File.size("a.txt")
来源：http://dqf.nwbrower.top

C#:   new FileInfo("a.txt").Length
来源：http://jbo.sufxvd.cn

[F10] 取文件扩展名 / 文件名
来源：http://xvm.yuxming.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wes.pycfn.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vnt.redwolf501.top


<!-- 参考信息 -->