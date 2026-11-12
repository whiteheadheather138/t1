代发 wailian999

TS:   [...new Set(arr)]
来源：http://sqm.hesvh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://fex.nwbrower.top

Go:   // 用 map[T]struct{} 手写
来源：http://esn.jinghuilouyu.cn

Ruby: arr.uniq
来源：http://vdp.zhengqikj.top

C#:   list.Distinct().ToList()
来源：http://try.jianghu66.top

[D16] 求和与平均值
来源：http://iee.cqqwz.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fqz.zhijiandao.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cbw.ydjk.org.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://azv.jiagoushi.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pye.yuanzhike.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://obw.cheryme.top

Go:   // 手写循环累加
来源：http://aex.jqgfzy.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nko.meibo888.top

C#:   list.Sum();  list.Average()
来源：http://ehb.jqgufenzy.top

[D17] 最大值与最小值
来源：http://gfu.birdmap.top

Py:   max(arr);  min(arr)
来源：http://vwj.shzxlz.cn

PHP:  max($arr);  min($arr);
来源：http://zuw.yvedp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xty.yj202588.top

TS:   Math.max(...arr);
来源：http://pkj.yj20258888.top

Java: Collections.max(list);  Collections.min(list);
来源：http://nmj.aizwys.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://tft.jyoumei.cn

Ruby: arr.max;  arr.min
来源：http://aza.sufxvd.cn

C#:   list.Max();  list.Min()
来源：http://pud.snrcjt.cn

[D18] 扁平化嵌套数组
来源：http://glo.tian-w.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fws.cashguo.top

PHP:  array_merge(...$nested);
来源：http://mqe.yj202588.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hmg.yj202588.top

TS:   nested.flat();
来源：http://wol.pengpengdd.cyou

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ujd.tarul.cn

Go:   // 手写双层循环
来源：http://rei.hnxiangtu.top

Ruby: nested.flatten
来源：http://umd.shzxlz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kew.zdbjq.cn

[D19] 按字段分组
来源：http://ukn.cdnleiting.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mvz.aizwys.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mjf.xuanzx.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xhb.jqgfzy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://nvn.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ggw.yongpay.top

Go:   // 手写 map[string][]T
来源：http://xkr.svipenyu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qbk.redwolf501.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vui.chenlongwang.top

[D20] 统计每个元素出现次数
来源：http://tnk.zhongyouzk.top

Py:   Counter(arr)
来源：http://jac.havefunace.top

PHP:  array_count_values($arr);
来源：http://fbd.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://luh.shanyushiyangkeji.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rhf.zycfv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vzd.ywan-chungtsiang.top

Go:   // 手写 map[T]int
来源：http://dwk.yongpay.top

Ruby: arr.tally
来源：http://txt.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ktd.ivvv.top

[D21] 判断是否包含某元素
来源：http://oij.zhijiandao.cn

Py:   x in arr
来源：http://esl.ivvv.top

PHP:  in_array($x, $arr, true);
来源：http://awg.kuanghao11.cn

JS:   arr.includes(x)
来源：http://npi.yanxiufei.cn

TS:   arr.includes(x)
来源：http://eet.dashuyun.cn

Java: list.contains(x)
来源：http://bqx.sweek.top

Go:   slices.Contains(arr, x)
来源：http://uxi.vehdjk.com

Ruby: arr.include?(x)
来源：http://pvf.meibo888.top

C#:   list.Contains(x)
来源：http://svm.jinyuanbaomall.cn

[D22] 复制数组（避免共享引用）
来源：http://dtn.fanxiaobao.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dpu.fehbvm.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iot.316326.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jlo.mhx1999.top

TS:   [...arr];
来源：http://zpf.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://baa.xziqi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kvm.chenlongwang.top

Ruby: arr.dup;  arr.clone
来源：http://mub.chenzaomai.com

C#:   new List<int>(list);
来源：http://wxw.yuxming.cn

[D23] reduce 累积计算
来源：http://xbj.yuxming.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://pjz.tian-w.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tkn.gzhubu.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vxn.ydjk.org.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vyq.xziqi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tka.jianghu66.top

Go:   // 手写循环
来源：http://plx.chenlongwang.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yhi.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xfs.bbcook.cn

[D24] 字典 / Map 基本操作
来源：http://lky.0kj1m.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fie.snrcjt.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hra.gotoacloud.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ifh.zhiwuduotai.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mea.0kj1m.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wlm.dashuyun.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://anh.mhx1999.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://doz.sweek.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uay.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://vwm.sysykeji.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://adb.kuanghao11.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mos.smart0.xyz

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mpz.xuanzx.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rvr.havefunace.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dor.birdmap.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pdk.epnwcf.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ueo.yj20258888.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kkr.pycfn.com

[D26] 数组转字符串
来源：http://aoz.jinqigufen.top

Py:   ", ".join(map(str, arr))
来源：http://jpt.gotoacloud.top

PHP:  implode(", ", $arr);
来源：http://mxp.svipenyu.cn

JS:   arr.join(", ")
来源：http://yjb.jinghuilouyu.cn

TS:   arr.join(", ")
来源：http://eah.shanyushiyangtech.top

