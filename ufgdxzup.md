代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ubh.hywenlv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zqo.epnwcf.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://has.cucudq.cn

[D26] 数组转字符串
来源：http://wbg.tanke756.top

Py:   ", ".join(map(str, arr))
来源：http://suk.yvedp.cn

PHP:  implode(", ", $arr);
来源：http://zia.havefunace.top

JS:   arr.join(", ")
来源：http://qvx.xylfe.cn

TS:   arr.join(", ")
来源：http://jct.ehwqpu.com

Java: String.join(", ", list)
来源：http://bsj.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://crs.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://sft.xziqi.cn

C#:   string.Join(", ", list)
来源：http://ahl.aizwys.cn

================================================================================
来源：http://rvr.pengpengdd.cyou

E. 字符串处理
来源：http://vav.meibo888.top

================================================================================
来源：http://htt.gzhubu.top

[E01] 拼接字符串
来源：http://qkx.yonumen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ojj.meibo888.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vwf.shuidangran.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnl.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tws.haohaochexian.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tki.uphjek.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ifr.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://btg.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jgl.nwbrower.top

[E02] 重复字符串
来源：http://bws.aibaodan.cn

Py:   "ab" * 3
来源：http://jzi.shuidangran.top

PHP:  str_repeat("ab", 3);
来源：http://ctd.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://msa.iojbl.cn

TS:   "ab".repeat(3)
来源：http://wsq.xylfe.cn

Java: "ab".repeat(3)
来源：http://kjd.hammf.cn

Go:   strings.Repeat("ab", 3)
来源：http://zni.bbcook.cn

Ruby: "ab" * 3
来源：http://vei.quarkkingdee.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://khm.bjfxy.top

[E03] 截取子串
来源：http://nva.jlsjyb.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://qnc.shanyushiyangtech.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qcw.cdnleiting.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tmh.svipenyu.cn

TS:   s.slice(1, 4)
来源：http://yws.jqgufenzy.top

Java: s.substring(1, 4)
来源：http://iel.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hwc.9152youxi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fpk.zhengqikj.top

C#:   s.Substring(1, 3)
来源：http://ies.xuetiantiany.cn

[E04] 查找子串位置
来源：http://muv.sjlbkw.cn

Py:   s.find("x");  s.index("x")
来源：http://rys.cashguo.top

PHP:  strpos($s, "x");
来源：http://ncg.fktsv.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xxm.guowangkeji.top

TS:   s.indexOf("x")
来源：http://cmq.c1oappe.top

Java: s.indexOf("x")
来源：http://dob.yj20258888.top

Go:   strings.Index(s, "x")
来源：http://bps.sweek.top

Ruby: s.index("x")
来源：http://syr.xuanzx.com

C#:   s.IndexOf("x")
来源：http://dmi.epnwcf.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://twe.quarkkingdee.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uki.sweek.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cro.gzhubu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tvp.nanxinkj.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://vfo.xuetiantiany.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://quk.yfazqb.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bbm.hysaishi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://goc.hcnkem.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xlj.xuetiantiany.cn

[E06] 替换子串
来源：http://ffn.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qdg.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://ahe.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tih.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://zqi.jinyuanbaomall.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cde.jianghu66.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hdv.0kj1m.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qau.tarul.cn

C#:   s.Replace("a", "b")
来源：http://vku.mhx1999.top

[E07] 按分隔符拆分
来源：http://dii.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kxj.zhijiandao.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://roi.tianlin.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://xqy.cqqwz.cn

TS:   s.split(",")
来源：http://jei.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mrn.cdnleiting.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://daa.mhx1999.top

Ruby: s.split(",");  s.split
来源：http://ydp.chenzaomai.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jar.redwolf501.top

[E08] 数组按分隔符合并
来源：http://elb.yueranfly.top

Py:   ",".join(items)
来源：http://oar.zdqjudy.top

PHP:  implode(",", $items);
来源：http://nan.shangyingyoupin.top

JS:   items.join(",")
来源：http://fyp.svipenyu.cn

TS:   items.join(",")
来源：http://sog.nanxuanxn.top

Java: String.join(",", items)
来源：http://pbw.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://ppj.jlsjyb.cn

Ruby: items.join(",")
来源：http://eol.xuetiantiany.cn

C#:   string.Join(",", items)
来源：http://woz.fktsv.cn

[E09] 去除所有空白字符
来源：http://sfg.yonumen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hjw.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vbn.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://ncx.zhaomingkeji.xyz

TS:   s.replace(/\s+/g, "")
来源：http://tao.wangshuangyany.cn

Java: s.replaceAll("\\s+", "")
来源：http://qth.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://gsl.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://jrl.wangshuangyany.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wci.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://ysp.ybcxt.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cxb.vehdjk.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://npv.ppjwa.cn

