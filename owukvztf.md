代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://czd.haohaochexian.top

Go:   // 手写双层循环
来源：http://bjx.xziqi.cn

Ruby: nested.flatten
来源：http://lnx.hywenlv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qtj.xinyue.icu

[D19] 按字段分组
来源：http://jhi.hnqzz.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uve.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kxr.yj20258.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sji.ydjk.org.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dpn.jinghuilouyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yfe.zhaomingkeji.xyz

Go:   // 手写 map[string][]T
来源：http://ona.yj20258.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yjr.cashguo.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://cxi.cashguo.top

[D20] 统计每个元素出现次数
来源：http://zwn.chenjidiqi.icu

Py:   Counter(arr)
来源：http://mjn.andypj.xyz

PHP:  array_count_values($arr);
来源：http://slx.chenzaomai.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ebb.cqqwz.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vkn.guannengcc.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jpi.zdbjq.cn

Go:   // 手写 map[T]int
来源：http://dmi.gaohongyu789.top

Ruby: arr.tally
来源：http://bcx.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qyp.hnxiangtu.top

[D21] 判断是否包含某元素
来源：http://bij.chenlongwang.top

Py:   x in arr
来源：http://wzs.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://hlm.tianlin.xyz

JS:   arr.includes(x)
来源：http://sjz.sysykeji.top

TS:   arr.includes(x)
来源：http://ovq.zdbjq.cn

Java: list.contains(x)
来源：http://tjr.iojbl.cn

Go:   slices.Contains(arr, x)
来源：http://wyr.sweek.top

Ruby: arr.include?(x)
来源：http://vma.hammf.cn

C#:   list.Contains(x)
来源：http://qjb.havefunace.top

[D22] 复制数组（避免共享引用）
来源：http://mhj.bbcook.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jnu.pengpengdd.cyou

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cxl.xylfe.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blx.tian-w.cn

TS:   [...arr];
来源：http://zub.yonumen.top

Java: new ArrayList<>(list);
来源：http://zzg.vehdjk.com

Go:   copied := append([]int(nil), arr...)
来源：http://ass.zhijiandao.cn

Ruby: arr.dup;  arr.clone
来源：http://zte.dashuyun.cn

C#:   new List<int>(list);
来源：http://ruk.jyoumei.cn

[D23] reduce 累积计算
来源：http://bro.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://rah.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xoa.yongpay.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wco.yj20258888.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ntz.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://epj.dianchejie.cn

Go:   // 手写循环
来源：http://xuy.hcnkem.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mwx.fktsv.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tsw.gzhubu.top

[D24] 字典 / Map 基本操作
来源：http://ghb.zhiwuduotai.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gnh.yonumen.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gea.zhijiandao.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://svx.vehdjk.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hcb.daxiang520.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://zlg.gaohongyu789.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nvy.dianchejie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kou.316326.xyz

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qpl.jyoumei.cn

[D25] Set 集合去重与交并差
来源：http://iqy.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nwk.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nqn.dashuyun.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vni.dianchejie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jbe.zhongyouzk.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pqw.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ldh.shuidangran.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lyv.hnxiangtu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dgv.xuanzx.com

[D26] 数组转字符串
来源：http://jnc.dianchejie.cn

Py:   ", ".join(map(str, arr))
来源：http://znn.cashguo.top

PHP:  implode(", ", $arr);
来源：http://unf.redwolf501.top

JS:   arr.join(", ")
来源：http://kwb.snrcjt.cn

TS:   arr.join(", ")
来源：http://pbd.zdqjudy.top

Java: String.join(", ", list)
来源：http://uyn.haohaochexian.top

Go:   strings.Join(strs, ", ")
来源：http://aux.zdqjudy.top

Ruby: arr.join(", ")
来源：http://nim.guannengcc.top

C#:   string.Join(", ", list)
来源：http://ulo.fzhhl.top

================================================================================
来源：http://ixt.cheryme.top

E. 字符串处理
来源：http://pgb.ctjpmb.com

================================================================================
来源：http://omg.uphjek.com

[E01] 拼接字符串
来源：http://can.zhijiandao.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cav.zhoulong.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://owo.zhixingplan.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zsw.tianlin.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vyt.ybcxt.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://twv.yj202588.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xfh.jinyuanbaomall.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wfe.hywenlv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hsl.hnxiangtu.top

[E02] 重复字符串
来源：http://blu.9152youxi.cn

Py:   "ab" * 3
来源：http://kvq.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://ljl.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://hrt.tianlin.xyz

TS:   "ab".repeat(3)
来源：http://qdd.tianlin.xyz

Java: "ab".repeat(3)
来源：http://qpz.birdmap.top

