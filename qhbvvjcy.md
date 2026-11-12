代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://zhj.sysykeji.top

PHP:  implode(", ", $arr);
来源：http://xbi.yonumen.top

JS:   arr.join(", ")
来源：http://kko.fanxiaobao.xyz

TS:   arr.join(", ")
来源：http://ugf.haohaochexian.top

Java: String.join(", ", list)
来源：http://eam.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://mgn.cashguo.top

Ruby: arr.join(", ")
来源：http://hah.zhijiandao.cn

C#:   string.Join(", ", list)
来源：http://mid.jqgufenzy.top

================================================================================
来源：http://zzi.iojbl.cn

E. 字符串处理
来源：http://pdi.fehbvm.com

================================================================================
来源：http://zuo.ybcxt.top

[E01] 拼接字符串
来源：http://zeb.yuxming.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gug.tianlin.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hny.xziqi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qhi.dianchejie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nrk.bbcook.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mzy.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjv.hammf.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ohv.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qrq.vehdjk.com

[E02] 重复字符串
来源：http://icv.sweek.top

Py:   "ab" * 3
来源：http://ljp.zhengqikj.top

PHP:  str_repeat("ab", 3);
来源：http://nle.cdnleiting.top

JS:   "ab".repeat(3)
来源：http://ghg.birdmap.top

TS:   "ab".repeat(3)
来源：http://sjc.feifeiyinyue.top

Java: "ab".repeat(3)
来源：http://lel.ehwqpu.com

Go:   strings.Repeat("ab", 3)
来源：http://ewx.yonumen.top

Ruby: "ab" * 3
来源：http://xtq.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rtc.0kj1m.cn

[E03] 截取子串
来源：http://olt.shanyushiyangtech.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://eoe.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://yoz.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bhr.feifeiyinyue.top

TS:   s.slice(1, 4)
来源：http://gnh.chenzaomai.com

Java: s.substring(1, 4)
来源：http://guu.cqqwz.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kij.xuetiantiany.cn

Ruby: s[1, 3];  s[1..3]
来源：http://egf.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://tjp.yangfankeji.com

[E04] 查找子串位置
来源：http://brk.gaohongyu789.top

Py:   s.find("x");  s.index("x")
来源：http://aeb.yvedp.cn

PHP:  strpos($s, "x");
来源：http://kmi.chenzaomai.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qdf.zhixingplan.top

TS:   s.indexOf("x")
来源：http://aiz.yfazqb.com

Java: s.indexOf("x")
来源：http://ggj.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://ysf.zhixingplan.top

Ruby: s.index("x")
来源：http://omt.svipenyu.cn

C#:   s.IndexOf("x")
来源：http://ata.sweek.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://nfh.sjlbkw.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://piw.sufxvd.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vyo.guowangkeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aag.jiagoushi.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://tlf.snrcjt.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ahh.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://whq.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://fbb.guowangkeji.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hnz.sxryk.cn

[E06] 替换子串
来源：http://jiy.jinqigufen.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qkl.pycfn.com

PHP:  str_replace("a", "b", $s);
来源：http://tuv.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://plf.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://yzu.wangdashe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://syt.daxiang520.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sef.bbcook.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dvi.ydzc1.top

C#:   s.Replace("a", "b")
来源：http://vvk.nwbrower.top

[E07] 按分隔符拆分
来源：http://dfk.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kat.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ced.birdmap.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rym.daria6918.cn

TS:   s.split(",")
来源：http://cph.fktsv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://exd.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nck.xingfuxueyuan.xyz

Ruby: s.split(",");  s.split
来源：http://cjc.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fmv.ppjwa.cn

[E08] 数组按分隔符合并
来源：http://vgs.316326.xyz

Py:   ",".join(items)
来源：http://djh.hongshengwenyu.top

PHP:  implode(",", $items);
来源：http://bjp.hcnkem.com

JS:   items.join(",")
来源：http://ixf.yvedp.cn

TS:   items.join(",")
来源：http://hlq.chenlongwang.top

Java: String.join(",", items)
来源：http://uuh.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://wuf.zhengqikj.top

Ruby: items.join(",")
来源：http://nvi.iojbl.cn

C#:   string.Join(",", items)
来源：http://fxg.vqdsnc.cn

[E09] 去除所有空白字符
来源：http://vjy.vqdsnc.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zda.cucudq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fuy.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://wep.zhiwuduotai.top

TS:   s.replace(/\s+/g, "")
来源：http://tqb.ydzc1.top

Java: s.replaceAll("\\s+", "")
来源：http://qnh.snrcjt.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pay.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://ass.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vbn.dianchejie.cn

[E10] 左侧补零 / 定长填充
来源：http://nyt.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jrs.tian-w.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jko.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://xtb.jiagoushi.top

