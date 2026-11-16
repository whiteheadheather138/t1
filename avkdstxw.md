代发 wailian999

[D15] 去重
来源：http://kio.chenlongwang.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wgf.zhengqikj.top

PHP:  array_unique($arr);
来源：http://ure.0kj1m.cn

JS:   [...new Set(arr)]
来源：http://rjb.chenjidiqi.icu

TS:   [...new Set(arr)]
来源：http://vge.fehbvm.com

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hwl.jianghu66.top

Go:   // 用 map[T]struct{} 手写
来源：http://clj.yuanzhike.top

Ruby: arr.uniq
来源：http://kjg.pengpengdd.cyou

C#:   list.Distinct().ToList()
来源：http://jst.cashguo.top

[D16] 求和与平均值
来源：http://iha.52xcode.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hxw.chenjidiqi.icu

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ehm.svipenyu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://foz.ctjpmb.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://pjd.jyoumei.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ias.gaohongyu789.top

Go:   // 手写循环累加
来源：http://htz.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://udd.cdnleiting.top

C#:   list.Sum();  list.Average()
来源：http://uvo.zhaomingkeji.xyz

[D17] 最大值与最小值
来源：http://nzg.ybcxt.top

Py:   max(arr);  min(arr)
来源：http://zqg.hysaishi.cn

PHP:  max($arr);  min($arr);
来源：http://rcg.jinqigfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tlw.dashuyun.cn

TS:   Math.max(...arr);
来源：http://mft.cheryme.top

Java: Collections.max(list);  Collections.min(list);
来源：http://unz.hfpthk.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://whh.hnqzz.top

Ruby: arr.max;  arr.min
来源：http://efx.ctjpmb.com

C#:   list.Max();  list.Min()
来源：http://orl.cheryme.top

[D18] 扁平化嵌套数组
来源：http://gej.52xcode.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fya.vehdjk.com

PHP:  array_merge(...$nested);
来源：http://fnr.meibo888.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gdk.dianchejie.cn

TS:   nested.flat();
来源：http://wro.daxiang520.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fho.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://jii.cdnleiting.top

Ruby: nested.flatten
来源：http://bva.nanxinkj.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dwn.shanyushiyangtech.top

[D19] 按字段分组
来源：http://jjr.mhx1999.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jim.kuanghao11.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kkm.nanxinkj.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dgt.cqqwz.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ywp.yueranfly.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://egu.shanyushiyangtech.top

Go:   // 手写 map[string][]T
来源：http://qrq.jinqigfzy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://fdi.gzhubu.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gzw.jinqigufen.top

[D20] 统计每个元素出现次数
来源：http://git.tanke756.top

Py:   Counter(arr)
来源：http://kih.epnwcf.com

PHP:  array_count_values($arr);
来源：http://gyl.shanyushiyangkeji.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uzl.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hsp.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jbv.meibo888.top

Go:   // 手写 map[T]int
来源：http://bni.hcnkem.com

Ruby: arr.tally
来源：http://ohw.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://udi.ywan-chungtsiang.top

[D21] 判断是否包含某元素
来源：http://nqm.zhongyouzk.top

Py:   x in arr
来源：http://jgo.yanxiufei.cn

PHP:  in_array($x, $arr, true);
来源：http://uon.shanyushiyangtech.top

JS:   arr.includes(x)
来源：http://obt.shuidangran.top

TS:   arr.includes(x)
来源：http://qyb.jinghuilouyu.cn

Java: list.contains(x)
来源：http://mtk.hnxiangtu.top

Go:   slices.Contains(arr, x)
来源：http://vvf.ydzc1.top

Ruby: arr.include?(x)
来源：http://rej.bjfxy.top

C#:   list.Contains(x)
来源：http://ind.ydzc1.top

[D22] 复制数组（避免共享引用）
来源：http://xmr.wangdashe.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://prs.yj20258.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dnl.quarkkingdee.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xnl.havefunace.top

TS:   [...arr];
来源：http://hht.fehbvm.com

Java: new ArrayList<>(list);
来源：http://ywb.hesvh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://uhj.snrcjt.cn

Ruby: arr.dup;  arr.clone
来源：http://yfs.iojbl.cn

C#:   new List<int>(list);
来源：http://too.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://nom.mhx1999.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zak.tanke756.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ldx.zhoulong.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qjd.uphjek.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://npl.0kj1m.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zir.fzhhl.top

Go:   // 手写循环
来源：http://non.xylfe.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gcu.zhixingplan.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://foy.sxryk.cn

[D24] 字典 / Map 基本操作
来源：http://qnt.xziqi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ihm.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ngs.haohaochexian.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cgv.xingfuxueyuan.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ugn.cashguo.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://rsz.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uji.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ugp.svipenyu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ukf.daria6918.cn

[D25] Set 集合去重与交并差
来源：http://pof.chenlongwang.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gkf.aibaodan.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rou.zhiwuduotai.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lsk.jinghuilouyu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xbe.bjfxy.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tbg.hysaishi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://biy.jyoumei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qys.yj20258.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qxb.yvedp.cn

