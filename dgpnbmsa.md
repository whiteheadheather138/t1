代发 wailian999

[D15] 去重
来源：http://zpk.c1oappe.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fop.hnqzz.top

PHP:  array_unique($arr);
来源：http://jjh.zycfv.cn

JS:   [...new Set(arr)]
来源：http://met.fehbvm.com

TS:   [...new Set(arr)]
来源：http://grs.aizwys.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wjm.jqgufenzy.top

Go:   // 用 map[T]struct{} 手写
来源：http://kcy.vehdjk.com

Ruby: arr.uniq
来源：http://svk.zhaomingkeji.xyz

C#:   list.Distinct().ToList()
来源：http://ljx.hammf.cn

[D16] 求和与平均值
来源：http://lvu.shanyushiyangtech.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lnp.sxryk.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://soz.chenlongwang.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zcw.jinyuanbaomall.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://omg.bjfxy.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pwy.yonumen.top

Go:   // 手写循环累加
来源：http://cwi.yj20258888.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iiy.ppjwa.cn

C#:   list.Sum();  list.Average()
来源：http://jrt.guowangkeji.top

[D17] 最大值与最小值
来源：http://eus.tanke756.top

Py:   max(arr);  min(arr)
来源：http://obs.zhijiandao.cn

PHP:  max($arr);  min($arr);
来源：http://ryj.hfpthk.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iwd.jqgfzy.top

TS:   Math.max(...arr);
来源：http://cwj.ydjk.org.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mbv.yongpay.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mzq.haohaochexian.top

Ruby: arr.max;  arr.min
来源：http://eki.fengsongda.top

C#:   list.Max();  list.Min()
来源：http://ppb.jinqigfzy.top

[D18] 扁平化嵌套数组
来源：http://hju.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dtf.cucudq.cn

PHP:  array_merge(...$nested);
来源：http://iyp.jianghu66.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cds.hysaishi.cn

TS:   nested.flat();
来源：http://zbs.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qpy.chenlongwang.top

Go:   // 手写双层循环
来源：http://sng.jinghuilouyu.cn

Ruby: nested.flatten
来源：http://tns.cqqwz.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ulr.chenjidiqi.icu

[D19] 按字段分组
来源：http://akz.snrcjt.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://khq.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://umt.jianghu66.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cgy.xuetiantiany.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hlw.yj20258888.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kcm.hesvh.cn

Go:   // 手写 map[string][]T
来源：http://mte.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://oju.fanxiaobao.xyz

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://evw.ywan-chungtsiang.top

[D20] 统计每个元素出现次数
来源：http://ihf.tanke756.top

Py:   Counter(arr)
来源：http://ttd.pycfn.com

PHP:  array_count_values($arr);
来源：http://ucu.ehwqpu.com

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fuf.9152youxi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wzw.sxryk.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://icy.fktsv.cn

Go:   // 手写 map[T]int
来源：http://czj.daria6918.cn

Ruby: arr.tally
来源：http://jce.zhengqikj.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gcz.jyoumei.cn

[D21] 判断是否包含某元素
来源：http://glz.9152youxi.cn

Py:   x in arr
来源：http://twv.tianlin.xyz

PHP:  in_array($x, $arr, true);
来源：http://uwg.zycfv.cn

JS:   arr.includes(x)
来源：http://kpb.cashguo.top

TS:   arr.includes(x)
来源：http://rko.shuidangran.top

Java: list.contains(x)
来源：http://zuz.jyoumei.cn

Go:   slices.Contains(arr, x)
来源：http://zrb.fanxiaobao.xyz

Ruby: arr.include?(x)
来源：http://rpz.nwbrower.top

C#:   list.Contains(x)
来源：http://hgz.zhiwuduotai.top

[D22] 复制数组（避免共享引用）
来源：http://nnj.meibo888.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://enq.jyoumei.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tlb.guannengcc.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://snh.ehwqpu.com

TS:   [...arr];
来源：http://bll.tian-w.cn

Java: new ArrayList<>(list);
来源：http://jbd.yonumen.top