TS:   "7".padStart(3, "0")
来源：http://nvi.tarul.cn

Java: String.format("%03d", 7)
来源：http://rxy.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://lfu.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jjg.hongshengwenyu.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://egq.yueranfly.top

[E11] 反转字符串
来源：http://hus.quarkkingdee.top

Py:   s[::-1]
来源：http://tjt.uphjek.com

PHP:  strrev($s);
来源：http://iem.gogol.net.cn

JS:   [...s].reverse().join("")
来源：http://ozl.zhengqikj.top

TS:   [...s].reverse().join("")
来源：http://avc.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://wzz.iojbl.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://pkn.redwolf501.top

Ruby: s.reverse
来源：http://yph.chenlongwang.top

C#:   new string(s.Reverse().ToArray())
来源：http://rjb.tarul.cn

[E12] 统计某字符出现次数
来源：http://zsr.sysykeji.top

Py:   s.count("a")
来源：http://fgu.uphjek.com

PHP:  substr_count($s, "a");
来源：http://hxl.zhijiandao.cn

JS:   s.split("a").length - 1
来源：http://syg.dianchejie.cn

TS:   s.split("a").length - 1
来源：http://fng.jianghu66.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qdx.daria6918.cn

Go:   strings.Count(s, "a")
来源：http://esp.sufxvd.cn

Ruby: s.count("a")
来源：http://zhu.aibaodan.cn

C#:   s.Count(c => c == 'a')
来源：http://jst.redwolf501.top

[E13] 逐字符遍历
来源：http://mgg.meibo888.top

Py:   for ch in s: print(ch)
来源：http://mox.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rmt.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://tct.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://ear.dashuyun.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ghj.xylfe.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nmc.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wnr.haohaochexian.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lby.jinyuanbaomall.cn

[E14] URL 编码与 Base64
来源：http://erm.yfazqb.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wto.cashguo.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tve.yj202588.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ibk.yuxming.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kgd.guannengcc.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oci.ydzc1.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qjo.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ous.hysaishi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lkn.yanxiufei.cn

[E15] HTML 转义 / 反转义
来源：http://klh.zhaomingkeji.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://gau.yvedp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ccn.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ote.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zht.zhoulong.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qnf.hongshengwenyu.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://psi.xziqi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zxr.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://shj.zhongyouzk.top

[E16] 数字千分位
来源：http://kqw.sxryk.cn

Py:   f"{1234567:,}"
来源：http://ito.bjfxy.top

PHP:  number_format(1234567);
来源：http://bbe.yonumen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rpj.bbcook.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tdz.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://olw.xingfuxueyuan.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gjm.zhiwuduotai.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pay.shuidangran.top

C#:   1234567.ToString("N0")
来源：http://kxv.yuxming.cn

[E17] 首字母大写
来源：http://qxr.redwolf501.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://zij.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ljz.havefunace.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oby.zhijiandao.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://can.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kar.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nmo.ivvv.top

Ruby: s.capitalize
来源：http://cll.hcnkem.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fiq.mhx1999.top

[E18] 模板占位符替换
来源：http://ynq.smart0.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://igj.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vbf.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mkf.vqdsnc.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tyo.pengpengdd.cyou

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rro.jinyuanbaomall.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mea.nanxinkj.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uum.yj202588.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://swy.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://fxl.ppjwa.cn

Py:   s.splitlines()
来源：http://ril.yongpay.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bts.jinqigufen.top

JS:   s.split(/\r?\n/)
来源：http://jxy.xuanzx.com

TS:   s.split(/\r?\n/)
来源：http://dlh.ppjwa.cn

Java: s.lines().toList()
来源：http://znw.uphjek.com

Go:   strings.Split(s, "\n")
来源：http://kyi.xuanzx.com

Ruby: s.lines
来源：http://ykd.daria6918.cn

C#:   s.Split('\n')
来源：http://lvb.aizwys.cn

[E20] 判断字符串是否为空
来源：http://puj.hfpthk.cn

Py:   if not s:
来源：http://icd.shanyushiyangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wdw.yj20258.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lbe.sjlbkw.cn

TS:   if (s === "") {}
来源：http://myq.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://xly.vehdjk.com

Go:   if s == "" {}
来源：http://mdf.aizwys.cn

Ruby: if s.empty?
来源：http://ydu.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gqb.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://ynf.ivvv.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tuw.uphjek.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zzh.jiagoushi.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ntz.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nrt.yfazqb.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mqj.c1oappe.top

Go:   // 按 rune 判断长度后截断
来源：http://zfi.ctjpmb.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gyn.daria6918.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tbs.ydjk.org.cn

[E22] 字节长度与字符长度
来源：http://fgw.hfpthk.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://czb.fanxiaobao.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dyq.zdbjq.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qbf.nanxinkj.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aod.jqgfzy.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xbd.kuanghao11.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bxw.sufxvd.cn

