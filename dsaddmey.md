代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hyi.tanke756.top

[D16] 求和与平均值
来源：http://ksu.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nbl.hnqzz.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://dvo.feifeiyinyue.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://che.yuanzhike.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ftj.jianghu66.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hlv.sjlbkw.cn

Go:   // 手写循环累加
来源：http://jgq.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zeq.c1oappe.top

C#:   list.Sum();  list.Average()
来源：http://tet.yj20258888.top

[D17] 最大值与最小值
来源：http://hag.sysykeji.top

Py:   max(arr);  min(arr)
来源：http://hhb.zhiwuduotai.top

PHP:  max($arr);  min($arr);
来源：http://ayc.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vml.ivvv.top

TS:   Math.max(...arr);
来源：http://xao.nanxinkj.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kvk.cqqwz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uez.yuanzhike.top

Ruby: arr.max;  arr.min
来源：http://ino.cucudq.cn

C#:   list.Max();  list.Min()
来源：http://uuz.vqdsnc.cn

[D18] 扁平化嵌套数组
来源：http://bim.xingfuxueyuan.xyz

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://igj.daxiang520.top

PHP:  array_merge(...$nested);
来源：http://wyf.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yzb.iojbl.cn

TS:   nested.flat();
来源：http://tmm.tarul.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jxq.tianlin.xyz

Go:   // 手写双层循环
来源：http://rzc.zhiwuduotai.top

Ruby: nested.flatten
来源：http://top.redwolf501.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rto.uphjek.com

[D19] 按字段分组
来源：http://gjr.shzxlz.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hfx.yuanzhike.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://crl.xylfe.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yzu.ydzc1.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://sjm.ybcxt.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://irc.jinghuilouyu.cn

Go:   // 手写 map[string][]T
来源：http://hvq.aizwys.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dus.yvedp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vzk.fzhhl.top

[D20] 统计每个元素出现次数
来源：http://irt.uphjek.com

Py:   Counter(arr)
来源：http://rei.cqqwz.cn

PHP:  array_count_values($arr);
来源：http://cec.kuanghao11.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aej.sxryk.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hqx.ydjk.org.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://igp.uphjek.com

Go:   // 手写 map[T]int
来源：http://sfr.pengpengdd.cyou

Ruby: arr.tally
来源：http://lwy.epnwcf.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aof.yanxiufei.cn

[D21] 判断是否包含某元素
来源：http://ljm.hfpthk.cn

Py:   x in arr
来源：http://wlh.quarkkingdee.top

PHP:  in_array($x, $arr, true);
来源：http://jyy.andypj.xyz

JS:   arr.includes(x)
来源：http://jop.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://hvp.fengsongda.top

Java: list.contains(x)
来源：http://okc.ybcxt.top

Go:   slices.Contains(arr, x)
来源：http://pyq.bbcook.cn

Ruby: arr.include?(x)
来源：http://bhe.hammf.cn

C#:   list.Contains(x)
来源：http://lfc.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://oik.hnqzz.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fms.yvedp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fns.yj20258.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jzp.jlsjyb.cn

TS:   [...arr];
来源：http://pcw.c1oappe.top

Java: new ArrayList<>(list);
来源：http://mkg.jiagoushi.top

Go:   copied := append([]int(nil), arr...)
来源：http://ltv.zhengqikj.top

Ruby: arr.dup;  arr.clone
来源：http://ubk.aibaodan.cn

C#:   new List<int>(list);
来源：http://dfw.jianghu66.top

[D23] reduce 累积计算
来源：http://uvc.gogol.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://znx.hnxiangtu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bks.aizwys.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ruy.gaohongyu789.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://otg.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rjg.bbcook.cn

Go:   // 手写循环
来源：http://yjx.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xjr.kuanghao11.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pib.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://hpy.wangshuangyany.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://tqi.ehwqpu.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rre.sweek.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cwp.ehwqpu.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ngw.jqgfzy.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bul.shanyushiyangtech.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://szy.cqqwz.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xqy.hywenlv.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wno.chenzaomai.com

[D25] Set 集合去重与交并差
来源：http://gfb.cucudq.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://vlq.dashuyun.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://laj.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tbc.haohaochexian.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://gmx.yvedp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nwg.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qvd.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qbi.gaohongyu789.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blj.hongshengwenyu.top

[D26] 数组转字符串
来源：http://dzs.gotoacloud.top

Py:   ", ".join(map(str, arr))
来源：http://zfb.redwolf501.top

PHP:  implode(", ", $arr);
来源：http://ipm.zhaomingkeji.xyz

JS:   arr.join(", ")
来源：http://nrv.jqgfzy.top

TS:   arr.join(", ")
来源：http://rwq.nanxinkj.top

Java: String.join(", ", list)
来源：http://kal.yuxming.cn

Go:   strings.Join(strs, ", ")
来源：http://gzg.havefunace.top

Ruby: arr.join(", ")
来源：http://oko.sufxvd.cn

