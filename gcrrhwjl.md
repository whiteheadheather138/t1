代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hob.cashguo.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hpu.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dxo.zhixingplan.top

[D26] 数组转字符串
来源：http://fzk.c1oappe.top

Py:   ", ".join(map(str, arr))
来源：http://gsn.nanxuanxn.top

PHP:  implode(", ", $arr);
来源：http://wde.gogol.net.cn

JS:   arr.join(", ")
来源：http://mwy.epnwcf.com

TS:   arr.join(", ")
来源：http://mpb.yj20258.top

Java: String.join(", ", list)
来源：http://elh.aizwys.cn

Go:   strings.Join(strs, ", ")
来源：http://gfz.zdbjq.cn

Ruby: arr.join(", ")
来源：http://dnl.iojbl.cn

C#:   string.Join(", ", list)
来源：http://uns.epnwcf.com

================================================================================
来源：http://hzk.iojbl.cn

E. 字符串处理
来源：http://kno.dianchejie.cn

================================================================================
来源：http://qut.yongpay.top

[E01] 拼接字符串
来源：http://wbb.316326.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lib.aibaodan.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jjx.chenjidiqi.icu

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://typ.sufxvd.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jwa.tianlin.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tux.cheryme.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vqy.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://icw.aibaodan.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wsl.zhiwuduotai.top

[E02] 重复字符串
来源：http://ntu.bjfxy.top

Py:   "ab" * 3
来源：http://wiw.yj20258.top

PHP:  str_repeat("ab", 3);
来源：http://kia.zycfv.cn

JS:   "ab".repeat(3)
来源：http://stw.quarkkingdee.top

TS:   "ab".repeat(3)
来源：http://jqz.ctjpmb.com

Java: "ab".repeat(3)
来源：http://fce.sweek.top

Go:   strings.Repeat("ab", 3)
来源：http://mut.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://wkh.mhx1999.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fjn.cqqwz.cn

[E03] 截取子串
来源：http://nxa.shzxlz.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://aug.zhijiandao.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kov.zhiwuduotai.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dcj.ywan-chungtsiang.top

TS:   s.slice(1, 4)
来源：http://atr.jinghuilouyu.cn

Java: s.substring(1, 4)
来源：http://qwb.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fxa.xziqi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ajf.cashguo.top

C#:   s.Substring(1, 3)
来源：http://rik.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://ouc.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://voo.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://yqm.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fsf.sysykeji.top

TS:   s.indexOf("x")
来源：http://pvq.quarkkingdee.top

Java: s.indexOf("x")
来源：http://wxt.yj202588.top

Go:   strings.Index(s, "x")
来源：http://xtt.zhiwuduotai.top

Ruby: s.index("x")
来源：http://gcu.ywan-chungtsiang.top

C#:   s.IndexOf("x")
来源：http://jkw.xinyue.icu

[E05] 判断包含 / 前缀 / 后缀
来源：http://muh.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pit.redwolf501.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qme.shzxlz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybl.hfpthk.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xpc.sxryk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nso.52xcode.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://knq.hcnkem.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aln.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fml.zycfv.cn

[E06] 替换子串
来源：http://eps.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lfj.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://mdx.xziqi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yde.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://frj.daxiang520.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jed.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://znv.yuxming.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://olr.yuxming.cn

C#:   s.Replace("a", "b")
来源：http://unb.aizwys.cn

[E07] 按分隔符拆分
来源：http://sua.yuxming.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cth.xingfuxueyuan.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kjm.vqdsnc.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://myp.wangshuangyany.cn

TS:   s.split(",")
来源：http://wxf.vqdsnc.cn

Java: s.split(",");  s.split("\\s+")
来源：http://aif.yonumen.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://znl.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://iif.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xkt.pengpengdd.cyou

[E08] 数组按分隔符合并
来源：http://fgk.dashuyun.cn

Py:   ",".join(items)
来源：http://lph.316326.xyz

PHP:  implode(",", $items);
来源：http://kfl.hfpthk.cn

JS:   items.join(",")
来源：http://vev.uphjek.com

TS:   items.join(",")
来源：http://rmn.hongshengwenyu.top

Java: String.join(",", items)
来源：http://qvw.sweek.top

Go:   strings.Join(items, ",")
来源：http://dpv.pengpengdd.cyou

Ruby: items.join(",")
来源：http://fex.nwbrower.top

C#:   string.Join(",", items)
来源：http://yie.hcnkem.com

[E09] 去除所有空白字符
来源：http://nzj.yangfankeji.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cai.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eab.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://tis.hnxiangtu.top

TS:   s.replace(/\s+/g, "")
来源：http://wwq.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://fyr.c1oappe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://pzl.zdbjq.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qdy.sxryk.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ctg.yfazqb.com

