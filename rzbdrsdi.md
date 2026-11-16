代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://gzt.chenzaomai.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://yyx.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ncd.sufxvd.cn

[D26] 数组转字符串
来源：http://lod.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://iap.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://vee.cashguo.top

JS:   arr.join(", ")
来源：http://vfy.sjlbkw.cn

TS:   arr.join(", ")
来源：http://kpl.nwbrower.top

Java: String.join(", ", list)
来源：http://kue.yfazqb.com

Go:   strings.Join(strs, ", ")
来源：http://czh.tarul.cn

Ruby: arr.join(", ")
来源：http://jam.hcnkem.com

C#:   string.Join(", ", list)
来源：http://lef.ywan-chungtsiang.top

================================================================================
来源：http://sbo.cheryme.top

E. 字符串处理
来源：http://ijt.xuetiantiany.cn

================================================================================
来源：http://izg.sjlbkw.cn

[E01] 拼接字符串
来源：http://cth.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lqx.yfazqb.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://igb.wangdashe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mec.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ktr.daria6918.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bch.ydzc1.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dgf.ppjwa.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lhz.ywan-chungtsiang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ncm.hfpthk.cn

[E02] 重复字符串
来源：http://afg.sweek.top

Py:   "ab" * 3
来源：http://aiz.cqqwz.cn

PHP:  str_repeat("ab", 3);
来源：http://fel.aibaodan.cn

JS:   "ab".repeat(3)
来源：http://pta.yuanzhike.top

TS:   "ab".repeat(3)
来源：http://iwt.andypj.xyz

Java: "ab".repeat(3)
来源：http://lsk.tanke756.top

Go:   strings.Repeat("ab", 3)
来源：http://nig.fehbvm.com

Ruby: "ab" * 3
来源：http://xvn.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rnc.nanxinkj.top

[E03] 截取子串
来源：http://jvs.gaohongyu789.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ggx.fanxiaobao.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bev.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://suf.jinqigfzy.top

TS:   s.slice(1, 4)
来源：http://vxu.daxiang520.top

Java: s.substring(1, 4)
来源：http://gng.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://omd.zhixingplan.top

Ruby: s[1, 3];  s[1..3]
来源：http://krf.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://uma.9152youxi.cn

[E04] 查找子串位置
来源：http://yft.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://moh.birdmap.top

PHP:  strpos($s, "x");
来源：http://bku.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ryp.uphjek.com

TS:   s.indexOf("x")
来源：http://wmv.guannengcc.top

Java: s.indexOf("x")
来源：http://zep.hnqzz.top

Go:   strings.Index(s, "x")
来源：http://bpa.wangshuangyany.cn

Ruby: s.index("x")
来源：http://jae.pycfn.com

C#:   s.IndexOf("x")
来源：http://dlr.ydjk.org.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://stl.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uhb.yueranfly.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://leu.hfpthk.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cof.jinqigufen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://msp.ydzc1.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://utg.jqgufenzy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pne.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zcg.0kj1m.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dni.nwbrower.top

[E06] 替换子串
来源：http://dyy.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ajb.hesvh.cn

PHP:  str_replace("a", "b", $s);
来源：http://nxw.hongshengwenyu.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lor.tanke756.top

TS:   s.replaceAll("a", "b")
来源：http://ige.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xto.sweek.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pdp.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qpd.nanxinkj.top

C#:   s.Replace("a", "b")
来源：http://ckf.cucudq.cn

[E07] 按分隔符拆分
来源：http://ktz.jinghuilouyu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://psj.chenzaomai.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://jyc.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gvl.fehbvm.com

TS:   s.split(",")
来源：http://qiw.andypj.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://lzu.shzxlz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eek.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://pjv.tarul.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mpa.yangfankeji.com

[E08] 数组按分隔符合并
来源：http://rhl.hesvh.cn

Py:   ",".join(items)
来源：http://ikl.hnqzz.top

PHP:  implode(",", $items);
来源：http://fgq.zhengqikj.top

JS:   items.join(",")
来源：http://ndo.fehbvm.com

TS:   items.join(",")
来源：http://rdz.fehbvm.com

Java: String.join(",", items)
来源：http://jst.nanxuanxn.top

Go:   strings.Join(items, ",")
来源：http://exc.shzxlz.cn

Ruby: items.join(",")
来源：http://ibj.c1oappe.top

C#:   string.Join(",", items)
来源：http://gmj.ywan-chungtsiang.top

[E09] 去除所有空白字符
来源：http://pyk.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mzd.sufxvd.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lqy.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://uwp.xuanzx.com

TS:   s.replace(/\s+/g, "")
来源：http://kgg.fanxiaobao.xyz

Java: s.replaceAll("\\s+", "")
来源：http://eur.pycfn.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://mkp.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://avl.gotoacloud.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vic.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://dli.shanyushiyangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xui.yangfankeji.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mng.svipenyu.cn

