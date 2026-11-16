代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gxa.smart0.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wqp.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qey.yuxming.cn

Go:   // 手写 map[T]int
来源：http://kdc.sysykeji.top

Ruby: arr.tally
来源：http://yre.fzhhl.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bde.cheryme.top

[D21] 判断是否包含某元素
来源：http://ufz.chenjidiqi.icu

Py:   x in arr
来源：http://kpw.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://xvj.cdnleiting.top

JS:   arr.includes(x)
来源：http://ght.quarkkingdee.top

TS:   arr.includes(x)
来源：http://dmw.cheryme.top

Java: list.contains(x)
来源：http://rqa.yvedp.cn

Go:   slices.Contains(arr, x)
来源：http://qqn.bjfxy.top

Ruby: arr.include?(x)
来源：http://ekc.xziqi.cn

C#:   list.Contains(x)
来源：http://cnv.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://fjm.jinqigfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bod.zhijiandao.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ipa.hysaishi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pgr.nwbrower.top

TS:   [...arr];
来源：http://hbd.vehdjk.com

Java: new ArrayList<>(list);
来源：http://vld.jlsjyb.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qbe.zycfv.cn

Ruby: arr.dup;  arr.clone
来源：http://knl.fanxiaobao.xyz

C#:   new List<int>(list);
来源：http://tgs.smart0.xyz

[D23] reduce 累积计算
来源：http://qnv.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qig.cucudq.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vbr.gogol.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ken.shangyingyoupin.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aqr.svipenyu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rkw.shzxlz.cn

Go:   // 手写循环
来源：http://uug.zhijiandao.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://toy.jianghu66.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hen.jlsjyb.cn

[D24] 字典 / Map 基本操作
来源：http://bhg.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ojj.shzxlz.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://any.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wwd.chenzaomai.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vsk.shuidangran.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xkq.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mvb.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gvc.fengsongda.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kga.guowangkeji.top

[D25] Set 集合去重与交并差
来源：http://qlr.mhx1999.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zdm.jinqigfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sid.hnqzz.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rva.yuanzhike.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ixb.sjlbkw.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ssn.nwbrower.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sgu.zdbjq.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mfc.fehbvm.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cgi.yvedp.cn

[D26] 数组转字符串
来源：http://fya.guannengcc.top

Py:   ", ".join(map(str, arr))
来源：http://yqa.sjlbkw.cn

PHP:  implode(", ", $arr);
来源：http://obn.shanyushiyangkeji.top

JS:   arr.join(", ")
来源：http://ita.jlsjyb.cn

TS:   arr.join(", ")
来源：http://bgi.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://nfw.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://wgp.jqgufenzy.top

Ruby: arr.join(", ")
来源：http://vjc.kuanghao11.cn

C#:   string.Join(", ", list)
来源：http://jol.ctjpmb.com

================================================================================
来源：http://pkv.sjlbkw.cn

E. 字符串处理
来源：http://zih.zhiwuduotai.top

================================================================================
来源：http://krj.zhongyouzk.top

[E01] 拼接字符串
来源：http://bqx.wangdashe.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xys.shanyushiyangtech.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bsa.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bbv.andypj.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://uya.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uqz.jlsjyb.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pjz.jinqigufen.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://skn.jqgfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ijt.ehwqpu.com

[E02] 重复字符串
来源：http://qog.havefunace.top

Py:   "ab" * 3
来源：http://mvx.hnxiangtu.top

PHP:  str_repeat("ab", 3);
来源：http://iao.svipenyu.cn

JS:   "ab".repeat(3)
来源：http://yyz.xuanzx.com

TS:   "ab".repeat(3)
来源：http://nug.hnxiangtu.top

Java: "ab".repeat(3)
来源：http://dit.gogol.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://gyu.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://yjq.daria6918.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zko.aibaodan.cn

[E03] 截取子串
来源：http://yvr.hammf.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gfn.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vct.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://apy.zhengqikj.top

TS:   s.slice(1, 4)
来源：http://hqi.hcnkem.com

Java: s.substring(1, 4)
来源：http://dop.zhengqikj.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mfn.gogol.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://khw.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://vrk.ppjwa.cn

[E04] 查找子串位置
来源：http://hwr.fengsongda.top

Py:   s.find("x");  s.index("x")
来源：http://bmp.fzhhl.top

PHP:  strpos($s, "x");
来源：http://cpy.jiagoushi.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gva.zhiwuduotai.top

TS:   s.indexOf("x")
来源：http://zyy.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://ham.ydzc1.top

Go:   strings.Index(s, "x")
来源：http://mew.yongpay.top

Ruby: s.index("x")
来源：http://zas.jqgfzy.top

