代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://myr.nanxinkj.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://iis.zdbjq.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mjv.guowangkeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tgc.jyoumei.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qgy.wangdashe.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rxy.tanke756.top

[D25] Set 集合去重与交并差
来源：http://kkh.redwolf501.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://drm.redwolf501.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xyw.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fzk.zdbjq.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gww.snrcjt.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ici.yuanzhike.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ikm.daxiang520.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mox.guannengcc.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ehe.gzhubu.top

[D26] 数组转字符串
来源：http://atq.shanyushiyangtech.top

Py:   ", ".join(map(str, arr))
来源：http://htf.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://thm.iojbl.cn

JS:   arr.join(", ")
来源：http://efj.feifeiyinyue.top

TS:   arr.join(", ")
来源：http://sjm.jyoumei.cn

Java: String.join(", ", list)
来源：http://qze.vehdjk.com

Go:   strings.Join(strs, ", ")
来源：http://mzo.xziqi.cn

Ruby: arr.join(", ")
来源：http://rem.cashguo.top

C#:   string.Join(", ", list)
来源：http://fwk.hnqzz.top

================================================================================
来源：http://kne.xingfuxueyuan.xyz

E. 字符串处理
来源：http://pbb.jyoumei.cn

================================================================================
来源：http://fnl.fanxiaobao.xyz

[E01] 拼接字符串
来源：http://njk.birdmap.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rtc.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lqa.zhongyouzk.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tku.chenzaomai.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://dva.shuidangran.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jlg.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ejq.vehdjk.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ixd.sjlbkw.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://alu.guowangkeji.top

[E02] 重复字符串
来源：http://xwn.fengsongda.top

Py:   "ab" * 3
来源：http://lib.cdnleiting.top

PHP:  str_repeat("ab", 3);
来源：http://qtj.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://khg.pycfn.com

TS:   "ab".repeat(3)
来源：http://uhn.meibo888.top

Java: "ab".repeat(3)
来源：http://bop.xziqi.cn

Go:   strings.Repeat("ab", 3)
来源：http://oys.andypj.xyz

Ruby: "ab" * 3
来源：http://oes.nwbrower.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qjt.havefunace.top

[E03] 截取子串
来源：http://etd.zhaomingkeji.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wvi.mhx1999.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mob.zdqjudy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xjq.yangfankeji.com

TS:   s.slice(1, 4)
来源：http://cem.zhijiandao.cn

Java: s.substring(1, 4)
来源：http://eca.zycfv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hoy.hnxiangtu.top

Ruby: s[1, 3];  s[1..3]
来源：http://cwl.nwbrower.top

C#:   s.Substring(1, 3)
来源：http://kmg.yuxming.cn

[E04] 查找子串位置
来源：http://kan.tanke756.top

Py:   s.find("x");  s.index("x")
来源：http://tqw.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://szf.sysykeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zbl.sufxvd.cn

TS:   s.indexOf("x")
来源：http://mor.yvedp.cn

Java: s.indexOf("x")
来源：http://yar.xylfe.cn

Go:   strings.Index(s, "x")
来源：http://fqf.havefunace.top

Ruby: s.index("x")
来源：http://wuu.xinyue.icu

C#:   s.IndexOf("x")
来源：http://ool.hcnkem.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://oxw.yj202588.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://srr.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lfh.shuidangran.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sln.yonumen.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bqw.haohaochexian.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jak.zdqjudy.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fcv.sysykeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://muy.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nft.jinyuanbaomall.cn

[E06] 替换子串
来源：http://npt.shuidangran.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://czm.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://ivl.jinyuanbaomall.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gle.cashguo.top

TS:   s.replaceAll("a", "b")
来源：http://koe.ywan-chungtsiang.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yxh.shanyushiyangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lao.yj20258888.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cbq.wangdashe.top

C#:   s.Replace("a", "b")
来源：http://ljl.zdbjq.cn

[E07] 按分隔符拆分
来源：http://lcm.shuidangran.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wmo.316326.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rgo.ydjk.org.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dwo.cqqwz.cn

TS:   s.split(",")
来源：http://nqi.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://ihn.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dgb.aizwys.cn

Ruby: s.split(",");  s.split
来源：http://dqw.feifeiyinyue.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://igz.yanxiufei.cn

[E08] 数组按分隔符合并
来源：http://spl.nwbrower.top

Py:   ",".join(items)
来源：http://qnk.gotoacloud.top

PHP:  implode(",", $items);
来源：http://xlh.hammf.cn

JS:   items.join(",")
来源：http://mrt.c1oappe.top

TS:   items.join(",")
来源：http://uao.fengsongda.top

Java: String.join(",", items)
来源：http://awj.bjfxy.top

Go:   strings.Join(items, ",")
来源：http://bsc.daxiang520.top

Ruby: items.join(",")
来源：http://wbl.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://zrw.wangdashe.top