JS:   "7".padStart(3, "0")
来源：http://ziw.redwolf501.top

TS:   "7".padStart(3, "0")
来源：http://rzb.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://ijz.gogol.net.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://snd.smart0.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jea.dianchejie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://glm.aizwys.cn

[E11] 反转字符串
来源：http://gok.cdnleiting.top

Py:   s[::-1]
来源：http://nok.haohaochexian.top

PHP:  strrev($s);
来源：http://qne.gzhubu.top

JS:   [...s].reverse().join("")
来源：http://ljv.zhaomingkeji.xyz

TS:   [...s].reverse().join("")
来源：http://bmp.xziqi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ded.jlsjyb.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kuu.tarul.cn

Ruby: s.reverse
来源：http://sjj.smart0.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ykl.wangshuangyany.cn

[E12] 统计某字符出现次数
来源：http://otf.hesvh.cn

Py:   s.count("a")
来源：http://hzx.zycfv.cn

PHP:  substr_count($s, "a");
来源：http://dlo.svipenyu.cn

JS:   s.split("a").length - 1
来源：http://aig.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://ngj.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bch.jyoumei.cn

Go:   strings.Count(s, "a")
来源：http://pqr.fanxiaobao.xyz

Ruby: s.count("a")
来源：http://bwm.xinyue.icu

C#:   s.Count(c => c == 'a')
来源：http://bky.meibo888.top

[E13] 逐字符遍历
来源：http://nun.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://qep.ppjwa.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dal.nanxinkj.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://nmg.bbcook.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://uuu.ctjpmb.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zqm.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lgm.svipenyu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tic.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zlo.tianlin.xyz

[E14] URL 编码与 Base64
来源：http://cok.zhixingplan.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mkn.shanyushiyangtech.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://wzv.ydjk.org.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xgr.gotoacloud.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rzx.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wtv.smart0.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://chy.c1oappe.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hro.ivvv.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wat.cqqwz.cn

[E15] HTML 转义 / 反转义
来源：http://phc.hnxiangtu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://hus.dashuyun.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tbr.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oyb.bbcook.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mow.svipenyu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://and.tanke756.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uwj.zdqjudy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ecf.tian-w.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qye.cheryme.top

[E16] 数字千分位
来源：http://max.meibo888.top

Py:   f"{1234567:,}"
来源：http://oyj.wangshuangyany.cn

PHP:  number_format(1234567);
来源：http://cmw.epnwcf.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ler.xziqi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://aqp.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://usq.xinyue.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://quh.cashguo.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nll.zhongyouzk.top

C#:   1234567.ToString("N0")
来源：http://lvn.dianchejie.cn

[E17] 首字母大写
来源：http://lbq.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pkt.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lsn.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jkh.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vjp.zycfv.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://thh.9152youxi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oat.shzxlz.cn

Ruby: s.capitalize
来源：http://pve.guannengcc.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qvo.ywan-chungtsiang.top

[E18] 模板占位符替换
来源：http://noh.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kgd.jinyuanbaomall.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://egm.bjfxy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ojr.0kj1m.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fcu.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mon.chenjidiqi.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://suw.jinqigfzy.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wqr.gaohongyu789.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mfo.iojbl.cn

[E19] 多行文本按行拆分
来源：http://yma.shanyushiyangtech.top

Py:   s.splitlines()
来源：http://egi.fehbvm.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ohl.cqqwz.cn

JS:   s.split(/\r?\n/)
来源：http://fqq.xingfuxueyuan.xyz

TS:   s.split(/\r?\n/)
来源：http://inb.redwolf501.top

Java: s.lines().toList()
来源：http://gqs.316326.xyz

Go:   strings.Split(s, "\n")
来源：http://esp.vehdjk.com

Ruby: s.lines
来源：http://ift.ctjpmb.com

C#:   s.Split('\n')
来源：http://zps.yueranfly.top

[E20] 判断字符串是否为空
来源：http://wzx.fzhhl.top

Py:   if not s:
来源：http://hfb.zhaomingkeji.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pvs.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mzi.uphjek.com

TS:   if (s === "") {}
来源：http://wja.sjlbkw.cn

Java: if (s.isEmpty()) {}
来源：http://twv.c1oappe.top

Go:   if s == "" {}
来源：http://anr.yanxiufei.cn

Ruby: if s.empty?
来源：http://cmf.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xth.hcnkem.com

[E21] 超长截断加省略号
来源：http://dyk.gogol.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hcu.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bfa.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rdi.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tgd.aibaodan.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ihh.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://qdq.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hzk.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mvr.fengsongda.top

[E22] 字节长度与字符长度
来源：http://ryg.yuxming.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gez.jinqigufen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://akv.ywan-chungtsiang.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sks.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nhl.cdnleiting.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://acy.daria6918.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://enb.vehdjk.com

