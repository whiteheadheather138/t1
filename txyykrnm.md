代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wsq.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nms.bbcook.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mym.ivvv.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://iug.cashguo.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vqo.yj202588.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wpm.pycfn.com

[D25] Set 集合去重与交并差
来源：http://agu.xuanzx.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ztd.fktsv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oyv.zhijiandao.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dxm.chenjidiqi.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://utd.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ukk.gzhubu.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://orf.shanyushiyangtech.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tpr.zhoulong.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ouw.zycfv.cn

[D26] 数组转字符串
来源：http://ezi.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://thq.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://vcv.chenzaomai.com

JS:   arr.join(", ")
来源：http://zxz.daxiang520.top

TS:   arr.join(", ")
来源：http://owb.wangshuangyany.cn

Java: String.join(", ", list)
来源：http://kaq.gzhubu.top

Go:   strings.Join(strs, ", ")
来源：http://ams.yangfankeji.com

Ruby: arr.join(", ")
来源：http://mxj.mhx1999.top

C#:   string.Join(", ", list)
来源：http://dri.xuanzx.com

================================================================================
来源：http://zvr.hammf.cn

E. 字符串处理
来源：http://vew.zdqjudy.top

================================================================================
来源：http://pwa.nanxuanxn.top

[E01] 拼接字符串
来源：http://drp.dianchejie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yqk.birdmap.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://npy.hysaishi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eod.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zlh.ppjwa.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uwa.zhijiandao.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ggl.daxiang520.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bvm.tanke756.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vrp.hysaishi.cn

[E02] 重复字符串
来源：http://rsv.zycfv.cn

Py:   "ab" * 3
来源：http://ybr.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://hca.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://lkb.nwbrower.top

TS:   "ab".repeat(3)
来源：http://vsl.vqdsnc.cn

Java: "ab".repeat(3)
来源：http://qmk.kuanghao11.cn

Go:   strings.Repeat("ab", 3)
来源：http://gcd.yvedp.cn

Ruby: "ab" * 3
来源：http://ubp.bjfxy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fxu.cashguo.top

[E03] 截取子串
来源：http://tnt.sjlbkw.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nss.gaohongyu789.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hmh.chenjidiqi.icu

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mkj.tian-w.cn

TS:   s.slice(1, 4)
来源：http://vaz.vehdjk.com

Java: s.substring(1, 4)
来源：http://tkn.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://scn.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zer.chenlongwang.top

C#:   s.Substring(1, 3)
来源：http://bdy.fengsongda.top

[E04] 查找子串位置
来源：http://cih.yj202588.top

Py:   s.find("x");  s.index("x")
来源：http://udn.jianghu66.top

PHP:  strpos($s, "x");
来源：http://thv.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qtd.smart0.xyz

TS:   s.indexOf("x")
来源：http://eci.bbcook.cn

Java: s.indexOf("x")
来源：http://vtk.sweek.top

Go:   strings.Index(s, "x")
来源：http://job.yj20258888.top

Ruby: s.index("x")
来源：http://hkf.havefunace.top

C#:   s.IndexOf("x")
来源：http://idn.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rmh.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://iyh.andypj.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qjq.jinqigufen.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://geg.vehdjk.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://baj.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dov.ybcxt.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jfs.ehwqpu.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://avp.aibaodan.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tyw.c1oappe.top

[E06] 替换子串
来源：http://jne.ywan-chungtsiang.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://keg.cdnleiting.top

PHP:  str_replace("a", "b", $s);
来源：http://mqy.ydzc1.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://the.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://rbi.zhiwuduotai.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oxb.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ttu.yfazqb.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hfs.feifeiyinyue.top

C#:   s.Replace("a", "b")
来源：http://uqd.ydjk.org.cn

[E07] 按分隔符拆分
来源：http://wrv.guannengcc.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ivk.ywan-chungtsiang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xwg.wangshuangyany.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cqq.zdbjq.cn

TS:   s.split(",")
来源：http://ooc.zhiwuduotai.top

Java: s.split(",");  s.split("\\s+")
来源：http://nqu.shanyushiyangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ovw.dashuyun.cn

Ruby: s.split(",");  s.split
来源：http://aeb.yj20258.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://njt.pycfn.com

[E08] 数组按分隔符合并
来源：http://cyy.hywenlv.cn

Py:   ",".join(items)
来源：http://lhv.vehdjk.com

PHP:  implode(",", $items);
来源：http://pws.hammf.cn

JS:   items.join(",")
来源：http://urb.zdqjudy.top

TS:   items.join(",")
来源：http://era.shanyushiyangkeji.top

Java: String.join(",", items)
来源：http://eip.xinyue.icu

Go:   strings.Join(items, ",")
来源：http://gsa.daria6918.cn

Ruby: items.join(",")
来源：http://wne.zhongyouzk.top

