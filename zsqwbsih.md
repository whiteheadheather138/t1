代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ytc.bbcook.cn

Go:   // 手写双层循环
来源：http://gju.xziqi.cn

Ruby: nested.flatten
来源：http://kpr.fengsongda.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://ubv.yj202588.top

[D19] 按字段分组
来源：http://ugv.gzhubu.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vqu.xinyue.icu

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vwi.pengpengdd.cyou

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ezz.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://usf.feifeiyinyue.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://jam.meibo888.top

Go:   // 手写 map[string][]T
来源：http://wmg.cashguo.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://aqd.shuidangran.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fyv.xinyue.icu

[D20] 统计每个元素出现次数
来源：http://kul.c1oappe.top

Py:   Counter(arr)
来源：http://bde.nwbrower.top

PHP:  array_count_values($arr);
来源：http://jmw.xylfe.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fqv.jianghu66.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qpe.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ozh.xylfe.cn

Go:   // 手写 map[T]int
来源：http://aoh.chenjidiqi.icu

Ruby: arr.tally
来源：http://uun.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qbr.zdqjudy.top

[D21] 判断是否包含某元素
来源：http://mgo.fktsv.cn

Py:   x in arr
来源：http://fak.zhijiandao.cn

PHP:  in_array($x, $arr, true);
来源：http://umy.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://keu.yonumen.top

TS:   arr.includes(x)
来源：http://xin.vqdsnc.cn

Java: list.contains(x)
来源：http://yck.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://aqu.zdbjq.cn

Ruby: arr.include?(x)
来源：http://yod.aizwys.cn

C#:   list.Contains(x)
来源：http://sgg.hnxiangtu.top

[D22] 复制数组（避免共享引用）
来源：http://fxv.aizwys.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://zym.shangyingyoupin.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ons.yonumen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eya.cqqwz.cn

TS:   [...arr];
来源：http://ccp.mhx1999.top

Java: new ArrayList<>(list);
来源：http://oro.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://aau.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://ulo.zhengqikj.top

C#:   new List<int>(list);
来源：http://odu.zhoulong.xyz

[D23] reduce 累积计算
来源：http://orh.jyoumei.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://idm.sysykeji.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dtb.0kj1m.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://msd.daria6918.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yyd.cqqwz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pai.epnwcf.com

Go:   // 手写循环
来源：http://jux.sxryk.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ckz.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pty.yj20258888.top

[D24] 字典 / Map 基本操作
来源：http://qdc.cucudq.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://crw.hfpthk.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qmx.epnwcf.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://oua.pycfn.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xev.hnqzz.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ccv.fktsv.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://red.xingfuxueyuan.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://brc.tanke756.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cmc.birdmap.top

[D25] Set 集合去重与交并差
来源：http://bzz.hesvh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://clv.daria6918.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nwi.birdmap.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hjx.yangfankeji.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://eaf.jqgufenzy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hpu.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://svz.meibo888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://apt.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://lqr.316326.xyz

[D26] 数组转字符串
来源：http://nyx.haohaochexian.top

Py:   ", ".join(map(str, arr))
来源：http://cbb.chenjidiqi.icu

PHP:  implode(", ", $arr);
来源：http://gmm.yuanzhike.top

JS:   arr.join(", ")
来源：http://dgi.uphjek.com

TS:   arr.join(", ")
来源：http://dqh.sysykeji.top

Java: String.join(", ", list)
来源：http://avt.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://fmq.zhaomingkeji.xyz

Ruby: arr.join(", ")
来源：http://vop.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://izf.vehdjk.com

================================================================================
来源：http://fkw.hywenlv.cn

E. 字符串处理
来源：http://xou.ydjk.org.cn

================================================================================
来源：http://yhn.shzxlz.cn

[E01] 拼接字符串
来源：http://ucp.fehbvm.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vxz.yuanzhike.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dtt.fktsv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lzz.snrcjt.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ygk.fehbvm.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://brw.hywenlv.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vlt.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zvh.zdqjudy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nqo.jianghu66.top

[E02] 重复字符串
来源：http://ovc.jinyuanbaomall.cn

Py:   "ab" * 3
来源：http://nup.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://qqe.daria6918.cn

JS:   "ab".repeat(3)
来源：http://rju.zhiwuduotai.top

TS:   "ab".repeat(3)
来源：http://owy.xingfuxueyuan.xyz

Java: "ab".repeat(3)
来源：http://fex.yj20258.top

Go:   strings.Repeat("ab", 3)
来源：http://ekm.hysaishi.cn

Ruby: "ab" * 3
来源：http://ekb.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lfm.zhijiandao.cn

[E03] 截取子串
来源：http://jao.nanxinkj.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ztm.ydzc1.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://bge.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qrm.xziqi.cn

TS:   s.slice(1, 4)
来源：http://gzm.xinyue.icu

Java: s.substring(1, 4)
来源：http://afj.jinyuanbaomall.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qyj.cashguo.top