Go:   copied := append([]int(nil), arr...)
来源：http://efy.jlsjyb.cn

Ruby: arr.dup;  arr.clone
来源：http://pxb.ppjwa.cn

C#:   new List<int>(list);
来源：http://fhf.pengpengdd.cyou

[D23] reduce 累积计算
来源：http://ulk.zdqjudy.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wrt.daxiang520.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qum.zhaomingkeji.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gms.jlsjyb.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lod.ydjk.org.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://auu.shangyingyoupin.top

Go:   // 手写循环
来源：http://ott.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xok.yongpay.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gdo.zhiwuduotai.top

[D24] 字典 / Map 基本操作
来源：http://axs.yongpay.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kny.dianchejie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://htv.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rto.havefunace.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ryn.ctjpmb.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fhf.wangdashe.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rum.yuxming.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://opk.yvedp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bxb.xingfuxueyuan.xyz

[D25] Set 集合去重与交并差
来源：http://cbc.jlsjyb.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://any.jiagoushi.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ame.gogol.net.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hhc.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zeu.yj20258.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nxk.haohaochexian.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xcj.hcnkem.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hug.snrcjt.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ejj.tianlin.xyz

[D26] 数组转字符串
来源：http://mbm.tianlin.xyz

Py:   ", ".join(map(str, arr))
来源：http://apv.gogol.net.cn

PHP:  implode(", ", $arr);
来源：http://siv.meibo888.top

JS:   arr.join(", ")
来源：http://ghr.aizwys.cn

TS:   arr.join(", ")
来源：http://twq.epnwcf.com

Java: String.join(", ", list)
来源：http://rsp.yj20258.top

Go:   strings.Join(strs, ", ")
来源：http://rri.snrcjt.cn

Ruby: arr.join(", ")
来源：http://kzs.cashguo.top

C#:   string.Join(", ", list)
来源：http://fcw.nanxinkj.top

================================================================================
来源：http://xeg.yanxiufei.cn

E. 字符串处理
来源：http://ypr.xziqi.cn

================================================================================
来源：http://til.bjfxy.top

[E01] 拼接字符串
来源：http://eib.xylfe.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rhk.fktsv.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rnf.yuanzhike.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://trl.yueranfly.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tgx.chenzaomai.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jtl.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xtt.yangfankeji.com

Ruby: "a" + "b";  ["a", "b"].join
来源：http://spb.svipenyu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zdo.pycfn.com

[E02] 重复字符串
来源：http://yyy.yfazqb.com

Py:   "ab" * 3
来源：http://jec.vehdjk.com

PHP:  str_repeat("ab", 3);
来源：http://pku.xinyue.icu

JS:   "ab".repeat(3)
来源：http://lfx.yongpay.top

TS:   "ab".repeat(3)
来源：http://skq.jqgufenzy.top

Java: "ab".repeat(3)
来源：http://jzg.vehdjk.com

Go:   strings.Repeat("ab", 3)
来源：http://olk.gogol.net.cn

Ruby: "ab" * 3
来源：http://sog.jiagoushi.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oku.zhaomingkeji.xyz

[E03] 截取子串
来源：http://mqh.yangfankeji.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ltd.vehdjk.com

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://lhj.uphjek.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kjw.tarul.cn

TS:   s.slice(1, 4)
来源：http://ezh.xuanzx.com

Java: s.substring(1, 4)
来源：http://jik.yongpay.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://frp.shanyushiyangkeji.top

Ruby: s[1, 3];  s[1..3]
来源：http://xzj.wangdashe.top

C#:   s.Substring(1, 3)
来源：http://bit.0kj1m.cn

[E04] 查找子串位置
来源：http://xby.chenzaomai.com

Py:   s.find("x");  s.index("x")
来源：http://fbm.birdmap.top

PHP:  strpos($s, "x");
来源：http://mee.chenjidiqi.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fqu.ydjk.org.cn

TS:   s.indexOf("x")
来源：http://llp.zhoulong.xyz

Java: s.indexOf("x")
来源：http://rgv.gotoacloud.top

