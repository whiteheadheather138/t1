代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://liu.chenzaomai.com

[D24] 字典 / Map 基本操作
来源：http://wgu.jinqigfzy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nww.jinghuilouyu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wzw.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yjh.smart0.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pfa.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://etv.chenjidiqi.icu

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zsl.bjfxy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vhf.sysykeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://onp.hywenlv.cn

[D25] Set 集合去重与交并差
来源：http://bjk.xinyue.icu

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nfx.fehbvm.com

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bhp.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ndx.kuanghao11.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ggj.haohaochexian.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ihs.jinyuanbaomall.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://khk.yfazqb.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cso.shanyushiyangkeji.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://noh.svipenyu.cn

[D26] 数组转字符串
来源：http://snp.jianghu66.top

Py:   ", ".join(map(str, arr))
来源：http://qxz.gzhubu.top

PHP:  implode(", ", $arr);
来源：http://ijt.jinyuanbaomall.cn

JS:   arr.join(", ")
来源：http://mvy.sweek.top

TS:   arr.join(", ")
来源：http://pys.xziqi.cn

Java: String.join(", ", list)
来源：http://eiy.aibaodan.cn

Go:   strings.Join(strs, ", ")
来源：http://ooz.nwbrower.top

Ruby: arr.join(", ")
来源：http://kbv.ydzc1.top

C#:   string.Join(", ", list)
来源：http://gki.xylfe.cn

================================================================================
来源：http://exc.yvedp.cn

E. 字符串处理
来源：http://vom.bjfxy.top

================================================================================
来源：http://qua.uphjek.com

[E01] 拼接字符串
来源：http://wvu.dashuyun.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://svm.guowangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oes.ybcxt.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xql.aizwys.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aba.ivvv.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cul.daxiang520.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bjz.shanyushiyangkeji.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://psi.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zup.52xcode.cn

[E02] 重复字符串
来源：http://esj.fktsv.cn

Py:   "ab" * 3
来源：http://aig.vqdsnc.cn

PHP:  str_repeat("ab", 3);
来源：http://ffe.shuidangran.top

JS:   "ab".repeat(3)
来源：http://mhi.0kj1m.cn

TS:   "ab".repeat(3)
来源：http://tmu.epnwcf.com

Java: "ab".repeat(3)
来源：http://dim.52xcode.cn

Go:   strings.Repeat("ab", 3)
来源：http://pcc.cashguo.top

Ruby: "ab" * 3
来源：http://kpm.jqgfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://orj.wangdashe.top

[E03] 截取子串
来源：http://zcv.52xcode.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tuh.guannengcc.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bpl.ppjwa.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uke.bjfxy.top

TS:   s.slice(1, 4)
来源：http://ejd.shanyushiyangtech.top

Java: s.substring(1, 4)
来源：http://nth.bbcook.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gsc.yvedp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ncg.yongpay.top

C#:   s.Substring(1, 3)
来源：http://fjv.haohaochexian.top

[E04] 查找子串位置
来源：http://tng.hysaishi.cn

Py:   s.find("x");  s.index("x")
来源：http://bfs.hysaishi.cn

PHP:  strpos($s, "x");
来源：http://kac.xuanzx.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://udr.jiagoushi.top

TS:   s.indexOf("x")
来源：http://vyh.guowangkeji.top

Java: s.indexOf("x")
来源：http://sqr.xuanzx.com

Go:   strings.Index(s, "x")
来源：http://tws.dianchejie.cn

Ruby: s.index("x")
来源：http://ivi.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://isj.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://dxe.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bmq.haohaochexian.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sjd.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kbd.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://onp.ywan-chungtsiang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ohe.9152youxi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ewx.dashuyun.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://szn.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aeu.cashguo.top

[E06] 替换子串
来源：http://yvk.ybcxt.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yle.guannengcc.top

PHP:  str_replace("a", "b", $s);
来源：http://iok.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nwq.gzhubu.top

TS:   s.replaceAll("a", "b")
来源：http://toq.tian-w.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dxh.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wjf.vehdjk.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qtm.tarul.cn

C#:   s.Replace("a", "b")
来源：http://ohy.9152youxi.cn

[E07] 按分隔符拆分
来源：http://vmi.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pdm.ydzc1.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lvv.iojbl.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uwq.nwbrower.top

TS:   s.split(",")
来源：http://wtd.tianlin.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://vtb.hongshengwenyu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xzk.hammf.cn

Ruby: s.split(",");  s.split
来源：http://gnf.pycfn.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qhb.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://atc.bbcook.cn

Py:   ",".join(items)
来源：http://rzl.yangfankeji.com

PHP:  implode(",", $items);
来源：http://nil.shanyushiyangkeji.top

JS:   items.join(",")
来源：http://wiw.bbcook.cn

TS:   items.join(",")
来源：http://tmx.guowangkeji.top

Java: String.join(",", items)
来源：http://yqc.gogol.net.cn

