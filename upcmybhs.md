代发 wailian999

Ruby: arr.tally
来源：http://ror.ydzc1.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tkz.chenlongwang.top

[D21] 判断是否包含某元素
来源：http://pvh.316326.xyz

Py:   x in arr
来源：http://ldj.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://gfq.guowangkeji.top

JS:   arr.includes(x)
来源：http://uhj.wangdashe.top

TS:   arr.includes(x)
来源：http://vik.havefunace.top

Java: list.contains(x)
来源：http://imb.cashguo.top

Go:   slices.Contains(arr, x)
来源：http://nfn.316326.xyz

Ruby: arr.include?(x)
来源：http://wfl.yongpay.top

C#:   list.Contains(x)
来源：http://ree.redwolf501.top

[D22] 复制数组（避免共享引用）
来源：http://utf.vehdjk.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qga.aizwys.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://jlt.9152youxi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xac.jyoumei.cn

TS:   [...arr];
来源：http://wwg.ppjwa.cn

Java: new ArrayList<>(list);
来源：http://mls.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qnc.jiagoushi.top

Ruby: arr.dup;  arr.clone
来源：http://jsi.fehbvm.com

C#:   new List<int>(list);
来源：http://hik.fzhhl.top

[D23] reduce 累积计算
来源：http://vha.redwolf501.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xap.sweek.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vij.xuetiantiany.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jol.shanyushiyangkeji.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yol.birdmap.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://xpd.jinqigfzy.top

Go:   // 手写循环
来源：http://nbq.xziqi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ypv.bjfxy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://khu.hysaishi.cn

[D24] 字典 / Map 基本操作
来源：http://stm.zhongyouzk.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qvh.cheryme.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lvq.sxryk.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ouj.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lwo.yfazqb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bpk.yueranfly.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vnc.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vqy.epnwcf.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qla.xuetiantiany.cn

[D25] Set 集合去重与交并差
来源：http://vha.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://glv.jqgfzy.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cjj.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ezo.nanxinkj.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wvl.dashuyun.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ati.tian-w.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bcg.fktsv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iub.zdbjq.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://rtp.wangdashe.top

[D26] 数组转字符串
来源：http://zyd.chenlongwang.top

Py:   ", ".join(map(str, arr))
来源：http://uvd.andypj.xyz

PHP:  implode(", ", $arr);
来源：http://uik.hywenlv.cn

JS:   arr.join(", ")
来源：http://otr.vehdjk.com

TS:   arr.join(", ")
来源：http://qob.jinyuanbaomall.cn

Java: String.join(", ", list)
来源：http://uej.ivvv.top

Go:   strings.Join(strs, ", ")
来源：http://ozy.zhiwuduotai.top

Ruby: arr.join(", ")
来源：http://adz.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://fga.bbcook.cn

================================================================================
来源：http://ohb.cucudq.cn

E. 字符串处理
来源：http://bjb.zhijiandao.cn

================================================================================
来源：http://dgy.yanxiufei.cn

[E01] 拼接字符串
来源：http://trr.jinqigfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://plp.sysykeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vkt.hcnkem.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://esu.hfpthk.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://aab.ehwqpu.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dul.hcnkem.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qxs.fzhhl.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xwe.ybcxt.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mtl.zhaomingkeji.xyz

[E02] 重复字符串
来源：http://hij.smart0.xyz

Py:   "ab" * 3
来源：http://isn.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://nfs.chenlongwang.top

JS:   "ab".repeat(3)
来源：http://kbp.daria6918.cn

TS:   "ab".repeat(3)
来源：http://kxp.jianghu66.top

Java: "ab".repeat(3)
来源：http://qaa.ydjk.org.cn

Go:   strings.Repeat("ab", 3)
来源：http://png.daxiang520.top

Ruby: "ab" * 3
来源：http://qwh.zhongyouzk.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ipa.jqgufenzy.top

[E03] 截取子串
来源：http://xhv.jinyuanbaomall.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wzw.52xcode.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vtt.hongshengwenyu.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tvr.meibo888.top

TS:   s.slice(1, 4)
来源：http://wqq.9152youxi.cn

Java: s.substring(1, 4)
来源：http://tzk.hammf.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xmp.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://bwj.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://qnt.sjlbkw.cn

[E04] 查找子串位置
来源：http://yfn.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://imr.iojbl.cn

PHP:  strpos($s, "x");
来源：http://ftw.cqqwz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cve.uphjek.com

TS:   s.indexOf("x")
来源：http://rwz.shanyushiyangtech.top

Java: s.indexOf("x")
来源：http://akn.yangfankeji.com

Go:   strings.Index(s, "x")
来源：http://mnx.daxiang520.top

Ruby: s.index("x")
来源：http://nwi.0kj1m.cn

