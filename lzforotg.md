代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vxo.gotoacloud.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pvn.gzhubu.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cax.bjfxy.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gzb.c1oappe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jea.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ole.sjlbkw.cn

[D25] Set 集合去重与交并差
来源：http://qcw.yuxming.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://oho.jqgufenzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyt.chenlongwang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xvw.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yir.feifeiyinyue.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tgg.yvedp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ewm.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qll.sjlbkw.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uty.pycfn.com

[D26] 数组转字符串
来源：http://agt.birdmap.top

Py:   ", ".join(map(str, arr))
来源：http://was.daria6918.cn

PHP:  implode(", ", $arr);
来源：http://phz.zhoulong.xyz

JS:   arr.join(", ")
来源：http://dhz.sxryk.cn

TS:   arr.join(", ")
来源：http://rws.hysaishi.cn

Java: String.join(", ", list)
来源：http://zky.sxryk.cn

Go:   strings.Join(strs, ", ")
来源：http://flj.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://uwt.hnqzz.top

C#:   string.Join(", ", list)
来源：http://ggl.hongshengwenyu.top

================================================================================
来源：http://ugr.daxiang520.top

E. 字符串处理
来源：http://akh.zhaomingkeji.xyz

================================================================================
来源：http://rvu.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://zhh.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vlm.zhengqikj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zkp.aibaodan.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dlp.ydzc1.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tvb.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wtd.shanyushiyangtech.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://krq.gogol.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://tky.yongpay.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hyy.yuanzhike.top

[E02] 重复字符串
来源：http://dfh.yfazqb.com

Py:   "ab" * 3
来源：http://dxz.aibaodan.cn

PHP:  str_repeat("ab", 3);
来源：http://luc.yuanzhike.top

JS:   "ab".repeat(3)
来源：http://zon.fengsongda.top

TS:   "ab".repeat(3)
来源：http://deb.vehdjk.com

Java: "ab".repeat(3)
来源：http://bhg.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://ahf.jlsjyb.cn

Ruby: "ab" * 3
来源：http://bov.snrcjt.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gth.jinqigfzy.top

[E03] 截取子串
来源：http://ivr.fanxiaobao.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://usc.cqqwz.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nlq.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xfx.yuxming.cn

TS:   s.slice(1, 4)
来源：http://zhw.zhoulong.xyz

Java: s.substring(1, 4)
来源：http://igr.ydzc1.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://goq.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://wzu.cheryme.top

C#:   s.Substring(1, 3)
来源：http://knf.jianghu66.top

[E04] 查找子串位置
来源：http://bde.hesvh.cn

Py:   s.find("x");  s.index("x")
来源：http://cik.bbcook.cn

PHP:  strpos($s, "x");
来源：http://day.gotoacloud.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jsp.vehdjk.com

TS:   s.indexOf("x")
来源：http://ump.meibo888.top

Java: s.indexOf("x")
来源：http://xrn.sysykeji.top

Go:   strings.Index(s, "x")
来源：http://yvi.ywan-chungtsiang.top

Ruby: s.index("x")
来源：http://qqf.yonumen.top

C#:   s.IndexOf("x")
来源：http://wwc.daria6918.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pyk.ybcxt.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pqi.jinyuanbaomall.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kpm.gogol.net.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lqd.yongpay.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://cgh.hammf.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ihm.sufxvd.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ruu.tian-w.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jgu.tanke756.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rwk.iojbl.cn

[E06] 替换子串
来源：http://hhh.hnxiangtu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://stm.ehwqpu.com

PHP:  str_replace("a", "b", $s);
来源：http://bnn.tanke756.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://krh.sxryk.cn

TS:   s.replaceAll("a", "b")
来源：http://deg.shanyushiyangkeji.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cgw.mhx1999.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://beq.yonumen.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kxf.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://aym.bjfxy.top

[E07] 按分隔符拆分
来源：http://uke.shanyushiyangtech.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://erl.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hjn.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eqd.yueranfly.top

TS:   s.split(",")
来源：http://xjm.snrcjt.cn

Java: s.split(",");  s.split("\\s+")
来源：http://fpb.jqgufenzy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wwg.jianghu66.top

Ruby: s.split(",");  s.split
来源：http://isi.hnxiangtu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vlk.9152youxi.cn

[E08] 数组按分隔符合并
来源：http://svj.jiagoushi.top

Py:   ",".join(items)
来源：http://adk.tanke756.top

PHP:  implode(",", $items);
来源：http://vfk.ivvv.top

JS:   items.join(",")
来源：http://mqz.cdnleiting.top

TS:   items.join(",")
来源：http://inz.quarkkingdee.top

Java: String.join(",", items)
来源：http://cil.vehdjk.com

Go:   strings.Join(items, ",")
来源：http://diw.yfazqb.com

Ruby: items.join(",")
来源：http://vro.daxiang520.top

