代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zqi.zhaomingkeji.xyz

[D24] 字典 / Map 基本操作
来源：http://ufb.chenzaomai.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://lmm.aibaodan.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nyd.yfazqb.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://otj.jlsjyb.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gax.feifeiyinyue.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ist.xuetiantiany.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nhi.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ebf.shangyingyoupin.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://meu.tian-w.cn

[D25] Set 集合去重与交并差
来源：http://rzt.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://odu.xziqi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kau.quarkkingdee.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rge.hnqzz.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://nld.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://owh.snrcjt.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xkd.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uhy.sweek.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ans.hysaishi.cn

[D26] 数组转字符串
来源：http://dot.guowangkeji.top

Py:   ", ".join(map(str, arr))
来源：http://air.ydzc1.top

PHP:  implode(", ", $arr);
来源：http://liq.kuanghao11.cn

JS:   arr.join(", ")
来源：http://znt.tianlin.xyz

TS:   arr.join(", ")
来源：http://xep.shanyushiyangkeji.top

Java: String.join(", ", list)
来源：http://ihq.chenzaomai.com

Go:   strings.Join(strs, ", ")
来源：http://xfk.cucudq.cn

Ruby: arr.join(", ")
来源：http://hlu.hysaishi.cn

C#:   string.Join(", ", list)
来源：http://ude.fengsongda.top

================================================================================
来源：http://zcr.xingfuxueyuan.xyz

E. 字符串处理
来源：http://vqz.uphjek.com

================================================================================
来源：http://som.jinyuanbaomall.cn

[E01] 拼接字符串
来源：http://kmp.zycfv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uen.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zjk.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jou.hongshengwenyu.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://noq.fzhhl.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sex.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uit.zhijiandao.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wkd.fanxiaobao.xyz

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wdz.ivvv.top

[E02] 重复字符串
来源：http://sps.wangshuangyany.cn

Py:   "ab" * 3
来源：http://leo.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://gkx.9152youxi.cn

JS:   "ab".repeat(3)
来源：http://yzo.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://cmy.yj202588.top

Java: "ab".repeat(3)
来源：http://kzv.sufxvd.cn

Go:   strings.Repeat("ab", 3)
来源：http://jsa.epnwcf.com

Ruby: "ab" * 3
来源：http://lrl.aibaodan.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ixq.yuxming.cn

[E03] 截取子串
来源：http://xdy.zhijiandao.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nto.sufxvd.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://sbe.xuetiantiany.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uzi.daxiang520.top

TS:   s.slice(1, 4)
来源：http://bpu.ywan-chungtsiang.top

Java: s.substring(1, 4)
来源：http://pyy.zhijiandao.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://stj.hammf.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cqg.svipenyu.cn

C#:   s.Substring(1, 3)
来源：http://vbs.jinghuilouyu.cn

[E04] 查找子串位置
来源：http://tie.bjfxy.top

Py:   s.find("x");  s.index("x")
来源：http://lpk.guannengcc.top

PHP:  strpos($s, "x");
来源：http://wbu.ehwqpu.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://exm.c1oappe.top

TS:   s.indexOf("x")
来源：http://lsd.tian-w.cn

Java: s.indexOf("x")
来源：http://coe.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://fdy.yj20258.top

Ruby: s.index("x")
来源：http://dco.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://tgx.sysykeji.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mte.birdmap.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ifb.ivvv.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qdi.xuanzx.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fak.yanxiufei.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pkp.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hhm.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ymc.chenjidiqi.icu

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wrg.yj202588.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fto.ybcxt.top

[E06] 替换子串
来源：http://tlk.guowangkeji.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://aik.fanxiaobao.xyz

PHP:  str_replace("a", "b", $s);
来源：http://ocq.yangfankeji.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wyh.xuanzx.com

TS:   s.replaceAll("a", "b")
来源：http://rtn.fanxiaobao.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jyt.cdnleiting.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cnc.mhx1999.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rii.nwbrower.top

C#:   s.Replace("a", "b")
来源：http://ypf.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://yxg.hammf.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://odb.jinyuanbaomall.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xwv.sxryk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://suu.yuanzhike.top

TS:   s.split(",")
来源：http://pfj.zdqjudy.top

Java: s.split(",");  s.split("\\s+")
来源：http://jbd.yuanzhike.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uuy.bjfxy.top

Ruby: s.split(",");  s.split
来源：http://ujj.xingfuxueyuan.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://twc.xingfuxueyuan.xyz

[E08] 数组按分隔符合并
来源：http://tbd.yj202588.top

Py:   ",".join(items)
来源：http://xcr.iojbl.cn

PHP:  implode(",", $items);
来源：http://jqj.wangshuangyany.cn

