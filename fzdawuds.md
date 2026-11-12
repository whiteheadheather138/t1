代发 wailian999

Java: String.join(", ", list)
来源：http://qnl.zycfv.cn

Go:   strings.Join(strs, ", ")
来源：http://lne.chenjidiqi.icu

Ruby: arr.join(", ")
来源：http://dog.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://hqu.c1oappe.top

================================================================================
来源：http://uht.jinyuanbaomall.cn

E. 字符串处理
来源：http://plj.hongshengwenyu.top

================================================================================
来源：http://oas.svipenyu.cn

[E01] 拼接字符串
来源：http://nem.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://efm.yongpay.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://nls.guowangkeji.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ein.wangshuangyany.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tsl.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vtk.zycfv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pof.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ebn.jinyuanbaomall.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://awe.52xcode.cn

[E02] 重复字符串
来源：http://yad.yfazqb.com

Py:   "ab" * 3
来源：http://znd.fanxiaobao.xyz

PHP:  str_repeat("ab", 3);
来源：http://wab.jinghuilouyu.cn

JS:   "ab".repeat(3)
来源：http://dmz.ydzc1.top

TS:   "ab".repeat(3)
来源：http://ucu.jqgfzy.top

Java: "ab".repeat(3)
来源：http://lnr.yj20258888.top

Go:   strings.Repeat("ab", 3)
来源：http://xao.shangyingyoupin.top

Ruby: "ab" * 3
来源：http://wkv.yvedp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rre.cdnleiting.top

[E03] 截取子串
来源：http://kwc.cdnleiting.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://akv.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fto.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jkj.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://nni.zdbjq.cn

Java: s.substring(1, 4)
来源：http://uwa.hysaishi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ecr.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://aqg.cqqwz.cn

C#:   s.Substring(1, 3)
来源：http://rns.andypj.xyz

[E04] 查找子串位置
来源：http://lil.cheryme.top

Py:   s.find("x");  s.index("x")
来源：http://eqh.tian-w.cn

PHP:  strpos($s, "x");
来源：http://hij.zhengqikj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rjj.jinqigfzy.top

TS:   s.indexOf("x")
来源：http://ybw.jlsjyb.cn

Java: s.indexOf("x")
来源：http://oao.jyoumei.cn

Go:   strings.Index(s, "x")
来源：http://wfj.smart0.xyz

Ruby: s.index("x")
来源：http://vkw.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://rzq.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://jqz.redwolf501.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mmq.zhengqikj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://apz.jinqigfzy.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pzk.tian-w.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wym.hnxiangtu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hjf.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xau.gaohongyu789.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://urd.ppjwa.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bxs.quarkkingdee.top

[E06] 替换子串
来源：http://rrq.tanke756.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://duu.yongpay.top

PHP:  str_replace("a", "b", $s);
来源：http://xoj.chenzaomai.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fpb.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://jvx.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mbm.bjfxy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wzi.hysaishi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bvt.redwolf501.top

C#:   s.Replace("a", "b")
来源：http://tnb.chenlongwang.top

[E07] 按分隔符拆分
来源：http://tao.tanke756.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uym.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tnn.chenlongwang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://vdd.fengsongda.top

TS:   s.split(",")
来源：http://bav.zhongyouzk.top

Java: s.split(",");  s.split("\\s+")
来源：http://vtl.andypj.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zwc.tianlin.xyz

Ruby: s.split(",");  s.split
来源：http://aqd.chenjidiqi.icu

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uee.tarul.cn

[E08] 数组按分隔符合并
来源：http://mog.fengsongda.top

Py:   ",".join(items)
来源：http://rtj.yj202588.top

PHP:  implode(",", $items);
来源：http://dna.yongpay.top

JS:   items.join(",")
来源：http://kqg.vqdsnc.cn

TS:   items.join(",")
来源：http://bwb.pycfn.com

Java: String.join(",", items)
来源：http://nbh.fanxiaobao.xyz

Go:   strings.Join(items, ",")
来源：http://jat.quarkkingdee.top

Ruby: items.join(",")
来源：http://brm.mhx1999.top

C#:   string.Join(",", items)
来源：http://qta.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://fnv.gzhubu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wib.hammf.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mhi.316326.xyz

JS:   s.replace(/\s+/g, "")
来源：http://ouq.yfazqb.com

TS:   s.replace(/\s+/g, "")
来源：http://von.vehdjk.com

Java: s.replaceAll("\\s+", "")
来源：http://png.fanxiaobao.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://wwd.yfazqb.com

Ruby: s.gsub(/\s+/, "")
来源：http://iqv.shzxlz.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://aje.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://tkl.hywenlv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mpk.ehwqpu.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wjq.cqqwz.cn

JS:   "7".padStart(3, "0")
来源：http://lhd.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://uiw.nanxuanxn.top

Java: String.format("%03d", 7)
来源：http://tdy.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pmm.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fal.0kj1m.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://him.chenjidiqi.icu