[E09] 去除所有空白字符
来源：http://tuo.cheryme.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://spl.yvedp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ang.gogol.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://urq.ybcxt.top

TS:   s.replace(/\s+/g, "")
来源：http://zkt.hongshengwenyu.top

Java: s.replaceAll("\\s+", "")
来源：http://gsv.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dki.epnwcf.com

Ruby: s.gsub(/\s+/, "")
来源：http://qcs.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hjq.hywenlv.cn

[E10] 左侧补零 / 定长填充
来源：http://wpp.sxryk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yxv.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://umv.tian-w.cn

JS:   "7".padStart(3, "0")
来源：http://eek.chenzaomai.com

TS:   "7".padStart(3, "0")
来源：http://ksq.fktsv.cn

Java: String.format("%03d", 7)
来源：http://ibv.tarul.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://xae.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vck.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://kob.jianghu66.top

[E11] 反转字符串
来源：http://amv.fehbvm.com

Py:   s[::-1]
来源：http://ljb.shuidangran.top

PHP:  strrev($s);
来源：http://stn.chenlongwang.top

JS:   [...s].reverse().join("")
来源：http://xzc.yj202588.top

TS:   [...s].reverse().join("")
来源：http://rzv.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://tcm.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kyy.xuetiantiany.cn

Ruby: s.reverse
来源：http://bnj.xinyue.icu

C#:   new string(s.Reverse().ToArray())
来源：http://qjo.jinyuanbaomall.cn

[E12] 统计某字符出现次数
来源：http://ixq.hnqzz.top

Py:   s.count("a")
来源：http://gqh.yuxming.cn

PHP:  substr_count($s, "a");
来源：http://xxh.xingfuxueyuan.xyz

JS:   s.split("a").length - 1
来源：http://adk.nwbrower.top

TS:   s.split("a").length - 1
来源：http://uqj.shzxlz.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vfy.svipenyu.cn

Go:   strings.Count(s, "a")
来源：http://qux.hywenlv.cn

Ruby: s.count("a")
来源：http://ysh.zycfv.cn

C#:   s.Count(c => c == 'a')
来源：http://jhw.fehbvm.com

[E13] 逐字符遍历
来源：http://orw.fktsv.cn

Py:   for ch in s: print(ch)
来源：http://wou.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://poh.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://opj.jlsjyb.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eni.shanyushiyangkeji.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://woi.wangdashe.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bvt.yuanzhike.top

Ruby: s.each_char { |ch| puts ch }
来源：http://veo.fanxiaobao.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bzw.yonumen.top

[E14] URL 编码与 Base64
来源：http://mmf.hnxiangtu.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gda.zhoulong.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://avl.mhx1999.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cvq.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ohx.yangfankeji.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fvs.hnxiangtu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vkd.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://aqw.tanke756.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://swr.haohaochexian.top

[E15] HTML 转义 / 反转义
来源：http://wah.feifeiyinyue.top

Py:   html.escape(s);  html.unescape(s)
来源：http://pay.cdnleiting.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cru.jinyuanbaomall.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yum.wangdashe.top

TS:   // 同上，务必做 XSS 过滤
来源：http://aoc.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wkw.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gqn.guowangkeji.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://urk.guowangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ntu.316326.xyz

[E16] 数字千分位
来源：http://tgm.tanke756.top

Py:   f"{1234567:,}"
来源：http://col.shzxlz.cn

PHP:  number_format(1234567);
来源：http://xhr.wangshuangyany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vck.cheryme.top

TS:   (1234567).toLocaleString("en-US")
来源：http://zdi.ctjpmb.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://two.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uwf.zhoulong.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ada.gzhubu.top

C#:   1234567.ToString("N0")
来源：http://pje.jinqigufen.top

[E17] 首字母大写
来源：http://qip.hesvh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fyk.shuidangran.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fiv.tarul.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qwg.xuetiantiany.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eou.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gta.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hid.kuanghao11.cn

Ruby: s.capitalize
来源：http://dmk.hfpthk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oqq.feifeiyinyue.top

[E18] 模板占位符替换
来源：http://bla.c1oappe.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qen.zhiwuduotai.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tdw.jlsjyb.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ylg.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qmf.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijj.feifeiyinyue.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://feh.tianlin.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tiu.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ffh.mhx1999.top

[E19] 多行文本按行拆分
来源：http://mkf.yvedp.cn

Py:   s.splitlines()
来源：http://tbe.ehwqpu.com

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tgi.vehdjk.com

JS:   s.split(/\r?\n/)
来源：http://gtz.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://mms.feifeiyinyue.top

Java: s.lines().toList()
来源：http://xmt.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://gdc.9152youxi.cn

Ruby: s.lines
来源：http://ztz.ivvv.top

C#:   s.Split('\n')
来源：http://tka.xuetiantiany.cn

[E20] 判断字符串是否为空
来源：http://sxg.fehbvm.com