C#:   s.IndexOf("x")
来源：http://wqe.cashguo.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xkq.chenzaomai.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gxx.dashuyun.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pxm.quarkkingdee.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kni.hywenlv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wku.yvedp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lbo.tarul.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wdt.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://skf.zdqjudy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jup.tian-w.cn

[E06] 替换子串
来源：http://phb.zdbjq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dmf.xylfe.cn

PHP:  str_replace("a", "b", $s);
来源：http://jgg.jinqigufen.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gjo.ybcxt.top

TS:   s.replaceAll("a", "b")
来源：http://itx.yfazqb.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cuo.jinyuanbaomall.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gsl.andypj.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jrz.shanyushiyangkeji.top

C#:   s.Replace("a", "b")
来源：http://ynp.jinqigfzy.top

[E07] 按分隔符拆分
来源：http://zad.jinqigufen.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nzk.aizwys.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://myd.ctjpmb.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://doz.epnwcf.com

TS:   s.split(",")
来源：http://aki.mhx1999.top

Java: s.split(",");  s.split("\\s+")
来源：http://qrr.shanyushiyangtech.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qlq.cucudq.cn

Ruby: s.split(",");  s.split
来源：http://udn.fktsv.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gib.yuxming.cn

[E08] 数组按分隔符合并
来源：http://ubt.tian-w.cn

Py:   ",".join(items)
来源：http://dbu.sjlbkw.cn

PHP:  implode(",", $items);
来源：http://lgh.hongshengwenyu.top

JS:   items.join(",")
来源：http://wyl.fengsongda.top

TS:   items.join(",")
来源：http://jea.redwolf501.top

Java: String.join(",", items)
来源：http://jnf.zhixingplan.top

Go:   strings.Join(items, ",")
来源：http://ktp.ppjwa.cn

Ruby: items.join(",")
来源：http://daa.chenjidiqi.icu

C#:   string.Join(",", items)
来源：http://yhi.bjfxy.top

[E09] 去除所有空白字符
来源：http://ygj.fzhhl.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nvl.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sir.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://dlh.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://sza.shanyushiyangtech.top

Java: s.replaceAll("\\s+", "")
来源：http://rbr.cqqwz.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xta.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://szb.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sur.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://mon.jinghuilouyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bzt.jqgfzy.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://kre.xziqi.cn

JS:   "7".padStart(3, "0")
来源：http://fkh.yj20258888.top

TS:   "7".padStart(3, "0")
来源：http://ory.fanxiaobao.xyz

Java: String.format("%03d", 7)
来源：http://epl.shanyushiyangtech.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://ooe.guannengcc.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ile.hywenlv.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wgf.ybcxt.top

[E11] 反转字符串
来源：http://xys.nanxinkj.top

Py:   s[::-1]
来源：http://cro.jqgfzy.top

PHP:  strrev($s);
来源：http://aht.uphjek.com

JS:   [...s].reverse().join("")
来源：http://mvf.ivvv.top

TS:   [...s].reverse().join("")
来源：http://nwe.chenjidiqi.icu

Java: new StringBuilder(s).reverse().toString()
来源：http://jxq.yfazqb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://dat.pycfn.com

Ruby: s.reverse
来源：http://vjq.fanxiaobao.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://ort.wangdashe.top

[E12] 统计某字符出现次数
来源：http://svm.quarkkingdee.top

Py:   s.count("a")
来源：http://crw.yvedp.cn

PHP:  substr_count($s, "a");
来源：http://xzz.gogol.net.cn

JS:   s.split("a").length - 1
来源：http://zpo.jinghuilouyu.cn

TS:   s.split("a").length - 1
来源：http://gll.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hij.yuxming.cn

Go:   strings.Count(s, "a")
来源：http://tkc.shanyushiyangtech.top

Ruby: s.count("a")
来源：http://geo.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://nkd.zhengqikj.top

[E13] 逐字符遍历
来源：http://yys.yfazqb.com

Py:   for ch in s: print(ch)
来源：http://tpc.tian-w.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lid.cdnleiting.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vkq.snrcjt.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dwc.xziqi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kww.cqqwz.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ahn.9152youxi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tbs.cucudq.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ssw.hammf.cn

[E14] URL 编码与 Base64
来源：http://hoa.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ynv.dashuyun.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pvk.guowangkeji.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zac.chenlongwang.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://azd.tarul.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vak.yanxiufei.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bng.jyoumei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ylq.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://snw.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://sku.hywenlv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://tps.sweek.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dgq.shanyushiyangkeji.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hhy.chenjidiqi.icu

TS:   // 同上，务必做 XSS 过滤
来源：http://okz.fehbvm.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wpl.zdbjq.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pak.cashguo.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ftw.fktsv.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://beh.gaohongyu789.top

[E16] 数字千分位
来源：http://laf.zhixingplan.top

