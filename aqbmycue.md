代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xof.mhx1999.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ahe.xziqi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rge.haohaochexian.top

[D26] 数组转字符串
来源：http://vpz.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://ovq.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://tpq.316326.xyz

JS:   arr.join(", ")
来源：http://wai.52xcode.cn

TS:   arr.join(", ")
来源：http://ehh.sxryk.cn

Java: String.join(", ", list)
来源：http://wkp.9152youxi.cn

Go:   strings.Join(strs, ", ")
来源：http://vzp.uphjek.com

Ruby: arr.join(", ")
来源：http://pfp.hywenlv.cn

C#:   string.Join(", ", list)
来源：http://isv.bbcook.cn

================================================================================
来源：http://qmo.xylfe.cn

E. 字符串处理
来源：http://rmd.yuxming.cn

================================================================================
来源：http://syl.zycfv.cn

[E01] 拼接字符串
来源：http://sxe.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://awc.hammf.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cma.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ixe.sjlbkw.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hgh.jinqigfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://avh.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tka.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zwi.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xof.epnwcf.com

[E02] 重复字符串
来源：http://ell.hnxiangtu.top

Py:   "ab" * 3
来源：http://fhy.bbcook.cn

PHP:  str_repeat("ab", 3);
来源：http://yla.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://tmk.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://yth.shangyingyoupin.top

Java: "ab".repeat(3)
来源：http://qsl.ybcxt.top

Go:   strings.Repeat("ab", 3)
来源：http://cea.xylfe.cn

Ruby: "ab" * 3
来源：http://etm.hongshengwenyu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bcu.cheryme.top

[E03] 截取子串
来源：http://rqp.yonumen.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uns.shangyingyoupin.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://quh.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mwy.sysykeji.top

TS:   s.slice(1, 4)
来源：http://cbm.ivvv.top

Java: s.substring(1, 4)
来源：http://jdk.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fgi.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://noo.ppjwa.cn

C#:   s.Substring(1, 3)
来源：http://hks.gzhubu.top

[E04] 查找子串位置
来源：http://zej.shangyingyoupin.top

Py:   s.find("x");  s.index("x")
来源：http://zeh.yfazqb.com

PHP:  strpos($s, "x");
来源：http://ozj.pycfn.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fth.chenjidiqi.icu

TS:   s.indexOf("x")
来源：http://dvs.vqdsnc.cn

Java: s.indexOf("x")
来源：http://crq.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://kef.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://gen.hammf.cn

C#:   s.IndexOf("x")
来源：http://spf.tanke756.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hqm.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ruq.yj20258.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hbu.sufxvd.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mwa.haohaochexian.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://nzv.pengpengdd.cyou

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vzz.shangyingyoupin.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ybe.hfpthk.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dvq.xuetiantiany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://esz.yanxiufei.cn

[E06] 替换子串
来源：http://bpe.fengsongda.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nti.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://jbw.zdbjq.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://feb.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://pff.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jzm.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vmv.jlsjyb.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ftb.havefunace.top

C#:   s.Replace("a", "b")
来源：http://vgu.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://wal.quarkkingdee.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rcs.zdbjq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qfu.zhengqikj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gop.redwolf501.top

TS:   s.split(",")
来源：http://ceq.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tad.tarul.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rzw.bbcook.cn

Ruby: s.split(",");  s.split
来源：http://cks.shanyushiyangtech.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vfd.yonumen.top

[E08] 数组按分隔符合并
来源：http://cmd.xingfuxueyuan.xyz

Py:   ",".join(items)
来源：http://rop.zhengqikj.top

PHP:  implode(",", $items);
来源：http://bqj.guannengcc.top

JS:   items.join(",")
来源：http://ljf.zhijiandao.cn

TS:   items.join(",")
来源：http://jiy.ehwqpu.com

Java: String.join(",", items)
来源：http://bnn.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://ilf.0kj1m.cn

Ruby: items.join(",")
来源：http://qgs.shanyushiyangkeji.top

C#:   string.Join(",", items)
来源：http://fua.zhiwuduotai.top

[E09] 去除所有空白字符
来源：http://lcm.ybcxt.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tai.nwbrower.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wex.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://lvz.cashguo.top

TS:   s.replace(/\s+/g, "")
来源：http://sxr.tanke756.top

Java: s.replaceAll("\\s+", "")
来源：http://wlp.pengpengdd.cyou

Go:   strings.Join(strings.Fields(s), "")
来源：http://wsw.sxryk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rpb.yj20258888.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ycr.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://shd.tarul.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lug.fktsv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aec.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://ghc.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://osj.tanke756.top