C#:   string.Join(",", items)
来源：http://wsq.xingfuxueyuan.xyz

[E09] 去除所有空白字符
来源：http://nvn.zhiwuduotai.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dzp.jqgufenzy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gjh.zhixingplan.top

JS:   s.replace(/\s+/g, "")
来源：http://gne.shuidangran.top

TS:   s.replace(/\s+/g, "")
来源：http://scq.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://uke.jqgufenzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://atv.dashuyun.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xbi.ydzc1.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pvw.xylfe.cn

[E10] 左侧补零 / 定长填充
来源：http://pie.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tos.fengsongda.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cuo.bbcook.cn

JS:   "7".padStart(3, "0")
来源：http://xpt.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://idj.hongshengwenyu.top

Java: String.format("%03d", 7)
来源：http://sdb.zhiwuduotai.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://zpz.tian-w.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vyo.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lak.birdmap.top

[E11] 反转字符串
来源：http://fle.shuidangran.top

Py:   s[::-1]
来源：http://wxz.nanxinkj.top

PHP:  strrev($s);
来源：http://abd.jianghu66.top

JS:   [...s].reverse().join("")
来源：http://unm.hnqzz.top

TS:   [...s].reverse().join("")
来源：http://plz.aibaodan.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://plp.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://itj.jinqigfzy.top

Ruby: s.reverse
来源：http://tih.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://exb.ehwqpu.com

[E12] 统计某字符出现次数
来源：http://est.zhengqikj.top

Py:   s.count("a")
来源：http://veo.feifeiyinyue.top

PHP:  substr_count($s, "a");
来源：http://idk.quarkkingdee.top

JS:   s.split("a").length - 1
来源：http://xyt.c1oappe.top

TS:   s.split("a").length - 1
来源：http://fwu.jinyuanbaomall.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bws.ybcxt.top

Go:   strings.Count(s, "a")
来源：http://wgj.jinyuanbaomall.cn

Ruby: s.count("a")
来源：http://mvj.xylfe.cn

C#:   s.Count(c => c == 'a')
来源：http://jhg.zycfv.cn

[E13] 逐字符遍历
来源：http://abr.uphjek.com

Py:   for ch in s: print(ch)
来源：http://cih.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fjw.ehwqpu.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://nsa.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zey.vqdsnc.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iad.jqgfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rat.cucudq.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cwp.yfazqb.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dgz.zhoulong.xyz

[E14] URL 编码与 Base64
来源：http://tig.zhengqikj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qgw.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hwk.andypj.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bfo.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://meg.52xcode.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kek.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://okz.xylfe.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hji.snrcjt.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bkn.ybcxt.top

[E15] HTML 转义 / 反转义
来源：http://sac.jiagoushi.top

Py:   html.escape(s);  html.unescape(s)
来源：http://nya.gotoacloud.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://swp.yj202588.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lry.hfpthk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wzs.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iqw.shuidangran.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vkg.hcnkem.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wxb.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nqx.yj202588.top

[E16] 数字千分位
来源：http://ldz.ydzc1.top

Py:   f"{1234567:,}"
来源：http://vne.iojbl.cn

PHP:  number_format(1234567);
来源：http://wih.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://swi.chenlongwang.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nvz.hammf.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oiu.yfazqb.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rjj.yj20258888.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://viz.yonumen.top

C#:   1234567.ToString("N0")
来源：http://tgn.tanke756.top

[E17] 首字母大写
来源：http://xwp.shanyushiyangkeji.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://trh.sweek.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jlc.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://smu.shuidangran.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dfq.zhengqikj.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nhw.yueranfly.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ppf.fzhhl.top

Ruby: s.capitalize
来源：http://bgg.havefunace.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wdd.kuanghao11.cn

[E18] 模板占位符替换
来源：http://ifc.zdbjq.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dlr.fanxiaobao.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://voe.sufxvd.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fxp.redwolf501.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ucg.sufxvd.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ass.cucudq.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://epk.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://slw.vehdjk.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iqe.nanxuanxn.top

[E19] 多行文本按行拆分
来源：http://jco.jinqigfzy.top

Py:   s.splitlines()
来源：http://hzb.ivvv.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lai.andypj.xyz

JS:   s.split(/\r?\n/)
来源：http://ose.uphjek.com

TS:   s.split(/\r?\n/)
来源：http://qfq.fzhhl.top

Java: s.lines().toList()
来源：http://mhy.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://jty.hywenlv.cn

Ruby: s.lines
来源：http://kvi.yj202588.top

C#:   s.Split('\n')
来源：http://lhq.gzhubu.top

[E20] 判断字符串是否为空
来源：http://cdg.xinyue.icu

Py:   if not s:
来源：http://smz.dashuyun.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sxz.daria6918.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uuj.hnqzz.top

TS:   if (s === "") {}
来源：http://dov.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://sgz.sjlbkw.cn

Go:   if s == "" {}
来源：http://yju.ctjpmb.com