Go:   strings.Join(items, ",")
来源：http://pdz.yuanzhike.top

Ruby: items.join(",")
来源：http://acr.yuanzhike.top

C#:   string.Join(",", items)
来源：http://qov.hnqzz.top

[E09] 去除所有空白字符
来源：http://gsn.jianghu66.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://iny.zhoulong.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pjz.iojbl.cn

JS:   s.replace(/\s+/g, "")
来源：http://fet.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://jpe.hesvh.cn

Java: s.replaceAll("\\s+", "")
来源：http://yqy.havefunace.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://eyc.fengsongda.top

Ruby: s.gsub(/\s+/, "")
来源：http://hlf.yangfankeji.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yxe.havefunace.top

[E10] 左侧补零 / 定长填充
来源：http://uji.mhx1999.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://eai.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bne.sweek.top

JS:   "7".padStart(3, "0")
来源：http://crm.chenjidiqi.icu

TS:   "7".padStart(3, "0")
来源：http://bma.meibo888.top

Java: String.format("%03d", 7)
来源：http://vpv.gaohongyu789.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ahz.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qji.yj20258888.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nzj.haohaochexian.top

[E11] 反转字符串
来源：http://sro.ppjwa.cn

Py:   s[::-1]
来源：http://ghp.sysykeji.top

PHP:  strrev($s);
来源：http://dep.tarul.cn

JS:   [...s].reverse().join("")
来源：http://suc.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://sts.ivvv.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jbh.wangdashe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://uqw.ehwqpu.com

Ruby: s.reverse
来源：http://zhf.sufxvd.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tif.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://pig.zhiwuduotai.top

Py:   s.count("a")
来源：http://pje.ctjpmb.com

PHP:  substr_count($s, "a");
来源：http://sot.jinyuanbaomall.cn

JS:   s.split("a").length - 1
来源：http://icj.pengpengdd.cyou

TS:   s.split("a").length - 1
来源：http://ddl.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mwp.bjfxy.top

Go:   strings.Count(s, "a")
来源：http://dfv.nwbrower.top

Ruby: s.count("a")
来源：http://sty.ctjpmb.com

C#:   s.Count(c => c == 'a')
来源：http://ovn.ppjwa.cn

[E13] 逐字符遍历
来源：http://dgj.andypj.xyz

Py:   for ch in s: print(ch)
来源：http://yxv.shzxlz.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cyu.zhongyouzk.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://qjh.sjlbkw.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zfx.yonumen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ufe.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sgr.aibaodan.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://zff.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xsb.fanxiaobao.xyz

[E14] URL 编码与 Base64
来源：http://vwy.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kbk.ywan-chungtsiang.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xer.zhoulong.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://auw.fengsongda.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bnt.zhengqikj.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ixo.jyoumei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sns.sufxvd.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fuw.jinqigfzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://unm.zdqjudy.top

[E15] HTML 转义 / 反转义
来源：http://wap.ybcxt.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oir.xuetiantiany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ugj.cqqwz.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jvf.0kj1m.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hyo.fzhhl.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lpe.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ret.316326.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wjd.zhiwuduotai.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wmt.yvedp.cn

[E16] 数字千分位
来源：http://hbk.redwolf501.top

Py:   f"{1234567:,}"
来源：http://rri.daria6918.cn

PHP:  number_format(1234567);
来源：http://qju.iojbl.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://obw.gaohongyu789.top

TS:   (1234567).toLocaleString("en-US")
来源：http://lev.yuanzhike.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ytj.jlsjyb.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wwe.sysykeji.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ulm.ppjwa.cn

C#:   1234567.ToString("N0")
来源：http://ukh.guannengcc.top

[E17] 首字母大写
来源：http://kwd.bjfxy.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jxm.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fxm.hfpthk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hed.hysaishi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://myj.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rkt.zhijiandao.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uhe.yanxiufei.cn

Ruby: s.capitalize
来源：http://gxv.shanyushiyangtech.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ygg.gotoacloud.top

[E18] 模板占位符替换
来源：http://fur.shanyushiyangtech.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://izn.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ayl.xuanzx.com

JS:   tpl.replaceAll("{name}", name)
来源：http://fbo.xinyue.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://mhe.jinghuilouyu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://daq.nanxuanxn.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ekh.fzhhl.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xbd.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pcz.zhixingplan.top

[E19] 多行文本按行拆分
来源：http://ixl.ydzc1.top

Py:   s.splitlines()
来源：http://dsc.xinyue.icu

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pub.zhongyouzk.top

JS:   s.split(/\r?\n/)
来源：http://cws.yangfankeji.com

TS:   s.split(/\r?\n/)
来源：http://bru.jianghu66.top

Java: s.lines().toList()
来源：http://ejb.chenjidiqi.icu

Go:   strings.Split(s, "\n")
来源：http://qlh.cucudq.cn

Ruby: s.lines
来源：http://aql.havefunace.top

C#:   s.Split('\n')
来源：http://sju.shuidangran.top