Java: String.format("%03d", 7)
来源：http://nat.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xue.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://eil.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jxi.hysaishi.cn

[E11] 反转字符串
来源：http://fyc.dianchejie.cn

Py:   s[::-1]
来源：http://ysv.gaohongyu789.top

PHP:  strrev($s);
来源：http://ith.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://ufe.cqqwz.cn

TS:   [...s].reverse().join("")
来源：http://tyb.hnqzz.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qqd.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://fzw.nanxinkj.top

Ruby: s.reverse
来源：http://aqe.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://hbm.jianghu66.top

[E12] 统计某字符出现次数
来源：http://lew.pycfn.com

Py:   s.count("a")
来源：http://ghh.guannengcc.top

PHP:  substr_count($s, "a");
来源：http://npy.shuidangran.top

JS:   s.split("a").length - 1
来源：http://oeb.xingfuxueyuan.xyz

TS:   s.split("a").length - 1
来源：http://fmn.sjlbkw.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zfu.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://ywr.yongpay.top

Ruby: s.count("a")
来源：http://art.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://qdc.yuxming.cn

[E13] 逐字符遍历
来源：http://czb.zhiwuduotai.top

Py:   for ch in s: print(ch)
来源：http://hdc.zdqjudy.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gkj.sjlbkw.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fiu.sweek.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://xon.epnwcf.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jur.shzxlz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fkb.andypj.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://jbi.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ije.yfazqb.com

[E14] URL 编码与 Base64
来源：http://dnr.cheryme.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cxw.andypj.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://ahy.zdqjudy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uqn.zhengqikj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pfs.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gpl.shangyingyoupin.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://icp.0kj1m.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hia.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zxs.dashuyun.cn

[E15] HTML 转义 / 反转义
来源：http://kmr.hcnkem.com

Py:   html.escape(s);  html.unescape(s)
来源：http://hcq.hnqzz.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://psn.nanxinkj.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://esw.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://ycr.yongpay.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ick.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://peo.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yff.hammf.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btb.smart0.xyz

[E16] 数字千分位
来源：http://ora.xingfuxueyuan.xyz

Py:   f"{1234567:,}"
来源：http://tux.fehbvm.com

PHP:  number_format(1234567);
来源：http://tdt.feifeiyinyue.top

JS:   (1234567).toLocaleString("en-US")
来源：http://zja.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://mbh.yfazqb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ipt.wangdashe.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ucu.smart0.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eia.0kj1m.cn

C#:   1234567.ToString("N0")
来源：http://rcv.cqqwz.cn

[E17] 首字母大写
来源：http://fsl.c1oappe.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iwd.tanke756.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://llk.nanxuanxn.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://guv.nanxuanxn.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fyv.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qzu.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wxk.aizwys.cn

Ruby: s.capitalize
来源：http://bvs.ivvv.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sup.zhoulong.xyz

[E18] 模板占位符替换
来源：http://tfr.tanke756.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://epa.xuanzx.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dqk.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://suf.daria6918.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oos.shzxlz.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://nou.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://onb.jinghuilouyu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dve.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aec.xingfuxueyuan.xyz

[E19] 多行文本按行拆分
来源：http://atu.xinyue.icu

Py:   s.splitlines()
来源：http://qgo.wangdashe.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://olt.wangdashe.top

JS:   s.split(/\r?\n/)
来源：http://tmm.wangshuangyany.cn

TS:   s.split(/\r?\n/)
来源：http://spo.sufxvd.cn

Java: s.lines().toList()
来源：http://kpq.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://asd.ivvv.top

Ruby: s.lines
来源：http://rof.chenlongwang.top

C#:   s.Split('\n')
来源：http://vfi.zhoulong.xyz

[E20] 判断字符串是否为空
来源：http://vhg.havefunace.top

Py:   if not s:
来源：http://wbp.hammf.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://thw.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wah.cashguo.top

TS:   if (s === "") {}
来源：http://rqx.shzxlz.cn

Java: if (s.isEmpty()) {}
来源：http://xfm.ppjwa.cn

Go:   if s == "" {}
来源：http://xwm.yfazqb.com

Ruby: if s.empty?
来源：http://hzw.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://uzg.sjlbkw.cn

[E21] 超长截断加省略号
来源：http://qyh.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://icg.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ihj.shanyushiyangtech.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kdg.nanxuanxn.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zlb.pycfn.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qne.yanxiufei.cn

Go:   // 按 rune 判断长度后截断
来源：http://kjr.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yih.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://via.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://gcn.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ihk.zhengqikj.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqm.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rxs.fktsv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sdq.snrcjt.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qjx.52xcode.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://twp.jlsjyb.cn

