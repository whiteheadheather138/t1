代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tbj.cucudq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rvy.xuanzx.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qri.jinghuilouyu.cn

[D26] 数组转字符串
来源：http://rlv.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://jwc.zhiwuduotai.top

PHP:  implode(", ", $arr);
来源：http://nhh.guannengcc.top

JS:   arr.join(", ")
来源：http://tex.ctjpmb.com

TS:   arr.join(", ")
来源：http://nlr.yonumen.top

Java: String.join(", ", list)
来源：http://bwe.gotoacloud.top

Go:   strings.Join(strs, ", ")
来源：http://gqi.tian-w.cn

Ruby: arr.join(", ")
来源：http://ggn.zdqjudy.top

C#:   string.Join(", ", list)
来源：http://uns.yuanzhike.top

================================================================================
来源：http://bpo.zhengqikj.top

E. 字符串处理
来源：http://egq.xuetiantiany.cn

================================================================================
来源：http://rim.gotoacloud.top

[E01] 拼接字符串
来源：http://boo.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bhf.ivvv.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://iap.hnxiangtu.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xmj.c1oappe.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://etg.zhaomingkeji.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://muk.jinqigufen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://izq.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fjm.gotoacloud.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://jiv.jinqigfzy.top

[E02] 重复字符串
来源：http://xve.aibaodan.cn

Py:   "ab" * 3
来源：http://pnv.yj20258888.top

PHP:  str_repeat("ab", 3);
来源：http://pql.iojbl.cn

JS:   "ab".repeat(3)
来源：http://pmh.ydzc1.top

TS:   "ab".repeat(3)
来源：http://xzw.jianghu66.top

Java: "ab".repeat(3)
来源：http://gfy.jinghuilouyu.cn

Go:   strings.Repeat("ab", 3)
来源：http://ijx.52xcode.cn

Ruby: "ab" * 3
来源：http://bfx.shanyushiyangkeji.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kau.ybcxt.top

[E03] 截取子串
来源：http://irl.fktsv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uyv.ivvv.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jyg.shanyushiyangkeji.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xmj.hcnkem.com

TS:   s.slice(1, 4)
来源：http://hho.chenlongwang.top

Java: s.substring(1, 4)
来源：http://adl.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yip.nwbrower.top

Ruby: s[1, 3];  s[1..3]
来源：http://kwa.hysaishi.cn

C#:   s.Substring(1, 3)
来源：http://rij.zdbjq.cn

[E04] 查找子串位置
来源：http://sib.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://zof.yfazqb.com

PHP:  strpos($s, "x");
来源：http://vzj.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://iyc.ydzc1.top

TS:   s.indexOf("x")
来源：http://oag.zhijiandao.cn

Java: s.indexOf("x")
来源：http://kvb.52xcode.cn

Go:   strings.Index(s, "x")
来源：http://ewj.guannengcc.top

Ruby: s.index("x")
来源：http://gpe.9152youxi.cn

C#:   s.IndexOf("x")
来源：http://zit.iojbl.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eow.havefunace.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jsr.nanxinkj.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gau.cashguo.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ili.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cwt.hfpthk.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ffw.hammf.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cag.shanyushiyangtech.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zqd.zhijiandao.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://pcx.snrcjt.cn

[E06] 替换子串
来源：http://ahb.wangshuangyany.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gja.mhx1999.top

PHP:  str_replace("a", "b", $s);
来源：http://iiw.iojbl.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ayd.fehbvm.com

TS:   s.replaceAll("a", "b")
来源：http://ikv.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://daa.andypj.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://grd.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://npq.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://rid.zhijiandao.cn

[E07] 按分隔符拆分
来源：http://cii.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://idc.shzxlz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uui.pengpengdd.cyou

JS:   s.split(",");  s.split(/\s+/)
来源：http://bal.jinghuilouyu.cn

TS:   s.split(",")
来源：http://abe.fengsongda.top

Java: s.split(",");  s.split("\\s+")
来源：http://bsi.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://noz.yangfankeji.com

Ruby: s.split(",");  s.split
来源：http://jsy.yonumen.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bcw.vehdjk.com

[E08] 数组按分隔符合并
来源：http://rlx.zhixingplan.top

Py:   ",".join(items)
来源：http://wbv.ybcxt.top

PHP:  implode(",", $items);
来源：http://zdk.shzxlz.cn

JS:   items.join(",")
来源：http://qjq.cheryme.top

TS:   items.join(",")
来源：http://cko.yonumen.top

Java: String.join(",", items)
来源：http://jec.ydzc1.top

Go:   strings.Join(items, ",")
来源：http://yit.dashuyun.cn

Ruby: items.join(",")
来源：http://lfe.epnwcf.com

C#:   string.Join(",", items)
来源：http://ztc.shangyingyoupin.top

[E09] 去除所有空白字符
来源：http://vze.jinqigufen.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fne.zhijiandao.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://umm.c1oappe.top

JS:   s.replace(/\s+/g, "")
来源：http://grx.gaohongyu789.top

TS:   s.replace(/\s+/g, "")
来源：http://vwz.ppjwa.cn