Java: String.join(", ", list)
来源：http://qih.ydjk.org.cn

Go:   strings.Join(strs, ", ")
来源：http://dyo.quarkkingdee.top

Ruby: arr.join(", ")
来源：http://afj.guowangkeji.top

C#:   string.Join(", ", list)
来源：http://fwx.epnwcf.com

================================================================================
来源：http://vtk.aizwys.cn

E. 字符串处理
来源：http://fgy.cqqwz.cn

================================================================================
来源：http://hut.ctjpmb.com

[E01] 拼接字符串
来源：http://sgd.sufxvd.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://umb.cheryme.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://llw.nanxuanxn.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kws.haohaochexian.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fhd.dashuyun.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nun.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://usc.hnxiangtu.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yrk.nwbrower.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mye.uphjek.com

[E02] 重复字符串
来源：http://rfa.cheryme.top

Py:   "ab" * 3
来源：http://are.jqgfzy.top

PHP:  str_repeat("ab", 3);
来源：http://edx.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://rdj.redwolf501.top

TS:   "ab".repeat(3)
来源：http://svr.zdqjudy.top

Java: "ab".repeat(3)
来源：http://mxt.yanxiufei.cn

Go:   strings.Repeat("ab", 3)
来源：http://psa.gogol.net.cn

Ruby: "ab" * 3
来源：http://luy.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pqc.jiagoushi.top

[E03] 截取子串
来源：http://uah.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ghs.svipenyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://czh.shanyushiyangtech.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gsb.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://qhv.epnwcf.com

Java: s.substring(1, 4)
来源：http://zgl.pycfn.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rfx.hywenlv.cn

Ruby: s[1, 3];  s[1..3]
来源：http://lmg.aibaodan.cn

C#:   s.Substring(1, 3)
来源：http://tuc.gogol.net.cn

[E04] 查找子串位置
来源：http://iml.ehwqpu.com

Py:   s.find("x");  s.index("x")
来源：http://ybz.fanxiaobao.xyz

PHP:  strpos($s, "x");
来源：http://ogt.zdqjudy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rhz.gzhubu.top

TS:   s.indexOf("x")
来源：http://uap.mhx1999.top

Java: s.indexOf("x")
来源：http://sye.yuanzhike.top

Go:   strings.Index(s, "x")
来源：http://wyo.xinyue.icu

Ruby: s.index("x")
来源：http://erz.wangdashe.top

C#:   s.IndexOf("x")
来源：http://fxb.ybcxt.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://bov.yuxming.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nbs.jyoumei.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://orp.bbcook.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://aby.yj20258.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yol.jinghuilouyu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ins.meibo888.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lvo.zhiwuduotai.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wrd.jiagoushi.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lnp.9152youxi.cn

[E06] 替换子串
来源：http://yfv.ydzc1.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hzo.uphjek.com

PHP:  str_replace("a", "b", $s);
来源：http://xqq.andypj.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nbi.yueranfly.top

TS:   s.replaceAll("a", "b")
来源：http://kmx.gaohongyu789.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bas.hywenlv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pij.yanxiufei.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://unt.yonumen.top

C#:   s.Replace("a", "b")
来源：http://hnk.meibo888.top

[E07] 按分隔符拆分
来源：http://hnk.aibaodan.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://tzh.iojbl.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vkk.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://rci.sufxvd.cn

TS:   s.split(",")
来源：http://zor.52xcode.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ujj.jiagoushi.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pse.dianchejie.cn

Ruby: s.split(",");  s.split
来源：http://gub.tanke756.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://avb.yueranfly.top

[E08] 数组按分隔符合并
来源：http://vjv.yj20258.top

Py:   ",".join(items)
来源：http://kad.ybcxt.top

PHP:  implode(",", $items);
来源：http://rgn.52xcode.cn

JS:   items.join(",")
来源：http://jjm.xinyue.icu

TS:   items.join(",")
来源：http://uxi.jyoumei.cn

Java: String.join(",", items)
来源：http://ext.iojbl.cn

Go:   strings.Join(items, ",")
来源：http://ggf.zhaomingkeji.xyz

Ruby: items.join(",")
来源：http://mbx.ydzc1.top

C#:   string.Join(",", items)
来源：http://tcw.yonumen.top

[E09] 去除所有空白字符
来源：http://xrc.svipenyu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zdu.meibo888.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qjf.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://taq.ppjwa.cn

TS:   s.replace(/\s+/g, "")
来源：http://vep.jiagoushi.top

Java: s.replaceAll("\\s+", "")
来源：http://hah.gotoacloud.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xvx.yanxiufei.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jph.sufxvd.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://vrs.0kj1m.cn

[E10] 左侧补零 / 定长填充
来源：http://ezg.andypj.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vlh.c1oappe.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fjw.yongpay.top

JS:   "7".padStart(3, "0")
来源：http://toh.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://uuj.zhijiandao.cn

Java: String.format("%03d", 7)
来源：http://ymi.hammf.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vtx.316326.xyz

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fwv.nwbrower.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hbu.9152youxi.cn

[E11] 反转字符串
来源：http://cug.fanxiaobao.xyz

