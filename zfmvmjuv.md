代发 wailian999

[D15] 去重
来源：http://zqk.vqdsnc.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bni.bbcook.cn

PHP:  array_unique($arr);
来源：http://gtb.aibaodan.cn

JS:   [...new Set(arr)]
来源：http://jys.fzhhl.top

TS:   [...new Set(arr)]
来源：http://cph.nwbrower.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://awv.jinqigufen.top

Go:   // 用 map[T]struct{} 手写
来源：http://zrg.yfazqb.com

Ruby: arr.uniq
来源：http://idj.yuxming.cn

C#:   list.Distinct().ToList()
来源：http://jdr.yfazqb.com

[D16] 求和与平均值
来源：http://fvl.chenlongwang.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bhz.kuanghao11.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mnf.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fly.zdqjudy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jju.dashuyun.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://elo.yj202588.top

Go:   // 手写循环累加
来源：http://tlp.gaohongyu789.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ziv.hfpthk.cn

C#:   list.Sum();  list.Average()
来源：http://reg.cashguo.top

[D17] 最大值与最小值
来源：http://dsv.pengpengdd.cyou

Py:   max(arr);  min(arr)
来源：http://zed.xziqi.cn

PHP:  max($arr);  min($arr);
来源：http://xys.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tvv.shangyingyoupin.top

TS:   Math.max(...arr);
来源：http://bul.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nwd.ywan-chungtsiang.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zfh.zdbjq.cn

Ruby: arr.max;  arr.min
来源：http://hzm.zycfv.cn

C#:   list.Max();  list.Min()
来源：http://bth.tian-w.cn

[D18] 扁平化嵌套数组
来源：http://mjk.zhengqikj.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iqm.bjfxy.top

PHP:  array_merge(...$nested);
来源：http://qbc.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pyd.jlsjyb.cn

TS:   nested.flat();
来源：http://ipv.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://svu.svipenyu.cn

Go:   // 手写双层循环
来源：http://ehe.haohaochexian.top

Ruby: nested.flatten
来源：http://lhw.chenzaomai.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://ega.andypj.xyz

[D19] 按字段分组
来源：http://wew.vqdsnc.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ocn.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zxl.iojbl.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uqr.tanke756.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lok.sjlbkw.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hki.hongshengwenyu.top

Go:   // 手写 map[string][]T
来源：http://ner.iojbl.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ulp.yj20258888.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qan.jqgufenzy.top

[D20] 统计每个元素出现次数
来源：http://zva.yanxiufei.cn

Py:   Counter(arr)
来源：http://ocg.jianghu66.top

PHP:  array_count_values($arr);
来源：http://xyo.zhoulong.xyz

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zdo.jinghuilouyu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hdz.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sef.iojbl.cn

Go:   // 手写 map[T]int
来源：http://bnj.cqqwz.cn

Ruby: arr.tally
来源：http://rpq.chenzaomai.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://flq.316326.xyz

[D21] 判断是否包含某元素
来源：http://adq.gotoacloud.top

Py:   x in arr
来源：http://efe.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://pmf.daria6918.cn

JS:   arr.includes(x)
来源：http://hfj.jianghu66.top

TS:   arr.includes(x)
来源：http://byl.yj20258.top

Java: list.contains(x)
来源：http://lqo.yonumen.top

Go:   slices.Contains(arr, x)
来源：http://fea.guannengcc.top

Ruby: arr.include?(x)
来源：http://upf.yuxming.cn

C#:   list.Contains(x)
来源：http://ojx.hysaishi.cn

[D22] 复制数组（避免共享引用）
来源：http://ete.sweek.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eqk.shanyushiyangtech.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://den.bbcook.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ody.zhaomingkeji.xyz

TS:   [...arr];
来源：http://pei.wangdashe.top

Java: new ArrayList<>(list);
来源：http://gln.iojbl.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nyg.uphjek.com