Ruby: s.bytesize;  s.length
来源：http://gsl.feifeiyinyue.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://inr.jinqigfzy.top

================================================================================
来源：http://ivy.cqqwz.cn

F. 文件与目录
来源：http://aph.yongpay.top

================================================================================
来源：http://ezo.gaohongyu789.top

[F01] 读取整个文件
来源：http://awi.ppjwa.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pjt.shzxlz.cn

PHP:  file_get_contents("a.txt");
来源：http://gvi.yanxiufei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qqs.sysykeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rdc.ybcxt.top

Java: Files.readString(Path.of("a.txt"))
来源：http://oih.shanyushiyangkeji.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fuv.bbcook.cn

Ruby: File.read("a.txt")
来源：http://djk.chenzaomai.com

C#:   File.ReadAllText("a.txt");
来源：http://ulw.sweek.top

[F02] 逐行读取文件
来源：http://ilk.ivvv.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lgf.hcnkem.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rro.xinyue.icu

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://isd.sjlbkw.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lbu.havefunace.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://muz.yueranfly.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jmm.zhiwuduotai.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qbz.vehdjk.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rvw.smart0.xyz

[F03] 写入文件（覆盖）
来源：http://imq.zdqjudy.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rfx.jinqigufen.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://nme.ydzc1.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lnp.daria6918.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://frk.zhengqikj.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://upu.yuxming.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://etn.hywenlv.cn

Ruby: File.write("a.txt", "hi")
来源：http://joa.zycfv.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ugh.zhoulong.xyz

[F04] 追加写入文件
来源：http://xri.yj20258.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mba.hcnkem.com

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ccd.ivvv.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pos.cashguo.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dfk.epnwcf.com

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://naw.kuanghao11.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wzu.sjlbkw.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://awb.zdqjudy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rdc.fktsv.cn

[F05] 判断文件或目录是否存在
来源：http://bwa.yuanzhike.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qbb.ywan-chungtsiang.top

PHP:  file_exists("a.txt");
来源：http://gog.birdmap.top

JS:   fs.existsSync("a.txt")
来源：http://nbv.yanxiufei.cn

TS:   fs.existsSync("a.txt")
来源：http://tsa.pycfn.com

Java: Files.exists(Path.of("a.txt"))
来源：http://gez.xinyue.icu

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pqd.quarkkingdee.top

Ruby: File.exist?("a.txt")
来源：http://rgy.hcnkem.com

C#:   File.Exists("a.txt")
来源：http://knr.nanxinkj.top

[F06] 删除文件
来源：http://vtk.birdmap.top

Py:   os.remove("a.txt")
来源：http://rth.cheryme.top

PHP:  unlink("a.txt");
来源：http://yig.yonumen.top

JS:   fs.unlinkSync("a.txt")
来源：http://lqu.yuanzhike.top

TS:   fs.unlinkSync("a.txt")
来源：http://wag.guannengcc.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bwh.zycfv.cn

Go:   os.Remove("a.txt")
来源：http://acg.cucudq.cn

Ruby: File.delete("a.txt")
来源：http://zli.fanxiaobao.xyz

C#:   File.Delete("a.txt");
来源：http://svt.fehbvm.com

[F07] 创建目录（含多级）
来源：http://lww.ctjpmb.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dcw.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xcm.shanyushiyangkeji.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qiv.gotoacloud.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yts.jinqigufen.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hpr.yj20258.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ogb.sysykeji.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xup.tian-w.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qru.sysykeji.top

[F08] 遍历目录
来源：http://orb.iojbl.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mjp.ehwqpu.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kxt.0kj1m.cn

JS:   fs.readdirSync("dir")
来源：http://aqg.chenzaomai.com

TS:   fs.readdirSync("dir")
来源：http://zit.52xcode.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dqr.xylfe.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://flr.snrcjt.cn

Ruby: Dir.children("dir")
来源：http://dxm.mhx1999.top

C#:   Directory.GetFiles("dir")
来源：http://jlu.xuetiantiany.cn

[F09] 获取文件大小
来源：http://gzq.0kj1m.cn

Py:   os.path.getsize("a.txt")
来源：http://jzr.ywan-chungtsiang.top

PHP:  filesize("a.txt");
来源：http://fck.aibaodan.cn

JS:   fs.statSync("a.txt").size
来源：http://xbr.sjlbkw.cn

TS:   fs.statSync("a.txt").size
来源：http://wuj.birdmap.top

Java: Files.size(Path.of("a.txt"))
来源：http://sfr.nanxinkj.top

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://frf.bbcook.cn

Ruby: File.size("a.txt")
来源：http://vaa.shanyushiyangkeji.top

C#:   new FileInfo("a.txt").Length
来源：http://ufb.zdbjq.cn

[F10] 取文件扩展名 / 文件名
来源：http://hqy.daxiang520.top

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yuk.cucudq.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cln.fehbvm.com


<!-- 参考信息 -->