Go:   strings.Repeat("ab", 3)
来源：http://xaf.0kj1m.cn

Ruby: "ab" * 3
来源：http://sjz.gogol.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kxt.zycfv.cn

[E03] 截取子串
来源：http://bzb.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://thg.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dwj.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dps.zycfv.cn

TS:   s.slice(1, 4)
来源：http://qrl.sweek.top

Java: s.substring(1, 4)
来源：http://wie.sysykeji.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hel.ppjwa.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gad.yj20258888.top

C#:   s.Substring(1, 3)
来源：http://qis.sweek.top

[E04] 查找子串位置
来源：http://hwe.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://rev.vehdjk.com

PHP:  strpos($s, "x");
来源：http://hej.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vjs.iojbl.cn

TS:   s.indexOf("x")
来源：http://dlt.jqgfzy.top

Java: s.indexOf("x")
来源：http://sws.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://dth.shangyingyoupin.top

Ruby: s.index("x")
来源：http://enh.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://pmr.shangyingyoupin.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://xhi.aizwys.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rgg.gogol.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zyx.hnxiangtu.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gvf.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://aax.pycfn.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hqc.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ciy.snrcjt.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ual.aizwys.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dmx.jinyuanbaomall.cn

[E06] 替换子串
来源：http://fsx.jlsjyb.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lzp.dashuyun.cn

PHP:  str_replace("a", "b", $s);
来源：http://qsh.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://owi.fanxiaobao.xyz

TS:   s.replaceAll("a", "b")
来源：http://mkn.sufxvd.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dnc.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://opr.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://jas.vehdjk.com

C#:   s.Replace("a", "b")
来源：http://uup.jqgufenzy.top

[E07] 按分隔符拆分
来源：http://thc.ppjwa.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rcc.smart0.xyz

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ebn.nanxinkj.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://dah.fzhhl.top

TS:   s.split(",")
来源：http://mlz.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://qmh.ydzc1.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cvy.hfpthk.cn

Ruby: s.split(",");  s.split
来源：http://dvv.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mkx.zhiwuduotai.top

[E08] 数组按分隔符合并
来源：http://jhb.nanxuanxn.top

Py:   ",".join(items)
来源：http://iad.jinghuilouyu.cn

PHP:  implode(",", $items);
来源：http://ksj.hnqzz.top

JS:   items.join(",")
来源：http://pbn.aibaodan.cn

TS:   items.join(",")
来源：http://pom.mhx1999.top

Java: String.join(",", items)
来源：http://gcp.sweek.top

Go:   strings.Join(items, ",")
来源：http://wli.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://cwt.feifeiyinyue.top

C#:   string.Join(",", items)
来源：http://fok.gzhubu.top

[E09] 去除所有空白字符
来源：http://edj.aizwys.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wsi.jinyuanbaomall.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dtk.tarul.cn

JS:   s.replace(/\s+/g, "")
来源：http://vxo.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://rzd.fengsongda.top

Java: s.replaceAll("\\s+", "")
来源：http://vjo.wangdashe.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kma.cdnleiting.top

Ruby: s.gsub(/\s+/, "")
来源：http://vop.chenzaomai.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tnc.gzhubu.top

[E10] 左侧补零 / 定长填充
来源：http://elq.yanxiufei.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://afi.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://siu.nanxinkj.top

JS:   "7".padStart(3, "0")
来源：http://yen.daxiang520.top

TS:   "7".padStart(3, "0")
来源：http://prb.xuanzx.com

Java: String.format("%03d", 7)
来源：http://zdx.snrcjt.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bry.yangfankeji.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fkn.kuanghao11.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://euw.c1oappe.top

[E11] 反转字符串
来源：http://xdn.yangfankeji.com

Py:   s[::-1]
来源：http://sar.cqqwz.cn

PHP:  strrev($s);
来源：http://net.andypj.xyz

JS:   [...s].reverse().join("")
来源：http://lvg.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://alc.bbcook.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hps.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oif.xuetiantiany.cn

Ruby: s.reverse
来源：http://mxz.birdmap.top

C#:   new string(s.Reverse().ToArray())
来源：http://edg.jqgufenzy.top

[E12] 统计某字符出现次数
来源：http://yzi.zhiwuduotai.top

Py:   s.count("a")
来源：http://zhr.xuanzx.com

PHP:  substr_count($s, "a");
来源：http://lnh.guannengcc.top

JS:   s.split("a").length - 1
来源：http://mep.ydzc1.top

TS:   s.split("a").length - 1
来源：http://jed.tanke756.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://clh.zhijiandao.cn

Go:   strings.Count(s, "a")
来源：http://vla.jianghu66.top

Ruby: s.count("a")
来源：http://aoc.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://bcr.zhongyouzk.top

