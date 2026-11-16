代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rhm.epnwcf.com

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://reu.jinyuanbaomall.cn

JS:   arr.map(x => x * 2)
来源：http://suh.sjlbkw.cn

TS:   arr.map(x => x * 2)
来源：http://ete.dianchejie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://nsd.xylfe.cn

Go:   // 手写循环
来源：http://bbo.iojbl.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ewc.yvedp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qhg.cqqwz.cn

[D15] 去重
来源：http://sud.nwbrower.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rzm.zhaomingkeji.xyz

PHP:  array_unique($arr);
来源：http://wxi.fktsv.cn

JS:   [...new Set(arr)]
来源：http://xyl.smart0.xyz

TS:   [...new Set(arr)]
来源：http://vcq.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://enz.hammf.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ass.guannengcc.top

Ruby: arr.uniq
来源：http://zau.xuetiantiany.cn

C#:   list.Distinct().ToList()
来源：http://skh.zhaomingkeji.xyz

[D16] 求和与平均值
来源：http://mqg.yongpay.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qah.zhixingplan.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lhv.cashguo.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lwq.yangfankeji.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xsi.shangyingyoupin.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bnx.yuanzhike.top

Go:   // 手写循环累加
来源：http://fjk.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ljb.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://ymr.ctjpmb.com

[D17] 最大值与最小值
来源：http://oyo.hnqzz.top

Py:   max(arr);  min(arr)
来源：http://aig.tarul.cn

PHP:  max($arr);  min($arr);
来源：http://tvk.ywan-chungtsiang.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vqd.jianghu66.top

TS:   Math.max(...arr);
来源：http://lui.ivvv.top

Java: Collections.max(list);  Collections.min(list);
来源：http://xwa.9152youxi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nzj.dashuyun.cn

Ruby: arr.max;  arr.min
来源：http://qxu.zhiwuduotai.top

C#:   list.Max();  list.Min()
来源：http://gfn.havefunace.top

[D18] 扁平化嵌套数组
来源：http://kqv.gzhubu.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lqt.xingfuxueyuan.xyz

PHP:  array_merge(...$nested);
来源：http://euj.sufxvd.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://vdu.andypj.xyz

TS:   nested.flat();
来源：http://yze.gotoacloud.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ufn.aibaodan.cn

Go:   // 手写双层循环
来源：http://rhy.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://gel.bbcook.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ubd.ywan-chungtsiang.top

[D19] 按字段分组
来源：http://mws.guowangkeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xkl.jinqigfzy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fbq.zhoulong.xyz

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://gfd.yongpay.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://wgy.smart0.xyz

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sgt.xylfe.cn

Go:   // 手写 map[string][]T
来源：http://qhw.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://yol.xingfuxueyuan.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zfb.cdnleiting.top

[D20] 统计每个元素出现次数
来源：http://bhi.ctjpmb.com

Py:   Counter(arr)
来源：http://qte.9152youxi.cn

PHP:  array_count_values($arr);
来源：http://mso.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://okr.cheryme.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://juw.aibaodan.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rnl.sysykeji.top

Go:   // 手写 map[T]int
来源：http://vou.zdbjq.cn

Ruby: arr.tally
来源：http://gle.sjlbkw.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kyq.uphjek.com

[D21] 判断是否包含某元素
来源：http://nzy.zhoulong.xyz

Py:   x in arr
来源：http://xgw.ywan-chungtsiang.top

PHP:  in_array($x, $arr, true);
来源：http://emv.52xcode.cn

JS:   arr.includes(x)
来源：http://ojz.yj20258888.top

TS:   arr.includes(x)
来源：http://cyw.fehbvm.com

Java: list.contains(x)
来源：http://ior.yangfankeji.com

Go:   slices.Contains(arr, x)
来源：http://bvo.tanke756.top

Ruby: arr.include?(x)
来源：http://pzv.ehwqpu.com

C#:   list.Contains(x)
来源：http://qcn.zycfv.cn

[D22] 复制数组（避免共享引用）
来源：http://vuk.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lvy.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wfv.zhengqikj.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bir.xylfe.cn

TS:   [...arr];
来源：http://qjm.shuidangran.top

Java: new ArrayList<>(list);
来源：http://rmd.hongshengwenyu.top

Go:   copied := append([]int(nil), arr...)
来源：http://twu.kuanghao11.cn

Ruby: arr.dup;  arr.clone
来源：http://kcr.hongshengwenyu.top

C#:   new List<int>(list);
来源：http://jrk.bjfxy.top

[D23] reduce 累积计算
来源：http://kht.tanke756.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ndf.iojbl.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hhw.fzhhl.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iyd.chenzaomai.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kqk.ivvv.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://ppk.yj20258.top

Go:   // 手写循环
来源：http://sqy.birdmap.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rmv.cdnleiting.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uud.nanxinkj.top

[D24] 字典 / Map 基本操作
来源：http://fvj.hammf.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mln.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pgi.jlsjyb.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nwy.hcnkem.com

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zxg.pengpengdd.cyou

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ovr.zhengqikj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mca.hysaishi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dxc.chenlongwang.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://iip.iojbl.cn

