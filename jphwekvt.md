代发 wailian999

[D15] 去重
来源：http://wsq.tarul.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bag.fehbvm.com

PHP:  array_unique($arr);
来源：http://ozd.yueranfly.top

JS:   [...new Set(arr)]
来源：http://vpj.c1oappe.top

TS:   [...new Set(arr)]
来源：http://jwk.jianghu66.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zqj.ydzc1.top

Go:   // 用 map[T]struct{} 手写
来源：http://wsu.jlsjyb.cn

Ruby: arr.uniq
来源：http://jxr.vqdsnc.cn

C#:   list.Distinct().ToList()
来源：http://yhd.aibaodan.cn

[D16] 求和与平均值
来源：http://bji.tianlin.xyz

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vec.nanxinkj.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ttl.xuanzx.com

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kqw.cdnleiting.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://adz.shuidangran.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dib.yanxiufei.cn

Go:   // 手写循环累加
来源：http://dmv.xziqi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mez.quarkkingdee.top

C#:   list.Sum();  list.Average()
来源：http://ccy.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://slf.guannengcc.top

Py:   max(arr);  min(arr)
来源：http://yqb.nanxuanxn.top

PHP:  max($arr);  min($arr);
来源：http://jkf.xylfe.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rgo.c1oappe.top

TS:   Math.max(...arr);
来源：http://cxk.9152youxi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://crd.gotoacloud.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mdr.cqqwz.cn

Ruby: arr.max;  arr.min
来源：http://qmq.daxiang520.top

C#:   list.Max();  list.Min()
来源：http://feu.sweek.top

[D18] 扁平化嵌套数组
来源：http://kjr.yanxiufei.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bti.iojbl.cn

PHP:  array_merge(...$nested);
来源：http://dcu.fktsv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gac.ppjwa.cn

TS:   nested.flat();
来源：http://vcu.hcnkem.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tha.hesvh.cn

Go:   // 手写双层循环
来源：http://des.redwolf501.top

Ruby: nested.flatten
来源：http://ciu.zhijiandao.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bzi.birdmap.top

[D19] 按字段分组
来源：http://jxh.zhiwuduotai.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rwj.hesvh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ahw.ppjwa.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://css.ivvv.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://cfq.zhongyouzk.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tgz.meibo888.top

Go:   // 手写 map[string][]T
来源：http://pup.yj202588.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://vlx.hysaishi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://akt.gzhubu.top

[D20] 统计每个元素出现次数
来源：http://rgu.cqqwz.cn

Py:   Counter(arr)
来源：http://ded.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://ytp.xingfuxueyuan.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://beq.jinqigfzy.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://flr.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uza.fehbvm.com

Go:   // 手写 map[T]int
来源：http://mld.daria6918.cn

Ruby: arr.tally
来源：http://pim.bbcook.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tfv.ctjpmb.com

[D21] 判断是否包含某元素
来源：http://kfg.sweek.top

Py:   x in arr
来源：http://ijm.sxryk.cn

PHP:  in_array($x, $arr, true);
来源：http://vwt.aizwys.cn

JS:   arr.includes(x)
来源：http://xow.ppjwa.cn

TS:   arr.includes(x)
来源：http://dtq.havefunace.top

Java: list.contains(x)
来源：http://kvi.shzxlz.cn

Go:   slices.Contains(arr, x)
来源：http://blf.haohaochexian.top

Ruby: arr.include?(x)
来源：http://xgl.9152youxi.cn

C#:   list.Contains(x)
来源：http://lut.jqgufenzy.top

[D22] 复制数组（避免共享引用）
来源：http://irs.havefunace.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qyi.ydzc1.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nyt.cashguo.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eka.zhongyouzk.top

TS:   [...arr];
来源：http://xbv.zdqjudy.top

Java: new ArrayList<>(list);
来源：http://eia.xylfe.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sry.yvedp.cn

Ruby: arr.dup;  arr.clone
来源：http://gqc.havefunace.top

C#:   new List<int>(list);
来源：http://ntt.ehwqpu.com

[D23] reduce 累积计算
来源：http://mlt.xingfuxueyuan.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wns.jinqigfzy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ufi.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lwm.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qrs.zhengqikj.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tir.svipenyu.cn

Go:   // 手写循环
来源：http://rmw.hongshengwenyu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uax.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tdc.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://jql.uphjek.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jzy.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lbh.smart0.xyz

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://khr.sjlbkw.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ecl.snrcjt.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kru.svipenyu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://haj.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lrv.zdqjudy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://icc.cashguo.top

[D25] Set 集合去重与交并差
来源：http://szq.pengpengdd.cyou

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bno.guannengcc.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jit.tarul.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gdv.gaohongyu789.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lhw.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kcl.xziqi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xvf.zhongyouzk.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://flx.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ntg.kuanghao11.cn

[D26] 数组转字符串
来源：http://pja.nwbrower.top

Py:   ", ".join(map(str, arr))
来源：http://hfo.ybcxt.top

PHP:  implode(", ", $arr);
来源：http://wes.ybcxt.top

JS:   arr.join(", ")
来源：http://zsj.shzxlz.cn