Go:   strings.Index(s, "x")
来源：http://gav.jinghuilouyu.cn

Ruby: s.index("x")
来源：http://ffe.yuxming.cn

C#:   s.IndexOf("x")
来源：http://wyh.zhoulong.xyz

[E05] 判断包含 / 前缀 / 后缀
来源：http://qqy.cucudq.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fln.ehwqpu.com

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://myn.ydjk.org.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://keu.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mrh.hnqzz.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ejj.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ueh.meibo888.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tou.yongpay.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rdn.pengpengdd.cyou

[E06] 替换子串
来源：http://nik.jinyuanbaomall.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qnz.hongshengwenyu.top

PHP:  str_replace("a", "b", $s);
来源：http://qah.jinghuilouyu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dfu.vqdsnc.cn

TS:   s.replaceAll("a", "b")
来源：http://zwh.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oqo.jqgufenzy.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uqs.xziqi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bar.iojbl.cn

C#:   s.Replace("a", "b")
来源：http://bsd.xuanzx.com

[E07] 按分隔符拆分
来源：http://icg.hcnkem.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://seh.svipenyu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xyt.hnxiangtu.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://jyx.guowangkeji.top

TS:   s.split(",")
来源：http://dte.xinyue.icu

Java: s.split(",");  s.split("\\s+")
来源：http://zsv.tian-w.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://saj.birdmap.top

Ruby: s.split(",");  s.split
来源：http://gju.hcnkem.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://stl.ydzc1.top

[E08] 数组按分隔符合并
来源：http://lyq.ctjpmb.com

Py:   ",".join(items)
来源：http://rcd.zhoulong.xyz

PHP:  implode(",", $items);
来源：http://xxv.nanxinkj.top

JS:   items.join(",")
来源：http://ohb.guannengcc.top

TS:   items.join(",")
来源：http://pnl.sufxvd.cn

Java: String.join(",", items)
来源：http://epp.smart0.xyz

Go:   strings.Join(items, ",")
来源：http://qrp.jianghu66.top

Ruby: items.join(",")
来源：http://vhd.hcnkem.com

C#:   string.Join(",", items)
来源：http://wqr.xinyue.icu

[E09] 去除所有空白字符
来源：http://ldx.snrcjt.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vvn.guannengcc.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ehd.ctjpmb.com

JS:   s.replace(/\s+/g, "")
来源：http://dwq.birdmap.top

TS:   s.replace(/\s+/g, "")
来源：http://txj.zhoulong.xyz

Java: s.replaceAll("\\s+", "")
来源：http://vii.gogol.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bhp.ehwqpu.com

Ruby: s.gsub(/\s+/, "")
来源：http://cjt.ydjk.org.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cox.nanxuanxn.top

[E10] 左侧补零 / 定长填充
来源：http://tqq.svipenyu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cxt.cheryme.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xvw.hongshengwenyu.top

JS:   "7".padStart(3, "0")
来源：http://bez.zdqjudy.top

TS:   "7".padStart(3, "0")
来源：http://gbh.haohaochexian.top

Java: String.format("%03d", 7)
来源：http://ipz.ybcxt.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://lqz.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uei.tarul.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cfl.hysaishi.cn

[E11] 反转字符串
来源：http://ffy.snrcjt.cn

Py:   s[::-1]
来源：http://cov.chenzaomai.com

PHP:  strrev($s);
来源：http://vdq.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://duc.havefunace.top

TS:   [...s].reverse().join("")
来源：http://mtg.zhiwuduotai.top

Java: new StringBuilder(s).reverse().toString()
来源：http://qso.hammf.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bkk.tian-w.cn

Ruby: s.reverse
来源：http://cwg.fzhhl.top

C#:   new string(s.Reverse().ToArray())
来源：http://osp.hnqzz.top

[E12] 统计某字符出现次数
来源：http://smz.xuetiantiany.cn

Py:   s.count("a")
来源：http://nhs.zhixingplan.top

PHP:  substr_count($s, "a");
来源：http://uge.ydjk.org.cn

JS:   s.split("a").length - 1
来源：http://elq.zhijiandao.cn

