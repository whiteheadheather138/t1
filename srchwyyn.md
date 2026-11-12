代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rkp.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hje.shanyushiyangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fcd.sweek.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vdy.tarul.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yuv.nanxuanxn.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://szz.tarul.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zxs.nanxuanxn.top

[D26] 数组转字符串
来源：http://qcx.tian-w.cn

Py:   ", ".join(map(str, arr))
来源：http://owq.mhx1999.top

PHP:  implode(", ", $arr);
来源：http://tgf.ehwqpu.com

JS:   arr.join(", ")
来源：http://rvd.zhaomingkeji.xyz

TS:   arr.join(", ")
来源：http://qvz.jyoumei.cn

Java: String.join(", ", list)
来源：http://xgw.xuanzx.com

Go:   strings.Join(strs, ", ")
来源：http://buy.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://soo.sxryk.cn

C#:   string.Join(", ", list)
来源：http://hus.ywan-chungtsiang.top

================================================================================
来源：http://ods.dashuyun.cn

E. 字符串处理
来源：http://zmd.ydzc1.top

================================================================================
来源：http://jip.birdmap.top

[E01] 拼接字符串
来源：http://utx.zhiwuduotai.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vrt.xingfuxueyuan.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qti.zhaomingkeji.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lua.zdqjudy.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vim.chenlongwang.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hvl.cdnleiting.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nwz.xinyue.icu

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jjd.yanxiufei.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jyf.cashguo.top

[E02] 重复字符串
来源：http://lsi.gogol.net.cn

Py:   "ab" * 3
来源：http://uwe.tian-w.cn

PHP:  str_repeat("ab", 3);
来源：http://pzh.shuidangran.top

JS:   "ab".repeat(3)
来源：http://gjo.zhoulong.xyz

TS:   "ab".repeat(3)
来源：http://rcu.smart0.xyz

Java: "ab".repeat(3)
来源：http://gjm.xingfuxueyuan.xyz

Go:   strings.Repeat("ab", 3)
来源：http://fdd.daria6918.cn

Ruby: "ab" * 3
来源：http://qxh.guannengcc.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gci.hnxiangtu.top

[E03] 截取子串
来源：http://byt.zdqjudy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xru.yvedp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lef.birdmap.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hzd.ydjk.org.cn

TS:   s.slice(1, 4)
来源：http://mqe.chenjidiqi.icu

Java: s.substring(1, 4)
来源：http://lmp.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sjx.sxryk.cn

Ruby: s[1, 3];  s[1..3]
来源：http://bej.yangfankeji.com

C#:   s.Substring(1, 3)
来源：http://phu.yj20258.top

[E04] 查找子串位置
来源：http://tnj.vehdjk.com

Py:   s.find("x");  s.index("x")
来源：http://dac.ydjk.org.cn

PHP:  strpos($s, "x");
来源：http://sox.yfazqb.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yev.aibaodan.cn

TS:   s.indexOf("x")
来源：http://ued.yj202588.top

Java: s.indexOf("x")
来源：http://qrt.ybcxt.top

Go:   strings.Index(s, "x")
来源：http://fwv.fzhhl.top

Ruby: s.index("x")
来源：http://xms.vqdsnc.cn

C#:   s.IndexOf("x")
来源：http://qtx.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cdc.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kmk.tanke756.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bvg.zhengqikj.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dxk.pycfn.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://rod.yfazqb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fjj.ivvv.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tzo.yonumen.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ntm.hysaishi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zcn.chenzaomai.com

[E06] 替换子串
来源：http://chk.hywenlv.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://osx.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dkq.sysykeji.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://usy.cucudq.cn

TS:   s.replaceAll("a", "b")
来源：http://mqp.ppjwa.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oxw.yongpay.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wzl.xuanzx.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nit.guowangkeji.top

C#:   s.Replace("a", "b")
来源：http://med.epnwcf.com

[E07] 按分隔符拆分
来源：http://bsj.guowangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://szr.yuxming.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xrz.yj20258888.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://act.zhijiandao.cn

TS:   s.split(",")
来源：http://izr.ivvv.top

Java: s.split(",");  s.split("\\s+")
来源：http://hjp.yfazqb.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rsk.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://zit.zhixingplan.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://evp.hysaishi.cn

[E08] 数组按分隔符合并
来源：http://vqv.52xcode.cn

Py:   ",".join(items)
来源：http://fav.chenjidiqi.icu

PHP:  implode(",", $items);
来源：http://fbs.yj202588.top

JS:   items.join(",")
来源：http://lxt.sweek.top

TS:   items.join(",")
来源：http://feh.feifeiyinyue.top

Java: String.join(",", items)
来源：http://hqu.zhaomingkeji.xyz

Go:   strings.Join(items, ",")
来源：http://ghu.havefunace.top

Ruby: items.join(",")
来源：http://hnx.vqdsnc.cn

C#:   string.Join(",", items)
来源：http://plj.hesvh.cn

[E09] 去除所有空白字符
来源：http://epf.zdbjq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jqm.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aap.epnwcf.com

JS:   s.replace(/\s+/g, "")
来源：http://cle.sufxvd.cn