[D26] 数组转字符串
来源：http://drs.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://oso.epnwcf.com

PHP:  implode(", ", $arr);
来源：http://hoi.tianlin.xyz

JS:   arr.join(", ")
来源：http://jjw.yfazqb.com

TS:   arr.join(", ")
来源：http://apx.sufxvd.cn

Java: String.join(", ", list)
来源：http://hog.zhoulong.xyz

Go:   strings.Join(strs, ", ")
来源：http://hcc.xuetiantiany.cn

Ruby: arr.join(", ")
来源：http://wlo.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://vtl.pengpengdd.cyou

================================================================================
来源：http://umz.xingfuxueyuan.xyz

E. 字符串处理
来源：http://wgg.chenzaomai.com

================================================================================
来源：http://pof.gzhubu.top

[E01] 拼接字符串
来源：http://eyg.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://liy.tarul.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vhx.hammf.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mnq.yonumen.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eif.snrcjt.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rpr.xuetiantiany.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gwr.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://upc.jinqigfzy.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vlm.fanxiaobao.xyz

[E02] 重复字符串
来源：http://wec.aizwys.cn

Py:   "ab" * 3
来源：http://pns.haohaochexian.top

PHP:  str_repeat("ab", 3);
来源：http://brm.redwolf501.top

JS:   "ab".repeat(3)
来源：http://per.dianchejie.cn

TS:   "ab".repeat(3)
来源：http://kgy.sufxvd.cn

Java: "ab".repeat(3)
来源：http://wwm.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://wtw.zhiwuduotai.top

Ruby: "ab" * 3
来源：http://tfj.jinqigfzy.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nfd.sxryk.cn

[E03] 截取子串
来源：http://uke.yvedp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yyb.smart0.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jpe.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://swu.cashguo.top

TS:   s.slice(1, 4)
来源：http://vnw.yj20258.top

Java: s.substring(1, 4)
来源：http://ets.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kfw.jinyuanbaomall.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jip.jqgufenzy.top

C#:   s.Substring(1, 3)
来源：http://wzs.yuanzhike.top

[E04] 查找子串位置
来源：http://wfn.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://pac.zhengqikj.top

PHP:  strpos($s, "x");
来源：http://odk.316326.xyz

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hlj.yangfankeji.com

TS:   s.indexOf("x")
来源：http://fll.uphjek.com

Java: s.indexOf("x")
来源：http://ptr.fehbvm.com

Go:   strings.Index(s, "x")
来源：http://leu.hnxiangtu.top

Ruby: s.index("x")
来源：http://esb.vehdjk.com

C#:   s.IndexOf("x")
来源：http://huz.wangdashe.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://oox.zhaomingkeji.xyz

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zik.iojbl.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://suy.shanyushiyangtech.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fln.hysaishi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zma.zhoulong.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cqj.yueranfly.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pqt.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vvz.mhx1999.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ttp.vqdsnc.cn

[E06] 替换子串
来源：http://kfd.jianghu66.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://odo.jinqigufen.top

PHP:  str_replace("a", "b", $s);
来源：http://ceo.fktsv.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://why.c1oappe.top

TS:   s.replaceAll("a", "b")
来源：http://ysz.xziqi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tbt.gaohongyu789.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jet.xingfuxueyuan.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ecj.pycfn.com

C#:   s.Replace("a", "b")
来源：http://zwv.zhongyouzk.top

[E07] 按分隔符拆分
来源：http://uqy.hfpthk.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dvp.cheryme.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nfu.redwolf501.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://evm.wangdashe.top

TS:   s.split(",")
来源：http://twa.yj20258.top

Java: s.split(",");  s.split("\\s+")
来源：http://ais.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yrk.jinqigfzy.top

Ruby: s.split(",");  s.split
来源：http://ycq.9152youxi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://djs.svipenyu.cn

[E08] 数组按分隔符合并
来源：http://kmu.yj20258.top

Py:   ",".join(items)
来源：http://clq.hywenlv.cn

PHP:  implode(",", $items);
来源：http://tig.fktsv.cn

JS:   items.join(",")
来源：http://udj.zhengqikj.top

TS:   items.join(",")
来源：http://hsc.ivvv.top

Java: String.join(",", items)
来源：http://lxs.chenzaomai.com

Go:   strings.Join(items, ",")
来源：http://ltz.fanxiaobao.xyz

Ruby: items.join(",")
来源：http://gof.mhx1999.top

C#:   string.Join(",", items)
来源：http://htk.ctjpmb.com

[E09] 去除所有空白字符
来源：http://gfk.yfazqb.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jsx.zdbjq.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://stf.daxiang520.top

JS:   s.replace(/\s+/g, "")
来源：http://yta.bbcook.cn

TS:   s.replace(/\s+/g, "")
来源：http://lrx.jyoumei.cn

Java: s.replaceAll("\\s+", "")
来源：http://xmi.cdnleiting.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qhb.zdqjudy.top

Ruby: s.gsub(/\s+/, "")
来源：http://ngx.zhoulong.xyz

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dtd.shanyushiyangtech.top

