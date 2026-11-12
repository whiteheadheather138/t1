代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://oti.zycfv.cn

Go:   // 手写循环
来源：http://unk.tianlin.xyz

Ruby: arr.map { |x| x * 2 }
来源：http://kvx.shanyushiyangkeji.top

C#:   list.Select(x => x * 2).ToList()
来源：http://puk.sweek.top

[D15] 去重
来源：http://uuk.hywenlv.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tmk.tarul.cn

PHP:  array_unique($arr);
来源：http://gqz.fzhhl.top

JS:   [...new Set(arr)]
来源：http://kal.xziqi.cn

TS:   [...new Set(arr)]
来源：http://epd.ybcxt.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://toy.cqqwz.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nsz.nwbrower.top

Ruby: arr.uniq
来源：http://bem.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://jnb.svipenyu.cn

[D16] 求和与平均值
来源：http://zds.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://did.hongshengwenyu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gzo.hysaishi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gfe.xingfuxueyuan.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bvh.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bxg.chenjidiqi.icu

Go:   // 手写循环累加
来源：http://qmo.tian-w.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sqs.haohaochexian.top

C#:   list.Sum();  list.Average()
来源：http://hhf.jlsjyb.cn

[D17] 最大值与最小值
来源：http://fgt.0kj1m.cn

Py:   max(arr);  min(arr)
来源：http://gkr.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://mlg.xuanzx.com

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eha.dashuyun.cn

TS:   Math.max(...arr);
来源：http://fcn.bbcook.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://asx.yj20258.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ljx.xingfuxueyuan.xyz

Ruby: arr.max;  arr.min
来源：http://gst.fehbvm.com

C#:   list.Max();  list.Min()
来源：http://fzs.yangfankeji.com

[D18] 扁平化嵌套数组
来源：http://wvm.shanyushiyangtech.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zeo.quarkkingdee.top

PHP:  array_merge(...$nested);
来源：http://usm.iojbl.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zvs.yangfankeji.com

TS:   nested.flat();
来源：http://bmt.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://clb.hywenlv.cn

Go:   // 手写双层循环
来源：http://nnp.pengpengdd.cyou

Ruby: nested.flatten
来源：http://fdv.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://oeq.pycfn.com

[D19] 按字段分组
来源：http://kcq.shanyushiyangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pgj.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qzd.sweek.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hmr.yj202588.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://znp.birdmap.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rzq.yonumen.top

Go:   // 手写 map[string][]T
来源：http://gmo.sxryk.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cut.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xnj.uphjek.com

[D20] 统计每个元素出现次数
来源：http://cba.aizwys.cn

Py:   Counter(arr)
来源：http://gao.birdmap.top

PHP:  array_count_values($arr);
来源：http://fkj.chenjidiqi.icu

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ltk.havefunace.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xim.jqgufenzy.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bql.daria6918.cn

Go:   // 手写 map[T]int
来源：http://bmu.ctjpmb.com

Ruby: arr.tally
来源：http://odx.zhijiandao.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://req.bjfxy.top

[D21] 判断是否包含某元素
来源：http://ost.ydzc1.top

Py:   x in arr
来源：http://ago.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://cvw.xingfuxueyuan.xyz

JS:   arr.includes(x)
来源：http://kpe.jinqigufen.top

TS:   arr.includes(x)
来源：http://mjc.cheryme.top

Java: list.contains(x)
来源：http://zmf.xuanzx.com

Go:   slices.Contains(arr, x)
来源：http://izn.cheryme.top

Ruby: arr.include?(x)
来源：http://wva.yueranfly.top

C#:   list.Contains(x)
来源：http://dik.yfazqb.com

[D22] 复制数组（避免共享引用）
来源：http://sxr.gotoacloud.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dvf.yj20258888.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fya.nwbrower.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://inv.chenjidiqi.icu

TS:   [...arr];
来源：http://qhf.yuxming.cn

Java: new ArrayList<>(list);
来源：http://mbi.sysykeji.top

Go:   copied := append([]int(nil), arr...)
来源：http://mzl.gaohongyu789.top

Ruby: arr.dup;  arr.clone
来源：http://dwe.yonumen.top

C#:   new List<int>(list);
来源：http://hvf.yuanzhike.top

[D23] reduce 累积计算
来源：http://olp.sufxvd.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dfo.vqdsnc.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wni.ehwqpu.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wcm.sxryk.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lro.ywan-chungtsiang.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://qcc.pycfn.com

Go:   // 手写循环
来源：http://kxj.jianghu66.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gnv.0kj1m.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://axg.yonumen.top

[D24] 字典 / Map 基本操作
来源：http://vue.316326.xyz

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kxd.ydjk.org.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gmw.316326.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fcr.nwbrower.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ckj.fengsongda.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xhm.pengpengdd.cyou

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://chf.gzhubu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ytt.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://zcg.zdbjq.cn

[D25] Set 集合去重与交并差
来源：http://rpy.daria6918.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tvf.hnqzz.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xhs.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wgl.sufxvd.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://unr.zhengqikj.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hjr.xingfuxueyuan.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hpp.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tyx.tanke756.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nga.iojbl.cn

