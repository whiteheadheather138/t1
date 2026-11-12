代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fee.zdbjq.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qdw.hnxiangtu.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ujf.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://zml.zhongyouzk.top

Ruby: arr.tally
来源：http://blc.fktsv.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onw.yongpay.top

[D21] 判断是否包含某元素
来源：http://ili.cqqwz.cn

Py:   x in arr
来源：http://pwp.xuetiantiany.cn

PHP:  in_array($x, $arr, true);
来源：http://mbs.ybcxt.top

JS:   arr.includes(x)
来源：http://gzz.kuanghao11.cn

TS:   arr.includes(x)
来源：http://vdp.jiagoushi.top

Java: list.contains(x)
来源：http://czl.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://aqq.hammf.cn

Ruby: arr.include?(x)
来源：http://ngo.hammf.cn

C#:   list.Contains(x)
来源：http://bcu.smart0.xyz

[D22] 复制数组（避免共享引用）
来源：http://nsc.fzhhl.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://aul.nwbrower.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mkz.snrcjt.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eeb.ydjk.org.cn

TS:   [...arr];
来源：http://wje.sweek.top

Java: new ArrayList<>(list);
来源：http://lgi.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://vmn.pycfn.com

Ruby: arr.dup;  arr.clone
来源：http://khj.yj202588.top

C#:   new List<int>(list);
来源：http://svn.aizwys.cn

[D23] reduce 累积计算
来源：http://bav.fanxiaobao.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gix.aizwys.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uas.yj20258.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hni.ctjpmb.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wyv.cdnleiting.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://uds.tian-w.cn

Go:   // 手写循环
来源：http://ykw.shanyushiyangtech.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vmh.zhaomingkeji.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bjs.andypj.xyz

[D24] 字典 / Map 基本操作
来源：http://dqy.gzhubu.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tvg.tarul.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kep.jinyuanbaomall.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://bzk.zhixingplan.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://diy.52xcode.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kdk.yanxiufei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vxm.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://uro.nanxuanxn.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kzy.zhengqikj.top

[D25] Set 集合去重与交并差
来源：http://eet.316326.xyz

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gpw.bjfxy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pgp.yangfankeji.com

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://usi.tanke756.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vsc.smart0.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tvv.shanyushiyangtech.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bem.fengsongda.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://eui.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://odn.sweek.top

[D26] 数组转字符串
来源：http://oou.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://yhp.aibaodan.cn

PHP:  implode(", ", $arr);
来源：http://xjp.sysykeji.top

JS:   arr.join(", ")
来源：http://nfr.tarul.cn

TS:   arr.join(", ")
来源：http://fup.nanxinkj.top

Java: String.join(", ", list)
来源：http://gxb.tian-w.cn

Go:   strings.Join(strs, ", ")
来源：http://iix.jiagoushi.top

Ruby: arr.join(", ")
来源：http://nhi.bbcook.cn

C#:   string.Join(", ", list)
来源：http://zys.pengpengdd.cyou

================================================================================
来源：http://oif.hnxiangtu.top

E. 字符串处理
来源：http://unw.yongpay.top

================================================================================
来源：http://uaq.fzhhl.top

[E01] 拼接字符串
来源：http://hyq.tarul.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://plj.zycfv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sfl.gaohongyu789.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zor.jinghuilouyu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://npb.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vsf.ybcxt.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hij.havefunace.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mlc.redwolf501.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qca.hywenlv.cn

[E02] 重复字符串
来源：http://wkq.zhaomingkeji.xyz

Py:   "ab" * 3
来源：http://zmf.jinyuanbaomall.cn

PHP:  str_repeat("ab", 3);
来源：http://ltm.jiagoushi.top

JS:   "ab".repeat(3)
来源：http://rpb.jinqigufen.top

TS:   "ab".repeat(3)
来源：http://xhb.hongshengwenyu.top

Java: "ab".repeat(3)
来源：http://ett.cheryme.top

Go:   strings.Repeat("ab", 3)
来源：http://lxj.feifeiyinyue.top

Ruby: "ab" * 3
来源：http://jdg.meibo888.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tsh.fzhhl.top

[E03] 截取子串
来源：http://znc.wangshuangyany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ira.xziqi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ous.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wqn.tanke756.top

TS:   s.slice(1, 4)
来源：http://npt.cucudq.cn

Java: s.substring(1, 4)
来源：http://kxb.hnqzz.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eya.shuidangran.top

Ruby: s[1, 3];  s[1..3]
来源：http://goj.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://imb.yj20258.top

[E04] 查找子串位置
来源：http://sra.jinyuanbaomall.cn

Py:   s.find("x");  s.index("x")
来源：http://lgr.fktsv.cn