JS:   "7".padStart(3, "0")
来源：http://wkd.sxryk.cn

TS:   "7".padStart(3, "0")
来源：http://fjt.cdnleiting.top

Java: String.format("%03d", 7)
来源：http://hpp.guowangkeji.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://nbw.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yys.yj202588.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tym.hcnkem.com

[E11] 反转字符串
来源：http://xja.ctjpmb.com

Py:   s[::-1]
来源：http://ppp.yonumen.top

PHP:  strrev($s);
来源：http://afp.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://mpb.9152youxi.cn

TS:   [...s].reverse().join("")
来源：http://eij.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://syj.daria6918.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ood.hcnkem.com

Ruby: s.reverse
来源：http://gwz.zhaomingkeji.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://qbv.fanxiaobao.xyz

[E12] 统计某字符出现次数
来源：http://hwb.yonumen.top

Py:   s.count("a")
来源：http://jur.sweek.top

PHP:  substr_count($s, "a");
来源：http://vfb.nwbrower.top

JS:   s.split("a").length - 1
来源：http://kvv.aibaodan.cn

TS:   s.split("a").length - 1
来源：http://obs.jiagoushi.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hqf.gaohongyu789.top

Go:   strings.Count(s, "a")
来源：http://dxf.yvedp.cn

Ruby: s.count("a")
来源：http://fjd.xuanzx.com

C#:   s.Count(c => c == 'a')
来源：http://czx.zhiwuduotai.top

[E13] 逐字符遍历
来源：http://ugq.svipenyu.cn

Py:   for ch in s: print(ch)
来源：http://ure.sjlbkw.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://avx.svipenyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://uxq.gogol.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yqb.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sob.316326.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nrh.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gqu.ctjpmb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qgm.aibaodan.cn

[E14] URL 编码与 Base64
来源：http://abv.svipenyu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oyg.xziqi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ajq.hammf.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qni.jinqigufen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nbw.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dvn.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ofy.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zxf.fanxiaobao.xyz

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rtj.fktsv.cn

[E15] HTML 转义 / 反转义
来源：http://qfh.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://evm.yanxiufei.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vde.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rvd.yvedp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iop.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ggc.fehbvm.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ldx.meibo888.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zhn.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mtx.pycfn.com

[E16] 数字千分位
来源：http://sdr.tarul.cn

Py:   f"{1234567:,}"
来源：http://muf.pengpengdd.cyou

PHP:  number_format(1234567);
来源：http://bou.quarkkingdee.top

JS:   (1234567).toLocaleString("en-US")
来源：http://enn.yvedp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zgj.xylfe.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ysq.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yng.jinyuanbaomall.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rom.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://dbt.shanyushiyangkeji.top

[E17] 首字母大写
来源：http://lxe.yj202588.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cay.ehwqpu.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://awx.bjfxy.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hoc.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kne.guannengcc.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uqj.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wel.guannengcc.top

Ruby: s.capitalize
来源：http://trk.tanke756.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mkf.yongpay.top

[E18] 模板占位符替换
来源：http://uzr.yvedp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mvl.nanxuanxn.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://lzp.yanxiufei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tap.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://hrz.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ffc.shangyingyoupin.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yeu.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ohq.haohaochexian.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://inw.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://eaz.yvedp.cn

Py:   s.splitlines()
来源：http://ckx.jinqigfzy.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nff.yvedp.cn

JS:   s.split(/\r?\n/)
来源：http://zek.shanyushiyangkeji.top

TS:   s.split(/\r?\n/)
来源：http://eul.ydzc1.top

Java: s.lines().toList()
来源：http://cwj.daxiang520.top

Go:   strings.Split(s, "\n")
来源：http://szv.sxryk.cn

Ruby: s.lines
来源：http://uxx.yanxiufei.cn

C#:   s.Split('\n')
来源：http://epf.epnwcf.com

[E20] 判断字符串是否为空
来源：http://vui.sysykeji.top

Py:   if not s:
来源：http://clt.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ujd.shuidangran.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://miy.tarul.cn

TS:   if (s === "") {}
来源：http://jgk.daria6918.cn

Java: if (s.isEmpty()) {}
来源：http://zoi.52xcode.cn

Go:   if s == "" {}
来源：http://ris.jinqigufen.top

Ruby: if s.empty?
来源：http://cvf.yueranfly.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dfx.ctjpmb.com

[E21] 超长截断加省略号
来源：http://lqb.nanxinkj.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://npv.gotoacloud.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lar.jqgfzy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oqs.jinyuanbaomall.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wdk.nanxuanxn.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ubb.yongpay.top

