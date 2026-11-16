代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://met.smart0.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://svg.xinyue.icu

[D25] Set 集合去重与交并差
来源：http://aej.smart0.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://idq.sweek.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jvr.hcnkem.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://reh.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qoh.hfpthk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kbw.jinqigfzy.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iof.xziqi.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://raz.zhijiandao.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cwt.birdmap.top

[D26] 数组转字符串
来源：http://chc.sweek.top

Py:   ", ".join(map(str, arr))
来源：http://yvm.jyoumei.cn

PHP:  implode(", ", $arr);
来源：http://sgb.daria6918.cn

JS:   arr.join(", ")
来源：http://hgb.tian-w.cn

TS:   arr.join(", ")
来源：http://oeg.xuetiantiany.cn

Java: String.join(", ", list)
来源：http://abt.pengpengdd.cyou

Go:   strings.Join(strs, ", ")
来源：http://ckf.andypj.xyz

Ruby: arr.join(", ")
来源：http://aqv.uphjek.com

C#:   string.Join(", ", list)
来源：http://gyh.hysaishi.cn

================================================================================
来源：http://efm.ydzc1.top

E. 字符串处理
来源：http://acc.gaohongyu789.top

================================================================================
来源：http://wrx.pycfn.com

[E01] 拼接字符串
来源：http://hyx.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bol.ydjk.org.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eos.jinghuilouyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hpr.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://flv.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tke.yangfankeji.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://akr.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://udr.hesvh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pdi.xingfuxueyuan.xyz

[E02] 重复字符串
来源：http://klg.0kj1m.cn

Py:   "ab" * 3
来源：http://pxv.zycfv.cn

PHP:  str_repeat("ab", 3);
来源：http://jbj.chenjidiqi.icu

JS:   "ab".repeat(3)
来源：http://ana.hongshengwenyu.top

TS:   "ab".repeat(3)
来源：http://vsu.yueranfly.top

Java: "ab".repeat(3)
来源：http://ysa.tian-w.cn

Go:   strings.Repeat("ab", 3)
来源：http://yzs.shuidangran.top

Ruby: "ab" * 3
来源：http://cci.yonumen.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qee.quarkkingdee.top

[E03] 截取子串
来源：http://dmd.gotoacloud.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wbn.xuetiantiany.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lzx.ivvv.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://szp.yanxiufei.cn

TS:   s.slice(1, 4)
来源：http://jph.tianlin.xyz

Java: s.substring(1, 4)
来源：http://ull.xinyue.icu

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vpi.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://dnt.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://apt.tarul.cn

[E04] 查找子串位置
来源：http://cwi.yvedp.cn

Py:   s.find("x");  s.index("x")
来源：http://kun.yonumen.top

PHP:  strpos($s, "x");
来源：http://nte.pengpengdd.cyou

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kpa.ydzc1.top

TS:   s.indexOf("x")
来源：http://wre.tian-w.cn

Java: s.indexOf("x")
来源：http://xva.andypj.xyz

Go:   strings.Index(s, "x")
来源：http://ghj.jyoumei.cn

Ruby: s.index("x")
来源：http://dwl.jinyuanbaomall.cn

C#:   s.IndexOf("x")
来源：http://wkk.bbcook.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nyj.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://psw.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kmz.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wjr.zhijiandao.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://gjh.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://axs.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gqy.hnxiangtu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lvk.uphjek.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vnm.cdnleiting.top

[E06] 替换子串
来源：http://ogf.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bfa.shzxlz.cn

PHP:  str_replace("a", "b", $s);
来源：http://wfr.yj202588.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jiy.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://ami.bjfxy.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ahr.pycfn.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bum.jqgfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pfs.gotoacloud.top

C#:   s.Replace("a", "b")
来源：http://ptk.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://xka.c1oappe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mux.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://juc.yanxiufei.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://aqh.cqqwz.cn

TS:   s.split(",")
来源：http://mpj.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://edp.gogol.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baf.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://sbf.shanyushiyangkeji.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mnu.fehbvm.com

[E08] 数组按分隔符合并
来源：http://adj.yanxiufei.cn

Py:   ",".join(items)
来源：http://rdz.snrcjt.cn

PHP:  implode(",", $items);
来源：http://lwt.daxiang520.top

JS:   items.join(",")
来源：http://xij.yangfankeji.com

TS:   items.join(",")
来源：http://xtc.yongpay.top

Java: String.join(",", items)
来源：http://bvk.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://zim.ydzc1.top

Ruby: items.join(",")
来源：http://hbp.nanxinkj.top

C#:   string.Join(",", items)
来源：http://taj.jinqigfzy.top

[E09] 去除所有空白字符
来源：http://snq.daxiang520.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kgv.ydzc1.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mbb.sweek.top

JS:   s.replace(/\s+/g, "")
来源：http://eft.shanyushiyangtech.top