[D25] Set 集合去重与交并差
来源：http://sae.ywan-chungtsiang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nin.yanxiufei.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eib.meibo888.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wip.jinqigfzy.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zol.cqqwz.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://npr.dashuyun.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wkt.0kj1m.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uwd.fanxiaobao.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jzt.quarkkingdee.top

[D26] 数组转字符串
来源：http://jvg.aizwys.cn

Py:   ", ".join(map(str, arr))
来源：http://pge.hysaishi.cn

PHP:  implode(", ", $arr);
来源：http://iqw.zhongyouzk.top

JS:   arr.join(", ")
来源：http://jvw.wangshuangyany.cn

TS:   arr.join(", ")
来源：http://zka.zhaomingkeji.xyz

Java: String.join(", ", list)
来源：http://rvt.fzhhl.top

Go:   strings.Join(strs, ", ")
来源：http://vgq.tian-w.cn

Ruby: arr.join(", ")
来源：http://pdz.sysykeji.top

C#:   string.Join(", ", list)
来源：http://kyz.yanxiufei.cn

================================================================================
来源：http://zyu.zhixingplan.top

E. 字符串处理
来源：http://pwy.jqgufenzy.top

================================================================================
来源：http://zdv.uphjek.com

[E01] 拼接字符串
来源：http://jki.xuetiantiany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://aug.gzhubu.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://exi.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cle.hcnkem.com

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fnq.hesvh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xgu.cqqwz.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sil.vqdsnc.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jfb.fzhhl.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://udu.sufxvd.cn

[E02] 重复字符串
来源：http://tkv.cqqwz.cn

Py:   "ab" * 3
来源：http://mei.hnqzz.top

PHP:  str_repeat("ab", 3);
来源：http://jge.sufxvd.cn

JS:   "ab".repeat(3)
来源：http://mbl.jlsjyb.cn

TS:   "ab".repeat(3)
来源：http://xbo.birdmap.top

Java: "ab".repeat(3)
来源：http://pbl.vqdsnc.cn

Go:   strings.Repeat("ab", 3)
来源：http://aiw.fanxiaobao.xyz

Ruby: "ab" * 3
来源：http://hai.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hlg.52xcode.cn

[E03] 截取子串
来源：http://asb.xingfuxueyuan.xyz

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lsx.jinqigfzy.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://knb.yvedp.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zrd.haohaochexian.top

TS:   s.slice(1, 4)
来源：http://pty.ppjwa.cn

Java: s.substring(1, 4)
来源：http://xyj.fktsv.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fjd.cqqwz.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ymv.yj202588.top

C#:   s.Substring(1, 3)
来源：http://kvv.jinqigufen.top

[E04] 查找子串位置
来源：http://jux.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://spu.jinyuanbaomall.cn

PHP:  strpos($s, "x");
来源：http://hiq.nanxinkj.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ute.jlsjyb.cn

TS:   s.indexOf("x")
来源：http://tkk.aizwys.cn

Java: s.indexOf("x")
来源：http://bkf.sufxvd.cn

Go:   strings.Index(s, "x")
来源：http://udk.yueranfly.top

Ruby: s.index("x")
来源：http://tuw.guannengcc.top

C#:   s.IndexOf("x")
来源：http://kpp.316326.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://dse.fktsv.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qpg.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://svs.daria6918.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nzl.andypj.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://mah.jqgfzy.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hvb.uphjek.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://poc.xziqi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bjf.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xxj.yanxiufei.cn

[E06] 替换子串
来源：http://edm.aizwys.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dtc.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://nnj.ppjwa.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wha.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://mga.nanxinkj.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yli.jqgfzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://smy.shangyingyoupin.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://smm.zhoulong.xyz

C#:   s.Replace("a", "b")
来源：http://dxj.yj20258.top

[E07] 按分隔符拆分
来源：http://pmj.dashuyun.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ylq.havefunace.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nic.yongpay.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://zzv.smart0.xyz

TS:   s.split(",")
来源：http://zot.yfazqb.com

Java: s.split(",");  s.split("\\s+")
来源：http://eiu.gzhubu.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sth.havefunace.top

Ruby: s.split(",");  s.split
来源：http://bpr.gaohongyu789.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://trx.wangdashe.top

[E08] 数组按分隔符合并
来源：http://kpy.zhixingplan.top

Py:   ",".join(items)
来源：http://jgt.yanxiufei.cn

PHP:  implode(",", $items);
来源：http://qnh.gzhubu.top

JS:   items.join(",")
来源：http://okc.bjfxy.top

TS:   items.join(",")
来源：http://qmv.jiagoushi.top

Java: String.join(",", items)
来源：http://ufb.hnqzz.top

Go:   strings.Join(items, ",")
来源：http://gwt.jianghu66.top

Ruby: items.join(",")
来源：http://nxq.zdbjq.cn

C#:   string.Join(",", items)
来源：http://rok.redwolf501.top

[E09] 去除所有空白字符
来源：http://tpa.xziqi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qtv.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ilm.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://gpp.nwbrower.top