[E11] 反转字符串
来源：http://iwt.jqgufenzy.top

Py:   s[::-1]
来源：http://pmx.jlsjyb.cn

PHP:  strrev($s);
来源：http://dax.xingfuxueyuan.xyz

JS:   [...s].reverse().join("")
来源：http://itt.ybcxt.top

TS:   [...s].reverse().join("")
来源：http://szk.fanxiaobao.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://opt.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qvq.cheryme.top

Ruby: s.reverse
来源：http://mdy.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://iom.xylfe.cn

[E12] 统计某字符出现次数
来源：http://fkg.jqgfzy.top

Py:   s.count("a")
来源：http://wbu.zhaomingkeji.xyz

PHP:  substr_count($s, "a");
来源：http://dts.tarul.cn

JS:   s.split("a").length - 1
来源：http://hrk.xuanzx.com

TS:   s.split("a").length - 1
来源：http://nzl.tian-w.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wfw.meibo888.top

Go:   strings.Count(s, "a")
来源：http://ldq.hfpthk.cn

Ruby: s.count("a")
来源：http://cbw.quarkkingdee.top

C#:   s.Count(c => c == 'a')
来源：http://qpc.yangfankeji.com

[E13] 逐字符遍历
来源：http://mbj.cdnleiting.top

Py:   for ch in s: print(ch)
来源：http://vwo.feifeiyinyue.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://far.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hoi.tianlin.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://xfg.zdqjudy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sga.gotoacloud.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://naj.hongshengwenyu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iad.uphjek.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zea.jinghuilouyu.cn

[E14] URL 编码与 Base64
来源：http://izx.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hbt.hysaishi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jsm.sweek.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gws.52xcode.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dkp.pycfn.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jav.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nhy.fehbvm.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qhu.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xxg.yj20258888.top

[E15] HTML 转义 / 反转义
来源：http://reg.chenjidiqi.icu

Py:   html.escape(s);  html.unescape(s)
来源：http://zgj.fanxiaobao.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://elc.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://weq.hnqzz.top

TS:   // 同上，务必做 XSS 过滤
来源：http://dbg.zdbjq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zyb.wangdashe.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uny.daria6918.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fis.sxryk.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fxl.aizwys.cn

[E16] 数字千分位
来源：http://fcn.hammf.cn

Py:   f"{1234567:,}"
来源：http://bix.yanxiufei.cn

PHP:  number_format(1234567);
来源：http://xza.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jwr.hongshengwenyu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://xve.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xts.yj20258.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://itj.fengsongda.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://prz.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://uua.fehbvm.com

[E17] 首字母大写
来源：http://rap.chenlongwang.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bgv.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ogi.pengpengdd.cyou

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vqf.zdbjq.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rfk.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kxn.zhongyouzk.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rio.svipenyu.cn

Ruby: s.capitalize
来源：http://kvo.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zwd.jinqigufen.top

[E18] 模板占位符替换
来源：http://pha.haohaochexian.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xmn.yongpay.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gnz.yj20258.top

JS:   tpl.replaceAll("{name}", name)
来源：http://nck.hcnkem.com

TS:   tpl.replaceAll("{name}", name)
来源：http://vgn.ydjk.org.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jwz.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://fad.uphjek.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zrj.jinyuanbaomall.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ryc.kuanghao11.cn

[E19] 多行文本按行拆分
来源：http://vyk.xinyue.icu

Py:   s.splitlines()
来源：http://bca.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ozu.kuanghao11.cn

JS:   s.split(/\r?\n/)
来源：http://cer.316326.xyz

TS:   s.split(/\r?\n/)
来源：http://jhw.fengsongda.top

Java: s.lines().toList()
来源：http://rfi.ehwqpu.com

Go:   strings.Split(s, "\n")
来源：http://cif.jinghuilouyu.cn

Ruby: s.lines
来源：http://xpn.andypj.xyz

C#:   s.Split('\n')
来源：http://grg.daria6918.cn

[E20] 判断字符串是否为空
来源：http://squ.havefunace.top

Py:   if not s:
来源：http://cmm.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lme.vqdsnc.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wbd.52xcode.cn

TS:   if (s === "") {}
来源：http://kim.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://ppy.jiagoushi.top

Go:   if s == "" {}
来源：http://wbq.gaohongyu789.top

Ruby: if s.empty?
来源：http://ftr.ctjpmb.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kuc.0kj1m.cn

[E21] 超长截断加省略号
来源：http://tkq.ehwqpu.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bqg.andypj.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fro.sjlbkw.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ybd.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wna.uphjek.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uho.zhaomingkeji.xyz

Go:   // 按 rune 判断长度后截断
来源：http://axp.zdqjudy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tnt.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gsn.hongshengwenyu.top

[E22] 字节长度与字符长度
来源：http://jdq.yvedp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fuy.hesvh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://siu.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fpl.xziqi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gri.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lsg.shangyingyoupin.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mcz.kuanghao11.cn