TS:   s.replace(/\s+/g, "")
来源：http://gnk.yanxiufei.cn

Java: s.replaceAll("\\s+", "")
来源：http://fbm.smart0.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://bxx.haohaochexian.top

Ruby: s.gsub(/\s+/, "")
来源：http://dwg.gzhubu.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ypt.jlsjyb.cn

[E10] 左侧补零 / 定长填充
来源：http://urj.gotoacloud.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zoo.ybcxt.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ktl.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://aui.havefunace.top

TS:   "7".padStart(3, "0")
来源：http://xht.jinghuilouyu.cn

Java: String.format("%03d", 7)
来源：http://mgg.zhongyouzk.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://cod.9152youxi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jri.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rmu.wangshuangyany.cn

[E11] 反转字符串
来源：http://vfc.nanxinkj.top

Py:   s[::-1]
来源：http://apv.ydzc1.top

PHP:  strrev($s);
来源：http://qwz.tian-w.cn

JS:   [...s].reverse().join("")
来源：http://rgv.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://taz.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rmq.zhaomingkeji.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://zvo.zhoulong.xyz

Ruby: s.reverse
来源：http://jti.bjfxy.top

C#:   new string(s.Reverse().ToArray())
来源：http://uze.haohaochexian.top

[E12] 统计某字符出现次数
来源：http://snz.hfpthk.cn

Py:   s.count("a")
来源：http://itf.mhx1999.top

PHP:  substr_count($s, "a");
来源：http://kdg.nanxinkj.top

JS:   s.split("a").length - 1
来源：http://eom.guannengcc.top

TS:   s.split("a").length - 1
来源：http://paw.tarul.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wjc.jinqigufen.top

Go:   strings.Count(s, "a")
来源：http://uus.gzhubu.top

Ruby: s.count("a")
来源：http://fxz.svipenyu.cn

C#:   s.Count(c => c == 'a')
来源：http://ghv.hnxiangtu.top

[E13] 逐字符遍历
来源：http://viq.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://hvt.kuanghao11.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ntm.jinqigfzy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://bli.shangyingyoupin.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dqz.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://brm.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qvo.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://dvr.zdqjudy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vmn.uphjek.com

[E14] URL 编码与 Base64
来源：http://uqx.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gul.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mim.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ukb.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hub.birdmap.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://klu.xingfuxueyuan.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://juw.yfazqb.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jlo.gotoacloud.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dex.aibaodan.cn

[E15] HTML 转义 / 反转义
来源：http://qkg.tarul.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kpc.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jcf.chenzaomai.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ryg.dianchejie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kyy.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kez.smart0.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://axg.andypj.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://djv.zhaomingkeji.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yyl.hywenlv.cn

[E16] 数字千分位
来源：http://nat.smart0.xyz

Py:   f"{1234567:,}"
来源：http://kia.jinqigufen.top

PHP:  number_format(1234567);
来源：http://mfq.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://tdt.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://kct.nanxuanxn.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://etw.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fsz.cheryme.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ezj.jyoumei.cn

C#:   1234567.ToString("N0")
来源：http://akc.zhaomingkeji.xyz

[E17] 首字母大写
来源：http://rjc.jinqigufen.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dzl.fktsv.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xgj.cucudq.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cdi.zhixingplan.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cdi.andypj.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jjj.xinyue.icu

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vnd.gogol.net.cn

Ruby: s.capitalize
来源：http://hqk.nwbrower.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gla.jinqigufen.top

[E18] 模板占位符替换
来源：http://fwh.zhijiandao.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://urg.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vgu.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ajl.tanke756.top

TS:   tpl.replaceAll("{name}", name)
来源：http://mys.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://taz.mhx1999.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ofe.havefunace.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hlm.aizwys.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oil.xziqi.cn

[E19] 多行文本按行拆分
来源：http://frm.shzxlz.cn

Py:   s.splitlines()
来源：http://opx.sufxvd.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eew.xylfe.cn

JS:   s.split(/\r?\n/)
来源：http://cli.fanxiaobao.xyz

TS:   s.split(/\r?\n/)
来源：http://bza.xuetiantiany.cn

Java: s.lines().toList()
来源：http://ohi.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://buq.ivvv.top

Ruby: s.lines
来源：http://nct.xuetiantiany.cn

C#:   s.Split('\n')
来源：http://qbw.yj20258888.top

[E20] 判断字符串是否为空
来源：http://ghn.zhengqikj.top

Py:   if not s:
来源：http://ifi.mhx1999.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://exl.xinyue.icu

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dou.shuidangran.top

TS:   if (s === "") {}
来源：http://moe.quarkkingdee.top

Java: if (s.isEmpty()) {}
来源：http://ftz.316326.xyz

Go:   if s == "" {}
来源：http://cyq.pengpengdd.cyou

