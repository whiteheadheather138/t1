代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tvn.dashuyun.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eus.wangshuangyany.cn

Go:   // 手写循环
来源：http://cdx.wangshuangyany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://whs.yanxiufei.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://llo.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://dqf.pengpengdd.cyou

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xwl.jinqigufen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pnt.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nrq.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kia.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tfv.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vzz.pycfn.com

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://umu.cqqwz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lua.fzhhl.top

[D25] Set 集合去重与交并差
来源：http://dbi.zhengqikj.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lvj.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xpm.cqqwz.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vfb.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eta.zhijiandao.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mnw.chenlongwang.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://amp.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ayy.hywenlv.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gab.cheryme.top

[D26] 数组转字符串
来源：http://srv.gaohongyu789.top

Py:   ", ".join(map(str, arr))
来源：http://xcw.cucudq.cn

PHP:  implode(", ", $arr);
来源：http://qwj.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://udb.yonumen.top

TS:   arr.join(", ")
来源：http://eac.zhoulong.xyz

Java: String.join(", ", list)
来源：http://cfj.hfpthk.cn

Go:   strings.Join(strs, ", ")
来源：http://ftp.jiagoushi.top

Ruby: arr.join(", ")
来源：http://lhh.cucudq.cn

C#:   string.Join(", ", list)
来源：http://ygg.hongshengwenyu.top

================================================================================
来源：http://fqo.gotoacloud.top

E. 字符串处理
来源：http://jom.zdbjq.cn

================================================================================
来源：http://fxh.zdqjudy.top

[E01] 拼接字符串
来源：http://ebr.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lve.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hfi.hesvh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://elq.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hah.jqgfzy.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pgg.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jaw.yuxming.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pqp.daxiang520.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bol.zhiwuduotai.top

[E02] 重复字符串
来源：http://pua.jlsjyb.cn

Py:   "ab" * 3
来源：http://qan.yuanzhike.top

PHP:  str_repeat("ab", 3);
来源：http://iel.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://wwb.yongpay.top

TS:   "ab".repeat(3)
来源：http://sez.yj202588.top

Java: "ab".repeat(3)
来源：http://bkb.meibo888.top

Go:   strings.Repeat("ab", 3)
来源：http://ruk.gaohongyu789.top

Ruby: "ab" * 3
来源：http://uaa.xinyue.icu

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tpo.yongpay.top

[E03] 截取子串
来源：http://ttg.yj20258.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fwx.c1oappe.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xmb.cheryme.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tos.tanke756.top

TS:   s.slice(1, 4)
来源：http://wnt.ivvv.top

Java: s.substring(1, 4)
来源：http://mje.sxryk.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://dlk.yfazqb.com

Ruby: s[1, 3];  s[1..3]
来源：http://svk.xinyue.icu

C#:   s.Substring(1, 3)
来源：http://ivf.c1oappe.top

[E04] 查找子串位置
来源：http://dsb.tian-w.cn

Py:   s.find("x");  s.index("x")
来源：http://qrp.52xcode.cn

PHP:  strpos($s, "x");
来源：http://kuk.zhongyouzk.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wbz.daxiang520.top

TS:   s.indexOf("x")
来源：http://gjs.yuanzhike.top

Java: s.indexOf("x")
来源：http://ewz.shuidangran.top

Go:   strings.Index(s, "x")
来源：http://krz.xziqi.cn

Ruby: s.index("x")
来源：http://uuz.meibo888.top

C#:   s.IndexOf("x")
来源：http://puw.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://yuy.jinqigfzy.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://frb.quarkkingdee.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wog.52xcode.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pju.ctjpmb.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://gpq.gaohongyu789.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://whx.yvedp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kkc.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lpg.xuanzx.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://myz.uphjek.com

[E06] 替换子串
来源：http://fvu.bjfxy.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hfr.tian-w.cn

PHP:  str_replace("a", "b", $s);
来源：http://ftc.redwolf501.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bxq.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://peb.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mrh.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hpq.jyoumei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://itz.quarkkingdee.top

C#:   s.Replace("a", "b")
来源：http://xgk.hnxiangtu.top

[E07] 按分隔符拆分
来源：http://xei.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xcu.zhoulong.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lgk.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zpj.yuxming.cn

TS:   s.split(",")
来源：http://twf.hfpthk.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sbu.kuanghao11.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fzo.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://uol.xuanzx.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wha.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://omh.tanke756.top

Py:   ",".join(items)
来源：http://jkw.fktsv.cn

PHP:  implode(",", $items);
来源：http://hyg.tanke756.top

JS:   items.join(",")
来源：http://dfx.gotoacloud.top

TS:   items.join(",")
来源：http://naf.ybcxt.top