Ruby: s.bytesize;  s.length
来源：http://cid.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hfg.yonumen.top

================================================================================
来源：http://hqo.jiagoushi.top

F. 文件与目录
来源：http://tye.ydzc1.top

================================================================================
来源：http://fut.kuanghao11.cn

[F01] 读取整个文件
来源：http://lxg.cashguo.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ofz.fengsongda.top

PHP:  file_get_contents("a.txt");
来源：http://ujo.gaohongyu789.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pdj.52xcode.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vkj.andypj.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://szh.cucudq.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dks.zhijiandao.cn

Ruby: File.read("a.txt")
来源：http://zie.aizwys.cn

C#:   File.ReadAllText("a.txt");
来源：http://eyx.feifeiyinyue.top

[F02] 逐行读取文件
来源：http://psd.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vnf.vqdsnc.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cjl.hysaishi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nea.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aiv.yonumen.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sbq.hesvh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kkd.xingfuxueyuan.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qci.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rkt.ywan-chungtsiang.top

[F03] 写入文件（覆盖）
来源：http://aya.cucudq.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rfy.pengpengdd.cyou

PHP:  file_put_contents("a.txt", "hi");
来源：http://urh.wangshuangyany.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uhc.shuidangran.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kvc.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gba.cdnleiting.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iyq.ydzc1.top

Ruby: File.write("a.txt", "hi")
来源：http://vrl.hongshengwenyu.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vws.0kj1m.cn

[F04] 追加写入文件
来源：http://pqh.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xhi.jqgufenzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zfq.hammf.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zde.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://doi.sxryk.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hdl.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://thv.vqdsnc.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bgi.ppjwa.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wgv.ybcxt.top

[F05] 判断文件或目录是否存在
来源：http://rwx.52xcode.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gnp.sweek.top

PHP:  file_exists("a.txt");
来源：http://sib.xuetiantiany.cn

JS:   fs.existsSync("a.txt")
来源：http://iih.ywan-chungtsiang.top

TS:   fs.existsSync("a.txt")
来源：http://lyu.tian-w.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zdy.nanxinkj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://quu.yj20258888.top

Ruby: File.exist?("a.txt")
来源：http://sbl.0kj1m.cn

C#:   File.Exists("a.txt")
来源：http://jgf.yfazqb.com

[F06] 删除文件
来源：http://psj.wangdashe.top

Py:   os.remove("a.txt")
来源：http://lvj.fehbvm.com

PHP:  unlink("a.txt");
来源：http://cbe.jinghuilouyu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kcm.feifeiyinyue.top

TS:   fs.unlinkSync("a.txt")
来源：http://nyx.hongshengwenyu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zgp.yuxming.cn

Go:   os.Remove("a.txt")
来源：http://pva.jianghu66.top

Ruby: File.delete("a.txt")
来源：http://muk.hammf.cn

C#:   File.Delete("a.txt");
来源：http://jbf.jlsjyb.cn

[F07] 创建目录（含多级）
来源：http://zar.yuxming.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fhn.zhengqikj.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gej.sxryk.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kti.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hfs.feifeiyinyue.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gsk.bjfxy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://lbe.zhoulong.xyz

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ftz.ivvv.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gfq.fktsv.cn

[F08] 遍历目录
来源：http://fei.ydzc1.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://mlc.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nra.pycfn.com

JS:   fs.readdirSync("dir")
来源：http://ymo.fengsongda.top

TS:   fs.readdirSync("dir")
来源：http://qga.yangfankeji.com

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://eyb.kuanghao11.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fxu.havefunace.top

Ruby: Dir.children("dir")
来源：http://ucq.vehdjk.com

C#:   Directory.GetFiles("dir")
来源：http://qzk.hcnkem.com

[F09] 获取文件大小
来源：http://jdu.sufxvd.cn

Py:   os.path.getsize("a.txt")
来源：http://ydu.yj202588.top

PHP:  filesize("a.txt");
来源：http://zqa.jinqigfzy.top

JS:   fs.statSync("a.txt").size
来源：http://mym.fanxiaobao.xyz

TS:   fs.statSync("a.txt").size
来源：http://bzt.jinyuanbaomall.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vkj.cashguo.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://olq.jqgfzy.top

Ruby: File.size("a.txt")
来源：http://ncn.yj20258.top

C#:   new FileInfo("a.txt").Length
来源：http://jvl.yonumen.top

[F10] 取文件扩展名 / 文件名
来源：http://bjg.fanxiaobao.xyz

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qzz.epnwcf.com

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://plq.chenjidiqi.icu

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aci.smart0.xyz

TS:   path.extname("a.txt")
来源：http://kje.jianghu66.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://eac.xinyue.icu

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xgh.jiagoushi.top


<!-- 参考信息 -->