TS:   s.split("a").length - 1
来源：http://oee.uphjek.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://frr.vqdsnc.cn

Go:   strings.Count(s, "a")
来源：http://ych.yvedp.cn

Ruby: s.count("a")
来源：http://kve.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://nmm.mhx1999.top

[E13] 逐字符遍历
来源：http://xxe.yangfankeji.com

Py:   for ch in s: print(ch)
来源：http://cho.shanyushiyangtech.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wfy.zhoulong.xyz

JS:   for (const ch of s) { console.log(ch); }
来源：http://cwm.havefunace.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://fep.zhengqikj.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lfz.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wxt.fehbvm.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tgl.daria6918.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jyi.ydzc1.top

[E14] URL 编码与 Base64
来源：http://crp.guowangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://umm.gotoacloud.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://ceh.bbcook.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://srh.9152youxi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://abe.xuanzx.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://frf.dianchejie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://epw.xuanzx.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qpp.c1oappe.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hhq.hysaishi.cn

[E15] HTML 转义 / 反转义
来源：http://wqu.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://rds.chenzaomai.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ygq.sxryk.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ytb.jyoumei.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pxt.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mcw.shanyushiyangkeji.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vrd.hywenlv.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pbc.meibo888.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bpd.smart0.xyz

[E16] 数字千分位
来源：http://nmq.hywenlv.cn

Py:   f"{1234567:,}"
来源：http://ttf.jinghuilouyu.cn

PHP:  number_format(1234567);
来源：http://jov.xuanzx.com

JS:   (1234567).toLocaleString("en-US")
来源：http://uft.316326.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://pfb.hysaishi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vvi.daxiang520.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://etx.hammf.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pck.snrcjt.cn

C#:   1234567.ToString("N0")
来源：http://szw.wangshuangyany.cn

[E17] 首字母大写
来源：http://uhk.ydzc1.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xlz.zdqjudy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://ihb.aizwys.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xlb.sweek.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lnj.zhijiandao.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uxa.cashguo.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fis.yuxming.cn

Ruby: s.capitalize
来源：http://ppm.hammf.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cbv.xinyue.icu

[E18] 模板占位符替换
来源：http://xit.cashguo.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://opz.zhixingplan.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vhs.shanyushiyangkeji.top

JS:   tpl.replaceAll("{name}", name)
来源：http://jot.guowangkeji.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ucn.fanxiaobao.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vnb.chenlongwang.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lhv.yangfankeji.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zqv.jqgufenzy.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gup.tanke756.top

[E19] 多行文本按行拆分
来源：http://pyd.gogol.net.cn

Py:   s.splitlines()
来源：http://jrv.redwolf501.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bbc.yj202588.top

JS:   s.split(/\r?\n/)
来源：http://ayc.jlsjyb.cn

TS:   s.split(/\r?\n/)
来源：http://jte.kuanghao11.cn

Java: s.lines().toList()
来源：http://ruy.hcnkem.com

Go:   strings.Split(s, "\n")
来源：http://gwu.jinyuanbaomall.cn

Ruby: s.lines
来源：http://rcd.shzxlz.cn

C#:   s.Split('\n')
来源：http://gdg.316326.xyz

[E20] 判断字符串是否为空
来源：http://zcf.tian-w.cn

Py:   if not s:
来源：http://vgw.chenzaomai.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tcv.jianghu66.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pkw.shangyingyoupin.top

TS:   if (s === "") {}
来源：http://gyh.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://agb.yj202588.top

Go:   if s == "" {}
来源：http://xqe.sxryk.cn

Ruby: if s.empty?
来源：http://exg.cashguo.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nfc.vehdjk.com

[E21] 超长截断加省略号
来源：http://wxr.jinghuilouyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ezz.jinyuanbaomall.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pbd.iojbl.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wcp.jinghuilouyu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ydn.52xcode.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wtu.sxryk.cn

Go:   // 按 rune 判断长度后截断
来源：http://ucz.daria6918.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://yhp.sysykeji.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://glq.meibo888.top


<!-- 参考信息 -->