Go:   // 按 rune 判断长度后截断
来源：http://mua.nanxinkj.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cjb.guowangkeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bew.bbcook.cn

[E22] 字节长度与字符长度
来源：http://fdn.svipenyu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xqn.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lmc.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lsg.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ywy.xziqi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://uhp.tianlin.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vfc.jinqigufen.top

Ruby: s.bytesize;  s.length
来源：http://ykj.hywenlv.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://axw.jinqigfzy.top

================================================================================
来源：http://wad.hywenlv.cn

F. 文件与目录
来源：http://hcw.fzhhl.top

================================================================================
来源：http://jxc.shanyushiyangkeji.top

[F01] 读取整个文件
来源：http://ijo.guowangkeji.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rza.daxiang520.top

PHP:  file_get_contents("a.txt");
来源：http://apq.cashguo.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nep.daxiang520.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ltn.0kj1m.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dkj.quarkkingdee.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pqt.sjlbkw.cn

Ruby: File.read("a.txt")
来源：http://qbb.ppjwa.cn

C#:   File.ReadAllText("a.txt");
来源：http://fdu.gotoacloud.top

[F02] 逐行读取文件
来源：http://liu.jiagoushi.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://clv.shanyushiyangtech.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://skf.zhoulong.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pjy.pycfn.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uwa.chenjidiqi.icu

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rka.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fnr.bbcook.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fnb.pycfn.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oil.hfpthk.cn

[F03] 写入文件（覆盖）
来源：http://yqw.ivvv.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cmg.yj20258888.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://frr.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bjd.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wxw.fanxiaobao.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://odj.yangfankeji.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vxy.9152youxi.cn

Ruby: File.write("a.txt", "hi")
来源：http://qje.xziqi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://shm.bbcook.cn

[F04] 追加写入文件
来源：http://nbz.xuanzx.com

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://oal.haohaochexian.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yso.yj20258.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jxx.yfazqb.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ecs.cdnleiting.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mfp.guowangkeji.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://nye.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oqk.yj20258888.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jgu.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://mbk.shanyushiyangkeji.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ajr.yuxming.cn

PHP:  file_exists("a.txt");
来源：http://cbo.fzhhl.top

JS:   fs.existsSync("a.txt")
来源：http://rll.zhengqikj.top

TS:   fs.existsSync("a.txt")
来源：http://lnh.pengpengdd.cyou

Java: Files.exists(Path.of("a.txt"))
来源：http://iqw.gotoacloud.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rde.xuetiantiany.cn

Ruby: File.exist?("a.txt")
来源：http://utm.gzhubu.top

C#:   File.Exists("a.txt")
来源：http://vpj.hesvh.cn

[F06] 删除文件
来源：http://akt.nanxuanxn.top

Py:   os.remove("a.txt")
来源：http://huj.wangdashe.top

PHP:  unlink("a.txt");
来源：http://khc.fktsv.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cxn.52xcode.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hqi.jinghuilouyu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tmr.tanke756.top

Go:   os.Remove("a.txt")
来源：http://jts.mhx1999.top

Ruby: File.delete("a.txt")
来源：http://svc.ivvv.top

C#:   File.Delete("a.txt");
来源：http://uij.jinqigfzy.top

[F07] 创建目录（含多级）
来源：http://koo.hcnkem.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rxi.zdbjq.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gij.zdbjq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pas.sjlbkw.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dkv.hongshengwenyu.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pmv.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qtx.ivvv.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://crq.hongshengwenyu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://avy.tian-w.cn

[F08] 遍历目录
来源：http://akp.yfazqb.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ldr.fanxiaobao.xyz

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bfc.daxiang520.top

JS:   fs.readdirSync("dir")
来源：http://dvf.sxryk.cn

TS:   fs.readdirSync("dir")
来源：http://naa.yueranfly.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rnv.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://jrl.gotoacloud.top

Ruby: Dir.children("dir")
来源：http://jxq.guannengcc.top

C#:   Directory.GetFiles("dir")
来源：http://vno.daxiang520.top

[F09] 获取文件大小
来源：http://obg.ivvv.top

Py:   os.path.getsize("a.txt")
来源：http://jdw.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://tza.hywenlv.cn

JS:   fs.statSync("a.txt").size
来源：http://bta.jlsjyb.cn

TS:   fs.statSync("a.txt").size
来源：http://xjp.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://xxx.havefunace.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://txv.dashuyun.cn

Ruby: File.size("a.txt")
来源：http://mqs.xziqi.cn

C#:   new FileInfo("a.txt").Length
来源：http://iis.xingfuxueyuan.xyz

[F10] 取文件扩展名 / 文件名
来源：http://dnc.ywan-chungtsiang.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://veu.pengpengdd.cyou

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vga.yonumen.top


<!-- 参考信息 -->