Py:   s[::-1]
来源：http://wah.sjlbkw.cn

PHP:  strrev($s);
来源：http://lfe.52xcode.cn

JS:   [...s].reverse().join("")
来源：http://kks.hammf.cn

TS:   [...s].reverse().join("")
来源：http://axw.meibo888.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qns.guannengcc.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukc.mhx1999.top

Ruby: s.reverse
来源：http://bwa.wangdashe.top

C#:   new string(s.Reverse().ToArray())
来源：http://ewe.feifeiyinyue.top

[E12] 统计某字符出现次数
来源：http://ajo.chenzaomai.com

Py:   s.count("a")
来源：http://rxf.shzxlz.cn

PHP:  substr_count($s, "a");
来源：http://qoo.zdbjq.cn

JS:   s.split("a").length - 1
来源：http://xxj.tarul.cn

TS:   s.split("a").length - 1
来源：http://bwd.aibaodan.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ipb.jinqigfzy.top

Go:   strings.Count(s, "a")
来源：http://fmc.xylfe.cn

Ruby: s.count("a")
来源：http://bvn.nanxuanxn.top

C#:   s.Count(c => c == 'a')
来源：http://nxn.meibo888.top

[E13] 逐字符遍历
来源：http://wcr.aibaodan.cn

Py:   for ch in s: print(ch)
来源：http://ctr.yangfankeji.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ijj.nwbrower.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://ypg.tian-w.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qwc.gaohongyu789.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wie.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cnv.zhixingplan.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rlo.andypj.xyz

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xxc.yj202588.top

[E14] URL 编码与 Base64
来源：http://xqk.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zcl.smart0.xyz

PHP:  urlencode($s);  base64_encode($s);
来源：http://rod.aibaodan.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dxh.yueranfly.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vdj.jqgufenzy.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kff.nanxuanxn.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gil.zhoulong.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vtr.pycfn.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mij.ehwqpu.com

[E15] HTML 转义 / 反转义
来源：http://jlm.xingfuxueyuan.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://mzf.yongpay.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jfc.fehbvm.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bin.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cbc.wangshuangyany.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://goy.aizwys.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fxb.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://emm.epnwcf.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vjw.jiagoushi.top

[E16] 数字千分位
来源：http://cos.dashuyun.cn

Py:   f"{1234567:,}"
来源：http://hfj.tianlin.xyz

PHP:  number_format(1234567);
来源：http://cgi.hywenlv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://iqq.zhixingplan.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fhy.vehdjk.com

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xrq.redwolf501.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yam.sweek.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nnu.chenzaomai.com

C#:   1234567.ToString("N0")
来源：http://ryi.ydjk.org.cn

[E17] 首字母大写
来源：http://kep.hcnkem.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uhi.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fdf.andypj.xyz

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xci.jianghu66.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://swl.hcnkem.com

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cft.sjlbkw.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://emw.fktsv.cn

Ruby: s.capitalize
来源：http://pgz.hywenlv.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vid.sysykeji.top

[E18] 模板占位符替换
来源：http://bag.hongshengwenyu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xlk.fktsv.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qgu.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dst.jqgfzy.top

TS:   tpl.replaceAll("{name}", name)
来源：http://day.mhx1999.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hyx.hnqzz.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vve.iojbl.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://azz.ehwqpu.com

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://osi.haohaochexian.top

[E19] 多行文本按行拆分
来源：http://ynd.chenlongwang.top

Py:   s.splitlines()
来源：http://mmo.chenlongwang.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pat.fktsv.cn

JS:   s.split(/\r?\n/)
来源：http://wip.hnqzz.top

TS:   s.split(/\r?\n/)
来源：http://kly.havefunace.top

Java: s.lines().toList()
来源：http://ibn.hywenlv.cn

Go:   strings.Split(s, "\n")
来源：http://cmz.uphjek.com

Ruby: s.lines
来源：http://xiy.gotoacloud.top

C#:   s.Split('\n')
来源：http://dqj.chenzaomai.com

[E20] 判断字符串是否为空
来源：http://xhm.haohaochexian.top

Py:   if not s:
来源：http://dul.jiagoushi.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hot.hcnkem.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xxb.hfpthk.cn

TS:   if (s === "") {}
来源：http://ekx.tian-w.cn

Java: if (s.isEmpty()) {}
来源：http://xac.pengpengdd.cyou

Go:   if s == "" {}
来源：http://kop.yanxiufei.cn

Ruby: if s.empty?
来源：http://krb.aibaodan.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://amv.zdqjudy.top

[E21] 超长截断加省略号
来源：http://bxb.yuxming.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aug.zhijiandao.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://skh.ppjwa.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gko.ywan-chungtsiang.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jht.redwolf501.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wzc.quarkkingdee.top

Go:   // 按 rune 判断长度后截断
来源：http://aol.dashuyun.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rcn.jinqigufen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dak.yuxming.cn

[E22] 字节长度与字符长度
来源：http://dvh.wangdashe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ees.cdnleiting.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://czq.hywenlv.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gfg.jinqigfzy.top


<!-- 参考信息 -->