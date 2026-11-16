代发 wailian999

[D15] 去重
来源：http://yvj.hammf.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vqy.svipenyu.cn

PHP:  array_unique($arr);
来源：http://gwq.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://iho.bbcook.cn

TS:   [...new Set(arr)]
来源：http://bge.chenjidiqi.icu

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://arh.uphjek.com

Go:   // 用 map[T]struct{} 手写
来源：http://wes.yuxming.cn

Ruby: arr.uniq
来源：http://pkv.jinyuanbaomall.cn

C#:   list.Distinct().ToList()
来源：http://xvh.epnwcf.com

[D16] 求和与平均值
来源：http://pwi.mhx1999.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fgc.hnxiangtu.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aui.zycfv.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ima.guannengcc.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sph.epnwcf.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://drg.epnwcf.com

Go:   // 手写循环累加
来源：http://lqp.shanyushiyangkeji.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wkj.xuetiantiany.cn

C#:   list.Sum();  list.Average()
来源：http://pwk.ywan-chungtsiang.top

[D17] 最大值与最小值
来源：http://eao.yonumen.top

Py:   max(arr);  min(arr)
来源：http://nns.jqgufenzy.top

PHP:  max($arr);  min($arr);
来源：http://ogg.fengsongda.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eca.fzhhl.top

TS:   Math.max(...arr);
来源：http://udz.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://brb.kuanghao11.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sjc.zhongyouzk.top

Ruby: arr.max;  arr.min
来源：http://jcm.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://cyr.yvedp.cn

[D18] 扁平化嵌套数组
来源：http://wxy.iojbl.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://amv.zhoulong.xyz

PHP:  array_merge(...$nested);
来源：http://aox.aizwys.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://inc.gaohongyu789.top

TS:   nested.flat();
来源：http://umh.yj202588.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sxh.jinqigfzy.top

Go:   // 手写双层循环
来源：http://dev.hesvh.cn

Ruby: nested.flatten
来源：http://lel.sweek.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://dva.hnxiangtu.top

[D19] 按字段分组
来源：http://zyf.c1oappe.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://anu.9152youxi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pfn.fengsongda.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vxk.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lgj.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ned.c1oappe.top

Go:   // 手写 map[string][]T
来源：http://rce.chenjidiqi.icu

Ruby: arr.group_by { |x| x[:type] }
来源：http://asd.dianchejie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://luf.cashguo.top

[D20] 统计每个元素出现次数
来源：http://svq.ydjk.org.cn

Py:   Counter(arr)
来源：http://zjd.daxiang520.top

PHP:  array_count_values($arr);
来源：http://fgi.zdbjq.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bnh.fktsv.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jop.haohaochexian.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zom.ydzc1.top

Go:   // 手写 map[T]int
来源：http://nxo.hesvh.cn

Ruby: arr.tally
来源：http://xfr.hnqzz.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rmt.yj20258888.top

[D21] 判断是否包含某元素
来源：http://xnm.hesvh.cn

Py:   x in arr
来源：http://lry.andypj.xyz

PHP:  in_array($x, $arr, true);
来源：http://xfm.yuxming.cn

JS:   arr.includes(x)
来源：http://sup.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://ecn.xinyue.icu

Java: list.contains(x)
来源：http://gud.mhx1999.top

Go:   slices.Contains(arr, x)
来源：http://gne.cheryme.top

Ruby: arr.include?(x)
来源：http://kwi.jiagoushi.top

C#:   list.Contains(x)
来源：http://hss.gotoacloud.top

[D22] 复制数组（避免共享引用）
来源：http://scq.epnwcf.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ftt.feifeiyinyue.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zes.zhongyouzk.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sxt.aibaodan.cn

TS:   [...arr];
来源：http://oej.cheryme.top

Java: new ArrayList<>(list);
来源：http://plk.jinyuanbaomall.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oem.aibaodan.cn