C#:   string.Join(",", items)
来源：http://tjt.tarul.cn

[E09] 去除所有空白字符
来源：http://pza.jinqigfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xxv.shzxlz.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://doi.9152youxi.cn

JS:   s.replace(/\s+/g, "")
来源：http://rni.sjlbkw.cn

TS:   s.replace(/\s+/g, "")
来源：http://jrd.chenlongwang.top

Java: s.replaceAll("\\s+", "")
来源：http://knp.yj202588.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xqm.nanxinkj.top

Ruby: s.gsub(/\s+/, "")
来源：http://lqr.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jzs.xuetiantiany.cn

[E10] 左侧补零 / 定长填充
来源：http://akd.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vgu.zhengqikj.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qrx.ybcxt.top

JS:   "7".padStart(3, "0")
来源：http://gyd.jinyuanbaomall.cn

TS:   "7".padStart(3, "0")
来源：http://ten.havefunace.top

Java: String.format("%03d", 7)
来源：http://wzo.hysaishi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fcd.chenlongwang.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ono.aibaodan.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lsd.cucudq.cn

[E11] 反转字符串
来源：http://djh.dianchejie.cn

Py:   s[::-1]
来源：http://pzm.fehbvm.com

PHP:  strrev($s);
来源：http://kuz.aizwys.cn

JS:   [...s].reverse().join("")
来源：http://dtz.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://gvf.ywan-chungtsiang.top

Java: new StringBuilder(s).reverse().toString()
来源：http://xub.ydzc1.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://dij.dashuyun.cn

Ruby: s.reverse
来源：http://zzi.nanxinkj.top

C#:   new string(s.Reverse().ToArray())
来源：http://qko.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://ykc.yongpay.top

Py:   s.count("a")
来源：http://ask.andypj.xyz

PHP:  substr_count($s, "a");
来源：http://iaa.tanke756.top

JS:   s.split("a").length - 1
来源：http://wbj.jyoumei.cn

TS:   s.split("a").length - 1
来源：http://boa.zhengqikj.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ivr.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://bej.yanxiufei.cn

Ruby: s.count("a")
来源：http://ujj.ydzc1.top

C#:   s.Count(c => c == 'a')
来源：http://fke.gaohongyu789.top

[E13] 逐字符遍历
来源：http://qat.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://wtw.cqqwz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vgo.iojbl.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rnf.xuanzx.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://qme.yangfankeji.com

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ctg.uphjek.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ijz.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://ohm.zycfv.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qee.cucudq.cn

[E14] URL 编码与 Base64
来源：http://god.iojbl.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zal.yonumen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://osg.jianghu66.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vja.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://szi.jyoumei.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bjl.zycfv.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jlw.meibo888.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kev.bbcook.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://doz.sjlbkw.cn

[E15] HTML 转义 / 反转义
来源：http://leh.hysaishi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ewy.cqqwz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://twk.zhaomingkeji.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://thk.quarkkingdee.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cvo.zhongyouzk.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sfu.vqdsnc.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jnu.zhengqikj.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://oub.jinqigfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://scq.vqdsnc.cn

[E16] 数字千分位
来源：http://dyd.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://eei.snrcjt.cn

PHP:  number_format(1234567);
来源：http://jdt.chenlongwang.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pnd.mhx1999.top

TS:   (1234567).toLocaleString("en-US")
来源：http://imr.316326.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vww.yj20258888.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jdj.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://irn.tian-w.cn

C#:   1234567.ToString("N0")
来源：http://hkh.ybcxt.top

[E17] 首字母大写
来源：http://uoj.zhaomingkeji.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xnr.kuanghao11.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aqv.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://khz.iojbl.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ibg.bbcook.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tom.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bwl.aibaodan.cn

Ruby: s.capitalize
来源：http://uqh.quarkkingdee.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ttk.xziqi.cn

[E18] 模板占位符替换
来源：http://dwm.ydzc1.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://czb.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gla.guannengcc.top

JS:   tpl.replaceAll("{name}", name)
来源：http://bij.yongpay.top

TS:   tpl.replaceAll("{name}", name)
来源：http://vor.pycfn.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://izc.gzhubu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://axl.zycfv.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zvd.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rhx.ybcxt.top

[E19] 多行文本按行拆分
来源：http://urx.zhoulong.xyz

Py:   s.splitlines()
来源：http://tgx.ybcxt.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jre.jinyuanbaomall.cn

JS:   s.split(/\r?\n/)
来源：http://mxf.sufxvd.cn

TS:   s.split(/\r?\n/)
来源：http://zes.c1oappe.top

Java: s.lines().toList()
来源：http://uhi.fzhhl.top

Go:   strings.Split(s, "\n")
来源：http://ijg.birdmap.top

Ruby: s.lines
来源：http://xgp.daxiang520.top

C#:   s.Split('\n')
来源：http://pmb.wangshuangyany.cn