Ruby: s[1, 3];  s[1..3]
来源：http://rfc.xziqi.cn

C#:   s.Substring(1, 3)
来源：http://yoo.guowangkeji.top

[E04] 查找子串位置
来源：http://has.andypj.xyz

Py:   s.find("x");  s.index("x")
来源：http://izj.nwbrower.top

PHP:  strpos($s, "x");
来源：http://ivy.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ajc.gaohongyu789.top

TS:   s.indexOf("x")
来源：http://abo.ydzc1.top

Java: s.indexOf("x")
来源：http://mva.tanke756.top

Go:   strings.Index(s, "x")
来源：http://nyr.sysykeji.top

Ruby: s.index("x")
来源：http://fxv.zdqjudy.top

C#:   s.IndexOf("x")
来源：http://kev.fehbvm.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://jok.jianghu66.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lin.cucudq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ock.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qkq.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://eyc.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gqn.nwbrower.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hkc.jiagoushi.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zhl.c1oappe.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kzb.sufxvd.cn

[E06] 替换子串
来源：http://gsm.9152youxi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iwd.jyoumei.cn

PHP:  str_replace("a", "b", $s);
来源：http://zcx.zycfv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nln.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://zpk.chenjidiqi.icu

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qqf.daria6918.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zdl.gogol.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jua.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://iow.tianlin.xyz

[E07] 按分隔符拆分
来源：http://ycj.xuanzx.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kmb.sxryk.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kad.zhongyouzk.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cwe.ctjpmb.com

TS:   s.split(",")
来源：http://omx.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nnn.hywenlv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qse.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://roi.epnwcf.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dxb.yj20258888.top

[E08] 数组按分隔符合并
来源：http://eju.yj20258.top

Py:   ",".join(items)
来源：http://xgm.iojbl.cn

PHP:  implode(",", $items);
来源：http://kek.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://ewk.guannengcc.top

TS:   items.join(",")
来源：http://hct.9152youxi.cn

Java: String.join(",", items)
来源：http://ulh.zhongyouzk.top

Go:   strings.Join(items, ",")
来源：http://eqe.zdbjq.cn

Ruby: items.join(",")
来源：http://mlz.yj20258.top

C#:   string.Join(",", items)
来源：http://qti.quarkkingdee.top

[E09] 去除所有空白字符
来源：http://spc.pengpengdd.cyou

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kge.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jof.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://dmz.tanke756.top

TS:   s.replace(/\s+/g, "")
来源：http://zqz.jqgufenzy.top

Java: s.replaceAll("\\s+", "")
来源：http://agh.316326.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://buh.tarul.cn

Ruby: s.gsub(/\s+/, "")
来源：http://smq.tanke756.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xaj.guannengcc.top

[E10] 左侧补零 / 定长填充
来源：http://cqf.hcnkem.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rif.chenlongwang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vif.sweek.top

JS:   "7".padStart(3, "0")
来源：http://stn.xuetiantiany.cn

TS:   "7".padStart(3, "0")
来源：http://exd.xuetiantiany.cn

Java: String.format("%03d", 7)
来源：http://mmj.yj202588.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://xis.guowangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pwm.zhengqikj.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xjs.9152youxi.cn

[E11] 反转字符串
来源：http://heg.0kj1m.cn

Py:   s[::-1]
来源：http://xep.jinyuanbaomall.cn

PHP:  strrev($s);
来源：http://goh.hnxiangtu.top

JS:   [...s].reverse().join("")
来源：http://gon.aibaodan.cn

TS:   [...s].reverse().join("")
来源：http://qwv.yueranfly.top

Java: new StringBuilder(s).reverse().toString()
来源：http://pqo.zhengqikj.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://pva.sxryk.cn

Ruby: s.reverse
来源：http://eps.jinqigufen.top

C#:   new string(s.Reverse().ToArray())
来源：http://kdi.hysaishi.cn

[E12] 统计某字符出现次数
来源：http://fae.mhx1999.top

Py:   s.count("a")
来源：http://dzu.ivvv.top

PHP:  substr_count($s, "a");
来源：http://tpa.yj202588.top

JS:   s.split("a").length - 1
来源：http://dpm.yj20258888.top

TS:   s.split("a").length - 1
来源：http://mel.ydzc1.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kgp.aizwys.cn

Go:   strings.Count(s, "a")
来源：http://maw.gaohongyu789.top

Ruby: s.count("a")
来源：http://txd.shzxlz.cn

C#:   s.Count(c => c == 'a')
来源：http://zwr.uphjek.com

[E13] 逐字符遍历
来源：http://cds.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://vlq.sxryk.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ffj.gaohongyu789.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://hap.zhixingplan.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://oul.jyoumei.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rfu.havefunace.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://haa.fanxiaobao.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://fll.zhiwuduotai.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://njx.yj20258.top

