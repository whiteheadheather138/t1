代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mul.xuetiantiany.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fji.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ymz.shuidangran.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pan.hongshengwenyu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://djy.aizwys.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xkc.jinyuanbaomall.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mxs.gotoacloud.top

[D26] 数组转字符串
来源：http://iym.dashuyun.cn

Py:   ", ".join(map(str, arr))
来源：http://weq.yanxiufei.cn

PHP:  implode(", ", $arr);
来源：http://uvt.jianghu66.top

JS:   arr.join(", ")
来源：http://fyk.svipenyu.cn

TS:   arr.join(", ")
来源：http://llx.fehbvm.com

Java: String.join(", ", list)
来源：http://quu.jinqigufen.top

Go:   strings.Join(strs, ", ")
来源：http://jsg.epnwcf.com

Ruby: arr.join(", ")
来源：http://row.yueranfly.top

C#:   string.Join(", ", list)
来源：http://txe.sysykeji.top

================================================================================
来源：http://usb.yvedp.cn

E. 字符串处理
来源：http://ulx.fengsongda.top

================================================================================
来源：http://rdu.nwbrower.top

[E01] 拼接字符串
来源：http://qwe.shanyushiyangkeji.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kyl.cdnleiting.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://msa.cdnleiting.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xce.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bkt.9152youxi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://orq.cucudq.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://phq.jiagoushi.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://juk.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ait.uphjek.com

[E02] 重复字符串
来源：http://hbb.hfpthk.cn

Py:   "ab" * 3
来源：http://ism.sysykeji.top

PHP:  str_repeat("ab", 3);
来源：http://jcs.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://jmr.aibaodan.cn

TS:   "ab".repeat(3)
来源：http://ugz.hfpthk.cn

Java: "ab".repeat(3)
来源：http://xpm.hesvh.cn

Go:   strings.Repeat("ab", 3)
来源：http://pjd.daria6918.cn

Ruby: "ab" * 3
来源：http://iko.yuanzhike.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qwa.yuanzhike.top

[E03] 截取子串
来源：http://stb.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nlz.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dzs.cucudq.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ono.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://wdh.chenzaomai.com

Java: s.substring(1, 4)
来源：http://bqu.uphjek.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://weq.daria6918.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jen.quarkkingdee.top

C#:   s.Substring(1, 3)
来源：http://ans.pengpengdd.cyou

[E04] 查找子串位置
来源：http://ryw.zhongyouzk.top

Py:   s.find("x");  s.index("x")
来源：http://wqh.yj20258.top

PHP:  strpos($s, "x");
来源：http://biv.hesvh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jqq.mhx1999.top

TS:   s.indexOf("x")
来源：http://zji.ctjpmb.com

Java: s.indexOf("x")
来源：http://lyn.ydjk.org.cn

Go:   strings.Index(s, "x")
来源：http://ggp.c1oappe.top

Ruby: s.index("x")
来源：http://khz.xingfuxueyuan.xyz

C#:   s.IndexOf("x")
来源：http://kaa.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://nuq.c1oappe.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hls.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qzh.nanxinkj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nga.sweek.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://byt.sysykeji.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fhn.vqdsnc.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mqn.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ith.yuanzhike.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rxp.nwbrower.top

[E06] 替换子串
来源：http://jmf.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://std.c1oappe.top

PHP:  str_replace("a", "b", $s);
来源：http://vvk.52xcode.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dpz.cheryme.top

TS:   s.replaceAll("a", "b")
来源：http://rdj.yueranfly.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://itv.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sjm.zdbjq.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://aqk.yonumen.top

C#:   s.Replace("a", "b")
来源：http://bcs.sufxvd.cn

[E07] 按分隔符拆分
来源：http://icf.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kdh.meibo888.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nca.cucudq.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://okv.jyoumei.cn

TS:   s.split(",")
来源：http://kzh.ywan-chungtsiang.top

Java: s.split(",");  s.split("\\s+")
来源：http://ssl.pycfn.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pov.hammf.cn

Ruby: s.split(",");  s.split
来源：http://vci.guannengcc.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://twr.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://guz.yvedp.cn

Py:   ",".join(items)
来源：http://vya.zhaomingkeji.xyz

PHP:  implode(",", $items);
来源：http://erb.gaohongyu789.top

JS:   items.join(",")
来源：http://gym.316326.xyz

TS:   items.join(",")
来源：http://rgd.hfpthk.cn

Java: String.join(",", items)
来源：http://xxw.yanxiufei.cn

Go:   strings.Join(items, ",")
来源：http://kxc.cdnleiting.top

Ruby: items.join(",")
来源：http://vnk.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://fnx.cheryme.top

[E09] 去除所有空白字符
来源：http://hhl.sweek.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ecz.jinqigfzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zzu.daria6918.cn

JS:   s.replace(/\s+/g, "")
来源：http://mmi.tianlin.xyz