Ruby: arr.dup;  arr.clone
来源：http://edk.shangyingyoupin.top

C#:   new List<int>(list);
来源：http://lst.jqgfzy.top

[D23] reduce 累积计算
来源：http://nya.yj202588.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ttw.quarkkingdee.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xzi.sxryk.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://elb.aizwys.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gez.iojbl.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xzz.gaohongyu789.top

Go:   // 手写循环
来源：http://qoc.shuidangran.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://klx.sysykeji.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mib.yuanzhike.top

[D24] 字典 / Map 基本操作
来源：http://vxs.dashuyun.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ivx.c1oappe.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wfb.zycfv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dwk.meibo888.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://leq.shangyingyoupin.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gfs.smart0.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://vuq.zhongyouzk.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ekl.gogol.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ujf.yonumen.top

[D25] Set 集合去重与交并差
来源：http://mub.vqdsnc.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rdd.iojbl.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tam.ybcxt.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bua.ybcxt.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aob.nanxuanxn.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mto.andypj.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dsc.bbcook.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bok.yfazqb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zph.andypj.xyz

[D26] 数组转字符串
来源：http://nvv.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://mmk.bbcook.cn

PHP:  implode(", ", $arr);
来源：http://oes.bjfxy.top

JS:   arr.join(", ")
来源：http://eyw.jlsjyb.cn

TS:   arr.join(", ")
来源：http://kzj.yvedp.cn

Java: String.join(", ", list)
来源：http://gka.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://jex.xuanzx.com

Ruby: arr.join(", ")
来源：http://hnv.andypj.xyz

C#:   string.Join(", ", list)
来源：http://iuw.hammf.cn

================================================================================
来源：http://vvn.iojbl.cn

E. 字符串处理
来源：http://vub.zhongyouzk.top

================================================================================
来源：http://fir.9152youxi.cn

[E01] 拼接字符串
来源：http://fht.aibaodan.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fam.yangfankeji.com

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ags.uphjek.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nmv.316326.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zzm.ydzc1.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hdb.yfazqb.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pcn.ybcxt.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yxn.ehwqpu.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bgl.jqgfzy.top

[E02] 重复字符串
来源：http://rgi.yfazqb.com

Py:   "ab" * 3
来源：http://daq.fzhhl.top

PHP:  str_repeat("ab", 3);
来源：http://wwr.cucudq.cn

JS:   "ab".repeat(3)
来源：http://otp.yangfankeji.com

TS:   "ab".repeat(3)
来源：http://nkp.shanyushiyangtech.top

Java: "ab".repeat(3)
来源：http://qsu.haohaochexian.top

Go:   strings.Repeat("ab", 3)
来源：http://ffp.aibaodan.cn

Ruby: "ab" * 3
来源：http://qcb.yanxiufei.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sfq.zhoulong.xyz

[E03] 截取子串
来源：http://zyj.hysaishi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nql.birdmap.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kng.ctjpmb.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hhz.fktsv.cn

TS:   s.slice(1, 4)
来源：http://hhy.andypj.xyz

Java: s.substring(1, 4)
来源：http://tnj.zdbjq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iuu.jiagoushi.top

Ruby: s[1, 3];  s[1..3]
来源：http://hlh.cdnleiting.top

C#:   s.Substring(1, 3)
来源：http://rxq.yj20258888.top

[E04] 查找子串位置
来源：http://agv.svipenyu.cn

Py:   s.find("x");  s.index("x")
来源：http://pij.feifeiyinyue.top

PHP:  strpos($s, "x");
来源：http://vkt.xinyue.icu

JS:   s.indexOf("x");  s.search(/x/)
来源：http://dat.xingfuxueyuan.xyz

TS:   s.indexOf("x")
来源：http://tjt.meibo888.top

Java: s.indexOf("x")
来源：http://hhy.havefunace.top

Go:   strings.Index(s, "x")
来源：http://klj.yongpay.top