[E10] 左侧补零 / 定长填充
来源：http://drg.tanke756.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yyp.fanxiaobao.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tbz.zhoulong.xyz

JS:   "7".padStart(3, "0")
来源：http://nft.ivvv.top

TS:   "7".padStart(3, "0")
来源：http://fgh.chenlongwang.top

Java: String.format("%03d", 7)
来源：http://zzw.ehwqpu.com

Go:   fmt.Sprintf("%03d", 7)
来源：http://rvl.zycfv.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zoc.daxiang520.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pda.sweek.top

[E11] 反转字符串
来源：http://hlq.svipenyu.cn

Py:   s[::-1]
来源：http://nit.ybcxt.top

PHP:  strrev($s);
来源：http://pxq.yuxming.cn

JS:   [...s].reverse().join("")
来源：http://hxu.xuanzx.com

TS:   [...s].reverse().join("")
来源：http://oid.snrcjt.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qfw.tian-w.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://dlg.wangshuangyany.cn

Ruby: s.reverse
来源：http://ltc.daria6918.cn

C#:   new string(s.Reverse().ToArray())
来源：http://htv.cucudq.cn

[E12] 统计某字符出现次数
来源：http://jcq.jlsjyb.cn

Py:   s.count("a")
来源：http://xpq.bbcook.cn

PHP:  substr_count($s, "a");
来源：http://oxl.hywenlv.cn

JS:   s.split("a").length - 1
来源：http://ioh.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://peo.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dxw.birdmap.top

Go:   strings.Count(s, "a")
来源：http://fgu.meibo888.top

Ruby: s.count("a")
来源：http://rqg.smart0.xyz

C#:   s.Count(c => c == 'a')
来源：http://jfx.shuidangran.top

[E13] 逐字符遍历
来源：http://iep.birdmap.top

Py:   for ch in s: print(ch)
来源：http://ybv.guannengcc.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hii.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://oen.dashuyun.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ifr.c1oappe.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://znb.xinyue.icu

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cev.yuxming.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://adh.yueranfly.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zng.gzhubu.top

[E14] URL 编码与 Base64
来源：http://nrq.hcnkem.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://juc.xuanzx.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://ifo.cdnleiting.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kng.jiagoushi.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xqm.cheryme.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://usc.hfpthk.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nam.smart0.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zin.nwbrower.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nuf.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://dpp.316326.xyz

Py:   html.escape(s);  html.unescape(s)
来源：http://zsu.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yxm.tianlin.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://buc.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ryw.smart0.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://efa.wangshuangyany.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ccn.daxiang520.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uwg.shuidangran.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://oda.xylfe.cn

[E16] 数字千分位
来源：http://hym.jyoumei.cn

Py:   f"{1234567:,}"
来源：http://cug.daxiang520.top

PHP:  number_format(1234567);
来源：http://rwj.ydzc1.top

JS:   (1234567).toLocaleString("en-US")
来源：http://tyb.fzhhl.top

TS:   (1234567).toLocaleString("en-US")
来源：http://dku.feifeiyinyue.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tai.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iqf.snrcjt.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ejn.jinghuilouyu.cn

C#:   1234567.ToString("N0")
来源：http://iiw.shzxlz.cn

[E17] 首字母大写
来源：http://pvn.svipenyu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://erc.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pcp.sxryk.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bol.jlsjyb.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jqv.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ajm.shangyingyoupin.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lgf.vqdsnc.cn

Ruby: s.capitalize
来源：http://joo.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yzp.tian-w.cn

[E18] 模板占位符替换
来源：http://uvh.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zzw.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://spt.shzxlz.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tob.jlsjyb.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bdh.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xup.quarkkingdee.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pht.zhongyouzk.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pjm.cucudq.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uxl.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://nse.hywenlv.cn

Py:   s.splitlines()
来源：http://soo.sysykeji.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cke.tarul.cn

JS:   s.split(/\r?\n/)
来源：http://bvl.daxiang520.top

TS:   s.split(/\r?\n/)
来源：http://uuo.tian-w.cn

Java: s.lines().toList()
来源：http://nxp.yj20258.top

Go:   strings.Split(s, "\n")
来源：http://flg.cdnleiting.top

Ruby: s.lines
来源：http://kto.jiagoushi.top

C#:   s.Split('\n')
来源：http://bro.cashguo.top

[E20] 判断字符串是否为空
来源：http://uwd.zycfv.cn

Py:   if not s:
来源：http://yml.fktsv.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vph.zycfv.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rdd.ydjk.org.cn

TS:   if (s === "") {}
来源：http://kow.guowangkeji.top

Java: if (s.isEmpty()) {}
来源：http://hyl.chenjidiqi.icu

Go:   if s == "" {}
来源：http://fbd.jinyuanbaomall.cn

Ruby: if s.empty?
来源：http://wey.guowangkeji.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dwd.chenlongwang.top

[E21] 超长截断加省略号
来源：http://gyb.shzxlz.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zry.xylfe.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vig.birdmap.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xfy.yuanzhike.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eni.hnqzz.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hsh.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://zaf.tian-w.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zul.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ner.xuanzx.com


<!-- 参考信息 -->