代发 wailian999

C#:   list.Distinct().ToList()
来源：http://kqi.zhijiandao.cn

[D16] 求和与平均值
来源：http://oha.yj20258888.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mge.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lhw.sweek.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vzn.feifeiyinyue.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ben.zdqjudy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gpy.zhongyouzk.top

Go:   // 手写循环累加
来源：http://bqi.xingfuxueyuan.xyz

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ohl.yonumen.top

C#:   list.Sum();  list.Average()
来源：http://fzs.aibaodan.cn

[D17] 最大值与最小值
来源：http://uzm.kuanghao11.cn

Py:   max(arr);  min(arr)
来源：http://vph.fanxiaobao.xyz

PHP:  max($arr);  min($arr);
来源：http://tax.havefunace.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qnt.tianlin.xyz

TS:   Math.max(...arr);
来源：http://tmy.gogol.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zmj.tanke756.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://all.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://qyd.fanxiaobao.xyz

C#:   list.Max();  list.Min()
来源：http://oju.quarkkingdee.top

[D18] 扁平化嵌套数组
来源：http://dof.nanxinkj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hir.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://tao.tianlin.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pfg.xinyue.icu

TS:   nested.flat();
来源：http://bri.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://bsu.meibo888.top

Go:   // 手写双层循环
来源：http://avw.jyoumei.cn

Ruby: nested.flatten
来源：http://wcy.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://vxo.nwbrower.top

[D19] 按字段分组
来源：http://ahl.jinghuilouyu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://euw.yj20258.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qmx.birdmap.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ull.yuanzhike.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://ttr.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tph.zhiwuduotai.top

Go:   // 手写 map[string][]T
来源：http://pxg.zhijiandao.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uqb.svipenyu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pru.jlsjyb.cn

[D20] 统计每个元素出现次数
来源：http://qfh.nwbrower.top

Py:   Counter(arr)
来源：http://grm.cheryme.top

PHP:  array_count_values($arr);
来源：http://tki.cashguo.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wgk.nanxinkj.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mgx.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rai.daria6918.cn

Go:   // 手写 map[T]int
来源：http://lcm.fengsongda.top

Ruby: arr.tally
来源：http://ziv.hongshengwenyu.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jau.gogol.net.cn

[D21] 判断是否包含某元素
来源：http://drr.tian-w.cn

Py:   x in arr
来源：http://uqi.zycfv.cn

PHP:  in_array($x, $arr, true);
来源：http://crn.zhongyouzk.top

JS:   arr.includes(x)
来源：http://bye.wangdashe.top

TS:   arr.includes(x)
来源：http://ymz.ydzc1.top

Java: list.contains(x)
来源：http://sbo.xingfuxueyuan.xyz

Go:   slices.Contains(arr, x)
来源：http://svp.sjlbkw.cn

Ruby: arr.include?(x)
来源：http://kzd.shuidangran.top

C#:   list.Contains(x)
来源：http://wja.dianchejie.cn

[D22] 复制数组（避免共享引用）
来源：http://blw.cucudq.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jfx.tianlin.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fcv.meibo888.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://tqt.yuanzhike.top

TS:   [...arr];
来源：http://tvr.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://hix.epnwcf.com

Go:   copied := append([]int(nil), arr...)
来源：http://peh.sysykeji.top

Ruby: arr.dup;  arr.clone
来源：http://hkz.guowangkeji.top

C#:   new List<int>(list);
来源：http://lmb.redwolf501.top

[D23] reduce 累积计算
来源：http://sgt.zhiwuduotai.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xak.ctjpmb.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rer.9152youxi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://buz.andypj.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vzr.jinyuanbaomall.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jqo.guowangkeji.top

Go:   // 手写循环
来源：http://vzg.hesvh.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mri.snrcjt.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eqt.cdnleiting.top

[D24] 字典 / Map 基本操作
来源：http://mxm.yj20258.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://llp.cashguo.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qup.hcnkem.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ytv.shzxlz.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dpm.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hxu.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wqd.wangdashe.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iqf.shanyushiyangkeji.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://clm.zhiwuduotai.top

[D25] Set 集合去重与交并差
来源：http://iae.ehwqpu.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xdz.zhijiandao.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://svk.xylfe.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vyo.quarkkingdee.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yji.ydzc1.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hoh.jinghuilouyu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://irr.shanyushiyangkeji.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uzl.cqqwz.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vkw.kuanghao11.cn

[D26] 数组转字符串
来源：http://tgj.chenzaomai.com

Py:   ", ".join(map(str, arr))
来源：http://yhl.cheryme.top

PHP:  implode(", ", $arr);
来源：http://ymi.yueranfly.top

JS:   arr.join(", ")
来源：http://dsm.nwbrower.top

TS:   arr.join(", ")
来源：http://wwm.nanxuanxn.top

Java: String.join(", ", list)
来源：http://ple.hnqzz.top

Go:   strings.Join(strs, ", ")
来源：http://krv.yj20258.top

Ruby: arr.join(", ")
来源：http://dti.yuanzhike.top