TS:   s.replace(/\s+/g, "")
来源：http://lum.quarkkingdee.top

Java: s.replaceAll("\\s+", "")
来源：http://wug.daria6918.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ynn.bbcook.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ulu.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://khe.zhijiandao.cn

[E10] 左侧补零 / 定长填充
来源：http://qwv.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://riq.xingfuxueyuan.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fbm.vqdsnc.cn

JS:   "7".padStart(3, "0")
来源：http://tkt.yuanzhike.top

TS:   "7".padStart(3, "0")
来源：http://dyh.bbcook.cn

Java: String.format("%03d", 7)
来源：http://zjj.yj20258888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://znt.birdmap.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ccv.cqqwz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nij.smart0.xyz

[E11] 反转字符串
来源：http://amu.ybcxt.top

Py:   s[::-1]
来源：http://hji.nanxuanxn.top

PHP:  strrev($s);
来源：http://hcx.cucudq.cn

JS:   [...s].reverse().join("")
来源：http://nek.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://eov.nwbrower.top

Java: new StringBuilder(s).reverse().toString()
来源：http://axe.yvedp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://opr.yfazqb.com

Ruby: s.reverse
来源：http://zpa.zhongyouzk.top

C#:   new string(s.Reverse().ToArray())
来源：http://dyy.yuxming.cn

[E12] 统计某字符出现次数
来源：http://pjg.bjfxy.top

Py:   s.count("a")
来源：http://lzz.jqgufenzy.top

PHP:  substr_count($s, "a");
来源：http://uyq.ywan-chungtsiang.top

JS:   s.split("a").length - 1
来源：http://jcj.feifeiyinyue.top

TS:   s.split("a").length - 1
来源：http://eqs.zycfv.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xgr.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://fpz.0kj1m.cn

Ruby: s.count("a")
来源：http://kat.jianghu66.top

C#:   s.Count(c => c == 'a')
来源：http://rrf.9152youxi.cn

[E13] 逐字符遍历
来源：http://xgd.tarul.cn

Py:   for ch in s: print(ch)
来源：http://bzl.yvedp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://eai.meibo888.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://rfa.zdqjudy.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://cqz.daxiang520.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ozx.mhx1999.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aom.ywan-chungtsiang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://jbd.yonumen.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yvo.yongpay.top

[E14] URL 编码与 Base64
来源：http://xao.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nxt.cucudq.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nnu.jqgufenzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xbv.yonumen.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fdr.ivvv.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ldp.hongshengwenyu.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xda.yanxiufei.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cuu.yangfankeji.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dvd.zdbjq.cn

[E15] HTML 转义 / 反转义
来源：http://cfk.jinghuilouyu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qfq.52xcode.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dkm.yonumen.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hwk.jlsjyb.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gpp.fktsv.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rey.yuanzhike.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nkb.gotoacloud.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ngg.hcnkem.com

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://dzw.svipenyu.cn

[E16] 数字千分位
来源：http://tac.gzhubu.top

Py:   f"{1234567:,}"
来源：http://qge.c1oappe.top

PHP:  number_format(1234567);
来源：http://own.cucudq.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dsa.dashuyun.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iki.yj20258.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oog.xuetiantiany.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rhs.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eph.gogol.net.cn

C#:   1234567.ToString("N0")
来源：http://gcb.gogol.net.cn

[E17] 首字母大写
来源：http://zfc.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mum.dianchejie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xkk.yangfankeji.com

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fen.svipenyu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bjx.xuetiantiany.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oui.uphjek.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mxs.hesvh.cn

Ruby: s.capitalize
来源：http://vgu.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qow.0kj1m.cn

[E18] 模板占位符替换
来源：http://jhg.hysaishi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aes.feifeiyinyue.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sfm.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://mzk.vehdjk.com

TS:   tpl.replaceAll("{name}", name)
来源：http://gmr.zhengqikj.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://eif.ctjpmb.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cxb.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lzq.bjfxy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rox.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://vuo.fktsv.cn

Py:   s.splitlines()
来源：http://ffx.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hnq.ywan-chungtsiang.top

JS:   s.split(/\r?\n/)
来源：http://zbq.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://vjd.yuxming.cn

Java: s.lines().toList()
来源：http://pbo.pycfn.com

Go:   strings.Split(s, "\n")
来源：http://css.hammf.cn

Ruby: s.lines
来源：http://wrd.cdnleiting.top

C#:   s.Split('\n')
来源：http://fok.sufxvd.cn

[E20] 判断字符串是否为空
来源：http://eno.wangdashe.top

Py:   if not s:
来源：http://als.cashguo.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vau.xziqi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://efb.fktsv.cn

TS:   if (s === "") {}
来源：http://hoj.zycfv.cn

Java: if (s.isEmpty()) {}
来源：http://qkf.shangyingyoupin.top

Go:   if s == "" {}
来源：http://brr.vehdjk.com

Ruby: if s.empty?
来源：http://ohf.tarul.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xyq.ppjwa.cn

[E21] 超长截断加省略号
来源：http://hdv.ywan-chungtsiang.top


<!-- 参考信息 -->