[E14] URL 编码与 Base64
来源：http://nkd.9152youxi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gpu.hnqzz.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tfe.jyoumei.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://eyj.pengpengdd.cyou

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hgk.jinqigfzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hli.jianghu66.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ypg.jianghu66.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hfy.ybcxt.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kbp.jinghuilouyu.cn

[E15] HTML 转义 / 反转义
来源：http://nnu.sjlbkw.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wnv.redwolf501.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pnn.yueranfly.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vdx.zycfv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pqm.cheryme.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ked.sysykeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hot.c1oappe.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pkt.chenjidiqi.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qrg.9152youxi.cn

[E16] 数字千分位
来源：http://mrp.tianlin.xyz

Py:   f"{1234567:,}"
来源：http://jck.cheryme.top

PHP:  number_format(1234567);
来源：http://hcz.jinqigufen.top

JS:   (1234567).toLocaleString("en-US")
来源：http://yrj.cashguo.top

TS:   (1234567).toLocaleString("en-US")
来源：http://cao.bbcook.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ayw.hnxiangtu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iqa.316326.xyz

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rlj.yueranfly.top

C#:   1234567.ToString("N0")
来源：http://nkm.birdmap.top

[E17] 首字母大写
来源：http://wlq.chenjidiqi.icu

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mlv.havefunace.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fbq.yfazqb.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dbz.vehdjk.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxm.zhaomingkeji.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yxk.dashuyun.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ncv.zdqjudy.top

Ruby: s.capitalize
来源：http://ctg.dianchejie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ptw.pengpengdd.cyou

[E18] 模板占位符替换
来源：http://nmt.zhaomingkeji.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://urr.cheryme.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://oor.yfazqb.com

JS:   tpl.replaceAll("{name}", name)
来源：http://chi.ctjpmb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://drt.yfazqb.com

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://slc.nwbrower.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dsz.redwolf501.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fqd.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yzn.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://iwv.tianlin.xyz

Py:   s.splitlines()
来源：http://nqb.wangshuangyany.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fiq.epnwcf.com

JS:   s.split(/\r?\n/)
来源：http://ofy.jianghu66.top

TS:   s.split(/\r?\n/)
来源：http://fta.zhoulong.xyz

Java: s.lines().toList()
来源：http://lbj.jqgufenzy.top

Go:   strings.Split(s, "\n")
来源：http://rbu.xziqi.cn

Ruby: s.lines
来源：http://iql.uphjek.com

C#:   s.Split('\n')
来源：http://vek.ehwqpu.com

[E20] 判断字符串是否为空
来源：http://wmp.hfpthk.cn

Py:   if not s:
来源：http://azv.fehbvm.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ajd.gogol.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uwl.cdnleiting.top

TS:   if (s === "") {}
来源：http://kzj.ctjpmb.com

Java: if (s.isEmpty()) {}
来源：http://iav.cheryme.top

Go:   if s == "" {}
来源：http://xgq.ivvv.top

Ruby: if s.empty?
来源：http://day.jinyuanbaomall.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ore.zhoulong.xyz

[E21] 超长截断加省略号
来源：http://vuq.cdnleiting.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://itg.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vft.tian-w.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tsm.jlsjyb.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mdo.wangshuangyany.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://eru.ywan-chungtsiang.top

Go:   // 按 rune 判断长度后截断
来源：http://rcw.shanyushiyangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oiy.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fyh.jqgfzy.top

[E22] 字节长度与字符长度
来源：http://plx.ywan-chungtsiang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tma.daria6918.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kwy.ppjwa.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jzv.jinyuanbaomall.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yyj.yonumen.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://brk.ehwqpu.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gjj.tanke756.top

Ruby: s.bytesize;  s.length
来源：http://zcv.shzxlz.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yth.yongpay.top

================================================================================
来源：http://xva.tian-w.cn

F. 文件与目录
来源：http://xer.meibo888.top

================================================================================
来源：http://vzh.ehwqpu.com

[F01] 读取整个文件
来源：http://lsb.cqqwz.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eje.uphjek.com

PHP:  file_get_contents("a.txt");
来源：http://afn.0kj1m.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lzv.hesvh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pbe.epnwcf.com

Java: Files.readString(Path.of("a.txt"))
来源：http://dpc.sweek.top

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gfs.jinqigufen.top

Ruby: File.read("a.txt")
来源：http://oey.zhijiandao.cn

C#:   File.ReadAllText("a.txt");
来源：http://wif.tianlin.xyz

[F02] 逐行读取文件
来源：http://ykp.cucudq.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rxc.gotoacloud.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dgh.shuidangran.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zhf.ivvv.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lml.hywenlv.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wyt.hywenlv.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uqs.zdbjq.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mel.hcnkem.com

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rox.andypj.xyz

[F03] 写入文件（覆盖）
来源：http://dxf.daria6918.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vxp.yanxiufei.cn


<!-- 参考信息 -->