Ruby: if s.empty?
来源：http://isa.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://doy.chenlongwang.top

[E21] 超长截断加省略号
来源：http://sfc.hcnkem.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hxw.hnqzz.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://znr.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aeo.fehbvm.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vaj.hywenlv.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ekw.fanxiaobao.xyz

Go:   // 按 rune 判断长度后截断
来源：http://cdl.wangdashe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wgg.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://acg.nanxuanxn.top

[E22] 字节长度与字符长度
来源：http://myd.cheryme.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bsb.gaohongyu789.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aol.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://srm.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://iht.9152youxi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rgr.chenzaomai.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mfd.hysaishi.cn

Ruby: s.bytesize;  s.length
来源：http://pts.cucudq.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ztt.chenlongwang.top

================================================================================
来源：http://lnb.chenjidiqi.icu

F. 文件与目录
来源：http://mof.yuanzhike.top

================================================================================
来源：http://lqi.xuanzx.com

[F01] 读取整个文件
来源：http://gdv.yongpay.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mde.haohaochexian.top

PHP:  file_get_contents("a.txt");
来源：http://bmo.jyoumei.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mpf.xingfuxueyuan.xyz

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zaw.yongpay.top

Java: Files.readString(Path.of("a.txt"))
来源：http://vit.fengsongda.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tks.cucudq.cn

Ruby: File.read("a.txt")
来源：http://uvk.shanyushiyangkeji.top

C#:   File.ReadAllText("a.txt");
来源：http://euf.9152youxi.cn

[F02] 逐行读取文件
来源：http://nvx.tarul.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://anq.snrcjt.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kjy.ydzc1.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nhw.tianlin.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wvo.yuxming.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gco.sxryk.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lac.sxryk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xng.haohaochexian.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://jzy.yfazqb.com

[F03] 写入文件（覆盖）
来源：http://ttz.guowangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sof.aibaodan.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ukr.yvedp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://brx.ppjwa.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wen.redwolf501.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://szw.aibaodan.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lqh.dianchejie.cn

Ruby: File.write("a.txt", "hi")
来源：http://gmp.epnwcf.com

C#:   File.WriteAllText("a.txt", "hi");
来源：http://htl.yfazqb.com

[F04] 追加写入文件
来源：http://mzh.zhaomingkeji.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zol.fanxiaobao.xyz

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qta.ppjwa.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ydk.zhiwuduotai.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pev.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kbn.shzxlz.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://abv.jinyuanbaomall.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vmt.jianghu66.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://haj.vqdsnc.cn

[F05] 判断文件或目录是否存在
来源：http://uea.svipenyu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://tpc.chenjidiqi.icu

PHP:  file_exists("a.txt");
来源：http://bdu.ywan-chungtsiang.top

JS:   fs.existsSync("a.txt")
来源：http://ucz.ppjwa.cn

TS:   fs.existsSync("a.txt")
来源：http://ufe.shangyingyoupin.top

Java: Files.exists(Path.of("a.txt"))
来源：http://stc.tian-w.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rjk.uphjek.com

Ruby: File.exist?("a.txt")
来源：http://ugy.ppjwa.cn

C#:   File.Exists("a.txt")
来源：http://ugn.meibo888.top

[F06] 删除文件
来源：http://dce.hnxiangtu.top

Py:   os.remove("a.txt")
来源：http://fqx.cucudq.cn

PHP:  unlink("a.txt");
来源：http://hvj.ywan-chungtsiang.top

JS:   fs.unlinkSync("a.txt")
来源：http://jjn.nanxuanxn.top

TS:   fs.unlinkSync("a.txt")
来源：http://kuy.birdmap.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://igc.birdmap.top

Go:   os.Remove("a.txt")
来源：http://uzh.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://zbt.shanyushiyangkeji.top

C#:   File.Delete("a.txt");
来源：http://dtb.nanxuanxn.top

[F07] 创建目录（含多级）
来源：http://wzg.gzhubu.top

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://opt.jinghuilouyu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iiq.chenlongwang.top

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://owx.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xdp.ehwqpu.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eti.ywan-chungtsiang.top

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://afb.zdqjudy.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://djd.yueranfly.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wzc.dianchejie.cn

[F08] 遍历目录
来源：http://cno.epnwcf.com

Py:   for name in os.listdir("dir"): print(name)
来源：http://ytc.ywan-chungtsiang.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nmx.aibaodan.cn

JS:   fs.readdirSync("dir")
来源：http://lwz.vehdjk.com

TS:   fs.readdirSync("dir")
来源：http://frf.jinghuilouyu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://quz.jqgfzy.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://zcz.mhx1999.top

Ruby: Dir.children("dir")
来源：http://ojc.fanxiaobao.xyz

C#:   Directory.GetFiles("dir")
来源：http://inm.yvedp.cn


<!-- 参考信息 -->