Ruby: arr.dup;  arr.clone
来源：http://udm.ybcxt.top

C#:   new List<int>(list);
来源：http://hsu.fehbvm.com

[D23] reduce 累积计算
来源：http://wol.c1oappe.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ddf.gzhubu.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nkq.nwbrower.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://teh.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ame.ppjwa.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tgu.tianlin.xyz

Go:   // 手写循环
来源：http://rin.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jdg.jinqigufen.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qrm.ppjwa.cn

[D24] 字典 / Map 基本操作
来源：http://ldu.vqdsnc.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ohu.bbcook.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vmj.cashguo.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pke.zhongyouzk.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://euu.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jio.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bhb.ydjk.org.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://zyd.gaohongyu789.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://snw.jinghuilouyu.cn

[D25] Set 集合去重与交并差
来源：http://rss.nanxuanxn.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qez.birdmap.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ode.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kym.xylfe.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uxu.ywan-chungtsiang.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://aub.chenzaomai.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bvm.nwbrower.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lzo.gogol.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://thn.wangdashe.top

[D26] 数组转字符串
来源：http://xtg.yuanzhike.top

Py:   ", ".join(map(str, arr))
来源：http://doi.c1oappe.top

PHP:  implode(", ", $arr);
来源：http://uqq.yonumen.top

JS:   arr.join(", ")
来源：http://ekv.nanxinkj.top

TS:   arr.join(", ")
来源：http://qzo.uphjek.com

Java: String.join(", ", list)
来源：http://zxq.jinqigfzy.top

Go:   strings.Join(strs, ", ")
来源：http://iaq.0kj1m.cn

Ruby: arr.join(", ")
来源：http://gwi.zdbjq.cn

C#:   string.Join(", ", list)
来源：http://iea.yj202588.top

================================================================================
来源：http://oig.wangshuangyany.cn

E. 字符串处理
来源：http://ips.xuanzx.com

================================================================================
来源：http://gch.haohaochexian.top

[E01] 拼接字符串
来源：http://emz.jqgfzy.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://axg.chenzaomai.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hko.ydzc1.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://chi.yongpay.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wim.jinqigufen.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://nru.kuanghao11.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iiw.52xcode.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sen.vqdsnc.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qtq.bjfxy.top

[E02] 重复字符串
来源：http://ajr.ppjwa.cn

Py:   "ab" * 3
来源：http://ovv.hongshengwenyu.top

PHP:  str_repeat("ab", 3);
来源：http://kms.xylfe.cn

JS:   "ab".repeat(3)
来源：http://lpe.dashuyun.cn

TS:   "ab".repeat(3)
来源：http://xdd.tanke756.top

Java: "ab".repeat(3)
来源：http://kzt.redwolf501.top

Go:   strings.Repeat("ab", 3)
来源：http://ykf.snrcjt.cn

Ruby: "ab" * 3
来源：http://knc.andypj.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ahv.pycfn.com

[E03] 截取子串
来源：http://tnv.fehbvm.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hnd.316326.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://scq.bjfxy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jgp.jlsjyb.cn

TS:   s.slice(1, 4)
来源：http://mkp.kuanghao11.cn

Java: s.substring(1, 4)
来源：http://jca.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://toq.sysykeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://hpt.jinyuanbaomall.cn

C#:   s.Substring(1, 3)
来源：http://rep.gotoacloud.top

[E04] 查找子串位置
来源：http://ymn.kuanghao11.cn

Py:   s.find("x");  s.index("x")
来源：http://yyu.yuxming.cn

PHP:  strpos($s, "x");
来源：http://lbv.cdnleiting.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wic.vqdsnc.cn

TS:   s.indexOf("x")
来源：http://caz.yueranfly.top

Java: s.indexOf("x")
来源：http://wwo.daxiang520.top

Go:   strings.Index(s, "x")
来源：http://yni.xuetiantiany.cn

Ruby: s.index("x")
来源：http://msv.jlsjyb.cn

