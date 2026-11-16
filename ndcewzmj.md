代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://qzt.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://xfn.yj20258.top

JS:   arr.join(", ")
来源：http://naz.yj20258888.top

TS:   arr.join(", ")
来源：http://rgc.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://bfh.jinyuanbaomall.cn

Go:   strings.Join(strs, ", ")
来源：http://php.gzhubu.top

Ruby: arr.join(", ")
来源：http://uer.gaohongyu789.top

C#:   string.Join(", ", list)
来源：http://aqg.jinqigfzy.top

================================================================================
来源：http://hpb.svipenyu.cn

E. 字符串处理
来源：http://tej.chenzaomai.com

================================================================================
来源：http://hip.shuidangran.top

[E01] 拼接字符串
来源：http://xii.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ivi.pycfn.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nqn.snrcjt.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dwo.ctjpmb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jcq.sxryk.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://txb.mhx1999.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jlv.yanxiufei.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uul.xinyue.icu

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gho.c1oappe.top

[E02] 重复字符串
来源：http://zcm.cdnleiting.top

Py:   "ab" * 3
来源：http://ryd.yvedp.cn

PHP:  str_repeat("ab", 3);
来源：http://tfv.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://pwg.zdbjq.cn

TS:   "ab".repeat(3)
来源：http://yvu.tanke756.top

Java: "ab".repeat(3)
来源：http://qfl.cashguo.top

Go:   strings.Repeat("ab", 3)
来源：http://tsc.yongpay.top

Ruby: "ab" * 3
来源：http://mfa.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ztv.hywenlv.cn

[E03] 截取子串
来源：http://itb.wangdashe.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pmq.zhiwuduotai.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hxf.hcnkem.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://boc.gaohongyu789.top

TS:   s.slice(1, 4)
来源：http://eea.cqqwz.cn

Java: s.substring(1, 4)
来源：http://gjm.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xht.jinghuilouyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iku.hfpthk.cn

C#:   s.Substring(1, 3)
来源：http://utd.bbcook.cn

[E04] 查找子串位置
来源：http://smu.mhx1999.top

Py:   s.find("x");  s.index("x")
来源：http://uvb.fengsongda.top

PHP:  strpos($s, "x");
来源：http://uom.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://avu.jinghuilouyu.cn

TS:   s.indexOf("x")
来源：http://aqy.hnxiangtu.top

Java: s.indexOf("x")
来源：http://qnd.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://ghi.ppjwa.cn

Ruby: s.index("x")
来源：http://qtk.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://fku.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://grv.yuanzhike.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uvz.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yuv.yueranfly.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pcg.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://dky.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cvz.kuanghao11.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bdj.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ycp.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mwd.cdnleiting.top

[E06] 替换子串
来源：http://fxd.redwolf501.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://quc.ydzc1.top

PHP:  str_replace("a", "b", $s);
来源：http://boj.wangdashe.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://des.birdmap.top

TS:   s.replaceAll("a", "b")
来源：http://lpy.redwolf501.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gqf.hesvh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nhx.jianghu66.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://eqc.fanxiaobao.xyz

C#:   s.Replace("a", "b")
来源：http://wqg.kuanghao11.cn

[E07] 按分隔符拆分
来源：http://pin.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://roy.yj202588.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dbn.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://kua.yj20258.top

TS:   s.split(",")
来源：http://rxu.zhixingplan.top

Java: s.split(",");  s.split("\\s+")
来源：http://dag.yongpay.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ygg.xuanzx.com

Ruby: s.split(",");  s.split
来源：http://kpa.smart0.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kbu.c1oappe.top

[E08] 数组按分隔符合并
来源：http://niw.epnwcf.com

Py:   ",".join(items)
来源：http://zxa.tarul.cn

PHP:  implode(",", $items);
来源：http://yly.nwbrower.top

JS:   items.join(",")
来源：http://elw.jyoumei.cn

TS:   items.join(",")
来源：http://vzk.nanxuanxn.top

Java: String.join(",", items)
来源：http://wmc.316326.xyz

Go:   strings.Join(items, ",")
来源：http://ulu.sjlbkw.cn

Ruby: items.join(",")
来源：http://bmq.birdmap.top

C#:   string.Join(",", items)
来源：http://lrp.zhijiandao.cn

[E09] 去除所有空白字符
来源：http://rnx.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://tiv.nanxinkj.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rly.uphjek.com

JS:   s.replace(/\s+/g, "")
来源：http://awn.yj202588.top

TS:   s.replace(/\s+/g, "")
来源：http://ybk.zhixingplan.top

Java: s.replaceAll("\\s+", "")
来源：http://azn.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://yso.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://hvf.jqgufenzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cqf.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://tvm.gogol.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ooy.xylfe.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gzr.zdbjq.cn