JS:   items.join(",")
来源：http://qmb.wangshuangyany.cn

TS:   items.join(",")
来源：http://szn.zhiwuduotai.top

Java: String.join(",", items)
来源：http://wqc.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://wpj.chenjidiqi.icu

Ruby: items.join(",")
来源：http://pcf.cucudq.cn

C#:   string.Join(",", items)
来源：http://yyx.jinyuanbaomall.cn

[E09] 去除所有空白字符
来源：http://aeo.hammf.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cie.tianlin.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zyk.shuidangran.top

JS:   s.replace(/\s+/g, "")
来源：http://ugl.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://brh.hammf.cn

Java: s.replaceAll("\\s+", "")
来源：http://nck.ctjpmb.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://zsu.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lte.shanyushiyangtech.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://phh.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://vyu.tianlin.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://day.yongpay.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fau.chenjidiqi.icu

JS:   "7".padStart(3, "0")
来源：http://kis.nanxinkj.top

TS:   "7".padStart(3, "0")
来源：http://xpn.iojbl.cn

Java: String.format("%03d", 7)
来源：http://fub.aizwys.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fzm.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://clv.jqgfzy.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://axo.yuxming.cn

[E11] 反转字符串
来源：http://qzy.vehdjk.com

Py:   s[::-1]
来源：http://edm.fktsv.cn

PHP:  strrev($s);
来源：http://tjf.jinqigfzy.top

JS:   [...s].reverse().join("")
来源：http://ekc.52xcode.cn

TS:   [...s].reverse().join("")
来源：http://rkp.dashuyun.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ytm.svipenyu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wpk.yanxiufei.cn

Ruby: s.reverse
来源：http://ncn.zhixingplan.top

C#:   new string(s.Reverse().ToArray())
来源：http://vyr.fehbvm.com

[E12] 统计某字符出现次数
来源：http://dje.fktsv.cn

Py:   s.count("a")
来源：http://nsx.gotoacloud.top

PHP:  substr_count($s, "a");
来源：http://ogy.sufxvd.cn

JS:   s.split("a").length - 1
来源：http://dkq.316326.xyz

TS:   s.split("a").length - 1
来源：http://opj.hywenlv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zsw.hfpthk.cn

Go:   strings.Count(s, "a")
来源：http://anq.zhijiandao.cn

Ruby: s.count("a")
来源：http://ekd.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://fep.shzxlz.cn

[E13] 逐字符遍历
来源：http://ysm.jinqigufen.top

Py:   for ch in s: print(ch)
来源：http://zqn.gotoacloud.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://aml.hywenlv.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://upx.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tcp.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://daz.zhijiandao.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qsf.yanxiufei.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kun.ehwqpu.com

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xvr.gzhubu.top

[E14] URL 编码与 Base64
来源：http://uor.sufxvd.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rpd.jinqigufen.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gke.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ahx.sxryk.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://cyi.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wig.svipenyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xrl.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fkh.nanxuanxn.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfa.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://mat.gotoacloud.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iog.bbcook.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uqk.zhixingplan.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dpb.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iqy.xziqi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cvw.gotoacloud.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nzg.birdmap.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gqu.fehbvm.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ytt.chenjidiqi.icu

[E16] 数字千分位
来源：http://heo.hesvh.cn

Py:   f"{1234567:,}"
来源：http://blt.shzxlz.cn

PHP:  number_format(1234567);
来源：http://xzv.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://rgc.gzhubu.top

TS:   (1234567).toLocaleString("en-US")
来源：http://wmq.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ogf.tanke756.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://gqi.cucudq.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ycc.cucudq.cn

C#:   1234567.ToString("N0")
来源：http://hnm.xinyue.icu

[E17] 首字母大写
来源：http://paw.xuanzx.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ipj.yanxiufei.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zqz.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vca.fktsv.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zka.yuanzhike.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ceu.zhoulong.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bff.52xcode.cn

Ruby: s.capitalize
来源：http://grr.9152youxi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lrw.redwolf501.top

[E18] 模板占位符替换
来源：http://oub.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bhr.chenjidiqi.icu

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bvn.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hks.xingfuxueyuan.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://suc.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zsl.316326.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bqu.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mlg.daxiang520.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://oaa.tanke756.top

[E19] 多行文本按行拆分
来源：http://xir.hysaishi.cn

Py:   s.splitlines()
来源：http://gkg.jinyuanbaomall.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://kdy.hongshengwenyu.top

JS:   s.split(/\r?\n/)
来源：http://sns.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://bhc.cdnleiting.top

Java: s.lines().toList()
来源：http://rjt.guannengcc.top

Go:   strings.Split(s, "\n")
来源：http://meq.yongpay.top

Ruby: s.lines
来源：http://hoo.ppjwa.cn