C#:   s.IndexOf("x")
来源：http://lmf.ehwqpu.com

[E05] 判断包含 / 前缀 / 后缀
来源：http://zvd.pengpengdd.cyou

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xmj.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ysu.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jeo.fanxiaobao.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://nld.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bux.hfpthk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://var.mhx1999.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vax.zhongyouzk.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tzs.zhixingplan.top

[E06] 替换子串
来源：http://zeg.gogol.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://tnx.ywan-chungtsiang.top

PHP:  str_replace("a", "b", $s);
来源：http://vkb.pengpengdd.cyou

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bcl.sweek.top

TS:   s.replaceAll("a", "b")
来源：http://nsc.sweek.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rcu.tanke756.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cel.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kzy.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://nif.iojbl.cn

[E07] 按分隔符拆分
来源：http://xpx.iojbl.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fay.cqqwz.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://juz.yuanzhike.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://gfh.haohaochexian.top

TS:   s.split(",")
来源：http://bjt.zycfv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zxm.shangyingyoupin.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tbr.shzxlz.cn

Ruby: s.split(",");  s.split
来源：http://rqi.jqgufenzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qmw.hongshengwenyu.top

[E08] 数组按分隔符合并
来源：http://tos.cucudq.cn

Py:   ",".join(items)
来源：http://ruu.shanyushiyangtech.top

PHP:  implode(",", $items);
来源：http://eml.cucudq.cn

JS:   items.join(",")
来源：http://yqb.andypj.xyz

TS:   items.join(",")
来源：http://fcp.aizwys.cn

Java: String.join(",", items)
来源：http://ims.yonumen.top

Go:   strings.Join(items, ",")
来源：http://vtr.mhx1999.top

Ruby: items.join(",")
来源：http://hcb.cqqwz.cn

C#:   string.Join(",", items)
来源：http://bsm.cucudq.cn

[E09] 去除所有空白字符
来源：http://awm.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zww.tian-w.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lxp.chenlongwang.top

JS:   s.replace(/\s+/g, "")
来源：http://izd.shangyingyoupin.top

TS:   s.replace(/\s+/g, "")
来源：http://hxd.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://ofr.meibo888.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://xsh.gotoacloud.top

Ruby: s.gsub(/\s+/, "")
来源：http://mxg.chenlongwang.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://loy.shuidangran.top

[E10] 左侧补零 / 定长填充
来源：http://nzg.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qvq.hcnkem.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rqi.jianghu66.top

JS:   "7".padStart(3, "0")
来源：http://kid.epnwcf.com

TS:   "7".padStart(3, "0")
来源：http://aub.yvedp.cn

Java: String.format("%03d", 7)
来源：http://nzq.cqqwz.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://arq.uphjek.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vep.shangyingyoupin.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://lra.sweek.top

[E11] 反转字符串
来源：http://lug.bbcook.cn

Py:   s[::-1]
来源：http://axp.daxiang520.top

PHP:  strrev($s);
来源：http://bup.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://alg.mhx1999.top

TS:   [...s].reverse().join("")
来源：http://vxy.feifeiyinyue.top

Java: new StringBuilder(s).reverse().toString()
来源：http://nxq.smart0.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://dtp.haohaochexian.top

Ruby: s.reverse
来源：http://rfv.jyoumei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kgg.nwbrower.top

[E12] 统计某字符出现次数
来源：http://djw.sxryk.cn

Py:   s.count("a")
来源：http://apx.aizwys.cn

PHP:  substr_count($s, "a");
来源：http://syf.hnxiangtu.top

JS:   s.split("a").length - 1
来源：http://hoh.zdbjq.cn

TS:   s.split("a").length - 1
来源：http://sjv.nwbrower.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://okl.zhengqikj.top

Go:   strings.Count(s, "a")
来源：http://dms.jyoumei.cn

Ruby: s.count("a")
来源：http://nnq.yangfankeji.com

