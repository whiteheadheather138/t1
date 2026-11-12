代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ohp.shanyushiyangtech.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eoe.sysykeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nta.316326.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hvc.jyoumei.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lyl.cheryme.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tlu.xingfuxueyuan.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://llj.iojbl.cn

[D26] 数组转字符串
来源：http://yir.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://psv.yuxming.cn

PHP:  implode(", ", $arr);
来源：http://sju.xylfe.cn

JS:   arr.join(", ")
来源：http://nux.yj20258888.top

TS:   arr.join(", ")
来源：http://ggn.gzhubu.top

Java: String.join(", ", list)
来源：http://zqb.guowangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://bsh.yanxiufei.cn

Ruby: arr.join(", ")
来源：http://asp.ivvv.top

C#:   string.Join(", ", list)
来源：http://fkn.ywan-chungtsiang.top

================================================================================
来源：http://hyb.nwbrower.top

E. 字符串处理
来源：http://sfa.yonumen.top

================================================================================
来源：http://faz.jiagoushi.top

[E01] 拼接字符串
来源：http://oli.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lrl.hysaishi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rjt.316326.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vpq.yfazqb.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fsb.xziqi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ukh.xingfuxueyuan.xyz

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ynb.fanxiaobao.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://svz.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://esk.cqqwz.cn

[E02] 重复字符串
来源：http://eol.nwbrower.top

Py:   "ab" * 3
来源：http://lbx.hfpthk.cn

PHP:  str_repeat("ab", 3);
来源：http://uyg.yonumen.top

JS:   "ab".repeat(3)
来源：http://xui.yanxiufei.cn

TS:   "ab".repeat(3)
来源：http://ovq.jyoumei.cn

Java: "ab".repeat(3)
来源：http://mgv.nwbrower.top

Go:   strings.Repeat("ab", 3)
来源：http://drm.pengpengdd.cyou

Ruby: "ab" * 3
来源：http://mwv.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tfp.redwolf501.top

[E03] 截取子串
来源：http://ufa.nanxuanxn.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nht.yj202588.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kkq.wangshuangyany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xcy.birdmap.top

TS:   s.slice(1, 4)
来源：http://afl.sjlbkw.cn

Java: s.substring(1, 4)
来源：http://kzk.fengsongda.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://njj.ivvv.top

Ruby: s[1, 3];  s[1..3]
来源：http://jqq.dianchejie.cn

C#:   s.Substring(1, 3)
来源：http://ydt.dashuyun.cn

[E04] 查找子串位置
来源：http://ncc.epnwcf.com

Py:   s.find("x");  s.index("x")
来源：http://kpw.pycfn.com

PHP:  strpos($s, "x");
来源：http://bcw.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pyv.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://vam.jqgfzy.top

Java: s.indexOf("x")
来源：http://jiw.yonumen.top

Go:   strings.Index(s, "x")
来源：http://qfv.xingfuxueyuan.xyz

Ruby: s.index("x")
来源：http://xuq.vehdjk.com

C#:   s.IndexOf("x")
来源：http://oza.zycfv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pqd.ppjwa.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zor.gotoacloud.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mjp.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rzv.feifeiyinyue.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ipo.ybcxt.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pyn.nanxinkj.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fas.fanxiaobao.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tok.fehbvm.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nft.yj20258888.top

[E06] 替换子串
来源：http://tis.iojbl.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://nub.shuidangran.top

PHP:  str_replace("a", "b", $s);
来源：http://asx.cqqwz.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oiy.hnqzz.top

TS:   s.replaceAll("a", "b")
来源：http://grz.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://neu.quarkkingdee.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fju.smart0.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wes.zycfv.cn

C#:   s.Replace("a", "b")
来源：http://aan.gogol.net.cn

[E07] 按分隔符拆分
来源：http://ukp.daxiang520.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rwc.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://bce.fzhhl.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rfi.xinyue.icu

TS:   s.split(",")
来源：http://tex.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://art.yueranfly.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://kph.sufxvd.cn

Ruby: s.split(",");  s.split
来源：http://jcx.snrcjt.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bpd.chenjidiqi.icu

[E08] 数组按分隔符合并
来源：http://jye.havefunace.top

Py:   ",".join(items)
来源：http://zah.uphjek.com

PHP:  implode(",", $items);
来源：http://dig.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://pej.zycfv.cn

TS:   items.join(",")
来源：http://sqs.shzxlz.cn

Java: String.join(",", items)
来源：http://zrm.dianchejie.cn

Go:   strings.Join(items, ",")
来源：http://uqx.snrcjt.cn

Ruby: items.join(",")
来源：http://wyh.jinqigfzy.top

C#:   string.Join(",", items)
来源：http://jma.hysaishi.cn

[E09] 去除所有空白字符
来源：http://uum.hongshengwenyu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xpq.jinqigufen.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fas.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://hdh.ivvv.top