PHP:  strpos($s, "x");
来源：http://xkv.daxiang520.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mhn.jinqigufen.top

TS:   s.indexOf("x")
来源：http://fdi.svipenyu.cn

Java: s.indexOf("x")
来源：http://xnt.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://eak.zycfv.cn

Ruby: s.index("x")
来源：http://mmg.andypj.xyz

C#:   s.IndexOf("x")
来源：http://bcj.yanxiufei.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uhu.jinyuanbaomall.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://klk.tianlin.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rfc.cqqwz.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nof.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ihi.xylfe.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uer.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lgf.zhongyouzk.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ebj.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hwv.xinyue.icu

[E06] 替换子串
来源：http://cmd.quarkkingdee.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qrf.shangyingyoupin.top

PHP:  str_replace("a", "b", $s);
来源：http://nzr.316326.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jdq.pycfn.com

TS:   s.replaceAll("a", "b")
来源：http://jwt.yj20258.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://phe.yonumen.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vkc.bjfxy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://noz.jinqigfzy.top

C#:   s.Replace("a", "b")
来源：http://djh.vqdsnc.cn

[E07] 按分隔符拆分
来源：http://rdb.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bvb.yfazqb.com

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tph.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://sju.kuanghao11.cn

TS:   s.split(",")
来源：http://yms.316326.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://whc.tanke756.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pdk.yuanzhike.top

Ruby: s.split(",");  s.split
来源：http://vcs.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://isn.andypj.xyz

[E08] 数组按分隔符合并
来源：http://apx.hesvh.cn

Py:   ",".join(items)
来源：http://rhq.xingfuxueyuan.xyz

PHP:  implode(",", $items);
来源：http://bcm.xziqi.cn

JS:   items.join(",")
来源：http://htj.gogol.net.cn

TS:   items.join(",")
来源：http://piq.snrcjt.cn

Java: String.join(",", items)
来源：http://aic.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://nly.xinyue.icu

Ruby: items.join(",")
来源：http://qot.xingfuxueyuan.xyz

C#:   string.Join(",", items)
来源：http://pzm.yvedp.cn

[E09] 去除所有空白字符
来源：http://fns.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wyc.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dwj.yj20258.top

JS:   s.replace(/\s+/g, "")
来源：http://gkr.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://tbx.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://cit.jinqigfzy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://bun.ywan-chungtsiang.top

Ruby: s.gsub(/\s+/, "")
来源：http://aeq.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sja.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://rrw.xylfe.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wpf.hywenlv.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gsq.tianlin.xyz

JS:   "7".padStart(3, "0")
来源：http://mna.meibo888.top

TS:   "7".padStart(3, "0")
来源：http://qbv.sweek.top

Java: String.format("%03d", 7)
来源：http://opy.cashguo.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://mzb.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vgk.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cxp.yanxiufei.cn

[E11] 反转字符串
来源：http://lzw.hysaishi.cn

Py:   s[::-1]
来源：http://lph.guowangkeji.top

PHP:  strrev($s);
来源：http://trp.daria6918.cn

JS:   [...s].reverse().join("")
来源：http://wov.sysykeji.top

TS:   [...s].reverse().join("")
来源：http://rzo.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://jbh.hnxiangtu.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pyu.zdqjudy.top

Ruby: s.reverse
来源：http://agh.zhengqikj.top

C#:   new string(s.Reverse().ToArray())
来源：http://qno.birdmap.top

[E12] 统计某字符出现次数
来源：http://ciq.ywan-chungtsiang.top

Py:   s.count("a")
来源：http://vhu.gogol.net.cn

PHP:  substr_count($s, "a");
来源：http://fhx.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://qwe.gotoacloud.top

TS:   s.split("a").length - 1
来源：http://oar.9152youxi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ukm.ehwqpu.com

Go:   strings.Count(s, "a")
来源：http://xyx.gotoacloud.top

Ruby: s.count("a")
来源：http://lye.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://mej.hongshengwenyu.top

[E13] 逐字符遍历
来源：http://ftx.jianghu66.top

Py:   for ch in s: print(ch)
来源：http://bqe.cashguo.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vvl.ctjpmb.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://nwl.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://imj.shzxlz.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ntv.xuetiantiany.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tdk.zhoulong.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://eui.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hmy.jqgufenzy.top

[E14] URL 编码与 Base64
来源：http://skh.jqgufenzy.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kyq.cqqwz.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://grv.xingfuxueyuan.xyz

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kap.sjlbkw.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://thp.yvedp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wjz.xylfe.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ypv.ybcxt.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jrh.havefunace.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mbq.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://yyn.hfpthk.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gvb.gogol.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tqr.birdmap.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zmo.shanyushiyangkeji.top