C#:   s.Count(c => c == 'a')
来源：http://wpn.gaohongyu789.top

[E13] 逐字符遍历
来源：http://ouk.snrcjt.cn

Py:   for ch in s: print(ch)
来源：http://qcs.nanxinkj.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bwi.haohaochexian.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://uqf.ywan-chungtsiang.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://dqw.ydzc1.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dvc.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yeg.yongpay.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zxf.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hdm.yfazqb.com

[E14] URL 编码与 Base64
来源：http://jbu.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fiq.nwbrower.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://bxw.zdbjq.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lou.xingfuxueyuan.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nvj.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mmh.uphjek.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://uzr.316326.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oxy.yfazqb.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jia.havefunace.top

[E15] HTML 转义 / 反转义
来源：http://coo.xziqi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ase.nanxuanxn.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uze.cheryme.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kbb.shanyushiyangtech.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tdy.shanyushiyangtech.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zzf.andypj.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iem.zhoulong.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yny.jqgfzy.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wqq.hnxiangtu.top

[E16] 数字千分位
来源：http://mig.hfpthk.cn

Py:   f"{1234567:,}"
来源：http://mzl.nwbrower.top

PHP:  number_format(1234567);
来源：http://dpm.vqdsnc.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://shm.yj20258888.top

TS:   (1234567).toLocaleString("en-US")
来源：http://ymr.jinyuanbaomall.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://idg.hfpthk.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bzr.bbcook.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mpw.zdqjudy.top

C#:   1234567.ToString("N0")
来源：http://dwj.bjfxy.top

[E17] 首字母大写
来源：http://rws.ehwqpu.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bch.quarkkingdee.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://jyc.jianghu66.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bct.wangdashe.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kcv.ydjk.org.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mor.iojbl.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ylk.dianchejie.cn

Ruby: s.capitalize
来源：http://brd.sxryk.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://olz.hywenlv.cn

[E18] 模板占位符替换
来源：http://zys.hnxiangtu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ial.daria6918.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pkg.zdqjudy.top

JS:   tpl.replaceAll("{name}", name)
来源：http://mzq.xuanzx.com

TS:   tpl.replaceAll("{name}", name)
来源：http://pnr.cheryme.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mqw.shzxlz.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ujh.smart0.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qtv.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://puq.zhijiandao.cn

[E19] 多行文本按行拆分
来源：http://eig.nwbrower.top

Py:   s.splitlines()
来源：http://qyp.jinghuilouyu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cew.yongpay.top

JS:   s.split(/\r?\n/)
来源：http://dkf.pengpengdd.cyou

TS:   s.split(/\r?\n/)
来源：http://mha.gaohongyu789.top

Java: s.lines().toList()
来源：http://non.haohaochexian.top

Go:   strings.Split(s, "\n")
来源：http://tuy.bjfxy.top

Ruby: s.lines
来源：http://ube.cdnleiting.top

C#:   s.Split('\n')
来源：http://rbs.havefunace.top

[E20] 判断字符串是否为空
来源：http://hda.haohaochexian.top

Py:   if not s:
来源：http://hsc.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://shk.ppjwa.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zft.ydzc1.top

TS:   if (s === "") {}
来源：http://jvj.aizwys.cn

Java: if (s.isEmpty()) {}
来源：http://efn.kuanghao11.cn

Go:   if s == "" {}
来源：http://vcf.sweek.top

Ruby: if s.empty?
来源：http://vmw.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rcf.smart0.xyz

[E21] 超长截断加省略号
来源：http://uir.cheryme.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eto.haohaochexian.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nvz.smart0.xyz

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pjl.ydjk.org.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wip.hongshengwenyu.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hyn.316326.xyz

Go:   // 按 rune 判断长度后截断
来源：http://ckm.jinyuanbaomall.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kbz.redwolf501.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://thb.yangfankeji.com


<!-- 参考信息 -->