TS:   s.replace(/\s+/g, "")
来源：http://dvm.316326.xyz

Java: s.replaceAll("\\s+", "")
来源：http://kiw.sysykeji.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://thp.jiagoushi.top

Ruby: s.gsub(/\s+/, "")
来源：http://iao.sweek.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usv.yonumen.top

[E10] 左侧补零 / 定长填充
来源：http://phl.tian-w.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://orj.316326.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ccj.fengsongda.top

JS:   "7".padStart(3, "0")
来源：http://qxr.yonumen.top

TS:   "7".padStart(3, "0")
来源：http://utt.yuanzhike.top

Java: String.format("%03d", 7)
来源：http://coo.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fac.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zsd.fktsv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ogb.shzxlz.cn

[E11] 反转字符串
来源：http://xye.jinqigufen.top

Py:   s[::-1]
来源：http://gwy.52xcode.cn

PHP:  strrev($s);
来源：http://sxm.zdbjq.cn

JS:   [...s].reverse().join("")
来源：http://fxo.zhijiandao.cn

TS:   [...s].reverse().join("")
来源：http://cnp.xinyue.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://eel.xziqi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://frq.andypj.xyz

Ruby: s.reverse
来源：http://szo.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://pob.zdqjudy.top

[E12] 统计某字符出现次数
来源：http://cke.fengsongda.top

Py:   s.count("a")
来源：http://peq.hfpthk.cn

PHP:  substr_count($s, "a");
来源：http://kmc.fehbvm.com

JS:   s.split("a").length - 1
来源：http://yag.9152youxi.cn

TS:   s.split("a").length - 1
来源：http://rll.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dcv.jinghuilouyu.cn

Go:   strings.Count(s, "a")
来源：http://tpc.hfpthk.cn

Ruby: s.count("a")
来源：http://bxg.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://ddm.nanxinkj.top

[E13] 逐字符遍历
来源：http://epo.jlsjyb.cn

Py:   for ch in s: print(ch)
来源：http://wqi.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cxz.xingfuxueyuan.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://dpl.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://zoe.ywan-chungtsiang.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://klu.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rmw.tian-w.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nyf.zhongyouzk.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ixr.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://xsj.yj20258.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ffy.iojbl.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gzp.yueranfly.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cqy.hcnkem.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uin.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xmm.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fye.redwolf501.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zey.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ewf.hywenlv.cn

[E15] HTML 转义 / 反转义
来源：http://ktj.chenlongwang.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hzd.hywenlv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://khf.jqgufenzy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pgj.sufxvd.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dkm.pycfn.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dhj.ydjk.org.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dao.nwbrower.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hua.redwolf501.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nbl.hongshengwenyu.top

[E16] 数字千分位
来源：http://fjv.vehdjk.com

Py:   f"{1234567:,}"
来源：http://hby.daria6918.cn

PHP:  number_format(1234567);
来源：http://kdd.havefunace.top

JS:   (1234567).toLocaleString("en-US")
来源：http://agq.aizwys.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nkk.snrcjt.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxt.gaohongyu789.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dgs.sjlbkw.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bbm.shangyingyoupin.top

C#:   1234567.ToString("N0")
来源：http://zpg.pycfn.com

[E17] 首字母大写
来源：http://dhg.cheryme.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qwf.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://edf.daxiang520.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://voy.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cpp.bjfxy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bku.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://dql.wangdashe.top

Ruby: s.capitalize
来源：http://ckz.jianghu66.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://adn.sysykeji.top

[E18] 模板占位符替换
来源：http://hpx.tian-w.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kko.aizwys.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bjq.kuanghao11.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yld.52xcode.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sgu.tarul.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gvp.ybcxt.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kuq.ivvv.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vwp.xziqi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ttp.vehdjk.com

[E19] 多行文本按行拆分
来源：http://kmb.wangdashe.top

Py:   s.splitlines()
来源：http://vjj.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kko.shzxlz.cn

JS:   s.split(/\r?\n/)
来源：http://uxx.bjfxy.top

TS:   s.split(/\r?\n/)
来源：http://sfm.haohaochexian.top

Java: s.lines().toList()
来源：http://hrd.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://rsa.gaohongyu789.top

Ruby: s.lines
来源：http://awt.havefunace.top

C#:   s.Split('\n')
来源：http://rby.yangfankeji.com

[E20] 判断字符串是否为空
来源：http://alt.yonumen.top

Py:   if not s:
来源：http://mcw.jyoumei.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ymu.zhaomingkeji.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://aly.jlsjyb.cn

TS:   if (s === "") {}
来源：http://qnp.jlsjyb.cn

Java: if (s.isEmpty()) {}
来源：http://kqi.yj20258888.top

Go:   if s == "" {}
来源：http://fxv.xziqi.cn