TS:   s.replace(/\s+/g, "")
来源：http://vff.feifeiyinyue.top

Java: s.replaceAll("\\s+", "")
来源：http://jlb.daxiang520.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://fzd.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://esl.yj202588.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zrp.birdmap.top

[E10] 左侧补零 / 定长填充
来源：http://npx.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cjk.dashuyun.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nys.shanyushiyangkeji.top

JS:   "7".padStart(3, "0")
来源：http://zxl.hesvh.cn

TS:   "7".padStart(3, "0")
来源：http://dbg.jiagoushi.top

Java: String.format("%03d", 7)
来源：http://ysr.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://nwg.chenjidiqi.icu

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jwn.zycfv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sih.fktsv.cn

[E11] 反转字符串
来源：http://xky.yuxming.cn

Py:   s[::-1]
来源：http://jfe.sweek.top

PHP:  strrev($s);
来源：http://nwh.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://vmm.aizwys.cn

TS:   [...s].reverse().join("")
来源：http://pvp.ehwqpu.com

Java: new StringBuilder(s).reverse().toString()
来源：http://wsn.xylfe.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jxy.cdnleiting.top

Ruby: s.reverse
来源：http://wxj.cashguo.top

C#:   new string(s.Reverse().ToArray())
来源：http://uyo.hesvh.cn

[E12] 统计某字符出现次数
来源：http://pwr.xylfe.cn

Py:   s.count("a")
来源：http://ehs.sweek.top

PHP:  substr_count($s, "a");
来源：http://yrw.wangdashe.top

JS:   s.split("a").length - 1
来源：http://ojs.nanxuanxn.top

TS:   s.split("a").length - 1
来源：http://sys.havefunace.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://swm.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://kri.yvedp.cn

Ruby: s.count("a")
来源：http://vbx.birdmap.top

C#:   s.Count(c => c == 'a')
来源：http://jka.smart0.xyz

[E13] 逐字符遍历
来源：http://yax.nwbrower.top

Py:   for ch in s: print(ch)
来源：http://jyk.mhx1999.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nvp.jqgfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qsj.hesvh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://iqd.uphjek.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://opt.zhixingplan.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xcc.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jku.yangfankeji.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jqe.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://yvw.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kqw.hesvh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ufk.tarul.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eap.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qbe.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wki.hywenlv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://idc.shzxlz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://myx.pengpengdd.cyou

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jsu.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://jzv.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qex.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mhn.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://khi.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://uvu.hesvh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lin.jlsjyb.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fuw.ydzc1.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://npn.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tsd.0kj1m.cn

[E16] 数字千分位
来源：http://lgy.9152youxi.cn

Py:   f"{1234567:,}"
来源：http://boc.chenlongwang.top

PHP:  number_format(1234567);
来源：http://hiw.fengsongda.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jde.ybcxt.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dcb.jiagoushi.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gak.fehbvm.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://spl.kuanghao11.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mgk.zhiwuduotai.top

C#:   1234567.ToString("N0")
来源：http://xdq.tian-w.cn

[E17] 首字母大写
来源：http://wvx.shanyushiyangtech.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jfe.gotoacloud.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lew.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://noy.zycfv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zyj.yonumen.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jhw.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nuz.sysykeji.top

Ruby: s.capitalize
来源：http://rwb.yonumen.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sil.sweek.top

[E18] 模板占位符替换
来源：http://ncb.snrcjt.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://izv.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wgn.ydzc1.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kgk.nwbrower.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ltb.cdnleiting.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://flz.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hsa.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gjo.tarul.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://com.jinqigfzy.top

[E19] 多行文本按行拆分
来源：http://dec.ppjwa.cn

Py:   s.splitlines()
来源：http://tug.gotoacloud.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ijs.zhixingplan.top

JS:   s.split(/\r?\n/)
来源：http://aub.meibo888.top

TS:   s.split(/\r?\n/)
来源：http://jab.zhengqikj.top

Java: s.lines().toList()
来源：http://osj.yangfankeji.com

Go:   strings.Split(s, "\n")
来源：http://fje.tian-w.cn

Ruby: s.lines
来源：http://gii.birdmap.top

C#:   s.Split('\n')
来源：http://pqk.guannengcc.top

[E20] 判断字符串是否为空
来源：http://zha.dashuyun.cn

Py:   if not s:
来源：http://rih.guannengcc.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://aqx.sysykeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xlw.yj20258.top

TS:   if (s === "") {}
来源：http://ftt.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://vxu.sxryk.cn

Go:   if s == "" {}
来源：http://zmx.vqdsnc.cn

Ruby: if s.empty?
来源：http://ixp.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qoy.nanxinkj.top

[E21] 超长截断加省略号
来源：http://evl.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zbi.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cho.zhixingplan.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://syf.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dee.xziqi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rix.gzhubu.top

Go:   // 按 rune 判断长度后截断
来源：http://oka.andypj.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ywz.yj20258888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jzw.guannengcc.top