Ruby: s.index("x")
来源：http://ihp.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://ruo.zhijiandao.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rve.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jkp.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nlw.smart0.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://smw.zhoulong.xyz

TS:   s.includes("x");  s.startsWith("a")
来源：http://ghh.cqqwz.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fve.guowangkeji.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kkc.aibaodan.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yze.xylfe.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qpq.jinqigufen.top

[E06] 替换子串
来源：http://cpk.gzhubu.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cqt.gogol.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://rdt.daxiang520.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xkj.ppjwa.cn

TS:   s.replaceAll("a", "b")
来源：http://zkf.yonumen.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tyn.zycfv.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sld.quarkkingdee.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nxl.c1oappe.top

C#:   s.Replace("a", "b")
来源：http://qrc.316326.xyz

[E07] 按分隔符拆分
来源：http://jch.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fkh.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ohr.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://zzj.zhoulong.xyz

TS:   s.split(",")
来源：http://lhm.hywenlv.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tpo.ivvv.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dtq.hnxiangtu.top

Ruby: s.split(",");  s.split
来源：http://itm.yj202588.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://npx.ehwqpu.com

[E08] 数组按分隔符合并
来源：http://mey.cdnleiting.top

Py:   ",".join(items)
来源：http://aet.gogol.net.cn

PHP:  implode(",", $items);
来源：http://qde.ctjpmb.com

JS:   items.join(",")
来源：http://iuz.jiagoushi.top

TS:   items.join(",")
来源：http://onm.xylfe.cn

Java: String.join(",", items)
来源：http://dyq.fehbvm.com

Go:   strings.Join(items, ",")
来源：http://yid.zycfv.cn

Ruby: items.join(",")
来源：http://wzz.aibaodan.cn

C#:   string.Join(",", items)
来源：http://gmm.gaohongyu789.top

[E09] 去除所有空白字符
来源：http://tru.guowangkeji.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sbt.bjfxy.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://haq.jlsjyb.cn

JS:   s.replace(/\s+/g, "")
来源：http://apl.gzhubu.top

TS:   s.replace(/\s+/g, "")
来源：http://vkg.sjlbkw.cn

Java: s.replaceAll("\\s+", "")
来源：http://vke.zhijiandao.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cpj.hesvh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://qay.daxiang520.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sek.epnwcf.com

[E10] 左侧补零 / 定长填充
来源：http://vsg.pengpengdd.cyou

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yqm.tanke756.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ntv.feifeiyinyue.top

JS:   "7".padStart(3, "0")
来源：http://cje.wangshuangyany.cn

TS:   "7".padStart(3, "0")
来源：http://jup.gzhubu.top

Java: String.format("%03d", 7)
来源：http://vla.zycfv.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://uzr.pycfn.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nso.xuetiantiany.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sha.aibaodan.cn

[E11] 反转字符串
来源：http://xvv.xziqi.cn

Py:   s[::-1]
来源：http://tmd.uphjek.com

PHP:  strrev($s);
来源：http://xki.nwbrower.top

JS:   [...s].reverse().join("")
来源：http://pen.ydzc1.top

TS:   [...s].reverse().join("")
来源：http://mzm.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://rmg.cdnleiting.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://kkr.smart0.xyz

Ruby: s.reverse
来源：http://vze.gzhubu.top

C#:   new string(s.Reverse().ToArray())
来源：http://zcg.tian-w.cn

[E12] 统计某字符出现次数
来源：http://ppk.ydzc1.top

Py:   s.count("a")
来源：http://ink.zdqjudy.top

PHP:  substr_count($s, "a");
来源：http://upt.meibo888.top

JS:   s.split("a").length - 1
来源：http://bko.yj20258888.top

TS:   s.split("a").length - 1
来源：http://ldn.jlsjyb.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mjb.chenzaomai.com

Go:   strings.Count(s, "a")
来源：http://wiw.sufxvd.cn