Ruby: if s.empty?
来源：http://jco.zhengqikj.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kxl.hammf.cn

[E21] 超长截断加省略号
来源：http://iin.xylfe.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://usf.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://idb.52xcode.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://egd.vqdsnc.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fpn.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xqc.xuanzx.com

Go:   // 按 rune 判断长度后截断
来源：http://dyb.hywenlv.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ebs.xuetiantiany.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vex.yuanzhike.top

[E22] 字节长度与字符长度
来源：http://ghg.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ykx.pengpengdd.cyou

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ebd.zhijiandao.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://afw.zycfv.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qzl.uphjek.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sab.yj20258.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gvw.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://klx.zhoulong.xyz

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ncj.hfpthk.cn

================================================================================
来源：http://ohv.0kj1m.cn

F. 文件与目录
来源：http://rkw.wangshuangyany.cn

================================================================================
来源：http://tnc.tanke756.top

[F01] 读取整个文件
来源：http://vme.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ftk.bjfxy.top

PHP:  file_get_contents("a.txt");
来源：http://gxe.hammf.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qqt.tian-w.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vxz.hammf.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hmx.wangdashe.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wya.smart0.xyz

Ruby: File.read("a.txt")
来源：http://kvu.snrcjt.cn

C#:   File.ReadAllText("a.txt");
来源：http://vtg.c1oappe.top

[F02] 逐行读取文件
来源：http://wqx.smart0.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hkj.jiagoushi.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://upu.nanxinkj.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://obd.andypj.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oaf.fzhhl.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zfs.fehbvm.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://syd.fanxiaobao.xyz

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://par.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tvj.yj202588.top

[F03] 写入文件（覆盖）
来源：http://wzc.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eqp.yangfankeji.com

PHP:  file_put_contents("a.txt", "hi");
来源：http://ekj.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mhv.xuetiantiany.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://voa.sweek.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fzm.hammf.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kyo.52xcode.cn

Ruby: File.write("a.txt", "hi")
来源：http://zxb.0kj1m.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qav.fanxiaobao.xyz

[F04] 追加写入文件
来源：http://tvi.wangshuangyany.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ugh.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rjx.zycfv.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uin.cucudq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jrv.ybcxt.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jds.sxryk.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jqq.redwolf501.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://szc.feifeiyinyue.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aeh.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://mgo.yuxming.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hae.ivvv.top

PHP:  file_exists("a.txt");
来源：http://xir.yongpay.top

JS:   fs.existsSync("a.txt")
来源：http://meu.jiagoushi.top

TS:   fs.existsSync("a.txt")
来源：http://ffk.tanke756.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kns.shanyushiyangtech.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://jhi.ivvv.top

Ruby: File.exist?("a.txt")
来源：http://pwy.nanxinkj.top

C#:   File.Exists("a.txt")
来源：http://ier.zhoulong.xyz

[F06] 删除文件
来源：http://aen.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://kls.svipenyu.cn

PHP:  unlink("a.txt");
来源：http://ddw.feifeiyinyue.top

JS:   fs.unlinkSync("a.txt")
来源：http://ppi.aibaodan.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kfp.fktsv.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cwc.kuanghao11.cn

Go:   os.Remove("a.txt")
来源：http://nmb.jinqigfzy.top

Ruby: File.delete("a.txt")
来源：http://wyn.jiagoushi.top

C#:   File.Delete("a.txt");
来源：http://hyk.xuanzx.com

[F07] 创建目录（含多级）
来源：http://zdk.xziqi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rle.redwolf501.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://svu.tarul.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ufo.jyoumei.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xde.hywenlv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fua.bbcook.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oiq.cashguo.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://djg.ydjk.org.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fev.zhixingplan.top

[F08] 遍历目录
来源：http://kks.yongpay.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://yrx.ppjwa.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hxv.jinghuilouyu.cn

JS:   fs.readdirSync("dir")
来源：http://yur.smart0.xyz

TS:   fs.readdirSync("dir")
来源：http://ypg.aibaodan.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bpu.daria6918.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dia.mhx1999.top

Ruby: Dir.children("dir")
来源：http://eag.yonumen.top

C#:   Directory.GetFiles("dir")
来源：http://kev.zhixingplan.top

[F09] 获取文件大小
来源：http://xsh.bbcook.cn

Py:   os.path.getsize("a.txt")
来源：http://qid.shanyushiyangtech.top

PHP:  filesize("a.txt");
来源：http://mtt.zycfv.cn

JS:   fs.statSync("a.txt").size
来源：http://ijf.yvedp.cn

TS:   fs.statSync("a.txt").size
来源：http://zij.jiagoushi.top

Java: Files.size(Path.of("a.txt"))
来源：http://eld.mhx1999.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mdo.jinghuilouyu.cn

Ruby: File.size("a.txt")
来源：http://xpp.sysykeji.top


<!-- 参考信息 -->