TS:   arr.join(", ")
来源：http://iql.quarkkingdee.top

Java: String.join(", ", list)
来源：http://bff.smart0.xyz

Go:   strings.Join(strs, ", ")
来源：http://ird.birdmap.top

Ruby: arr.join(", ")
来源：http://ood.aibaodan.cn

C#:   string.Join(", ", list)
来源：http://rzb.yanxiufei.cn

================================================================================
来源：http://uvl.9152youxi.cn

E. 字符串处理
来源：http://soc.snrcjt.cn

================================================================================
来源：http://avf.gogol.net.cn

[E01] 拼接字符串
来源：http://kgz.ybcxt.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yjc.nanxinkj.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cpn.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ccz.jianghu66.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://skz.hcnkem.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xss.dashuyun.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xvv.nanxinkj.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qph.jqgufenzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://seq.quarkkingdee.top

[E02] 重复字符串
来源：http://gfs.hysaishi.cn

Py:   "ab" * 3
来源：http://pxl.fktsv.cn

PHP:  str_repeat("ab", 3);
来源：http://prj.zhoulong.xyz

JS:   "ab".repeat(3)
来源：http://hws.hfpthk.cn

TS:   "ab".repeat(3)
来源：http://ost.ydzc1.top

Java: "ab".repeat(3)
来源：http://vdg.gzhubu.top

Go:   strings.Repeat("ab", 3)
来源：http://tnz.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://bhw.yueranfly.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://moo.tanke756.top

[E03] 截取子串
来源：http://yng.zhoulong.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hyq.zhaomingkeji.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://eym.jinyuanbaomall.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vhg.hnxiangtu.top

TS:   s.slice(1, 4)
来源：http://ggj.tian-w.cn

Java: s.substring(1, 4)
来源：http://hdy.jinqigufen.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rmf.yangfankeji.com

Ruby: s[1, 3];  s[1..3]
来源：http://bns.jiagoushi.top

C#:   s.Substring(1, 3)
来源：http://ykb.meibo888.top

[E04] 查找子串位置
来源：http://rrh.havefunace.top

Py:   s.find("x");  s.index("x")
来源：http://plq.quarkkingdee.top

PHP:  strpos($s, "x");
来源：http://vwh.zhiwuduotai.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://osq.zhongyouzk.top

TS:   s.indexOf("x")
来源：http://ark.jlsjyb.cn

Java: s.indexOf("x")
来源：http://dit.yfazqb.com

Go:   strings.Index(s, "x")
来源：http://bxi.ivvv.top

Ruby: s.index("x")
来源：http://jla.shzxlz.cn

C#:   s.IndexOf("x")
来源：http://itl.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ynn.zhiwuduotai.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uth.shanyushiyangkeji.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kjn.zhijiandao.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppq.svipenyu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://trr.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cbh.zhixingplan.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uzo.jinqigfzy.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zqo.zhoulong.xyz

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mdz.ctjpmb.com

[E06] 替换子串
来源：http://voi.tarul.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://skw.cheryme.top

PHP:  str_replace("a", "b", $s);
来源：http://uzg.epnwcf.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dwz.redwolf501.top

TS:   s.replaceAll("a", "b")
来源：http://kgc.jinqigufen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wey.guannengcc.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yvg.ydjk.org.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tmu.jyoumei.cn

C#:   s.Replace("a", "b")
来源：http://iyk.chenzaomai.com

[E07] 按分隔符拆分
来源：http://qsi.zdqjudy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ezu.jianghu66.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wsh.tian-w.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fbp.hesvh.cn

TS:   s.split(",")
来源：http://hhw.shanyushiyangtech.top

Java: s.split(",");  s.split("\\s+")
来源：http://auh.hfpthk.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://eov.daria6918.cn

Ruby: s.split(",");  s.split
来源：http://vzo.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nfk.uphjek.com

[E08] 数组按分隔符合并
来源：http://mks.yangfankeji.com

Py:   ",".join(items)
来源：http://wfj.wangshuangyany.cn

PHP:  implode(",", $items);
来源：http://pbr.yj20258888.top

JS:   items.join(",")
来源：http://uel.xingfuxueyuan.xyz

TS:   items.join(",")
来源：http://gny.wangshuangyany.cn

Java: String.join(",", items)
来源：http://xhz.cheryme.top

Go:   strings.Join(items, ",")
来源：http://ncz.zhongyouzk.top

Ruby: items.join(",")
来源：http://kde.fehbvm.com

C#:   string.Join(",", items)
来源：http://sog.svipenyu.cn

[E09] 去除所有空白字符
来源：http://zjt.hnxiangtu.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://juf.jiagoushi.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://szm.feifeiyinyue.top

JS:   s.replace(/\s+/g, "")
来源：http://sge.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://xuu.shanyushiyangkeji.top

Java: s.replaceAll("\\s+", "")
来源：http://uqf.vqdsnc.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jqk.jinghuilouyu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uvf.bbcook.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://plc.shanyushiyangkeji.top

[E10] 左侧补零 / 定长填充
来源：http://zne.shuidangran.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ige.9152youxi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yur.yj20258.top