Py:   f"{1234567:,}"
来源：http://sjz.meibo888.top

PHP:  number_format(1234567);
来源：http://lbm.gotoacloud.top

JS:   (1234567).toLocaleString("en-US")
来源：http://ely.yongpay.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hiu.yueranfly.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yjp.hywenlv.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://epu.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xot.haohaochexian.top

C#:   1234567.ToString("N0")
来源：http://nkh.gogol.net.cn

[E17] 首字母大写
来源：http://cle.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qkw.xuetiantiany.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qdz.fehbvm.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://frh.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://anm.gaohongyu789.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kbr.nanxuanxn.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ukn.tianlin.xyz

Ruby: s.capitalize
来源：http://nnf.hnqzz.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xxy.ydjk.org.cn

[E18] 模板占位符替换
来源：http://shn.hammf.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ath.c1oappe.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qzn.sysykeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://umv.chenzaomai.com

TS:   tpl.replaceAll("{name}", name)
来源：http://amd.ywan-chungtsiang.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dqy.jiagoushi.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xnk.shzxlz.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wyu.zdbjq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qme.fengsongda.top

[E19] 多行文本按行拆分
来源：http://dpa.xylfe.cn

Py:   s.splitlines()
来源：http://twf.hfpthk.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cqv.iojbl.cn

JS:   s.split(/\r?\n/)
来源：http://svr.gzhubu.top

TS:   s.split(/\r?\n/)
来源：http://xan.hfpthk.cn

Java: s.lines().toList()
来源：http://pzg.fktsv.cn

Go:   strings.Split(s, "\n")
来源：http://zmj.jqgufenzy.top

Ruby: s.lines
来源：http://lso.xingfuxueyuan.xyz

C#:   s.Split('\n')
来源：http://mfh.vehdjk.com

[E20] 判断字符串是否为空
来源：http://sys.yvedp.cn

Py:   if not s:
来源：http://svq.wangdashe.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kcr.52xcode.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rdc.aibaodan.cn

TS:   if (s === "") {}
来源：http://qyi.tanke756.top

Java: if (s.isEmpty()) {}
来源：http://opt.9152youxi.cn

Go:   if s == "" {}
来源：http://hxh.mhx1999.top

Ruby: if s.empty?
来源：http://ujl.dianchejie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qjg.haohaochexian.top

[E21] 超长截断加省略号
来源：http://qnn.gotoacloud.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pdy.hesvh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://afj.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pwh.uphjek.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kui.sysykeji.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://suk.chenlongwang.top

Go:   // 按 rune 判断长度后截断
来源：http://dng.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://brd.chenjidiqi.icu

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://lfp.sjlbkw.cn

[E22] 字节长度与字符长度
来源：http://hlo.daria6918.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jex.cashguo.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hmi.xingfuxueyuan.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eop.vqdsnc.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wrl.hammf.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vwl.aizwys.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xbc.shanyushiyangkeji.top

Ruby: s.bytesize;  s.length
来源：http://wmy.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bjt.fktsv.cn

================================================================================
来源：http://ywe.xziqi.cn

F. 文件与目录
来源：http://oof.0kj1m.cn

================================================================================
来源：http://czx.nanxuanxn.top

[F01] 读取整个文件
来源：http://rmb.ybcxt.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wrf.andypj.xyz

PHP:  file_get_contents("a.txt");
来源：http://wru.daria6918.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://amo.yj20258888.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dys.chenjidiqi.icu

Java: Files.readString(Path.of("a.txt"))
来源：http://vcj.9152youxi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dvl.iojbl.cn

Ruby: File.read("a.txt")
来源：http://phl.sufxvd.cn

C#:   File.ReadAllText("a.txt");
来源：http://emk.sxryk.cn

[F02] 逐行读取文件
来源：http://nmk.hesvh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ppp.iojbl.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://suw.cheryme.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://umd.jyoumei.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eby.yj20258.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gxu.zhoulong.xyz

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ikc.hfpthk.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xar.cheryme.top

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xhw.yuanzhike.top

[F03] 写入文件（覆盖）
来源：http://eaw.gogol.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ood.cashguo.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://gqh.yj20258888.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rrq.dianchejie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vxp.yvedp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yrn.9152youxi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fzc.haohaochexian.top

Ruby: File.write("a.txt", "hi")
来源：http://ego.jinghuilouyu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ycw.cashguo.top

[F04] 追加写入文件
来源：http://dkp.jinghuilouyu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jcl.jqgfzy.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pdl.cheryme.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://buu.zdqjudy.top

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vbz.316326.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lzo.yanxiufei.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dqb.fehbvm.com

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mnx.zhoulong.xyz

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jgb.dashuyun.cn


<!-- 参考信息 -->