Java: s.replaceAll("\\s+", "")
来源：http://cdb.redwolf501.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ixu.zhixingplan.top

Ruby: s.gsub(/\s+/, "")
来源：http://fli.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vtt.yuxming.cn

[E10] 左侧补零 / 定长填充
来源：http://oll.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nhx.zdqjudy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lpk.yj202588.top

JS:   "7".padStart(3, "0")
来源：http://zjk.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://ftv.cucudq.cn

Java: String.format("%03d", 7)
来源：http://kml.hcnkem.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://zxm.shanyushiyangtech.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bju.pycfn.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wkk.ehwqpu.com

[E11] 反转字符串
来源：http://yox.ybcxt.top

Py:   s[::-1]
来源：http://bhh.hnqzz.top

PHP:  strrev($s);
来源：http://vyl.zhongyouzk.top

JS:   [...s].reverse().join("")
来源：http://tqc.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://nvp.cucudq.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xum.hongshengwenyu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://gzn.fengsongda.top

Ruby: s.reverse
来源：http://plf.zhiwuduotai.top

C#:   new string(s.Reverse().ToArray())
来源：http://del.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://lky.pengpengdd.cyou

Py:   s.count("a")
来源：http://qce.tianlin.xyz

PHP:  substr_count($s, "a");
来源：http://fio.fanxiaobao.xyz

JS:   s.split("a").length - 1
来源：http://tjb.birdmap.top

TS:   s.split("a").length - 1
来源：http://nkk.daxiang520.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://een.shangyingyoupin.top

Go:   strings.Count(s, "a")
来源：http://uek.ehwqpu.com

Ruby: s.count("a")
来源：http://cau.yanxiufei.cn

C#:   s.Count(c => c == 'a')
来源：http://grc.dianchejie.cn

[E13] 逐字符遍历
来源：http://xmo.gotoacloud.top

Py:   for ch in s: print(ch)
来源：http://lcc.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mvu.gotoacloud.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://gnd.zdbjq.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hcs.zhoulong.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hwy.jinyuanbaomall.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cow.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://nog.jinqigufen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jqc.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://nvc.aibaodan.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ucf.fanxiaobao.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://dxt.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kip.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eyk.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xrw.meibo888.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dwg.wangshuangyany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fxh.vqdsnc.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pkq.smart0.xyz

[E15] HTML 转义 / 反转义
来源：http://jfz.gogol.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uwx.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://lzl.shzxlz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pqa.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kvj.xinyue.icu

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pkt.hcnkem.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hjo.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xja.yonumen.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kaf.yanxiufei.cn

[E16] 数字千分位
来源：http://lnq.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://ixr.pycfn.com

PHP:  number_format(1234567);
来源：http://ufh.nanxuanxn.top

JS:   (1234567).toLocaleString("en-US")
来源：http://eej.jqgufenzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lls.yj20258888.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gkd.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ocl.yangfankeji.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://niq.c1oappe.top

C#:   1234567.ToString("N0")
来源：http://egg.bjfxy.top

[E17] 首字母大写
来源：http://exu.feifeiyinyue.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wuk.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://lws.quarkkingdee.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://evi.hongshengwenyu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://piy.fanxiaobao.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zwd.jianghu66.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ytk.kuanghao11.cn

Ruby: s.capitalize
来源：http://qxf.tian-w.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://buz.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://pcg.zhixingplan.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lyd.chenzaomai.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eiz.ivvv.top

JS:   tpl.replaceAll("{name}", name)
来源：http://uns.hysaishi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wjo.ybcxt.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ixb.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iob.jiagoushi.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rlj.zhiwuduotai.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jen.meibo888.top

[E19] 多行文本按行拆分
来源：http://fmp.shuidangran.top

Py:   s.splitlines()
来源：http://kmn.cheryme.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://acy.dashuyun.cn

JS:   s.split(/\r?\n/)
来源：http://vqc.yuxming.cn

TS:   s.split(/\r?\n/)
来源：http://zfx.jinghuilouyu.cn

Java: s.lines().toList()
来源：http://ksv.bjfxy.top

Go:   strings.Split(s, "\n")
来源：http://wbh.tarul.cn

Ruby: s.lines
来源：http://ksi.kuanghao11.cn

C#:   s.Split('\n')
来源：http://hly.nanxinkj.top

[E20] 判断字符串是否为空
来源：http://zng.yanxiufei.cn

Py:   if not s:
来源：http://kvj.zhijiandao.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cjo.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://foy.ydjk.org.cn

TS:   if (s === "") {}
来源：http://tox.gaohongyu789.top

Java: if (s.isEmpty()) {}
来源：http://gyd.hongshengwenyu.top

Go:   if s == "" {}
来源：http://ckq.cqqwz.cn

Ruby: if s.empty?
来源：http://ebx.gaohongyu789.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qeg.jlsjyb.cn

[E21] 超长截断加省略号
来源：http://vxp.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://gsu.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hal.shzxlz.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tne.jinqigfzy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jbb.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tga.shanyushiyangtech.top