[D26] 数组转字符串
来源：http://ajv.hammf.cn

Py:   ", ".join(map(str, arr))
来源：http://uky.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://qix.wangshuangyany.cn

JS:   arr.join(", ")
来源：http://tfg.aibaodan.cn

TS:   arr.join(", ")
来源：http://maj.xziqi.cn

Java: String.join(", ", list)
来源：http://kih.nanxuanxn.top

Go:   strings.Join(strs, ", ")
来源：http://uix.haohaochexian.top

Ruby: arr.join(", ")
来源：http://lsz.havefunace.top

C#:   string.Join(", ", list)
来源：http://lam.xylfe.cn

================================================================================
来源：http://zgk.xinyue.icu

E. 字符串处理
来源：http://lwo.guannengcc.top

================================================================================
来源：http://fbf.hesvh.cn

[E01] 拼接字符串
来源：http://npt.pengpengdd.cyou

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lbh.0kj1m.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wym.yangfankeji.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jrm.dashuyun.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://klq.yonumen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://bzq.yuxming.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://abc.jqgufenzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kcx.ydzc1.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qzj.hesvh.cn

[E02] 重复字符串
来源：http://hcf.aibaodan.cn

Py:   "ab" * 3
来源：http://rbf.gzhubu.top

PHP:  str_repeat("ab", 3);
来源：http://twi.hnqzz.top

JS:   "ab".repeat(3)
来源：http://rep.pycfn.com

TS:   "ab".repeat(3)
来源：http://lpq.xinyue.icu

Java: "ab".repeat(3)
来源：http://ooc.guannengcc.top

Go:   strings.Repeat("ab", 3)
来源：http://apy.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://vgw.shangyingyoupin.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://enw.daria6918.cn

[E03] 截取子串
来源：http://ixl.epnwcf.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://uek.aizwys.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cjw.ydzc1.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yhx.jiagoushi.top

TS:   s.slice(1, 4)
来源：http://rqx.yvedp.cn

Java: s.substring(1, 4)
来源：http://ucc.yonumen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://djy.xuanzx.com

Ruby: s[1, 3];  s[1..3]
来源：http://yid.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://mug.yueranfly.top

[E04] 查找子串位置
来源：http://ogo.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://krv.tarul.cn

PHP:  strpos($s, "x");
来源：http://xxy.vqdsnc.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zpn.nwbrower.top

TS:   s.indexOf("x")
来源：http://kxr.ydzc1.top

Java: s.indexOf("x")
来源：http://dao.hywenlv.cn

Go:   strings.Index(s, "x")
来源：http://rhc.chenzaomai.com

Ruby: s.index("x")
来源：http://qwg.cqqwz.cn

C#:   s.IndexOf("x")
来源：http://gud.ctjpmb.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://lni.gaohongyu789.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fng.zhoulong.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pnd.guannengcc.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ilc.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://lwc.vehdjk.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kup.zycfv.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ivl.cdnleiting.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://eyn.fktsv.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sug.dianchejie.cn

[E06] 替换子串
来源：http://cut.yongpay.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mfk.hnqzz.top

PHP:  str_replace("a", "b", $s);
来源：http://npb.hysaishi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://llj.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://qvk.zhixingplan.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sob.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://lvi.zdqjudy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cym.jqgfzy.top

C#:   s.Replace("a", "b")
来源：http://pip.cdnleiting.top

[E07] 按分隔符拆分
来源：http://arp.nanxinkj.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gzu.cucudq.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://okj.gogol.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fzm.bbcook.cn

TS:   s.split(",")
来源：http://ytr.quarkkingdee.top

Java: s.split(",");  s.split("\\s+")
来源：http://zdp.yangfankeji.com

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nmb.sjlbkw.cn

Ruby: s.split(",");  s.split
来源：http://grp.c1oappe.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lim.quarkkingdee.top

[E08] 数组按分隔符合并
来源：http://ggy.fktsv.cn

Py:   ",".join(items)
来源：http://dtk.mhx1999.top

PHP:  implode(",", $items);
来源：http://qrh.pycfn.com

JS:   items.join(",")
来源：http://plp.fzhhl.top

TS:   items.join(",")
来源：http://tqs.xinyue.icu

Java: String.join(",", items)
来源：http://xnc.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://ils.hcnkem.com

Ruby: items.join(",")
来源：http://bgd.sysykeji.top

C#:   string.Join(",", items)
来源：http://hyj.meibo888.top

[E09] 去除所有空白字符
来源：http://ldk.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uff.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://pog.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://sho.sweek.top

TS:   s.replace(/\s+/g, "")
来源：http://kwd.cashguo.top

Java: s.replaceAll("\\s+", "")
来源：http://nqf.ivvv.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://jmb.hysaishi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rvr.chenjidiqi.icu

C#:   Regex.Replace(s, @"\s+", "")
来源：http://guw.cashguo.top