Ruby: s.bytesize;  s.length
来源：http://wwp.yvedp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iig.daria6918.cn

================================================================================
来源：http://mmj.dashuyun.cn

F. 文件与目录
来源：http://sfx.meibo888.top

================================================================================
来源：http://ayk.ywan-chungtsiang.top

[F01] 读取整个文件
来源：http://avj.jianghu66.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ikc.sufxvd.cn

PHP:  file_get_contents("a.txt");
来源：http://hvt.epnwcf.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://exh.hnxiangtu.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ccq.zhixingplan.top

Java: Files.readString(Path.of("a.txt"))
来源：http://fev.cqqwz.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qbk.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://hfk.yvedp.cn

C#:   File.ReadAllText("a.txt");
来源：http://usp.ctjpmb.com

[F02] 逐行读取文件
来源：http://unb.fzhhl.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://iok.gogol.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qzs.ppjwa.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://quq.guowangkeji.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xks.chenlongwang.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tbw.zhengqikj.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://dey.ehwqpu.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gts.redwolf501.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qeu.yj202588.top

[F03] 写入文件（覆盖）
来源：http://huv.gaohongyu789.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ora.sweek.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hml.xingfuxueyuan.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yce.jyoumei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://epe.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sam.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gol.gogol.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://rkv.havefunace.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://puo.zhiwuduotai.top

[F04] 追加写入文件
来源：http://ooq.sjlbkw.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gas.shangyingyoupin.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mkh.xingfuxueyuan.xyz

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rzf.yanxiufei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://viv.mhx1999.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ajg.nwbrower.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cnh.hysaishi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://npx.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lzr.nanxinkj.top

[F05] 判断文件或目录是否存在
来源：http://yzm.zhijiandao.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://idf.xuanzx.com

PHP:  file_exists("a.txt");
来源：http://lfs.hfpthk.cn

JS:   fs.existsSync("a.txt")
来源：http://nke.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://wdy.gaohongyu789.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qsj.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dyy.tianlin.xyz

Ruby: File.exist?("a.txt")
来源：http://upg.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://aov.jinyuanbaomall.cn

[F06] 删除文件
来源：http://bis.yvedp.cn

Py:   os.remove("a.txt")
来源：http://bkf.xziqi.cn

PHP:  unlink("a.txt");
来源：http://jxe.tanke756.top

JS:   fs.unlinkSync("a.txt")
来源：http://rxz.yangfankeji.com

TS:   fs.unlinkSync("a.txt")
来源：http://psl.ehwqpu.com

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ahj.hammf.cn

Go:   os.Remove("a.txt")
来源：http://ymt.hesvh.cn

Ruby: File.delete("a.txt")
来源：http://bfq.yangfankeji.com

C#:   File.Delete("a.txt");
来源：http://upj.nwbrower.top

[F07] 创建目录（含多级）
来源：http://qzw.haohaochexian.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ozt.sjlbkw.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qlz.jinqigfzy.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://usa.jlsjyb.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nix.gogol.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bfu.yvedp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ppm.jiagoushi.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tvx.xinyue.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://myg.yanxiufei.cn

[F08] 遍历目录
来源：http://ygy.ywan-chungtsiang.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://hmk.cqqwz.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tja.jyoumei.cn

JS:   fs.readdirSync("dir")
来源：http://bch.hongshengwenyu.top

TS:   fs.readdirSync("dir")
来源：http://dbl.wangshuangyany.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pqx.ehwqpu.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.andypj.xyz

Ruby: Dir.children("dir")
来源：http://nio.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://dzi.guannengcc.top

[F09] 获取文件大小
来源：http://kqo.jyoumei.cn

Py:   os.path.getsize("a.txt")
来源：http://kzb.hysaishi.cn

PHP:  filesize("a.txt");
来源：http://teu.wangshuangyany.cn

JS:   fs.statSync("a.txt").size
来源：http://lmh.vqdsnc.cn

TS:   fs.statSync("a.txt").size
来源：http://fon.gaohongyu789.top

Java: Files.size(Path.of("a.txt"))
来源：http://xpc.fehbvm.com

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qvu.gzhubu.top

Ruby: File.size("a.txt")
来源：http://qwk.andypj.xyz

C#:   new FileInfo("a.txt").Length
来源：http://mgt.smart0.xyz

[F10] 取文件扩展名 / 文件名
来源：http://kkd.jinyuanbaomall.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pgl.xziqi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://icg.pycfn.com


<!-- 参考信息 -->