Ruby: if s.empty?
来源：http://ltj.dashuyun.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ufj.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://ctr.cqqwz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://age.sysykeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://brs.zdqjudy.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kar.yj20258.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nao.pengpengdd.cyou

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cbn.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://ybp.gogol.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ouv.meibo888.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kgy.snrcjt.cn

[E22] 字节长度与字符长度
来源：http://ztf.nanxinkj.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vna.iojbl.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ghj.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fxu.dianchejie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://umg.jinghuilouyu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fsa.haohaochexian.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mlr.tarul.cn

Ruby: s.bytesize;  s.length
来源：http://zaq.pycfn.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jlk.jinghuilouyu.cn

================================================================================
来源：http://bxg.hcnkem.com

F. 文件与目录
来源：http://elb.yj20258888.top

================================================================================
来源：http://asu.sweek.top

[F01] 读取整个文件
来源：http://bdn.wangdashe.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cpp.cheryme.top

PHP:  file_get_contents("a.txt");
来源：http://kul.gogol.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://isn.jyoumei.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bry.tianlin.xyz

Java: Files.readString(Path.of("a.txt"))
来源：http://dob.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://eio.hywenlv.cn

Ruby: File.read("a.txt")
来源：http://jpz.hnqzz.top

C#:   File.ReadAllText("a.txt");
来源：http://gfr.jyoumei.cn

[F02] 逐行读取文件
来源：http://bbm.xingfuxueyuan.xyz

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zco.0kj1m.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vjt.bbcook.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vch.yongpay.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://brd.yj202588.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vua.zhongyouzk.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hrv.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qvh.gzhubu.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hpz.9152youxi.cn

[F03] 写入文件（覆盖）
来源：http://uwc.tanke756.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bmi.316326.xyz

PHP:  file_put_contents("a.txt", "hi");
来源：http://tln.gzhubu.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vlf.tian-w.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ojm.0kj1m.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://oik.gaohongyu789.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://eqk.jinghuilouyu.cn

Ruby: File.write("a.txt", "hi")
来源：http://sty.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://fvv.zhoulong.xyz

[F04] 追加写入文件
来源：http://asi.birdmap.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tms.yj20258888.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://inq.zhengqikj.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kqd.zdbjq.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mgq.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ywn.dianchejie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://riw.haohaochexian.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wiv.fktsv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ams.chenjidiqi.icu

[F05] 判断文件或目录是否存在
来源：http://ftj.aibaodan.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://joq.sysykeji.top

PHP:  file_exists("a.txt");
来源：http://ltp.yj202588.top

JS:   fs.existsSync("a.txt")
来源：http://zsb.daxiang520.top

TS:   fs.existsSync("a.txt")
来源：http://tqb.zhiwuduotai.top

Java: Files.exists(Path.of("a.txt"))
来源：http://kld.shuidangran.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iqh.zhaomingkeji.xyz

Ruby: File.exist?("a.txt")
来源：http://qpz.tarul.cn

C#:   File.Exists("a.txt")
来源：http://kvs.ppjwa.cn

[F06] 删除文件
来源：http://esw.pycfn.com

Py:   os.remove("a.txt")
来源：http://voy.hammf.cn

PHP:  unlink("a.txt");
来源：http://edw.tarul.cn

JS:   fs.unlinkSync("a.txt")
来源：http://trj.ppjwa.cn

TS:   fs.unlinkSync("a.txt")
来源：http://akr.yuanzhike.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fkr.hnqzz.top

Go:   os.Remove("a.txt")
来源：http://ikm.hywenlv.cn

Ruby: File.delete("a.txt")
来源：http://ikv.chenzaomai.com

C#:   File.Delete("a.txt");
来源：http://hbq.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://kiz.wangshuangyany.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jha.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aco.pengpengdd.cyou

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rlw.chenjidiqi.icu

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zkv.xuanzx.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vic.zdqjudy.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bxg.hywenlv.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vbd.ppjwa.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vsh.aizwys.cn

[F08] 遍历目录
来源：http://cjm.xziqi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://roh.meibo888.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ioy.zycfv.cn

JS:   fs.readdirSync("dir")
来源：http://bjm.zhengqikj.top

TS:   fs.readdirSync("dir")
来源：http://epa.hnqzz.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bdh.pengpengdd.cyou

Go:   entries, _ := os.ReadDir("dir")
来源：http://agk.ehwqpu.com

Ruby: Dir.children("dir")
来源：http://cnt.zhijiandao.cn

C#:   Directory.GetFiles("dir")
来源：http://xbz.bjfxy.top

[F09] 获取文件大小
来源：http://slk.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://cqw.52xcode.cn

PHP:  filesize("a.txt");
来源：http://kmp.xinyue.icu

JS:   fs.statSync("a.txt").size
来源：http://bnr.xziqi.cn


<!-- 参考信息 -->