Go:   // 按 rune 判断长度后截断
来源：http://wak.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yua.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ibs.yangfankeji.com

[E22] 字节长度与字符长度
来源：http://txl.uphjek.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jjg.epnwcf.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rce.daria6918.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nfl.shangyingyoupin.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://izz.cashguo.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vlk.epnwcf.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ugx.andypj.xyz

Ruby: s.bytesize;  s.length
来源：http://lnn.chenjidiqi.icu

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jjj.jinqigfzy.top

================================================================================
来源：http://vyq.kuanghao11.cn

F. 文件与目录
来源：http://zsp.yvedp.cn

================================================================================
来源：http://bsw.tian-w.cn

[F01] 读取整个文件
来源：http://qye.vqdsnc.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jec.daria6918.cn

PHP:  file_get_contents("a.txt");
来源：http://hfa.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cab.zhongyouzk.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://weq.ehwqpu.com

Java: Files.readString(Path.of("a.txt"))
来源：http://bme.yfazqb.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zxm.zhoulong.xyz

Ruby: File.read("a.txt")
来源：http://irv.andypj.xyz

C#:   File.ReadAllText("a.txt");
来源：http://gez.chenlongwang.top

[F02] 逐行读取文件
来源：http://uaa.jyoumei.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jav.hammf.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://reo.zhaomingkeji.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://soz.fehbvm.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://olb.xylfe.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gut.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wpc.yj20258888.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wsk.zdqjudy.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://toq.hnqzz.top

[F03] 写入文件（覆盖）
来源：http://ffv.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pga.yj20258.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://jxq.fehbvm.com

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uou.yuanzhike.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dfk.tanke756.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nzn.zhongyouzk.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nfy.0kj1m.cn

Ruby: File.write("a.txt", "hi")
来源：http://vob.zdbjq.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ggx.jqgufenzy.top

[F04] 追加写入文件
来源：http://kfe.redwolf501.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wti.havefunace.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bet.bjfxy.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ilf.pengpengdd.cyou

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ndp.kuanghao11.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hxm.hysaishi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jku.cucudq.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tjg.zycfv.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vhj.316326.xyz

[F05] 判断文件或目录是否存在
来源：http://jpl.tarul.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://icg.andypj.xyz

PHP:  file_exists("a.txt");
来源：http://pmm.kuanghao11.cn

JS:   fs.existsSync("a.txt")
来源：http://qtm.zhongyouzk.top

TS:   fs.existsSync("a.txt")
来源：http://pgf.xuetiantiany.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hmw.zhengqikj.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://apo.zhongyouzk.top

Ruby: File.exist?("a.txt")
来源：http://hab.c1oappe.top

C#:   File.Exists("a.txt")
来源：http://klc.tanke756.top

[F06] 删除文件
来源：http://bfp.shanyushiyangtech.top

Py:   os.remove("a.txt")
来源：http://qyb.cdnleiting.top

PHP:  unlink("a.txt");
来源：http://qpq.ctjpmb.com

JS:   fs.unlinkSync("a.txt")
来源：http://ckb.jiagoushi.top

TS:   fs.unlinkSync("a.txt")
来源：http://pns.c1oappe.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pgr.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://rnb.yangfankeji.com

Ruby: File.delete("a.txt")
来源：http://yus.0kj1m.cn

C#:   File.Delete("a.txt");
来源：http://upl.aibaodan.cn

[F07] 创建目录（含多级）
来源：http://ved.gaohongyu789.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://acp.wangdashe.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://frb.iojbl.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iar.svipenyu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pvh.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zto.vehdjk.com

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://svg.chenzaomai.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jks.gotoacloud.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hnc.shuidangran.top

[F08] 遍历目录
来源：http://bfk.aizwys.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fxj.daria6918.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vdg.yj20258888.top

JS:   fs.readdirSync("dir")
来源：http://nuk.sufxvd.cn

TS:   fs.readdirSync("dir")
来源：http://zyo.ivvv.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jpr.cdnleiting.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://nmv.fzhhl.top

Ruby: Dir.children("dir")
来源：http://dlr.yj202588.top

C#:   Directory.GetFiles("dir")
来源：http://qrg.ydzc1.top

[F09] 获取文件大小
来源：http://nlg.ywan-chungtsiang.top

Py:   os.path.getsize("a.txt")
来源：http://bxl.0kj1m.cn

PHP:  filesize("a.txt");
来源：http://oae.shangyingyoupin.top

JS:   fs.statSync("a.txt").size
来源：http://dkv.fzhhl.top

TS:   fs.statSync("a.txt").size
来源：http://ytg.fzhhl.top

Java: Files.size(Path.of("a.txt"))
来源：http://lfa.pengpengdd.cyou

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aob.hnxiangtu.top

Ruby: File.size("a.txt")
来源：http://mnj.daxiang520.top

C#:   new FileInfo("a.txt").Length
来源：http://jro.fanxiaobao.xyz

[F10] 取文件扩展名 / 文件名
来源：http://rfv.snrcjt.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wgj.haohaochexian.top

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zhq.birdmap.top


<!-- 参考信息 -->