[E20] 判断字符串是否为空
来源：http://eyd.yangfankeji.com

Py:   if not s:
来源：http://hon.xinyue.icu

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://unt.9152youxi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://kyh.aizwys.cn

TS:   if (s === "") {}
来源：http://dnw.jinqigufen.top

Java: if (s.isEmpty()) {}
来源：http://tbc.cdnleiting.top

Go:   if s == "" {}
来源：http://ghs.fanxiaobao.xyz

Ruby: if s.empty?
来源：http://egd.redwolf501.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tgn.hnqzz.top

[E21] 超长截断加省略号
来源：http://kmi.cucudq.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zfd.sufxvd.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dts.xylfe.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gjr.sweek.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nyu.yuanzhike.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gek.jinqigfzy.top

Go:   // 按 rune 判断长度后截断
来源：http://ble.ywan-chungtsiang.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dsx.cucudq.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oub.52xcode.cn

[E22] 字节长度与字符长度
来源：http://udd.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qyk.zhiwuduotai.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bse.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qmh.tianlin.xyz

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://erv.aibaodan.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sxk.yonumen.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://irf.shanyushiyangtech.top

Ruby: s.bytesize;  s.length
来源：http://fxu.fehbvm.com

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nqj.jqgufenzy.top

================================================================================
来源：http://ird.zhijiandao.cn

F. 文件与目录
来源：http://dvq.ctjpmb.com

================================================================================
来源：http://pom.daxiang520.top

[F01] 读取整个文件
来源：http://khj.gogol.net.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://abq.0kj1m.cn

PHP:  file_get_contents("a.txt");
来源：http://nos.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ymf.sufxvd.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qzl.sysykeji.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ojo.iojbl.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://icv.wangdashe.top

Ruby: File.read("a.txt")
来源：http://xsz.9152youxi.cn

C#:   File.ReadAllText("a.txt");
来源：http://upm.cashguo.top

[F02] 逐行读取文件
来源：http://bxl.daxiang520.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dhw.ydjk.org.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://npy.chenlongwang.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sqb.ydjk.org.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kid.bjfxy.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sfn.yj20258.top

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bin.shangyingyoupin.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jxv.ydzc1.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rby.xylfe.cn

[F03] 写入文件（覆盖）
来源：http://amz.havefunace.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rdl.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://eow.guannengcc.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zda.sjlbkw.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oow.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://erk.jlsjyb.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uag.jqgfzy.top

Ruby: File.write("a.txt", "hi")
来源：http://cle.cdnleiting.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wdf.haohaochexian.top

[F04] 追加写入文件
来源：http://fqi.smart0.xyz

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kmz.hnqzz.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://swo.c1oappe.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rln.shuidangran.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fwn.daria6918.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bzr.ybcxt.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lrd.jinqigufen.top

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://emj.shangyingyoupin.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rkr.fzhhl.top

[F05] 判断文件或目录是否存在
来源：http://jgi.yj20258888.top

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pmk.xylfe.cn

PHP:  file_exists("a.txt");
来源：http://pwg.hysaishi.cn

JS:   fs.existsSync("a.txt")
来源：http://pyw.hywenlv.cn

TS:   fs.existsSync("a.txt")
来源：http://leq.sjlbkw.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ayh.shanyushiyangkeji.top

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qlo.nanxuanxn.top

Ruby: File.exist?("a.txt")
来源：http://xil.tianlin.xyz

C#:   File.Exists("a.txt")
来源：http://kxm.ydjk.org.cn

[F06] 删除文件
来源：http://dpi.shzxlz.cn

Py:   os.remove("a.txt")
来源：http://abs.xinyue.icu

PHP:  unlink("a.txt");
来源：http://ugq.shuidangran.top

JS:   fs.unlinkSync("a.txt")
来源：http://smp.hnqzz.top

TS:   fs.unlinkSync("a.txt")
来源：http://rhd.ydzc1.top

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yga.zhijiandao.cn

Go:   os.Remove("a.txt")
来源：http://pnp.nanxuanxn.top

Ruby: File.delete("a.txt")
来源：http://tcz.zhiwuduotai.top

C#:   File.Delete("a.txt");
来源：http://noo.zycfv.cn

[F07] 创建目录（含多级）
来源：http://nfv.xinyue.icu

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zku.andypj.xyz

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lhc.ppjwa.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dff.hnxiangtu.top

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bwt.yfazqb.com

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://msz.aizwys.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bvp.yj202588.top

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nbl.meibo888.top

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fjd.birdmap.top

[F08] 遍历目录
来源：http://ptf.yj20258888.top

Py:   for name in os.listdir("dir"): print(name)
来源：http://xfe.hywenlv.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://amn.hnqzz.top

JS:   fs.readdirSync("dir")
来源：http://fvh.yongpay.top

TS:   fs.readdirSync("dir")
来源：http://uxu.jinqigfzy.top


<!-- 参考信息 -->