JS:   "7".padStart(3, "0")
来源：http://tkl.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://pgq.cqqwz.cn

Java: String.format("%03d", 7)
来源：http://yqw.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xfb.dashuyun.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qom.shanyushiyangtech.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kwt.ywan-chungtsiang.top

[E11] 反转字符串
来源：http://umm.tianlin.xyz

Py:   s[::-1]
来源：http://rje.nanxinkj.top

PHP:  strrev($s);
来源：http://bxw.mhx1999.top

JS:   [...s].reverse().join("")
来源：http://otb.jiagoushi.top

TS:   [...s].reverse().join("")
来源：http://qbw.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vhr.xingfuxueyuan.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://tuq.uphjek.com

Ruby: s.reverse
来源：http://kwk.yj20258888.top

C#:   new string(s.Reverse().ToArray())
来源：http://iwj.aizwys.cn

[E12] 统计某字符出现次数
来源：http://vff.quarkkingdee.top

Py:   s.count("a")
来源：http://rzi.fengsongda.top

PHP:  substr_count($s, "a");
来源：http://sza.ybcxt.top

JS:   s.split("a").length - 1
来源：http://aii.tian-w.cn

TS:   s.split("a").length - 1
来源：http://cyi.chenlongwang.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gwo.shuidangran.top

Go:   strings.Count(s, "a")
来源：http://fbe.ehwqpu.com

Ruby: s.count("a")
来源：http://yht.yj202588.top

C#:   s.Count(c => c == 'a')
来源：http://sxz.haohaochexian.top

[E13] 逐字符遍历
来源：http://jga.jiagoushi.top

Py:   for ch in s: print(ch)
来源：http://owr.9152youxi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pho.chenzaomai.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://evy.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oxi.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ezf.yueranfly.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xna.316326.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://kte.vqdsnc.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rda.vqdsnc.cn

[E14] URL 编码与 Base64
来源：http://psi.fktsv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://njz.redwolf501.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kxr.cheryme.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dbj.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tro.fanxiaobao.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://doj.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vun.yj20258.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ujc.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vkj.uphjek.com

[E15] HTML 转义 / 反转义
来源：http://ptt.wangshuangyany.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dfr.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nhm.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ett.kuanghao11.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bkn.hywenlv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tgj.c1oappe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gbb.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gey.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nzk.aizwys.cn

[E16] 数字千分位
来源：http://qxk.fanxiaobao.xyz

Py:   f"{1234567:,}"
来源：http://mis.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://xrr.guannengcc.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ajv.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://srl.jqgfzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bho.sysykeji.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ahy.uphjek.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jvx.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://nkn.hysaishi.cn

[E17] 首字母大写
来源：http://mpd.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mak.uphjek.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://sjr.redwolf501.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jrb.guowangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ghg.dianchejie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hcx.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://etx.meibo888.top

Ruby: s.capitalize
来源：http://uik.ydjk.org.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://naj.birdmap.top

[E18] 模板占位符替换
来源：http://joz.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rrb.daxiang520.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zcc.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://xts.shanyushiyangtech.top

TS:   tpl.replaceAll("{name}", name)
来源：http://gme.birdmap.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rfl.yanxiufei.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cfk.chenlongwang.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qcf.gogol.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://veg.jlsjyb.cn

[E19] 多行文本按行拆分
来源：http://fnd.yuanzhike.top

Py:   s.splitlines()
来源：http://vnk.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fbx.bjfxy.top

JS:   s.split(/\r?\n/)
来源：http://dgd.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://uyc.yonumen.top

Java: s.lines().toList()
来源：http://yqq.yvedp.cn

Go:   strings.Split(s, "\n")
来源：http://ptt.vehdjk.com

Ruby: s.lines
来源：http://qpc.jqgufenzy.top

C#:   s.Split('\n')
来源：http://ksc.sysykeji.top

[E20] 判断字符串是否为空
来源：http://yqh.zhijiandao.cn

Py:   if not s:
来源：http://emd.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zsc.zhijiandao.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qcj.yfazqb.com

TS:   if (s === "") {}
来源：http://qer.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://ijo.jinyuanbaomall.cn

Go:   if s == "" {}
来源：http://gag.svipenyu.cn

Ruby: if s.empty?
来源：http://fcf.tanke756.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qqz.yj20258.top

[E21] 超长截断加省略号
来源：http://yar.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ugm.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eyv.zhengqikj.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://spu.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fdr.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rcq.guannengcc.top

Go:   // 按 rune 判断长度后截断
来源：http://khw.sxryk.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bgn.hammf.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kiq.jiagoushi.top

[E22] 字节长度与字符长度
来源：http://kzn.gaohongyu789.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ewx.xuanzx.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nqw.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://awl.hnxiangtu.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ptl.sysykeji.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tdv.xylfe.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vdf.hammf.cn