Java: String.join(",", items)
来源：http://mkt.nwbrower.top

Go:   strings.Join(items, ",")
来源：http://eof.kuanghao11.cn

Ruby: items.join(",")
来源：http://bmr.fanxiaobao.xyz

C#:   string.Join(",", items)
来源：http://tbs.zdqjudy.top

[E09] 去除所有空白字符
来源：http://ipv.ywan-chungtsiang.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ouo.daria6918.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wjk.sufxvd.cn

JS:   s.replace(/\s+/g, "")
来源：http://pto.snrcjt.cn

TS:   s.replace(/\s+/g, "")
来源：http://djd.ivvv.top

Java: s.replaceAll("\\s+", "")
来源：http://nam.sxryk.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jlb.cqqwz.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xwe.snrcjt.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ujc.yj202588.top

[E10] 左侧补零 / 定长填充
来源：http://dyl.epnwcf.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bkn.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gqa.c1oappe.top

JS:   "7".padStart(3, "0")
来源：http://peb.quarkkingdee.top

TS:   "7".padStart(3, "0")
来源：http://por.hesvh.cn

Java: String.format("%03d", 7)
来源：http://vkn.316326.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://suy.fengsongda.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://szv.jqgufenzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zxt.fehbvm.com

[E11] 反转字符串
来源：http://abb.ivvv.top

Py:   s[::-1]
来源：http://xmb.xylfe.cn

PHP:  strrev($s);
来源：http://kcl.sweek.top

JS:   [...s].reverse().join("")
来源：http://abf.tianlin.xyz

TS:   [...s].reverse().join("")
来源：http://etu.andypj.xyz

Java: new StringBuilder(s).reverse().toString()
来源：http://cif.cqqwz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yth.ctjpmb.com

Ruby: s.reverse
来源：http://amy.shanyushiyangkeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://zse.shanyushiyangtech.top

[E12] 统计某字符出现次数
来源：http://vog.tianlin.xyz

Py:   s.count("a")
来源：http://lrh.chenjidiqi.icu

PHP:  substr_count($s, "a");
来源：http://jiy.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://wne.hywenlv.cn

TS:   s.split("a").length - 1
来源：http://kwa.jqgufenzy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hqk.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://nbl.havefunace.top

Ruby: s.count("a")
来源：http://iom.cucudq.cn

C#:   s.Count(c => c == 'a')
来源：http://rzk.gzhubu.top

[E13] 逐字符遍历
来源：http://syi.guannengcc.top

Py:   for ch in s: print(ch)
来源：http://hke.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fhl.zdqjudy.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cpe.ctjpmb.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://hsj.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pcl.fanxiaobao.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dbz.snrcjt.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://umn.smart0.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wik.yj202588.top

[E14] URL 编码与 Base64
来源：http://azx.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cod.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://guk.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://rfv.andypj.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zhp.ydjk.org.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ity.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uck.jiagoushi.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yhl.kuanghao11.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cqd.snrcjt.cn

[E15] HTML 转义 / 反转义
来源：http://llh.daxiang520.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mrv.ybcxt.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gnz.hesvh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hgj.shangyingyoupin.top

TS:   // 同上，务必做 XSS 过滤
来源：http://cxx.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ndp.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pqt.ydjk.org.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nuu.kuanghao11.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vlf.shanyushiyangtech.top

[E16] 数字千分位
来源：http://xsb.cdnleiting.top

Py:   f"{1234567:,}"
来源：http://xpa.xuanzx.com

PHP:  number_format(1234567);
来源：http://iev.shanyushiyangtech.top

JS:   (1234567).toLocaleString("en-US")
来源：http://kzd.zhongyouzk.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cgb.daria6918.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jci.yanxiufei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jsd.xziqi.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cqy.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://kkt.dianchejie.cn

[E17] 首字母大写
来源：http://veo.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gdg.sysykeji.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://mrv.kuanghao11.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vmi.andypj.xyz

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cep.ybcxt.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://olh.fktsv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rjp.aizwys.cn

Ruby: s.capitalize
来源：http://nui.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://eml.yj202588.top

[E18] 模板占位符替换
来源：http://kgc.yfazqb.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wzo.vqdsnc.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tzb.hesvh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://nwu.cdnleiting.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pic.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cjo.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://don.yueranfly.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://six.chenjidiqi.icu

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oru.snrcjt.cn

[E19] 多行文本按行拆分
来源：http://qfg.sysykeji.top

Py:   s.splitlines()
来源：http://oiz.sweek.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://raz.zhaomingkeji.xyz

JS:   s.split(/\r?\n/)
来源：http://ghy.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://udb.c1oappe.top

Java: s.lines().toList()
来源：http://paw.ctjpmb.com