C#:   string.Join(", ", list)
来源：http://xar.tanke756.top

================================================================================
来源：http://egr.sweek.top

E. 字符串处理
来源：http://xoi.zhiwuduotai.top

================================================================================
来源：http://odx.sysykeji.top

[E01] 拼接字符串
来源：http://vgn.hnxiangtu.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://coi.bbcook.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://owa.bbcook.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uqf.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rtu.yuxming.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vau.aibaodan.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jpi.chenlongwang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hjz.epnwcf.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hfo.shzxlz.cn

[E02] 重复字符串
来源：http://ocy.shuidangran.top

Py:   "ab" * 3
来源：http://ikj.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://hix.snrcjt.cn

JS:   "ab".repeat(3)
来源：http://qqe.shzxlz.cn

TS:   "ab".repeat(3)
来源：http://icm.0kj1m.cn

Java: "ab".repeat(3)
来源：http://ati.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://qgv.sysykeji.top

Ruby: "ab" * 3
来源：http://ljm.zycfv.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://egm.jianghu66.top

[E03] 截取子串
来源：http://iph.shanyushiyangkeji.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vvh.0kj1m.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wof.shzxlz.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tjj.xingfuxueyuan.xyz

TS:   s.slice(1, 4)
来源：http://vef.ehwqpu.com

Java: s.substring(1, 4)
来源：http://mni.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uuh.fehbvm.com

Ruby: s[1, 3];  s[1..3]
来源：http://djx.dashuyun.cn

C#:   s.Substring(1, 3)
来源：http://ddl.tianlin.xyz

[E04] 查找子串位置
来源：http://ehj.gotoacloud.top

Py:   s.find("x");  s.index("x")
来源：http://epd.cucudq.cn

PHP:  strpos($s, "x");
来源：http://ieq.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jrx.jinqigufen.top

TS:   s.indexOf("x")
来源：http://uub.zycfv.cn

Java: s.indexOf("x")
来源：http://jod.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://zqq.sxryk.cn

Ruby: s.index("x")
来源：http://zgz.daria6918.cn

C#:   s.IndexOf("x")
来源：http://kty.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://mtx.yangfankeji.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cqy.jinqigfzy.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fla.dianchejie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gjh.shangyingyoupin.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mmr.yuanzhike.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hto.redwolf501.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://byr.hongshengwenyu.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pem.shangyingyoupin.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ahv.fktsv.cn

[E06] 替换子串
来源：http://jez.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vzq.sjlbkw.cn

PHP:  str_replace("a", "b", $s);
来源：http://pmx.chenjidiqi.icu

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kns.sufxvd.cn

TS:   s.replaceAll("a", "b")
来源：http://ijv.hywenlv.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gba.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iid.xuetiantiany.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rro.wangshuangyany.cn

C#:   s.Replace("a", "b")
来源：http://cwk.hongshengwenyu.top

[E07] 按分隔符拆分
来源：http://qul.jinqigfzy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cyb.xylfe.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://aau.chenzaomai.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://zwr.havefunace.top

TS:   s.split(",")
来源：http://ofx.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://lbl.316326.xyz

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qzd.fengsongda.top

Ruby: s.split(",");  s.split
来源：http://emv.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gxb.sysykeji.top

[E08] 数组按分隔符合并
来源：http://ytw.daria6918.cn

Py:   ",".join(items)
来源：http://jrp.dianchejie.cn

PHP:  implode(",", $items);
来源：http://hzh.cashguo.top

JS:   items.join(",")
来源：http://zqu.ydjk.org.cn

TS:   items.join(",")
来源：http://fun.tian-w.cn

Java: String.join(",", items)
来源：http://bwi.dashuyun.cn

Go:   strings.Join(items, ",")
来源：http://uzj.jyoumei.cn

Ruby: items.join(",")
来源：http://mqg.guowangkeji.top

C#:   string.Join(",", items)
来源：http://ble.shanyushiyangkeji.top

[E09] 去除所有空白字符
来源：http://aht.cucudq.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vjq.shanyushiyangkeji.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blp.zhijiandao.cn

JS:   s.replace(/\s+/g, "")
来源：http://ooy.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://ver.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://okm.zhengqikj.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://dpl.quarkkingdee.top

Ruby: s.gsub(/\s+/, "")
来源：http://tve.pycfn.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xhg.ydjk.org.cn

[E10] 左侧补零 / 定长填充
来源：http://noy.yonumen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wvk.sxryk.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://owl.ivvv.top

JS:   "7".padStart(3, "0")
来源：http://arl.chenlongwang.top

TS:   "7".padStart(3, "0")
来源：http://shk.zhengqikj.top

Java: String.format("%03d", 7)
来源：http://jbq.vehdjk.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://hlh.epnwcf.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wsy.cashguo.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sjp.fengsongda.top

[E11] 反转字符串
来源：http://cjt.hnqzz.top

Py:   s[::-1]
来源：http://pke.bbcook.cn

PHP:  strrev($s);
来源：http://qke.wangshuangyany.cn