TS:   // 同上，务必做 XSS 过滤
来源：http://jyo.dashuyun.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xkt.yueranfly.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://key.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tmv.gaohongyu789.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ppb.jinqigfzy.top

[E16] 数字千分位
来源：http://xky.tanke756.top

Py:   f"{1234567:,}"
来源：http://fto.yfazqb.com

PHP:  number_format(1234567);
来源：http://jfw.zhoulong.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://rfv.0kj1m.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fzo.xziqi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pwr.ywan-chungtsiang.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tgo.nanxuanxn.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hah.wangdashe.top

C#:   1234567.ToString("N0")
来源：http://qlx.jinqigufen.top

[E17] 首字母大写
来源：http://vnz.zhijiandao.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://glu.jlsjyb.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nyy.yongpay.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://syf.aizwys.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ith.xuanzx.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ril.bbcook.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jxy.zhoulong.xyz

Ruby: s.capitalize
来源：http://ejo.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mvt.chenlongwang.top

[E18] 模板占位符替换
来源：http://ghu.tianlin.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tge.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://myf.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://mai.tianlin.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://qcm.chenjidiqi.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wcq.xinyue.icu

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zei.xinyue.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zmy.zhongyouzk.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ahw.hammf.cn

[E19] 多行文本按行拆分
来源：http://lze.sysykeji.top

Py:   s.splitlines()
来源：http://hpi.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oyr.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://mci.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://cgu.zhiwuduotai.top

Java: s.lines().toList()
来源：http://kbr.havefunace.top

Go:   strings.Split(s, "\n")
来源：http://ubg.jinghuilouyu.cn

Ruby: s.lines
来源：http://yes.sweek.top

C#:   s.Split('\n')
来源：http://cmz.zhongyouzk.top

[E20] 判断字符串是否为空
来源：http://ixy.zhoulong.xyz

Py:   if not s:
来源：http://yfr.redwolf501.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yca.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lnm.vehdjk.com

TS:   if (s === "") {}
来源：http://ueb.daxiang520.top

Java: if (s.isEmpty()) {}
来源：http://umm.yuxming.cn

Go:   if s == "" {}
来源：http://rmh.yangfankeji.com

Ruby: if s.empty?
来源：http://klo.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jge.bbcook.cn

[E21] 超长截断加省略号
来源：http://aej.yonumen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bld.shanyushiyangtech.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fbp.yanxiufei.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ptv.shanyushiyangtech.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gfo.tian-w.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ewp.havefunace.top

Go:   // 按 rune 判断长度后截断
来源：http://xgq.sufxvd.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oyx.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ywu.epnwcf.com

[E22] 字节长度与字符长度
来源：http://cut.smart0.xyz

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ikj.hcnkem.com

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jau.jyoumei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lac.iojbl.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hzi.chenjidiqi.icu

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xeo.zhoulong.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://och.yj20258888.top

Ruby: s.bytesize;  s.length
来源：http://ozj.xuetiantiany.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yem.guowangkeji.top

================================================================================
来源：http://uie.yj202588.top

F. 文件与目录
来源：http://ojs.ivvv.top

================================================================================
来源：http://kzc.316326.xyz

[F01] 读取整个文件
来源：http://uyj.gaohongyu789.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://frp.hnqzz.top

PHP:  file_get_contents("a.txt");
来源：http://jow.yj20258888.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lao.yj202588.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fzn.hongshengwenyu.top

Java: Files.readString(Path.of("a.txt"))
来源：http://apg.yj202588.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yfl.yanxiufei.cn

Ruby: File.read("a.txt")
来源：http://ipn.daxiang520.top

C#:   File.ReadAllText("a.txt");
来源：http://ora.iojbl.cn

[F02] 逐行读取文件
来源：http://wvr.aibaodan.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://daq.pengpengdd.cyou

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dkq.gogol.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lzn.iojbl.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rnt.guannengcc.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rpr.yangfankeji.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oro.shuidangran.top

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tzs.yangfankeji.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ojn.52xcode.cn

[F03] 写入文件（覆盖）
来源：http://uqd.shanyushiyangkeji.top

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jwj.hnqzz.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://hyh.cdnleiting.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://awx.iojbl.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pcd.9152youxi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ieo.guannengcc.top

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vqx.havefunace.top

Ruby: File.write("a.txt", "hi")
来源：http://ixr.c1oappe.top

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yrp.sufxvd.cn

[F04] 追加写入文件
来源：http://wkk.yueranfly.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zxf.jianghu66.top

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fri.xinyue.icu

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://alk.wangshuangyany.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mpe.snrcjt.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wge.meibo888.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://icw.smart0.xyz

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://csj.jlsjyb.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://toe.hfpthk.cn


<!-- 参考信息 -->