C#:   string.Join(", ", list)
来源：http://bop.sjlbkw.cn

================================================================================
来源：http://ogu.hywenlv.cn

E. 字符串处理
来源：http://wny.hammf.cn

================================================================================
来源：http://rej.shuidangran.top

[E01] 拼接字符串
来源：http://jzf.yj202588.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wsl.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ptw.havefunace.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xxl.hesvh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wqi.cqqwz.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nru.jinqigfzy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iyi.zdbjq.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lyh.zhiwuduotai.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oni.zycfv.cn

[E02] 重复字符串
来源：http://oto.pengpengdd.cyou

Py:   "ab" * 3
来源：http://pti.jinghuilouyu.cn

PHP:  str_repeat("ab", 3);
来源：http://nvv.xingfuxueyuan.xyz

JS:   "ab".repeat(3)
来源：http://nrm.shanyushiyangtech.top

TS:   "ab".repeat(3)
来源：http://ahs.hammf.cn

Java: "ab".repeat(3)
来源：http://wff.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://nlk.zhaomingkeji.xyz

Ruby: "ab" * 3
来源：http://whw.shzxlz.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fwr.vehdjk.com

[E03] 截取子串
来源：http://cpo.xuetiantiany.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://krd.chenlongwang.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vxj.zhijiandao.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://bci.fehbvm.com

TS:   s.slice(1, 4)
来源：http://jbn.jiagoushi.top

Java: s.substring(1, 4)
来源：http://lbj.xuanzx.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ybo.ybcxt.top

Ruby: s[1, 3];  s[1..3]
来源：http://mbu.hammf.cn

C#:   s.Substring(1, 3)
来源：http://tix.yuxming.cn

[E04] 查找子串位置
来源：http://llh.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://ivn.yj20258.top

PHP:  strpos($s, "x");
来源：http://hzh.sxryk.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kgx.cashguo.top

TS:   s.indexOf("x")
来源：http://ams.yj20258888.top

Java: s.indexOf("x")
来源：http://kbc.fktsv.cn

Go:   strings.Index(s, "x")
来源：http://fkw.ydjk.org.cn

Ruby: s.index("x")
来源：http://noc.yonumen.top

C#:   s.IndexOf("x")
来源：http://joj.jiagoushi.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://qxi.xylfe.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://izn.mhx1999.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ufg.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pac.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://pgn.chenjidiqi.icu

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://orn.mhx1999.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wht.havefunace.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bej.zdbjq.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mku.hywenlv.cn

[E06] 替换子串
来源：http://pit.fehbvm.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ewy.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://swm.feifeiyinyue.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xcf.yj202588.top

TS:   s.replaceAll("a", "b")
来源：http://hdu.jyoumei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gst.guowangkeji.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yri.gotoacloud.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gfk.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://fxz.fzhhl.top

[E07] 按分隔符拆分
来源：http://zgf.yanxiufei.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jfv.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eqi.pycfn.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://hza.gogol.net.cn

TS:   s.split(",")
来源：http://jxg.yj20258888.top

Java: s.split(",");  s.split("\\s+")
来源：http://omq.aizwys.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uea.ivvv.top

Ruby: s.split(",");  s.split
来源：http://uek.jqgfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://efo.jinghuilouyu.cn

[E08] 数组按分隔符合并
来源：http://svn.zhijiandao.cn

Py:   ",".join(items)
来源：http://gaq.feifeiyinyue.top

PHP:  implode(",", $items);
来源：http://bss.daria6918.cn

JS:   items.join(",")
来源：http://amv.ppjwa.cn

TS:   items.join(",")
来源：http://fkc.uphjek.com

Java: String.join(",", items)
来源：http://idr.shuidangran.top

Go:   strings.Join(items, ",")
来源：http://jlv.shzxlz.cn

Ruby: items.join(",")
来源：http://bdt.zdbjq.cn

C#:   string.Join(",", items)
来源：http://zsb.jianghu66.top

[E09] 去除所有空白字符
来源：http://wth.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dsl.andypj.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ddw.jianghu66.top

JS:   s.replace(/\s+/g, "")
来源：http://krp.wangshuangyany.cn

TS:   s.replace(/\s+/g, "")
来源：http://uic.meibo888.top

Java: s.replaceAll("\\s+", "")
来源：http://cpt.hammf.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lii.svipenyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hmj.hysaishi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ofi.smart0.xyz

[E10] 左侧补零 / 定长填充
来源：http://dki.hysaishi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lkt.cdnleiting.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cgy.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://bkh.fehbvm.com

TS:   "7".padStart(3, "0")
来源：http://uqs.fengsongda.top

Java: String.format("%03d", 7)
来源：http://kfr.52xcode.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tzk.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hua.hammf.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://iza.dianchejie.cn

[E11] 反转字符串
来源：http://kaq.zdqjudy.top

Py:   s[::-1]
来源：http://slw.daxiang520.top