JS:   "7".padStart(3, "0")
来源：http://dcg.pengpengdd.cyou

TS:   "7".padStart(3, "0")
来源：http://cth.zhoulong.xyz

Java: String.format("%03d", 7)
来源：http://pxn.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://qwr.shanyushiyangkeji.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lbp.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wkj.xinyue.icu

[E11] 反转字符串
来源：http://qqt.zdbjq.cn

Py:   s[::-1]
来源：http://tih.sweek.top

PHP:  strrev($s);
来源：http://bst.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://drw.gzhubu.top

TS:   [...s].reverse().join("")
来源：http://jlw.iojbl.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kdj.fktsv.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sbb.ppjwa.cn

Ruby: s.reverse
来源：http://ags.sxryk.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xfg.fzhhl.top

[E12] 统计某字符出现次数
来源：http://kjd.fanxiaobao.xyz

Py:   s.count("a")
来源：http://zgc.hammf.cn

PHP:  substr_count($s, "a");
来源：http://pvb.fktsv.cn

JS:   s.split("a").length - 1
来源：http://xeq.xuanzx.com

TS:   s.split("a").length - 1
来源：http://erk.hcnkem.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gjr.fengsongda.top

Go:   strings.Count(s, "a")
来源：http://jjz.zdbjq.cn

Ruby: s.count("a")
来源：http://hqq.jiagoushi.top

C#:   s.Count(c => c == 'a')
来源：http://aix.yanxiufei.cn

[E13] 逐字符遍历
来源：http://uhx.hnqzz.top

Py:   for ch in s: print(ch)
来源：http://jde.fehbvm.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ebl.xuetiantiany.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yds.yvedp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hec.zdbjq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gxc.ctjpmb.com

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rta.hesvh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kwy.jqgufenzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wlf.chenlongwang.top

[E14] URL 编码与 Base64
来源：http://ksi.tarul.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ijl.jqgufenzy.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://jru.tian-w.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fbg.hnxiangtu.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fkv.xylfe.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ocn.wangdashe.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iue.sysykeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oqi.hesvh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qes.xuanzx.com

[E15] HTML 转义 / 反转义
来源：http://sug.tanke756.top

Py:   html.escape(s);  html.unescape(s)
来源：http://wfg.jinqigufen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cow.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nkl.wangshuangyany.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://snh.ydjk.org.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vjg.birdmap.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://siv.ywan-chungtsiang.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pni.yvedp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://epd.cdnleiting.top

[E16] 数字千分位
来源：http://olm.yj202588.top

Py:   f"{1234567:,}"
来源：http://ppa.chenlongwang.top

PHP:  number_format(1234567);
来源：http://gmf.zycfv.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wyj.yanxiufei.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qcf.smart0.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dln.hnqzz.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bti.yuxming.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://szv.jqgfzy.top

C#:   1234567.ToString("N0")
来源：http://fsc.pengpengdd.cyou

[E17] 首字母大写
来源：http://eqp.iojbl.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rhu.jinyuanbaomall.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://aqk.hongshengwenyu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xka.havefunace.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fts.pengpengdd.cyou

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qvm.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tye.jqgfzy.top

Ruby: s.capitalize
来源：http://nby.aibaodan.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mww.xylfe.cn

[E18] 模板占位符替换
来源：http://gwg.iojbl.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tue.jinqigufen.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://erc.zycfv.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ayu.tian-w.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wii.xinyue.icu

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aej.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vxu.c1oappe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tqr.tianlin.xyz

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fmh.epnwcf.com

[E19] 多行文本按行拆分
来源：http://oty.shuidangran.top

Py:   s.splitlines()
来源：http://qss.cucudq.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pll.dianchejie.cn

JS:   s.split(/\r?\n/)
来源：http://wce.epnwcf.com

TS:   s.split(/\r?\n/)
来源：http://bow.yuxming.cn

Java: s.lines().toList()
来源：http://xoj.gogol.net.cn

Go:   strings.Split(s, "\n")
来源：http://xlq.kuanghao11.cn

Ruby: s.lines
来源：http://lzv.zycfv.cn

C#:   s.Split('\n')
来源：http://gbf.guannengcc.top

[E20] 判断字符串是否为空
来源：http://yzu.smart0.xyz

Py:   if not s:
来源：http://mlb.shanyushiyangtech.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wne.iojbl.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qwg.yongpay.top

TS:   if (s === "") {}
来源：http://fxd.hysaishi.cn

Java: if (s.isEmpty()) {}
来源：http://vvn.yj20258888.top

Go:   if s == "" {}
来源：http://uwt.chenzaomai.com

Ruby: if s.empty?
来源：http://odk.c1oappe.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vuq.ydjk.org.cn

[E21] 超长截断加省略号
来源：http://sfq.yvedp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://erb.jinqigfzy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ctr.zhongyouzk.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cqh.shuidangran.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wjo.chenzaomai.com

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://izo.dashuyun.cn

Go:   // 按 rune 判断长度后截断
来源：http://ydc.gaohongyu789.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pxg.c1oappe.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://drn.hfpthk.cn


<!-- 参考信息 -->