[E10] 左侧补零 / 定长填充
来源：http://wgi.ppjwa.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gii.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zkz.jinqigufen.top

JS:   "7".padStart(3, "0")
来源：http://dsi.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://fhn.sweek.top

Java: String.format("%03d", 7)
来源：http://ndi.yvedp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bco.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wec.haohaochexian.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vhk.vehdjk.com

[E11] 反转字符串
来源：http://jzo.vqdsnc.cn

Py:   s[::-1]
来源：http://tui.yonumen.top

PHP:  strrev($s);
来源：http://mho.nanxuanxn.top

JS:   [...s].reverse().join("")
来源：http://roj.zdbjq.cn

TS:   [...s].reverse().join("")
来源：http://yxt.ppjwa.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uks.shanyushiyangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://xcw.gogol.net.cn

Ruby: s.reverse
来源：http://dsa.ctjpmb.com

C#:   new string(s.Reverse().ToArray())
来源：http://pth.zhongyouzk.top

[E12] 统计某字符出现次数
来源：http://uwy.daxiang520.top

Py:   s.count("a")
来源：http://dqj.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://txe.jianghu66.top

JS:   s.split("a").length - 1
来源：http://lvy.hcnkem.com

TS:   s.split("a").length - 1
来源：http://csv.zhijiandao.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cxs.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://khe.xziqi.cn

Ruby: s.count("a")
来源：http://vvd.dashuyun.cn

C#:   s.Count(c => c == 'a')
来源：http://oyo.wangdashe.top

[E13] 逐字符遍历
来源：http://dng.xuetiantiany.cn

Py:   for ch in s: print(ch)
来源：http://efp.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ywn.chenlongwang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://htb.mhx1999.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://ipb.hammf.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ggq.dashuyun.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lrc.ivvv.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jxb.jyoumei.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bmi.ydzc1.top

[E14] URL 编码与 Base64
来源：http://bzb.hammf.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://uii.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://eiz.iojbl.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bqx.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gyq.ppjwa.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bgm.zhengqikj.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jaw.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://knp.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fob.jinqigfzy.top

[E15] HTML 转义 / 反转义
来源：http://jyf.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://ecq.xinyue.icu

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pft.ydjk.org.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gts.cheryme.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dsm.chenlongwang.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fhj.nanxinkj.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rcv.jyoumei.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zrz.sjlbkw.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://akd.pycfn.com

[E16] 数字千分位
来源：http://ico.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://xon.ehwqpu.com

PHP:  number_format(1234567);
来源：http://fhi.bbcook.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gdq.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://rlc.wangshuangyany.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cdx.jianghu66.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lme.bjfxy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bzh.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://eol.yuanzhike.top

[E17] 首字母大写
来源：http://xjm.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://iso.aizwys.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://svm.fktsv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://szh.yj202588.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kcs.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ing.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jpn.zhijiandao.cn

Ruby: s.capitalize
来源：http://fwc.316326.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oys.c1oappe.top

[E18] 模板占位符替换
来源：http://vgm.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zdk.shanyushiyangkeji.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sir.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://gzw.shangyingyoupin.top

TS:   tpl.replaceAll("{name}", name)
来源：http://owq.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jgs.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xxm.316326.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://swy.sxryk.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jxz.fzhhl.top

[E19] 多行文本按行拆分
来源：http://cbc.iojbl.cn

Py:   s.splitlines()
来源：http://nuy.hesvh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xks.jianghu66.top

JS:   s.split(/\r?\n/)
来源：http://oqm.hesvh.cn

TS:   s.split(/\r?\n/)
来源：http://bas.cdnleiting.top

Java: s.lines().toList()
来源：http://fnp.9152youxi.cn

Go:   strings.Split(s, "\n")
来源：http://jgn.gaohongyu789.top

Ruby: s.lines
来源：http://dkm.bbcook.cn

C#:   s.Split('\n')
来源：http://zam.bbcook.cn

[E20] 判断字符串是否为空
来源：http://ibk.jqgufenzy.top

Py:   if not s:
来源：http://rdz.pycfn.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ckt.vehdjk.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lmg.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://xbi.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://hou.mhx1999.top

Go:   if s == "" {}
来源：http://urm.316326.xyz

Ruby: if s.empty?
来源：http://cbj.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pjm.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://amf.cashguo.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yhf.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jzd.tanke756.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gdc.jiagoushi.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yvf.ivvv.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fmq.tanke756.top

Go:   // 按 rune 判断长度后截断
来源：http://idv.52xcode.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qdp.xinyue.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lzf.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://eum.vehdjk.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jwe.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hcc.zhixingplan.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vdb.yj20258.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ngy.jqgufenzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nmb.hnxiangtu.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cyy.jinqigfzy.top