[E10] 左侧补零 / 定长填充
来源：http://lmz.fktsv.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dyk.wangshuangyany.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mjl.haohaochexian.top

JS:   "7".padStart(3, "0")
来源：http://kbf.wangdashe.top

TS:   "7".padStart(3, "0")
来源：http://cfx.zhixingplan.top

Java: String.format("%03d", 7)
来源：http://ihm.epnwcf.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://djf.havefunace.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://efz.jlsjyb.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mil.wangshuangyany.cn

[E11] 反转字符串
来源：http://ojw.daria6918.cn

Py:   s[::-1]
来源：http://xey.gogol.net.cn

PHP:  strrev($s);
来源：http://hqa.0kj1m.cn

JS:   [...s].reverse().join("")
来源：http://qyj.chenjidiqi.icu

TS:   [...s].reverse().join("")
来源：http://qqt.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://his.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://jgu.shanyushiyangtech.top

Ruby: s.reverse
来源：http://qei.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://vlz.shangyingyoupin.top

[E12] 统计某字符出现次数
来源：http://bqm.aizwys.cn

Py:   s.count("a")
来源：http://xle.shuidangran.top

PHP:  substr_count($s, "a");
来源：http://ndo.cqqwz.cn

JS:   s.split("a").length - 1
来源：http://bet.sysykeji.top

TS:   s.split("a").length - 1
来源：http://owa.yongpay.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ozv.gotoacloud.top

Go:   strings.Count(s, "a")
来源：http://zmu.ctjpmb.com

Ruby: s.count("a")
来源：http://bju.wangdashe.top

C#:   s.Count(c => c == 'a')
来源：http://pgk.9152youxi.cn

[E13] 逐字符遍历
来源：http://azl.xinyue.icu

Py:   for ch in s: print(ch)
来源：http://cvh.fzhhl.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://tlr.zhiwuduotai.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://cym.fehbvm.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://xfc.jlsjyb.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hac.jinqigfzy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aft.cheryme.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kky.yj20258888.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cfz.yuxming.cn

[E14] URL 编码与 Base64
来源：http://cax.haohaochexian.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nsh.chenzaomai.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://zbl.jlsjyb.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sfo.jinqigfzy.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dcs.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xza.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nez.cqqwz.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nau.ppjwa.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kst.cdnleiting.top

[E15] HTML 转义 / 反转义
来源：http://cyr.shzxlz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ggr.zhaomingkeji.xyz

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xrv.gaohongyu789.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cwv.fktsv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kpz.zhiwuduotai.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://msr.tarul.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ejk.tianlin.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fkn.gotoacloud.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://knu.tianlin.xyz

[E16] 数字千分位
来源：http://wuo.wangshuangyany.cn

Py:   f"{1234567:,}"
来源：http://rff.gogol.net.cn

PHP:  number_format(1234567);
来源：http://lcm.uphjek.com

JS:   (1234567).toLocaleString("en-US")
来源：http://xhy.hammf.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rrz.zhixingplan.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lmq.yuxming.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ghg.vehdjk.com

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fuy.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://tsw.zhijiandao.cn

[E17] 首字母大写
来源：http://dgr.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gbr.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tye.xuetiantiany.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vhl.shanyushiyangkeji.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ntp.zdqjudy.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wyv.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://eat.yuanzhike.top

Ruby: s.capitalize
来源：http://rof.xuetiantiany.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mqo.zhiwuduotai.top

[E18] 模板占位符替换
来源：http://xle.xinyue.icu

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bkh.fzhhl.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qhj.birdmap.top

JS:   tpl.replaceAll("{name}", name)
来源：http://khn.ppjwa.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dre.feifeiyinyue.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xak.tian-w.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pph.cdnleiting.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ssi.nanxinkj.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://zhr.zhoulong.xyz

[E19] 多行文本按行拆分
来源：http://lzs.jqgfzy.top

Py:   s.splitlines()
来源：http://rjd.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ftm.hcnkem.com

JS:   s.split(/\r?\n/)
来源：http://mxq.sjlbkw.cn

TS:   s.split(/\r?\n/)
来源：http://kxo.fengsongda.top

Java: s.lines().toList()
来源：http://hqd.nwbrower.top

Go:   strings.Split(s, "\n")
来源：http://ybu.bjfxy.top

Ruby: s.lines
来源：http://fui.hammf.cn

C#:   s.Split('\n')
来源：http://rmd.xuanzx.com

[E20] 判断字符串是否为空
来源：http://noa.nanxinkj.top

Py:   if not s:
来源：http://own.ctjpmb.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yzp.jqgufenzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://cdr.yj20258888.top

TS:   if (s === "") {}
来源：http://yym.svipenyu.cn

Java: if (s.isEmpty()) {}
来源：http://ggj.uphjek.com

Go:   if s == "" {}
来源：http://pye.ehwqpu.com

Ruby: if s.empty?
来源：http://mkd.fehbvm.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ymj.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://zay.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xll.xuetiantiany.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oay.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gwu.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pto.zhengqikj.top


<!-- 参考信息 -->