[E20] 判断字符串是否为空
来源：http://bik.yvedp.cn

Py:   if not s:
来源：http://ite.andypj.xyz

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kmv.sufxvd.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kxh.hywenlv.cn

TS:   if (s === "") {}
来源：http://ija.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://dsq.yfazqb.com

Go:   if s == "" {}
来源：http://gdw.zhengqikj.top

Ruby: if s.empty?
来源：http://qnx.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://keu.yj20258.top

[E21] 超长截断加省略号
来源：http://tam.zhiwuduotai.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iyu.jiagoushi.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rop.cdnleiting.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://noc.gzhubu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://epi.xylfe.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qhj.zhiwuduotai.top

Go:   // 按 rune 判断长度后截断
来源：http://ecz.epnwcf.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yxu.fengsongda.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://puf.wangshuangyany.cn

[E22] 字节长度与字符长度
来源：http://kfk.9152youxi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ute.jqgfzy.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ohn.aizwys.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lvr.jqgufenzy.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yox.nanxuanxn.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zjq.zdqjudy.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://txz.redwolf501.top

Ruby: s.bytesize;  s.length
来源：http://bxz.guannengcc.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://app.cucudq.cn

================================================================================
来源：http://nji.tanke756.top

F. 文件与目录
来源：http://xve.jinqigfzy.top

================================================================================
来源：http://vab.yonumen.top

[F01] 读取整个文件
来源：http://cqv.shuidangran.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xvh.cdnleiting.top

PHP:  file_get_contents("a.txt");
来源：http://zfl.yueranfly.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sjk.nwbrower.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qit.jqgfzy.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ykh.ivvv.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xey.uphjek.com

Ruby: File.read("a.txt")
来源：http://hmi.yfazqb.com

C#:   File.ReadAllText("a.txt");
来源：http://lag.fehbvm.com

[F02] 逐行读取文件
来源：http://lvr.chenjidiqi.icu

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://slc.yj202588.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kgz.9152youxi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vwe.shzxlz.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jdc.xziqi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://suv.cashguo.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://kgk.ctjpmb.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mbt.316326.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sqz.hywenlv.cn

[F03] 写入文件（覆盖）
来源：http://hnj.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dlk.iojbl.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://odn.shangyingyoupin.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cjm.fengsongda.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hxv.shanyushiyangkeji.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nmq.fanxiaobao.xyz

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wvu.zhijiandao.cn

Ruby: File.write("a.txt", "hi")
来源：http://xhm.jiagoushi.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dfe.shangyingyoupin.top

[F04] 追加写入文件
来源：http://tvj.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://flp.guowangkeji.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://psu.yonumen.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gqc.yvedp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mbu.andypj.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://aey.gzhubu.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dke.yongpay.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qjj.yueranfly.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uth.jlsjyb.cn

[F05] 判断文件或目录是否存在
来源：http://qdt.jlsjyb.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eem.smart0.xyz

PHP:  file_exists("a.txt");
来源：http://qkw.nanxinkj.top

JS:   fs.existsSync("a.txt")
来源：http://nvf.tian-w.cn

TS:   fs.existsSync("a.txt")
来源：http://kyh.yj20258.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nkm.jlsjyb.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ndc.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://klm.shzxlz.cn

C#:   File.Exists("a.txt")
来源：http://cjt.jinqigfzy.top

[F06] 删除文件
来源：http://lgd.hammf.cn

Py:   os.remove("a.txt")
来源：http://pmi.jyoumei.cn

PHP:  unlink("a.txt");
来源：http://myg.meibo888.top

JS:   fs.unlinkSync("a.txt")
来源：http://qtv.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://ltv.sweek.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fpj.ivvv.top

Go:   os.Remove("a.txt")
来源：http://plj.jinyuanbaomall.cn

Ruby: File.delete("a.txt")
来源：http://kxd.ywan-chungtsiang.top

C#:   File.Delete("a.txt");
来源：http://nbg.52xcode.cn

[F07] 创建目录（含多级）
来源：http://ubr.9152youxi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cav.fehbvm.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://acj.aizwys.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://noe.jinyuanbaomall.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sdo.kuanghao11.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pcq.hesvh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qfu.yuanzhike.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nqd.zhixingplan.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mna.fktsv.cn

[F08] 遍历目录
来源：http://dre.pycfn.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://oqg.ctjpmb.com

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://edr.redwolf501.top

JS:   fs.readdirSync("dir")
来源：http://irf.daria6918.cn

TS:   fs.readdirSync("dir")
来源：http://xaq.gzhubu.top

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fxi.fzhhl.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://neq.jlsjyb.cn

Ruby: Dir.children("dir")
来源：http://yoe.hnqzz.top

C#:   Directory.GetFiles("dir")
来源：http://ndy.haohaochexian.top


<!-- 参考信息 -->