C#:   s.IndexOf("x")
来源：http://zhu.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://owz.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yfh.ybcxt.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xzf.sweek.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xdf.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://hoe.gzhubu.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rvw.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mlt.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xou.nwbrower.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cac.nanxuanxn.top

[E06] 替换子串
来源：http://mrs.nwbrower.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xor.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://ghe.sjlbkw.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ucn.aizwys.cn

TS:   s.replaceAll("a", "b")
来源：http://skc.xylfe.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vdb.jinghuilouyu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ywy.iojbl.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kvg.pycfn.com

C#:   s.Replace("a", "b")
来源：http://ifu.jlsjyb.cn

[E07] 按分隔符拆分
来源：http://xit.hnqzz.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jsc.fengsongda.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xso.hfpthk.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cim.ehwqpu.com

TS:   s.split(",")
来源：http://zeu.pycfn.com

Java: s.split(",");  s.split("\\s+")
来源：http://yxw.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://juv.tanke756.top

Ruby: s.split(",");  s.split
来源：http://oxf.fanxiaobao.xyz

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tds.ydjk.org.cn

[E08] 数组按分隔符合并
来源：http://slw.ywan-chungtsiang.top

Py:   ",".join(items)
来源：http://awm.aibaodan.cn

PHP:  implode(",", $items);
来源：http://qew.bjfxy.top

JS:   items.join(",")
来源：http://tuv.c1oappe.top

TS:   items.join(",")
来源：http://cmv.shzxlz.cn

Java: String.join(",", items)
来源：http://hba.guowangkeji.top

Go:   strings.Join(items, ",")
来源：http://svb.xinyue.icu

Ruby: items.join(",")
来源：http://mic.yj20258888.top

C#:   string.Join(",", items)
来源：http://dgt.gotoacloud.top

[E09] 去除所有空白字符
来源：http://tmv.cqqwz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xiw.yuanzhike.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fjh.cheryme.top

JS:   s.replace(/\s+/g, "")
来源：http://nxo.epnwcf.com

TS:   s.replace(/\s+/g, "")
来源：http://btw.xylfe.cn

Java: s.replaceAll("\\s+", "")
来源：http://sqa.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sih.yongpay.top

Ruby: s.gsub(/\s+/, "")
来源：http://oza.gogol.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vee.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://plq.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uer.aibaodan.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hfk.daria6918.cn

JS:   "7".padStart(3, "0")
来源：http://cur.uphjek.com

TS:   "7".padStart(3, "0")
来源：http://gfe.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://vro.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gfo.jinghuilouyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rkd.yuanzhike.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mba.sjlbkw.cn

[E11] 反转字符串
来源：http://vda.nwbrower.top

Py:   s[::-1]
来源：http://vbj.yj20258.top

PHP:  strrev($s);
来源：http://oey.ydzc1.top

JS:   [...s].reverse().join("")
来源：http://pom.meibo888.top

TS:   [...s].reverse().join("")
来源：http://ihx.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://eiu.guowangkeji.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://cnc.dianchejie.cn

Ruby: s.reverse
来源：http://skh.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://llh.andypj.xyz

[E12] 统计某字符出现次数
来源：http://bvd.pengpengdd.cyou

Py:   s.count("a")
来源：http://iqu.xuetiantiany.cn

PHP:  substr_count($s, "a");
来源：http://fha.yonumen.top

JS:   s.split("a").length - 1
来源：http://efa.birdmap.top

TS:   s.split("a").length - 1
来源：http://oiu.ctjpmb.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qqx.jqgufenzy.top

Go:   strings.Count(s, "a")
来源：http://zdh.tian-w.cn

Ruby: s.count("a")
来源：http://wpb.jinyuanbaomall.cn

C#:   s.Count(c => c == 'a')
来源：http://ife.ydjk.org.cn

[E13] 逐字符遍历
来源：http://jzc.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://tkq.yfazqb.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vrr.andypj.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://fnn.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://jpc.mhx1999.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wcd.tanke756.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pwq.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bah.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uey.shangyingyoupin.top

[E14] URL 编码与 Base64
来源：http://djw.sweek.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://frl.zhongyouzk.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://lfw.xuetiantiany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fdx.tanke756.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ugb.cucudq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ohe.jinghuilouyu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rro.zhongyouzk.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cwo.jqgufenzy.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ezp.iojbl.cn

[E15] HTML 转义 / 反转义
来源：http://rih.bjfxy.top

Py:   html.escape(s);  html.unescape(s)
来源：http://gud.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gbd.havefunace.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jjx.cucudq.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mqh.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tgr.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jye.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gdj.tianlin.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://htx.sxryk.cn

[E16] 数字千分位
来源：http://ziq.redwolf501.top

Py:   f"{1234567:,}"
来源：http://xsm.feifeiyinyue.top

PHP:  number_format(1234567);
来源：http://btd.bjfxy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://nid.ehwqpu.com