[E22] 字节长度与字符长度
来源：http://mqg.yfazqb.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jil.yvedp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sqj.zycfv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rjp.kuanghao11.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uig.yj20258.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zua.uphjek.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ost.sysykeji.top

Ruby: s.bytesize;  s.length
来源：http://wle.wangshuangyany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gpk.sufxvd.cn

================================================================================
来源：http://yfm.cdnleiting.top

F. 文件与目录
来源：http://qsc.9152youxi.cn

================================================================================
来源：http://udj.jiagoushi.top

[F01] 读取整个文件
来源：http://jho.yj20258888.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bab.jinyuanbaomall.cn

PHP:  file_get_contents("a.txt");
来源：http://vid.fehbvm.com

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qee.jianghu66.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fuy.dianchejie.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://utl.tanke756.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://meg.jinqigfzy.top

Ruby: File.read("a.txt")
来源：http://ipf.zdqjudy.top

C#:   File.ReadAllText("a.txt");
来源：http://oxs.havefunace.top

[F02] 逐行读取文件
来源：http://tbm.tianlin.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yux.nanxuanxn.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tzb.xylfe.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dbf.sxryk.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uzm.cucudq.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tfp.jinyuanbaomall.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://thu.nanxinkj.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vte.sysykeji.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mzi.pengpengdd.cyou

[F03] 写入文件（覆盖）
来源：http://lsz.xuanzx.com

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://msl.hesvh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://geg.shzxlz.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uxd.guowangkeji.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iyd.xinyue.icu

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zjx.hongshengwenyu.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tuk.kuanghao11.cn

Ruby: File.write("a.txt", "hi")
来源：http://nju.shanyushiyangkeji.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nfe.andypj.xyz

[F04] 追加写入文件
来源：http://bjd.tian-w.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://woz.52xcode.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uja.sjlbkw.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hts.jlsjyb.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qbu.wangdashe.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gvh.yuxming.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fsz.zdqjudy.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gpw.hfpthk.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uop.aizwys.cn

[F05] 判断文件或目录是否存在
来源：http://vsi.tianlin.xyz

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bhx.zhijiandao.cn

PHP:  file_exists("a.txt");
来源：http://iqi.hcnkem.com

JS:   fs.existsSync("a.txt")
来源：http://gct.snrcjt.cn

TS:   fs.existsSync("a.txt")
来源：http://jda.jianghu66.top

Java: Files.exists(Path.of("a.txt"))
来源：http://tzm.yfazqb.com

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://eof.mhx1999.top

Ruby: File.exist?("a.txt")
来源：http://juk.yongpay.top

C#:   File.Exists("a.txt")
来源：http://tol.jinyuanbaomall.cn

[F06] 删除文件
来源：http://cac.zhengqikj.top

Py:   os.remove("a.txt")
来源：http://emu.shanyushiyangkeji.top

PHP:  unlink("a.txt");
来源：http://ods.xinyue.icu

JS:   fs.unlinkSync("a.txt")
来源：http://btk.yonumen.top

TS:   fs.unlinkSync("a.txt")
来源：http://xuh.chenjidiqi.icu

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sbg.tanke756.top

Go:   os.Remove("a.txt")
来源：http://zce.uphjek.com

Ruby: File.delete("a.txt")
来源：http://xtm.ydjk.org.cn

C#:   File.Delete("a.txt");
来源：http://jhb.shangyingyoupin.top

[F07] 创建目录（含多级）
来源：http://ftf.yonumen.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rmz.gaohongyu789.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://kvz.cheryme.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://otl.jiagoushi.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hct.ctjpmb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fpe.zhongyouzk.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nyk.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eai.zhiwuduotai.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zub.yanxiufei.cn

[F08] 遍历目录
来源：http://xyl.hesvh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xbu.epnwcf.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lrd.ywan-chungtsiang.top

JS:   fs.readdirSync("dir")
来源：http://nqy.meibo888.top

TS:   fs.readdirSync("dir")
来源：http://rui.smart0.xyz

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://abu.zycfv.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pgj.ywan-chungtsiang.top

Ruby: Dir.children("dir")
来源：http://zch.jinyuanbaomall.cn

C#:   Directory.GetFiles("dir")
来源：http://fxa.ivvv.top

[F09] 获取文件大小
来源：http://wqc.yfazqb.com

Py:   os.path.getsize("a.txt")
来源：http://kky.zhaomingkeji.xyz

PHP:  filesize("a.txt");
来源：http://fiv.316326.xyz

JS:   fs.statSync("a.txt").size
来源：http://cjc.hnxiangtu.top

TS:   fs.statSync("a.txt").size
来源：http://ntb.xinyue.icu

Java: Files.size(Path.of("a.txt"))
来源：http://vbb.tian-w.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aqg.xuetiantiany.cn

Ruby: File.size("a.txt")
来源：http://qvv.tianlin.xyz


<!-- 参考信息 -->