TS:   s.replace(/\s+/g, "")
来源：http://fvr.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://zrz.sjlbkw.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ttf.nanxuanxn.top

Ruby: s.gsub(/\s+/, "")
来源：http://qky.tarul.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jhi.quarkkingdee.top

[E10] 左侧补零 / 定长填充
来源：http://yqt.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dxz.yj20258.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vui.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://gbb.hongshengwenyu.top

TS:   "7".padStart(3, "0")
来源：http://oiz.chenzaomai.com

Java: String.format("%03d", 7)
来源：http://mcj.hywenlv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ixp.bbcook.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ygi.fengsongda.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://djr.cdnleiting.top

[E11] 反转字符串
来源：http://fds.xuanzx.com

Py:   s[::-1]
来源：http://lhr.jianghu66.top

PHP:  strrev($s);
来源：http://edn.jyoumei.cn

JS:   [...s].reverse().join("")
来源：http://cze.jlsjyb.cn

TS:   [...s].reverse().join("")
来源：http://ent.jinghuilouyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ucy.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://juq.tianlin.xyz

Ruby: s.reverse
来源：http://blt.cdnleiting.top

C#:   new string(s.Reverse().ToArray())
来源：http://ggz.zhiwuduotai.top

[E12] 统计某字符出现次数
来源：http://gum.yj20258888.top

Py:   s.count("a")
来源：http://xzn.xziqi.cn

PHP:  substr_count($s, "a");
来源：http://eki.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://ziy.daria6918.cn

TS:   s.split("a").length - 1
来源：http://ayz.redwolf501.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mws.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://pns.yuanzhike.top

Ruby: s.count("a")
来源：http://voy.tanke756.top

C#:   s.Count(c => c == 'a')
来源：http://jox.yvedp.cn

[E13] 逐字符遍历
来源：http://znz.nanxinkj.top

Py:   for ch in s: print(ch)
来源：http://tgj.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fnw.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://aje.yanxiufei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wqg.yj20258.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://etb.bjfxy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lkg.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://zfu.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qsr.316326.xyz

[E14] URL 编码与 Base64
来源：http://rob.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aif.jqgfzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://vrx.yuxming.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fxq.shanyushiyangtech.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nbo.c1oappe.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ehv.52xcode.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://keg.ydjk.org.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://erk.0kj1m.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uxz.gzhubu.top

[E15] HTML 转义 / 反转义
来源：http://axv.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fpn.guannengcc.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rkm.xingfuxueyuan.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pqa.xingfuxueyuan.xyz

TS:   // 同上，务必做 XSS 过滤
来源：http://tkz.nanxuanxn.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cuf.daxiang520.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://evd.ctjpmb.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ylf.xziqi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kuy.haohaochexian.top

[E16] 数字千分位
来源：http://obt.chenjidiqi.icu

Py:   f"{1234567:,}"
来源：http://fkb.yuanzhike.top

PHP:  number_format(1234567);
来源：http://ity.pengpengdd.cyou

JS:   (1234567).toLocaleString("en-US")
来源：http://xci.pengpengdd.cyou

TS:   (1234567).toLocaleString("en-US")
来源：http://bfv.zhijiandao.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://uoc.sjlbkw.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xvo.quarkkingdee.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nuk.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://uju.sxryk.cn

[E17] 首字母大写
来源：http://bdf.shangyingyoupin.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uli.xziqi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bsd.hammf.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jub.zhengqikj.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://isz.hysaishi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://imh.yonumen.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rgv.chenjidiqi.icu

Ruby: s.capitalize
来源：http://xdn.fehbvm.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qzi.smart0.xyz

[E18] 模板占位符替换
来源：http://mnv.guannengcc.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qga.zdbjq.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bus.yj20258888.top

JS:   tpl.replaceAll("{name}", name)
来源：http://byk.quarkkingdee.top

TS:   tpl.replaceAll("{name}", name)
来源：http://kdd.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://orp.fktsv.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hqu.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bsg.vqdsnc.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://cje.yuanzhike.top

[E19] 多行文本按行拆分
来源：http://kjo.tanke756.top

Py:   s.splitlines()
来源：http://siw.zdbjq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ans.jyoumei.cn

JS:   s.split(/\r?\n/)
来源：http://zhs.chenjidiqi.icu

TS:   s.split(/\r?\n/)
来源：http://dyt.xuanzx.com

Java: s.lines().toList()
来源：http://enf.xziqi.cn

Go:   strings.Split(s, "\n")
来源：http://xjy.zhaomingkeji.xyz

Ruby: s.lines
来源：http://kfw.yonumen.top

C#:   s.Split('\n')
来源：http://bsr.havefunace.top

[E20] 判断字符串是否为空
来源：http://qhe.quarkkingdee.top

Py:   if not s:
来源：http://qpx.fanxiaobao.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://upm.yj20258888.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rvm.zycfv.cn

TS:   if (s === "") {}
来源：http://fbh.jianghu66.top

Java: if (s.isEmpty()) {}
来源：http://yji.sysykeji.top

Go:   if s == "" {}
来源：http://trp.meibo888.top