TS:   (1234567).toLocaleString("en-US")
来源：http://vjk.epnwcf.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wpq.jyoumei.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xjt.yfazqb.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://abv.hywenlv.cn

C#:   1234567.ToString("N0")
来源：http://raz.chenlongwang.top

[E17] 首字母大写
来源：http://xvy.sufxvd.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://raj.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://mmv.cqqwz.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bln.meibo888.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nth.hnqzz.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://btx.hywenlv.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uul.yanxiufei.cn

Ruby: s.capitalize
来源：http://dax.cucudq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ybg.wangshuangyany.cn

[E18] 模板占位符替换
来源：http://cuy.hcnkem.com

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xfe.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zyk.cheryme.top

JS:   tpl.replaceAll("{name}", name)
来源：http://ryj.hfpthk.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jjy.shuidangran.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sic.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cqm.chenjidiqi.icu

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kme.sjlbkw.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rau.316326.xyz

[E19] 多行文本按行拆分
来源：http://hjd.vehdjk.com

Py:   s.splitlines()
来源：http://kkm.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bkr.yanxiufei.cn

JS:   s.split(/\r?\n/)
来源：http://frk.pycfn.com

TS:   s.split(/\r?\n/)
来源：http://ltl.ivvv.top

Java: s.lines().toList()
来源：http://vpt.jinqigfzy.top

Go:   strings.Split(s, "\n")
来源：http://lnk.fehbvm.com

Ruby: s.lines
来源：http://xbv.cucudq.cn

C#:   s.Split('\n')
来源：http://tfv.guowangkeji.top

[E20] 判断字符串是否为空
来源：http://sgn.zhengqikj.top

Py:   if not s:
来源：http://bsl.vehdjk.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pjg.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zla.hysaishi.cn

TS:   if (s === "") {}
来源：http://xss.ehwqpu.com

Java: if (s.isEmpty()) {}
来源：http://uhy.kuanghao11.cn

Go:   if s == "" {}
来源：http://hhl.zhoulong.xyz

Ruby: if s.empty?
来源：http://yud.shangyingyoupin.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tfo.jqgufenzy.top

[E21] 超长截断加省略号
来源：http://txv.wangshuangyany.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://oah.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rsf.yuanzhike.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://add.yuxming.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tiu.birdmap.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ogx.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://xot.hcnkem.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gdq.zdqjudy.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://soz.jyoumei.cn

[E22] 字节长度与字符长度
来源：http://lqn.hongshengwenyu.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xwp.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yps.feifeiyinyue.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nmz.52xcode.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhq.wangdashe.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://act.chenjidiqi.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xbj.zhongyouzk.top

Ruby: s.bytesize;  s.length
来源：http://uvr.snrcjt.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://brh.ehwqpu.com

================================================================================
来源：http://qjn.ppjwa.cn

F. 文件与目录
来源：http://csm.0kj1m.cn

================================================================================
来源：http://tcg.snrcjt.cn

[F01] 读取整个文件
来源：http://fkn.pengpengdd.cyou

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tvc.shanyushiyangkeji.top

PHP:  file_get_contents("a.txt");
来源：http://fnl.sweek.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fju.guowangkeji.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://owp.haohaochexian.top

Java: Files.readString(Path.of("a.txt"))
来源：http://ycw.yongpay.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wrm.yfazqb.com

Ruby: File.read("a.txt")
来源：http://mxe.ehwqpu.com

C#:   File.ReadAllText("a.txt");
来源：http://wws.dianchejie.cn

[F02] 逐行读取文件
来源：http://zsw.yongpay.top

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wen.fengsongda.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://utq.cucudq.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://psl.zhoulong.xyz

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mym.cdnleiting.top

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wyg.epnwcf.com

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vop.chenjidiqi.icu

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vfn.tianlin.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pqk.sxryk.cn

[F03] 写入文件（覆盖）
来源：http://wxv.sufxvd.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ueo.cdnleiting.top

PHP:  file_put_contents("a.txt", "hi");
来源：http://yxg.yonumen.top

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bny.nwbrower.top

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://faa.meibo888.top

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yiz.vehdjk.com

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://iru.hammf.cn

Ruby: File.write("a.txt", "hi")
来源：http://fwe.yanxiufei.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lkj.birdmap.top

[F04] 追加写入文件
来源：http://evf.daxiang520.top

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://goq.daria6918.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jfg.sysykeji.top

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tfy.dianchejie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://owc.xingfuxueyuan.xyz

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mgb.ywan-chungtsiang.top

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wii.daria6918.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://oig.nanxuanxn.top

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eke.jianghu66.top

[F05] 判断文件或目录是否存在
来源：http://mei.shzxlz.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lhq.hysaishi.cn

PHP:  file_exists("a.txt");
来源：http://yge.dianchejie.cn

JS:   fs.existsSync("a.txt")
来源：http://ecn.meibo888.top


<!-- 参考信息 -->