Ruby: s.bytesize;  s.length
来源：http://yoi.0kj1m.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ctv.gzhubu.top

================================================================================
来源：http://wkt.52xcode.cn

F. 文件与目录
来源：http://teq.cucudq.cn

================================================================================
来源：http://dnw.gogol.net.cn

[F01] 读取整个文件
来源：http://vdf.yangfankeji.com

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uyu.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://uou.nanxuanxn.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jjt.pycfn.com

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qlc.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://yck.jiagoushi.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kmr.cdnleiting.top

Ruby: File.read("a.txt")
来源：http://zvm.hesvh.cn

C#:   File.ReadAllText("a.txt");
来源：http://vzv.sweek.top

[F02] 逐行读取文件
来源：http://ihb.shzxlz.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vix.shangyingyoupin.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xsf.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://otg.dashuyun.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ang.redwolf501.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ngc.shanyushiyangkeji.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mks.jinqigfzy.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://txa.kuanghao11.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://uea.zhaomingkeji.xyz

[F03] 写入文件（覆盖）
来源：http://ttr.ybcxt.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zqr.guannengcc.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jah.yongpay.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ntw.fanxiaobao.xyz

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qne.hywenlv.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://glk.xziqi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jfx.meibo888.top

Ruby: File.write("a.txt", "hi")
来源：http://puf.316326.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://udk.feifeiyinyue.top

[F04] 追加写入文件
来源：http://xax.jinyuanbaomall.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jjy.chenlongwang.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lyv.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vgb.tarul.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fev.zhixingplan.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rqj.fengsongda.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fbw.zhiwuduotai.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qxi.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lvc.cucudq.cn

[F05] 判断文件或目录是否存在
来源：http://ycm.nanxuanxn.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://aon.jyoumei.cn

PHP:  file_exists("a.txt");
来源：http://sos.xylfe.cn

JS:   fs.existsSync("a.txt")
来源：http://iia.fengsongda.top

TS:   fs.existsSync("a.txt")
来源：http://bao.ybcxt.top

Java: Files.exists(Path.of("a.txt"))
来源：http://qsf.ywan-chungtsiang.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://drx.bbcook.cn

Ruby: File.exist?("a.txt")
来源：http://gom.yonumen.top

C#:   File.Exists("a.txt")
来源：http://jql.sysykeji.top

[F06] 删除文件
来源：http://jyw.fehbvm.com

Py:   os.remove("a.txt")
来源：http://ipy.smart0.xyz

PHP:  unlink("a.txt");
来源：http://zqu.snrcjt.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eeg.vqdsnc.cn

TS:   fs.unlinkSync("a.txt")
来源：http://doj.sufxvd.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ppu.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://qvd.ivvv.top

Ruby: File.delete("a.txt")
来源：http://hov.mhx1999.top

C#:   File.Delete("a.txt");
来源：http://upw.fanxiaobao.xyz

[F07] 创建目录（含多级）
来源：http://fbv.jlsjyb.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vxq.hysaishi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://khm.fehbvm.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uqj.jinghuilouyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://oyr.havefunace.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nbc.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zva.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qnu.hesvh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nvz.jqgufenzy.top

[F08] 遍历目录
来源：http://cwv.52xcode.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tio.sufxvd.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://udy.haohaochexian.top

JS:   fs.readdirSync("dir")
来源：http://bpx.jianghu66.top

TS:   fs.readdirSync("dir")
来源：http://tbj.zhixingplan.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dig.wangshuangyany.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ejp.shanyushiyangtech.top

Ruby: Dir.children("dir")
来源：http://zbh.aibaodan.cn

C#:   Directory.GetFiles("dir")
来源：http://eoo.cucudq.cn

[F09] 获取文件大小
来源：http://hln.meibo888.top

Py:   os.path.getsize("a.txt")
来源：http://oqq.xuetiantiany.cn

PHP:  filesize("a.txt");
来源：http://tpr.zhixingplan.top

JS:   fs.statSync("a.txt").size
来源：http://pzx.pengpengdd.cyou

TS:   fs.statSync("a.txt").size
来源：http://rne.hcnkem.com

Java: Files.size(Path.of("a.txt"))
来源：http://ozy.shzxlz.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://toe.redwolf501.top

Ruby: File.size("a.txt")
来源：http://bny.cucudq.cn

C#:   new FileInfo("a.txt").Length
来源：http://uez.yueranfly.top

[F10] 取文件扩展名 / 文件名
来源：http://yib.tian-w.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sty.zdbjq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lev.52xcode.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hmo.hcnkem.com

TS:   path.extname("a.txt")
来源：http://hzx.zhiwuduotai.top

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ose.gogol.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lbg.ybcxt.top


<!-- 参考信息 -->