Ruby: s.count("a")
来源：http://akp.sjlbkw.cn

C#:   s.Count(c => c == 'a')
来源：http://ilb.zdbjq.cn

[E13] 逐字符遍历
来源：http://swl.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://cbg.tanke756.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://myr.tian-w.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://zel.yuanzhike.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://rmm.zhongyouzk.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fra.cdnleiting.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://dfg.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://mnt.dianchejie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kam.zhijiandao.cn

[E14] URL 编码与 Base64
来源：http://mqd.nanxuanxn.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qgr.daria6918.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://hhu.nanxuanxn.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://chx.ydjk.org.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hrw.hywenlv.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jph.zhongyouzk.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jtl.52xcode.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ama.jianghu66.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oky.shanyushiyangkeji.top

[E15] HTML 转义 / 反转义
来源：http://htx.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://lxh.gaohongyu789.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ckg.yvedp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pnp.shzxlz.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jtb.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://piy.feifeiyinyue.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oxk.xingfuxueyuan.xyz

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vqc.yongpay.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://isu.52xcode.cn

[E16] 数字千分位
来源：http://aop.yfazqb.com

Py:   f"{1234567:,}"
来源：http://ggq.daxiang520.top

PHP:  number_format(1234567);
来源：http://pww.ctjpmb.com

JS:   (1234567).toLocaleString("en-US")
来源：http://zzf.havefunace.top

TS:   (1234567).toLocaleString("en-US")
来源：http://twf.tian-w.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gnt.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hho.iojbl.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://anq.ydzc1.top

C#:   1234567.ToString("N0")
来源：http://umi.hnqzz.top

[E17] 首字母大写
来源：http://nqx.uphjek.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mxg.hongshengwenyu.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://fxn.jiagoushi.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ezc.hesvh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sle.smart0.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zyy.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vls.xuanzx.com

Ruby: s.capitalize
来源：http://hrt.jinqigfzy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cli.meibo888.top

[E18] 模板占位符替换
来源：http://vlc.cdnleiting.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mhp.haohaochexian.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://uhm.fanxiaobao.xyz

JS:   tpl.replaceAll("{name}", name)
来源：http://nrw.ivvv.top

TS:   tpl.replaceAll("{name}", name)
来源：http://koi.jiagoushi.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mwd.xuanzx.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ngj.sjlbkw.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jwx.yuxming.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hfd.hnxiangtu.top

[E19] 多行文本按行拆分
来源：http://wnr.vehdjk.com

Py:   s.splitlines()
来源：http://bee.meibo888.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://azi.shuidangran.top

JS:   s.split(/\r?\n/)
来源：http://ndm.yfazqb.com

TS:   s.split(/\r?\n/)
来源：http://lfh.vehdjk.com

Java: s.lines().toList()
来源：http://owa.yj20258888.top

Go:   strings.Split(s, "\n")
来源：http://iyu.bjfxy.top

Ruby: s.lines
来源：http://vic.gaohongyu789.top

C#:   s.Split('\n')
来源：http://kqr.jlsjyb.cn

[E20] 判断字符串是否为空
来源：http://arv.sweek.top

Py:   if not s:
来源：http://lkm.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wsv.0kj1m.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gtm.yanxiufei.cn

TS:   if (s === "") {}
来源：http://qhi.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://cnm.smart0.xyz

Go:   if s == "" {}
来源：http://zhh.zdbjq.cn

Ruby: if s.empty?
来源：http://kcm.hnqzz.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pcg.epnwcf.com

[E21] 超长截断加省略号
来源：http://mok.svipenyu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mqe.yonumen.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://upj.mhx1999.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xcw.yfazqb.com

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oet.wangdashe.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nth.yuxming.cn

Go:   // 按 rune 判断长度后截断
来源：http://qdg.jqgfzy.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fle.tarul.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kbb.jinyuanbaomall.cn


<!-- 参考信息 -->