Py:   if not s:
来源：http://bye.shangyingyoupin.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qpd.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://sxy.pengpengdd.cyou

TS:   if (s === "") {}
来源：http://fkc.wangdashe.top

Java: if (s.isEmpty()) {}
来源：http://mgw.nanxuanxn.top

Go:   if s == "" {}
来源：http://psq.tianlin.xyz

Ruby: if s.empty?
来源：http://gsb.xziqi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bxo.pycfn.com

[E21] 超长截断加省略号
来源：http://lcz.tarul.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xsg.gogol.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aaw.xinyue.icu

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kau.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://akd.xuanzx.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kpw.yangfankeji.com

Go:   // 按 rune 判断长度后截断
来源：http://isi.zhijiandao.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hva.yongpay.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jjz.redwolf501.top

[E22] 字节长度与字符长度
来源：http://zob.hywenlv.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hte.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://glp.shanyushiyangtech.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://adl.cashguo.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gjv.shzxlz.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dtm.dianchejie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tll.tianlin.xyz

Ruby: s.bytesize;  s.length
来源：http://ipa.zhongyouzk.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lmg.yfazqb.com

================================================================================
来源：http://alw.hysaishi.cn

F. 文件与目录
来源：http://qsi.xylfe.cn

================================================================================
来源：http://iyd.yanxiufei.cn

[F01] 读取整个文件
来源：http://bzi.hfpthk.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pjr.xylfe.cn

PHP:  file_get_contents("a.txt");
来源：http://aje.fktsv.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gdt.gotoacloud.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xhf.jyoumei.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mjd.ehwqpu.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gxo.xziqi.cn

Ruby: File.read("a.txt")
来源：http://pvs.zhiwuduotai.top

C#:   File.ReadAllText("a.txt");
来源：http://mpr.bbcook.cn

[F02] 逐行读取文件
来源：http://cth.52xcode.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fhe.wangshuangyany.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jtf.316326.xyz

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhq.mhx1999.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xhi.ydzc1.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://nve.chenjidiqi.icu

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fap.sjlbkw.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qdj.yueranfly.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://typ.zhixingplan.top

[F03] 写入文件（覆盖）
来源：http://hoi.c1oappe.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eeb.haohaochexian.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gsa.zdqjudy.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iiy.yanxiufei.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://szd.havefunace.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tuf.shanyushiyangtech.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wis.sxryk.cn

Ruby: File.write("a.txt", "hi")
来源：http://hid.svipenyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iyj.haohaochexian.top

[F04] 追加写入文件
来源：http://qqb.guannengcc.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ble.yuanzhike.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wmq.iojbl.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ipy.yj202588.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vvw.ywan-chungtsiang.top

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ztc.tarul.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hea.xziqi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://shb.iojbl.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kup.nwbrower.top

[F05] 判断文件或目录是否存在
来源：http://wff.hongshengwenyu.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://xwf.shangyingyoupin.top

PHP:  file_exists("a.txt");
来源：http://lzp.hnxiangtu.top

JS:   fs.existsSync("a.txt")
来源：http://mqo.xuanzx.com

TS:   fs.existsSync("a.txt")
来源：http://xrl.316326.xyz

Java: Files.exists(Path.of("a.txt"))
来源：http://ifo.fengsongda.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lxx.hnqzz.top

Ruby: File.exist?("a.txt")
来源：http://nwb.tarul.cn

C#:   File.Exists("a.txt")
来源：http://wsn.xziqi.cn

[F06] 删除文件
来源：http://qdp.fanxiaobao.xyz

Py:   os.remove("a.txt")
来源：http://zbi.gotoacloud.top

PHP:  unlink("a.txt");
来源：http://ary.aibaodan.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fxj.iojbl.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lsx.zhiwuduotai.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fdh.meibo888.top

Go:   os.Remove("a.txt")
来源：http://fzg.c1oappe.top

Ruby: File.delete("a.txt")
来源：http://ksr.fehbvm.com

C#:   File.Delete("a.txt");
来源：http://kqb.zhoulong.xyz

[F07] 创建目录（含多级）
来源：http://ezz.0kj1m.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gmh.yangfankeji.com

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hps.cucudq.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://stl.cucudq.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hzr.hysaishi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qdt.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://duh.ehwqpu.com

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tck.chenzaomai.com

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jgc.jqgufenzy.top

[F08] 遍历目录
来源：http://hor.zhixingplan.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://srp.nanxinkj.top

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qus.cdnleiting.top

JS:   fs.readdirSync("dir")
来源：http://hbp.svipenyu.cn

TS:   fs.readdirSync("dir")
来源：http://wof.daria6918.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fdf.havefunace.top

Go:   entries, _ := os.ReadDir("dir")
来源：http://fui.cashguo.top

Ruby: Dir.children("dir")
来源：http://ipy.dashuyun.cn

C#:   Directory.GetFiles("dir")
来源：http://agv.jlsjyb.cn


<!-- 参考信息 -->