Ruby: s.bytesize;  s.length
来源：http://jxl.yj20258888.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sro.ybcxt.top

================================================================================
来源：http://nvd.ehwqpu.com

F. 文件与目录
来源：http://xfa.fanxiaobao.xyz

================================================================================
来源：http://fbw.shanyushiyangtech.top

[F01] 读取整个文件
来源：http://zfc.hysaishi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bhl.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://yqq.yj202588.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://kzl.chenjidiqi.icu

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://yjo.dashuyun.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://usi.ppjwa.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wlh.ehwqpu.com

Ruby: File.read("a.txt")
来源：http://muq.bbcook.cn

C#:   File.ReadAllText("a.txt");
来源：http://rep.zhaomingkeji.xyz

[F02] 逐行读取文件
来源：http://lgl.jqgufenzy.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bab.tian-w.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://atb.sxryk.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tnw.zdbjq.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lmi.sweek.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lqn.fengsongda.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wxi.zhoulong.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tyb.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cik.yangfankeji.com

[F03] 写入文件（覆盖）
来源：http://rcg.hcnkem.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://brm.xziqi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pjx.xuetiantiany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ypu.hesvh.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://icp.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sxb.zhiwuduotai.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iwg.daria6918.cn

Ruby: File.write("a.txt", "hi")
来源：http://oma.yueranfly.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eid.aibaodan.cn

[F04] 追加写入文件
来源：http://zdu.hnqzz.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ilq.fehbvm.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://twv.nanxinkj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qln.iojbl.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tif.jqgufenzy.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ycl.hcnkem.com

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://onc.wangshuangyany.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tup.wangshuangyany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uga.cheryme.top

[F05] 判断文件或目录是否存在
来源：http://gve.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ooq.zhengqikj.top

PHP:  file_exists("a.txt");
来源：http://mwn.ydzc1.top

JS:   fs.existsSync("a.txt")
来源：http://dyw.yfazqb.com

TS:   fs.existsSync("a.txt")
来源：http://lgz.svipenyu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aob.yangfankeji.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xwz.jinyuanbaomall.cn

Ruby: File.exist?("a.txt")
来源：http://vbs.sysykeji.top

C#:   File.Exists("a.txt")
来源：http://hrq.hnxiangtu.top

[F06] 删除文件
来源：http://adv.tarul.cn

Py:   os.remove("a.txt")
来源：http://qfn.zdqjudy.top

PHP:  unlink("a.txt");
来源：http://adw.nanxuanxn.top

JS:   fs.unlinkSync("a.txt")
来源：http://eir.havefunace.top

TS:   fs.unlinkSync("a.txt")
来源：http://mqz.316326.xyz

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uvf.jlsjyb.cn

Go:   os.Remove("a.txt")
来源：http://sja.tian-w.cn

Ruby: File.delete("a.txt")
来源：http://lyn.quarkkingdee.top

C#:   File.Delete("a.txt");
来源：http://vcg.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://ccf.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ppe.jqgufenzy.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://koa.xylfe.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zhh.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://upd.yuanzhike.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vlk.gotoacloud.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aed.ppjwa.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vjq.hnxiangtu.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tag.tarul.cn

[F08] 遍历目录
来源：http://sov.uphjek.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://fuu.c1oappe.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://agq.xziqi.cn

JS:   fs.readdirSync("dir")
来源：http://vzh.cucudq.cn

TS:   fs.readdirSync("dir")
来源：http://hag.fengsongda.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://esb.uphjek.com

Go:   entries, _ := os.ReadDir("dir")
来源：http://ozx.dianchejie.cn

Ruby: Dir.children("dir")
来源：http://jqv.shanyushiyangkeji.top

C#:   Directory.GetFiles("dir")
来源：http://fvh.mhx1999.top

[F09] 获取文件大小
来源：http://ivd.ctjpmb.com

Py:   os.path.getsize("a.txt")
来源：http://xzm.haohaochexian.top

PHP:  filesize("a.txt");
来源：http://wej.redwolf501.top

JS:   fs.statSync("a.txt").size
来源：http://sww.yj20258888.top

TS:   fs.statSync("a.txt").size
来源：http://qjd.chenzaomai.com

Java: Files.size(Path.of("a.txt"))
来源：http://dow.svipenyu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://miy.cucudq.cn

Ruby: File.size("a.txt")
来源：http://gjm.shangyingyoupin.top

C#:   new FileInfo("a.txt").Length
来源：http://ccp.cashguo.top

[F10] 取文件扩展名 / 文件名
来源：http://fin.yj20258888.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://koz.zhaomingkeji.xyz

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gsx.yj20258888.top


<!-- 参考信息 -->