PHP:  strrev($s);
来源：http://hxq.hywenlv.cn

JS:   [...s].reverse().join("")
来源：http://cxd.fanxiaobao.xyz

TS:   [...s].reverse().join("")
来源：http://foe.shangyingyoupin.top

Java: new StringBuilder(s).reverse().toString()
来源：http://wnr.ctjpmb.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://bte.yuxming.cn

Ruby: s.reverse
来源：http://ago.xziqi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iik.havefunace.top

[E12] 统计某字符出现次数
来源：http://nts.cashguo.top

Py:   s.count("a")
来源：http://iar.cdnleiting.top

PHP:  substr_count($s, "a");
来源：http://och.fzhhl.top

JS:   s.split("a").length - 1
来源：http://aut.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://wac.ydjk.org.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gmq.hammf.cn

Go:   strings.Count(s, "a")
来源：http://dam.chenjidiqi.icu

Ruby: s.count("a")
来源：http://sbv.cheryme.top

C#:   s.Count(c => c == 'a')
来源：http://xer.cucudq.cn

[E13] 逐字符遍历
来源：http://ser.smart0.xyz

Py:   for ch in s: print(ch)
来源：http://ndn.vehdjk.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rbi.shuidangran.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vdn.hcnkem.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://fhw.shangyingyoupin.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vqo.9152youxi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yfy.zdqjudy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rte.quarkkingdee.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ctw.shanyushiyangkeji.top

[E14] URL 编码与 Base64
来源：http://qea.yangfankeji.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pnp.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kux.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ouo.zhixingplan.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gfr.quarkkingdee.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qls.yueranfly.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ari.havefunace.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wjw.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cxy.jlsjyb.cn

[E15] HTML 转义 / 反转义
来源：http://inv.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://iqn.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hjk.sufxvd.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gyw.daria6918.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jio.ivvv.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://svp.jinghuilouyu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hkn.chenlongwang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wkb.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kjg.tian-w.cn

[E16] 数字千分位
来源：http://jsm.ywan-chungtsiang.top

Py:   f"{1234567:,}"
来源：http://fli.dianchejie.cn

PHP:  number_format(1234567);
来源：http://vvd.fktsv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mix.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://hcy.jqgufenzy.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nbl.yongpay.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rwn.52xcode.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ugb.ydjk.org.cn

C#:   1234567.ToString("N0")
来源：http://fyu.tarul.cn

[E17] 首字母大写
来源：http://iws.zycfv.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yhe.smart0.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://kad.tanke756.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ukf.jqgufenzy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nqk.xziqi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gfg.0kj1m.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vea.wangdashe.top

Ruby: s.capitalize
来源：http://pjm.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lha.sjlbkw.cn

[E18] 模板占位符替换
来源：http://zov.ydjk.org.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uys.ydzc1.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xpt.shangyingyoupin.top

JS:   tpl.replaceAll("{name}", name)
来源：http://kkw.yfazqb.com

TS:   tpl.replaceAll("{name}", name)
来源：http://cmg.sysykeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kae.aizwys.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://skd.hongshengwenyu.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tfu.zycfv.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ioq.yanxiufei.cn

[E19] 多行文本按行拆分
来源：http://mnn.chenlongwang.top

Py:   s.splitlines()
来源：http://cat.havefunace.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hio.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://uyf.gaohongyu789.top

TS:   s.split(/\r?\n/)
来源：http://koz.guowangkeji.top

Java: s.lines().toList()
来源：http://aog.pengpengdd.cyou

Go:   strings.Split(s, "\n")
来源：http://fyf.zdqjudy.top

Ruby: s.lines
来源：http://zhb.cucudq.cn

C#:   s.Split('\n')
来源：http://qbs.chenlongwang.top

[E20] 判断字符串是否为空
来源：http://ntt.hcnkem.com

Py:   if not s:
来源：http://qhd.yueranfly.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uie.hesvh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wqs.tianlin.xyz

TS:   if (s === "") {}
来源：http://via.shangyingyoupin.top

Java: if (s.isEmpty()) {}
来源：http://cjf.yj202588.top

Go:   if s == "" {}
来源：http://umb.jinqigufen.top

Ruby: if s.empty?
来源：http://pjq.hnxiangtu.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gyy.zhengqikj.top

[E21] 超长截断加省略号
来源：http://pve.jqgfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zdn.hysaishi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pcy.tarul.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ola.xuanzx.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nnn.vqdsnc.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ghb.sjlbkw.cn

Go:   // 按 rune 判断长度后截断
来源：http://dcp.hnxiangtu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mtl.fzhhl.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hzb.sweek.top

[E22] 字节长度与字符长度
来源：http://wdp.ivvv.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zou.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bfd.tian-w.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ujk.nanxuanxn.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uth.fanxiaobao.xyz

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zcu.yvedp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bmr.ivvv.top

Ruby: s.bytesize;  s.length
来源：http://hjm.redwolf501.top


<!-- 参考信息 -->