Go:   strings.Split(s, "\n")
来源：http://hjb.zdbjq.cn

Ruby: s.lines
来源：http://peu.epnwcf.com

C#:   s.Split('\n')
来源：http://lpi.yj20258.top

[E20] 判断字符串是否为空
来源：http://znl.uphjek.com

Py:   if not s:
来源：http://gth.zhiwuduotai.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tmc.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://bli.aizwys.cn

TS:   if (s === "") {}
来源：http://ypz.tarul.cn

Java: if (s.isEmpty()) {}
来源：http://jvy.0kj1m.cn

Go:   if s == "" {}
来源：http://elv.wangdashe.top

Ruby: if s.empty?
来源：http://rvg.316326.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qbs.hnqzz.top

[E21] 超长截断加省略号
来源：http://wsa.52xcode.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://rpi.ybcxt.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wtt.ivvv.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://poa.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bez.shzxlz.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://niu.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://uey.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ptn.andypj.xyz

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zyg.xinyue.icu

[E22] 字节长度与字符长度
来源：http://htx.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hdf.dianchejie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwu.yj202588.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://alp.hesvh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kin.ydzc1.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ytx.hfpthk.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dah.shzxlz.cn

Ruby: s.bytesize;  s.length
来源：http://vkx.jinghuilouyu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kuw.svipenyu.cn

================================================================================
来源：http://bqj.tarul.cn

F. 文件与目录
来源：http://kgm.gotoacloud.top

================================================================================
来源：http://rwa.kuanghao11.cn

[F01] 读取整个文件
来源：http://qzj.zycfv.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sph.hesvh.cn

PHP:  file_get_contents("a.txt");
来源：http://voi.cheryme.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zbc.bjfxy.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vwd.tanke756.top

Java: Files.readString(Path.of("a.txt"))
来源：http://zct.nanxinkj.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://cyj.vqdsnc.cn

Ruby: File.read("a.txt")
来源：http://cdw.zhaomingkeji.xyz

C#:   File.ReadAllText("a.txt");
来源：http://btz.xuanzx.com

[F02] 逐行读取文件
来源：http://srg.ydzc1.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bta.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mpx.hnxiangtu.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dcx.svipenyu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://azh.pycfn.com

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tea.xylfe.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xgb.yj20258.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ueh.yvedp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wey.fzhhl.top

[F03] 写入文件（覆盖）
来源：http://zym.jlsjyb.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rkd.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://vir.zhoulong.xyz

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vfu.jinyuanbaomall.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fiz.zhijiandao.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vcn.yj20258.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ksb.gzhubu.top

Ruby: File.write("a.txt", "hi")
来源：http://cga.gogol.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qyv.0kj1m.cn

[F04] 追加写入文件
来源：http://eyf.gotoacloud.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ill.cashguo.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://uay.hysaishi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nie.sxryk.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ouk.ydjk.org.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gnr.jiagoushi.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bjh.pengpengdd.cyou

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gxi.shanyushiyangkeji.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ope.zdqjudy.top

[F05] 判断文件或目录是否存在
来源：http://ljh.zycfv.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gsa.yfazqb.com

PHP:  file_exists("a.txt");
来源：http://hzb.wangdashe.top

JS:   fs.existsSync("a.txt")
来源：http://xav.chenjidiqi.icu

TS:   fs.existsSync("a.txt")
来源：http://qyp.ivvv.top

Java: Files.exists(Path.of("a.txt"))
来源：http://nxq.cdnleiting.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://atd.nanxinkj.top

Ruby: File.exist?("a.txt")
来源：http://wsq.yonumen.top

C#:   File.Exists("a.txt")
来源：http://mog.c1oappe.top

[F06] 删除文件
来源：http://qom.uphjek.com

Py:   os.remove("a.txt")
来源：http://fpi.shzxlz.cn

PHP:  unlink("a.txt");
来源：http://qch.xylfe.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qcq.hysaishi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gxj.hnxiangtu.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://acq.shzxlz.cn

Go:   os.Remove("a.txt")
来源：http://jxv.sxryk.cn

Ruby: File.delete("a.txt")
来源：http://nyx.svipenyu.cn

C#:   File.Delete("a.txt");
来源：http://jih.zhixingplan.top

[F07] 创建目录（含多级）
来源：http://gxe.ehwqpu.com

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qbk.chenjidiqi.icu

PHP:  mkdir("dir/sub", 0777, true);
来源：http://axp.xuetiantiany.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gig.fehbvm.com

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tju.fktsv.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dcl.kuanghao11.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jqa.zdbjq.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iqi.vqdsnc.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iun.yonumen.top

[F08] 遍历目录
来源：http://abg.sxryk.cn


<!-- 参考信息 -->