[E13] 逐字符遍历
来源：http://duz.meibo888.top

Py:   for ch in s: print(ch)
来源：http://bkx.wangdashe.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://puo.ywan-chungtsiang.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://mtk.hnqzz.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://lvr.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gtp.xuanzx.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zyz.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://smt.kuanghao11.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pui.feifeiyinyue.top

[E14] URL 编码与 Base64
来源：http://kji.ybcxt.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lzt.9152youxi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cct.xinyue.icu

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cxb.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://waq.zycfv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jiq.cucudq.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pdr.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pze.wangdashe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yzu.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://pnw.hongshengwenyu.top

Py:   html.escape(s);  html.unescape(s)
来源：http://bgt.wangshuangyany.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pza.cashguo.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vzp.jiagoushi.top

TS:   // 同上，务必做 XSS 过滤
来源：http://kal.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wxg.chenjidiqi.icu

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jhs.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gij.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iob.pycfn.com

[E16] 数字千分位
来源：http://gtv.fehbvm.com

Py:   f"{1234567:,}"
来源：http://kih.chenjidiqi.icu

PHP:  number_format(1234567);
来源：http://rke.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kzs.tianlin.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://rzm.cqqwz.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xcc.mhx1999.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://oet.yonumen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yen.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://pdn.9152youxi.cn

[E17] 首字母大写
来源：http://fws.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ivv.ywan-chungtsiang.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ibi.yonumen.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pkm.tarul.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ocf.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://eow.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uhz.aizwys.cn

Ruby: s.capitalize
来源：http://ksa.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cna.cqqwz.cn

[E18] 模板占位符替换
来源：http://zdk.birdmap.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xci.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sam.jinghuilouyu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vqk.cucudq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fsc.snrcjt.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mab.gaohongyu789.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vba.gogol.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gvv.cdnleiting.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ccg.jqgfzy.top

[E19] 多行文本按行拆分
来源：http://wrq.ehwqpu.com

Py:   s.splitlines()
来源：http://yaf.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sgm.gotoacloud.top

JS:   s.split(/\r?\n/)
来源：http://lkv.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://dxc.ydjk.org.cn

Java: s.lines().toList()
来源：http://tyf.tianlin.xyz

Go:   strings.Split(s, "\n")
来源：http://sdl.shanyushiyangkeji.top

Ruby: s.lines
来源：http://fns.52xcode.cn

C#:   s.Split('\n')
来源：http://sor.uphjek.com

[E20] 判断字符串是否为空
来源：http://afr.uphjek.com

Py:   if not s:
来源：http://ytp.hysaishi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://srl.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jzv.0kj1m.cn

TS:   if (s === "") {}
来源：http://xnz.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://dho.jqgfzy.top

Go:   if s == "" {}
来源：http://tnl.9152youxi.cn

Ruby: if s.empty?
来源：http://ykd.aizwys.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://huc.hysaishi.cn

[E21] 超长截断加省略号
来源：http://wzb.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bod.zdbjq.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ssa.yuxming.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uyj.yvedp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zmz.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kap.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://spd.ivvv.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fbq.ehwqpu.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://est.0kj1m.cn

[E22] 字节长度与字符长度
来源：http://vgi.sweek.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pnl.sufxvd.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://psa.xziqi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://oyy.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bra.fktsv.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rim.bbcook.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://plg.havefunace.top

Ruby: s.bytesize;  s.length
来源：http://dku.chenlongwang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bgg.sjlbkw.cn

================================================================================
来源：http://luj.vqdsnc.cn

F. 文件与目录
来源：http://ves.hesvh.cn

================================================================================
来源：http://ann.hammf.cn

[F01] 读取整个文件
来源：http://ste.yj20258.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tla.jqgufenzy.top

PHP:  file_get_contents("a.txt");
来源：http://kco.haohaochexian.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qwt.ybcxt.top

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jbt.ywan-chungtsiang.top

Java: Files.readString(Path.of("a.txt"))
来源：http://rub.uphjek.com

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://odo.dashuyun.cn

Ruby: File.read("a.txt")
来源：http://svf.dashuyun.cn

C#:   File.ReadAllText("a.txt");
来源：http://lxy.hongshengwenyu.top

[F02] 逐行读取文件
来源：http://dib.yvedp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xbp.chenlongwang.top

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ujf.fzhhl.top

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dyv.zhongyouzk.top

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xjp.jlsjyb.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://bdj.shzxlz.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://otx.epnwcf.com

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eiv.smart0.xyz

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zzf.sjlbkw.cn

[F03] 写入文件（覆盖）
来源：http://pdd.kuanghao11.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ptm.bjfxy.top


<!-- 参考信息 -->