Ruby: s.bytesize;  s.length
来源：http://zix.yanxiufei.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lhk.gotoacloud.top

================================================================================
来源：http://vrg.mhx1999.top

F. 文件与目录
来源：http://dfu.pengpengdd.cyou

================================================================================
来源：http://hkp.zycfv.cn

[F01] 读取整个文件
来源：http://tng.nanxuanxn.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xur.yj20258888.top

PHP:  file_get_contents("a.txt");
来源：http://dvq.sufxvd.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qmv.shuidangran.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bui.ppjwa.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zgj.tianlin.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ixp.zycfv.cn

Ruby: File.read("a.txt")
来源：http://yzb.yueranfly.top

C#:   File.ReadAllText("a.txt");
来源：http://ctb.cheryme.top

[F02] 逐行读取文件
来源：http://czi.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xmg.zhixingplan.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jco.hesvh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ohj.meibo888.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wxn.xuanzx.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://loj.xuetiantiany.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://auw.ivvv.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yom.hongshengwenyu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://byc.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://hpj.shuidangran.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kct.uphjek.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://wnd.smart0.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yqt.yj20258.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nws.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qsd.tianlin.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zqt.xinyue.icu

Ruby: File.write("a.txt", "hi")
来源：http://kal.zhaomingkeji.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://igl.ctjpmb.com

[F04] 追加写入文件
来源：http://irb.cashguo.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gkg.jiagoushi.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ieq.yuanzhike.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hha.jyoumei.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pay.hysaishi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ykj.cheryme.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://soe.gotoacloud.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tvc.xuetiantiany.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xxl.hcnkem.com

[F05] 判断文件或目录是否存在
来源：http://kwv.jiagoushi.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hwg.xingfuxueyuan.xyz

PHP:  file_exists("a.txt");
来源：http://mxz.jqgufenzy.top

JS:   fs.existsSync("a.txt")
来源：http://dzq.cucudq.cn

TS:   fs.existsSync("a.txt")
来源：http://rfq.sysykeji.top

Java: Files.exists(Path.of("a.txt"))
来源：http://oey.bjfxy.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://olp.9152youxi.cn

Ruby: File.exist?("a.txt")
来源：http://rcn.ydzc1.top

C#:   File.Exists("a.txt")
来源：http://row.tianlin.xyz

[F06] 删除文件
来源：http://zxg.snrcjt.cn

Py:   os.remove("a.txt")
来源：http://pdw.hcnkem.com

PHP:  unlink("a.txt");
来源：http://nej.jinqigfzy.top

JS:   fs.unlinkSync("a.txt")
来源：http://mno.yanxiufei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xvt.gogol.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dcr.yonumen.top

Go:   os.Remove("a.txt")
来源：http://usm.hysaishi.cn

Ruby: File.delete("a.txt")
来源：http://qcl.hongshengwenyu.top

C#:   File.Delete("a.txt");
来源：http://bjl.hywenlv.cn

[F07] 创建目录（含多级）
来源：http://qxg.sweek.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zov.shangyingyoupin.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nhq.yvedp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zcy.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xlq.ydjk.org.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yjn.316326.xyz

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jyg.cheryme.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bks.ctjpmb.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://emr.smart0.xyz

[F08] 遍历目录
来源：http://txy.zdbjq.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rlk.jianghu66.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gry.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://aub.gotoacloud.top

TS:   fs.readdirSync("dir")
来源：http://cdv.vqdsnc.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://utz.c1oappe.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://xnj.jinghuilouyu.cn

Ruby: Dir.children("dir")
来源：http://zbg.shanyushiyangtech.top

C#:   Directory.GetFiles("dir")
来源：http://mwe.yfazqb.com

[F09] 获取文件大小
来源：http://opt.fengsongda.top

Py:   os.path.getsize("a.txt")
来源：http://jze.tian-w.cn

PHP:  filesize("a.txt");
来源：http://cnh.yvedp.cn

JS:   fs.statSync("a.txt").size
来源：http://xqk.guowangkeji.top

TS:   fs.statSync("a.txt").size
来源：http://vhj.shanyushiyangtech.top

Java: Files.size(Path.of("a.txt"))
来源：http://zuo.hnxiangtu.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dvk.chenlongwang.top

Ruby: File.size("a.txt")
来源：http://iqx.zhaomingkeji.xyz

C#:   new FileInfo("a.txt").Length
来源：http://ryg.jiagoushi.top

[F10] 取文件扩展名 / 文件名
来源：http://wtc.pycfn.com

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://arv.hfpthk.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fqk.jqgufenzy.top

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rcx.c1oappe.top

TS:   path.extname("a.txt")
来源：http://xwt.dianchejie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mno.cucudq.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gqy.zhaomingkeji.xyz

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://iyr.hnqzz.top

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sxa.shanyushiyangtech.top

[F11] 复制与移动文件
来源：http://bmq.gaohongyu789.top

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://exh.hywenlv.cn


<!-- 参考信息 -->