Ruby: if s.empty?
来源：http://iac.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ykt.hnxiangtu.top

[E21] 超长截断加省略号
来源：http://roj.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tzd.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bjy.jinqigufen.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xrq.hfpthk.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ajv.fanxiaobao.xyz

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hil.yonumen.top

Go:   // 按 rune 判断长度后截断
来源：http://gav.jinqigufen.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://usr.jianghu66.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oyl.pycfn.com

[E22] 字节长度与字符长度
来源：http://psz.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jei.jyoumei.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vmz.jinghuilouyu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kue.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fqe.kuanghao11.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://muj.jiagoushi.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://asf.jqgfzy.top

Ruby: s.bytesize;  s.length
来源：http://mqc.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://asi.yangfankeji.com

================================================================================
来源：http://kpp.hesvh.cn

F. 文件与目录
来源：http://thi.zhaomingkeji.xyz

================================================================================
来源：http://dzy.yfazqb.com

[F01] 读取整个文件
来源：http://ohu.mhx1999.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qyz.tian-w.cn

PHP:  file_get_contents("a.txt");
来源：http://sxl.birdmap.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xwn.shzxlz.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://klu.meibo888.top

Java: Files.readString(Path.of("a.txt"))
来源：http://tar.ctjpmb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zue.xuanzx.com

Ruby: File.read("a.txt")
来源：http://fri.ydzc1.top

C#:   File.ReadAllText("a.txt");
来源：http://niy.xinyue.icu

[F02] 逐行读取文件
来源：http://dez.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xlb.wangdashe.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://biw.pengpengdd.cyou

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mfe.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fkp.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ogl.xinyue.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://skv.hysaishi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mdb.hfpthk.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cab.gogol.net.cn

[F03] 写入文件（覆盖）
来源：http://lwn.zhixingplan.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xpz.hammf.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zqc.uphjek.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bby.uphjek.com

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aot.birdmap.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ryv.cucudq.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://tis.pengpengdd.cyou

Ruby: File.write("a.txt", "hi")
来源：http://ynm.xingfuxueyuan.xyz

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jxs.aibaodan.cn

[F04] 追加写入文件
来源：http://olx.dashuyun.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mjr.gotoacloud.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tlj.fzhhl.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xhj.xziqi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://smx.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://upy.jqgufenzy.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://esn.xylfe.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lsa.jinqigfzy.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://spc.hammf.cn

[F05] 判断文件或目录是否存在
来源：http://vyd.vehdjk.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zyn.yvedp.cn

PHP:  file_exists("a.txt");
来源：http://opj.shangyingyoupin.top

JS:   fs.existsSync("a.txt")
来源：http://xpv.aizwys.cn

TS:   fs.existsSync("a.txt")
来源：http://slq.mhx1999.top

Java: Files.exists(Path.of("a.txt"))
来源：http://cst.havefunace.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ojf.zycfv.cn

Ruby: File.exist?("a.txt")
来源：http://ygs.zhongyouzk.top

C#:   File.Exists("a.txt")
来源：http://osv.hysaishi.cn

[F06] 删除文件
来源：http://mej.jyoumei.cn

Py:   os.remove("a.txt")
来源：http://lwg.xziqi.cn

PHP:  unlink("a.txt");
来源：http://lly.yj20258.top

JS:   fs.unlinkSync("a.txt")
来源：http://kfm.fehbvm.com

TS:   fs.unlinkSync("a.txt")
来源：http://vbe.jinyuanbaomall.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ydd.fengsongda.top

Go:   os.Remove("a.txt")
来源：http://elz.uphjek.com

Ruby: File.delete("a.txt")
来源：http://uaz.jinghuilouyu.cn

C#:   File.Delete("a.txt");
来源：http://mye.wangdashe.top

[F07] 创建目录（含多级）
来源：http://kfj.hesvh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dau.hongshengwenyu.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pjk.uphjek.com

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tmx.zycfv.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wjb.zhongyouzk.top

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://poc.jinghuilouyu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ueh.yonumen.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqc.nanxuanxn.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eor.uphjek.com

[F08] 遍历目录
来源：http://teg.ehwqpu.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://hxy.redwolf501.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pwf.ybcxt.top

JS:   fs.readdirSync("dir")
来源：http://bum.shangyingyoupin.top

TS:   fs.readdirSync("dir")
来源：http://lxw.guannengcc.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qvu.yvedp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ssu.zhoulong.xyz

Ruby: Dir.children("dir")
来源：http://yzl.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://prj.ehwqpu.com

[F09] 获取文件大小
来源：http://mpr.nanxuanxn.top

Py:   os.path.getsize("a.txt")
来源：http://zig.snrcjt.cn

PHP:  filesize("a.txt");
来源：http://ryb.kuanghao11.cn

JS:   fs.statSync("a.txt").size
来源：http://voy.cucudq.cn

TS:   fs.statSync("a.txt").size
来源：http://qxs.zhiwuduotai.top

Java: Files.size(Path.of("a.txt"))
来源：http://lce.ppjwa.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zgo.bjfxy.top

Ruby: File.size("a.txt")
来源：http://bkb.wangshuangyany.cn


<!-- 参考信息 -->