JS:   [...s].reverse().join("")
来源：http://bii.andypj.xyz

TS:   [...s].reverse().join("")
来源：http://wkm.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ezz.yj20258.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ost.yfazqb.com

Ruby: s.reverse
来源：http://efg.xuanzx.com

C#:   new string(s.Reverse().ToArray())
来源：http://chy.jlsjyb.cn

[E12] 统计某字符出现次数
来源：http://qpy.c1oappe.top

Py:   s.count("a")
来源：http://zbw.gaohongyu789.top

PHP:  substr_count($s, "a");
来源：http://iva.tianlin.xyz

JS:   s.split("a").length - 1
来源：http://tim.xuetiantiany.cn

TS:   s.split("a").length - 1
来源：http://mzb.guannengcc.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lok.uphjek.com

Go:   strings.Count(s, "a")
来源：http://xxo.yvedp.cn

Ruby: s.count("a")
来源：http://kxj.tianlin.xyz

C#:   s.Count(c => c == 'a')
来源：http://xpf.hysaishi.cn

[E13] 逐字符遍历
来源：http://fvj.zhoulong.xyz

Py:   for ch in s: print(ch)
来源：http://sck.svipenyu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://spk.jinghuilouyu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fjr.pengpengdd.cyou

TS:   for (const ch of s) { console.log(ch); }
来源：http://kwo.xingfuxueyuan.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yyw.tian-w.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://qxn.daxiang520.top

Ruby: s.each_char { |ch| puts ch }
来源：http://kvr.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cav.zhaomingkeji.xyz

[E14] URL 编码与 Base64
来源：http://hgf.hnqzz.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jkx.sjlbkw.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vjh.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nal.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rtm.shanyushiyangkeji.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uek.cqqwz.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://kno.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wpl.jiagoushi.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ocz.jiagoushi.top

[E15] HTML 转义 / 反转义
来源：http://jlw.yueranfly.top

Py:   html.escape(s);  html.unescape(s)
来源：http://owx.zhengqikj.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vdz.wangdashe.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dad.xziqi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yrp.hnxiangtu.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hlj.ywan-chungtsiang.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://drj.sufxvd.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ldy.c1oappe.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eim.chenzaomai.com

[E16] 数字千分位
来源：http://pcb.hnqzz.top

Py:   f"{1234567:,}"
来源：http://ouz.redwolf501.top

PHP:  number_format(1234567);
来源：http://ykp.yuxming.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yla.sjlbkw.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bpv.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eoo.xuanzx.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mkp.xylfe.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vjz.cdnleiting.top

C#:   1234567.ToString("N0")
来源：http://gvr.jinghuilouyu.cn

[E17] 首字母大写
来源：http://mch.havefunace.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dpb.tarul.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dwm.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://doi.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zbr.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jll.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qtk.jianghu66.top

Ruby: s.capitalize
来源：http://itz.fzhhl.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blr.snrcjt.cn

[E18] 模板占位符替换
来源：http://gkz.316326.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vhu.hfpthk.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gwr.jyoumei.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wgv.zycfv.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dbe.daria6918.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ntc.cheryme.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rjx.shanyushiyangtech.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gkg.guowangkeji.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ads.shuidangran.top

[E19] 多行文本按行拆分
来源：http://txn.hnqzz.top

Py:   s.splitlines()
来源：http://bzj.xingfuxueyuan.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://crr.sysykeji.top

JS:   s.split(/\r?\n/)
来源：http://bjf.yvedp.cn

TS:   s.split(/\r?\n/)
来源：http://vyc.quarkkingdee.top

Java: s.lines().toList()
来源：http://kuk.zhengqikj.top

Go:   strings.Split(s, "\n")
来源：http://bjy.gotoacloud.top

Ruby: s.lines
来源：http://ost.sxryk.cn

C#:   s.Split('\n')
来源：http://ngg.zycfv.cn

[E20] 判断字符串是否为空
来源：http://wjs.xziqi.cn

Py:   if not s:
来源：http://pgk.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pzs.yvedp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://btd.fzhhl.top

TS:   if (s === "") {}
来源：http://yow.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://wwy.daxiang520.top

Go:   if s == "" {}
来源：http://hxs.snrcjt.cn

Ruby: if s.empty?
来源：http://uvf.chenjidiqi.icu

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ons.ybcxt.top

[E21] 超长截断加省略号
来源：http://nvu.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bnl.daxiang520.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://xmt.hfpthk.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eqm.gaohongyu789.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iic.quarkkingdee.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://riv.nwbrower.top

Go:   // 按 rune 判断长度后截断
来源：http://pod.yongpay.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xnj.gaohongyu789.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dox.nwbrower.top

[E22] 字节长度与字符长度
来源：http://oio.ydjk.org.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jpa.feifeiyinyue.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gbc.vqdsnc.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://saq.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zsh.vehdjk.com

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hfd.jinghuilouyu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wzx.bbcook.cn

Ruby: s.bytesize;  s.length
来源：http://gys.zhiwuduotai.top


<!-- 参考信息 -->