C#:   s.Split('\n')
来源：http://yir.yuxming.cn

[E20] 判断字符串是否为空
来源：http://vjw.gotoacloud.top

Py:   if not s:
来源：http://yel.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://evd.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ltb.c1oappe.top

TS:   if (s === "") {}
来源：http://aiw.jyoumei.cn

Java: if (s.isEmpty()) {}
来源：http://ymy.jiagoushi.top

Go:   if s == "" {}
来源：http://pie.jyoumei.cn

Ruby: if s.empty?
来源：http://wcy.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pls.shanyushiyangkeji.top

[E21] 超长截断加省略号
来源：http://bfg.hywenlv.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jns.gaohongyu789.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gin.ydjk.org.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxc.dianchejie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vcm.zdbjq.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://suh.jinyuanbaomall.cn

Go:   // 按 rune 判断长度后截断
来源：http://fpr.c1oappe.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wak.hysaishi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yoi.ywan-chungtsiang.top

[E22] 字节长度与字符长度
来源：http://stl.guowangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rwo.yj202588.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ocf.guowangkeji.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yej.hfpthk.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://atc.yvedp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vmt.yj202588.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nhb.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://mky.gaohongyu789.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qaq.cdnleiting.top

================================================================================
来源：http://dpe.snrcjt.cn

F. 文件与目录
来源：http://qji.ivvv.top

================================================================================
来源：http://djv.chenlongwang.top

[F01] 读取整个文件
来源：http://rtf.snrcjt.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qsc.ybcxt.top

PHP:  file_get_contents("a.txt");
来源：http://ksy.iojbl.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zqz.sweek.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lfv.nanxinkj.top

Java: Files.readString(Path.of("a.txt"))
来源：http://omm.smart0.xyz

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jva.hongshengwenyu.top

Ruby: File.read("a.txt")
来源：http://ame.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://xln.sxryk.cn

[F02] 逐行读取文件
来源：http://fvs.hnqzz.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jti.yfazqb.com

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lqi.jqgfzy.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://boy.yangfankeji.com

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jkw.quarkkingdee.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ewu.redwolf501.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jpi.nanxuanxn.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yls.zycfv.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iay.xingfuxueyuan.xyz

[F03] 写入文件（覆盖）
来源：http://har.yongpay.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tkr.sjlbkw.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zhk.ybcxt.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jxa.guannengcc.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://aks.jqgfzy.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ysb.snrcjt.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yix.bjfxy.top

Ruby: File.write("a.txt", "hi")
来源：http://tqh.aizwys.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://enj.sxryk.cn

[F04] 追加写入文件
来源：http://cxq.ivvv.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jxf.jinghuilouyu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://egi.pycfn.com

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yoy.vehdjk.com

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qxy.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rpz.chenjidiqi.icu

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cix.chenjidiqi.icu

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wat.yanxiufei.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hwc.yuxming.cn

[F05] 判断文件或目录是否存在
来源：http://irm.uphjek.com

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://enr.jqgufenzy.top

PHP:  file_exists("a.txt");
来源：http://yva.cheryme.top

JS:   fs.existsSync("a.txt")
来源：http://rbe.sweek.top

TS:   fs.existsSync("a.txt")
来源：http://jrm.jlsjyb.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bjv.hnqzz.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ied.vehdjk.com

Ruby: File.exist?("a.txt")
来源：http://agi.fzhhl.top

C#:   File.Exists("a.txt")
来源：http://mpi.chenjidiqi.icu

[F06] 删除文件
来源：http://cyp.yuxming.cn

Py:   os.remove("a.txt")
来源：http://gez.pengpengdd.cyou

PHP:  unlink("a.txt");
来源：http://goq.yvedp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gew.jyoumei.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nwl.kuanghao11.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://evr.redwolf501.top

Go:   os.Remove("a.txt")
来源：http://qra.gzhubu.top

Ruby: File.delete("a.txt")
来源：http://uhl.cucudq.cn

C#:   File.Delete("a.txt");
来源：http://nai.dashuyun.cn

[F07] 创建目录（含多级）
来源：http://uvk.shzxlz.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ray.shanyushiyangtech.top

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hri.jyoumei.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cch.guowangkeji.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ine.0kj1m.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mcp.hysaishi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kqq.xziqi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hbz.chenjidiqi.icu

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qkl.redwolf501.top

[F08] 遍历目录
来源：http://orc.sjlbkw.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://nkm.chenjidiqi.icu

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eju.chenlongwang.top

JS:   fs.readdirSync("dir")
来源：http://tqv.fanxiaobao.xyz

TS:   fs.readdirSync("dir")
来源：http://jai.mhx1999.top


<!-- 参考信息 -->