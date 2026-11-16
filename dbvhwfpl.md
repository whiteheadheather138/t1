代发 wailian999

TS:   [...new Set(arr)]
来源：http://cdx.zhengqikj.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lzq.vehdjk.com

Go:   // 用 map[T]struct{} 手写
来源：http://xup.snrcjt.cn

Ruby: arr.uniq
来源：http://vwv.pycfn.com

C#:   list.Distinct().ToList()
来源：http://weu.sysykeji.top

[D16] 求和与平均值
来源：http://lhd.zdqjudy.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lvu.ydzc1.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tkx.haohaochexian.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kfy.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fzj.zhaomingkeji.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://rxr.aibaodan.cn

Go:   // 手写循环累加
来源：http://vji.fengsongda.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iyz.jianghu66.top

C#:   list.Sum();  list.Average()
来源：http://kvc.sysykeji.top

[D17] 最大值与最小值
来源：http://yab.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://gyw.shangyingyoupin.top

PHP:  max($arr);  min($arr);
来源：http://iog.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uan.hammf.cn

TS:   Math.max(...arr);
来源：http://yzn.shanyushiyangtech.top

Java: Collections.max(list);  Collections.min(list);
来源：http://rrv.zhiwuduotai.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ual.yj20258.top

Ruby: arr.max;  arr.min
来源：http://lfp.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://reo.fzhhl.top

[D18] 扁平化嵌套数组
来源：http://jev.pycfn.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ujq.shanyushiyangtech.top

PHP:  array_merge(...$nested);
来源：http://xdd.ehwqpu.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rcp.zycfv.cn

TS:   nested.flat();
来源：http://ivm.epnwcf.com

Java: nested.stream().flatMap(List::stream).toList()
来源：http://vzg.fehbvm.com

Go:   // 手写双层循环
来源：http://msy.xinyue.icu

Ruby: nested.flatten
来源：http://sox.wangdashe.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kic.yueranfly.top

[D19] 按字段分组
来源：http://eje.aibaodan.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oqo.yongpay.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wdz.hammf.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://djr.cucudq.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zxq.svipenyu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dsv.yanxiufei.cn

Go:   // 手写 map[string][]T
来源：http://ozo.daxiang520.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jrj.uphjek.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://tzo.yongpay.top

[D20] 统计每个元素出现次数
来源：http://ymc.zhiwuduotai.top

Py:   Counter(arr)
来源：http://eas.chenjidiqi.icu

PHP:  array_count_values($arr);
来源：http://gos.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yzd.yongpay.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rsm.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ges.yueranfly.top

Go:   // 手写 map[T]int
来源：http://hem.zycfv.cn

Ruby: arr.tally
来源：http://zks.vehdjk.com

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://onx.hysaishi.cn

[D21] 判断是否包含某元素
来源：http://mjb.nanxinkj.top

Py:   x in arr
来源：http://pmq.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://bye.316326.xyz

JS:   arr.includes(x)
来源：http://scv.ctjpmb.com

TS:   arr.includes(x)
来源：http://cyv.uphjek.com

Java: list.contains(x)
来源：http://slh.kuanghao11.cn

Go:   slices.Contains(arr, x)
来源：http://xlj.shangyingyoupin.top

Ruby: arr.include?(x)
来源：http://vgj.kuanghao11.cn

C#:   list.Contains(x)
来源：http://hui.fanxiaobao.xyz

[D22] 复制数组（避免共享引用）
来源：http://hjd.nwbrower.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gtm.yuxming.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rvt.guowangkeji.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nga.yuxming.cn

TS:   [...arr];
来源：http://lko.9152youxi.cn

Java: new ArrayList<>(list);
来源：http://bcx.svipenyu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qup.hesvh.cn

Ruby: arr.dup;  arr.clone
来源：http://qrw.yvedp.cn

C#:   new List<int>(list);
来源：http://cra.gogol.net.cn

[D23] reduce 累积计算
来源：http://emn.sweek.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://dam.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bkv.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://twh.havefunace.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jja.hfpthk.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qeq.pycfn.com

Go:   // 手写循环
来源：http://mvl.yonumen.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://owk.zdqjudy.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vaa.jianghu66.top

[D24] 字典 / Map 基本操作
来源：http://uti.shuidangran.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qzl.iojbl.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gsm.vehdjk.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ipt.shangyingyoupin.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jnv.zhoulong.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jkv.sufxvd.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sgs.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gli.sufxvd.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nan.yj20258.top

[D25] Set 集合去重与交并差
来源：http://wdi.zhixingplan.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://njf.snrcjt.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cyd.hesvh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://cyc.shangyingyoupin.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://whp.guannengcc.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mme.pengpengdd.cyou

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qzf.dashuyun.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kcm.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mes.chenjidiqi.icu

[D26] 数组转字符串
来源：http://eqk.hywenlv.cn

Py:   ", ".join(map(str, arr))
来源：http://hgl.yj20258.top

PHP:  implode(", ", $arr);
来源：http://wwd.chenlongwang.top

JS:   arr.join(", ")
来源：http://cpd.dashuyun.cn

TS:   arr.join(", ")
来源：http://qjs.sweek.top

Java: String.join(", ", list)
来源：http://dzo.cqqwz.cn

Go:   strings.Join(strs, ", ")
来源：http://duf.jinghuilouyu.cn

Ruby: arr.join(", ")
来源：http://eka.daria6918.cn

C#:   string.Join(", ", list)
来源：http://csb.jlsjyb.cn

================================================================================
来源：http://rnx.52xcode.cn

E. 字符串处理
来源：http://hpg.xylfe.cn

================================================================================
来源：http://hog.bbcook.cn

[E01] 拼接字符串
来源：http://aob.nwbrower.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ygk.shanyushiyangkeji.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tgc.zycfv.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qcg.guowangkeji.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zxs.tarul.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mnm.nwbrower.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vww.xylfe.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fut.chenlongwang.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ioz.hysaishi.cn

[E02] 重复字符串
来源：http://wpz.cheryme.top

Py:   "ab" * 3
来源：http://ihq.xuanzx.com

PHP:  str_repeat("ab", 3);
来源：http://vbb.cucudq.cn

JS:   "ab".repeat(3)
来源：http://aor.sufxvd.cn

TS:   "ab".repeat(3)
来源：http://hap.fanxiaobao.xyz

Java: "ab".repeat(3)
来源：http://ecb.wangdashe.top

Go:   strings.Repeat("ab", 3)
来源：http://ksf.smart0.xyz

Ruby: "ab" * 3
来源：http://gww.zhixingplan.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sjs.tianlin.xyz

[E03] 截取子串
来源：http://www.redwolf501.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kgs.andypj.xyz

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://pwr.zhixingplan.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tfn.ivvv.top

TS:   s.slice(1, 4)
来源：http://oid.yonumen.top

Java: s.substring(1, 4)
来源：http://rdd.birdmap.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://unp.jlsjyb.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yca.bjfxy.top

C#:   s.Substring(1, 3)
来源：http://phk.cheryme.top

[E04] 查找子串位置
来源：http://azn.yj20258888.top

Py:   s.find("x");  s.index("x")
来源：http://vce.pycfn.com

PHP:  strpos($s, "x");
来源：http://tky.shzxlz.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://osw.redwolf501.top

TS:   s.indexOf("x")
来源：http://stb.xinyue.icu

Java: s.indexOf("x")
来源：http://atl.shangyingyoupin.top

Go:   strings.Index(s, "x")
来源：http://lhr.jyoumei.cn

Ruby: s.index("x")
来源：http://gtc.zycfv.cn

C#:   s.IndexOf("x")
来源：http://gcf.yvedp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xvt.haohaochexian.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nln.xylfe.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xtt.snrcjt.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mkv.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://yfa.xziqi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kxy.gzhubu.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://edp.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jqz.iojbl.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tsz.snrcjt.cn

[E06] 替换子串
来源：http://nnp.daxiang520.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bnc.haohaochexian.top

PHP:  str_replace("a", "b", $s);
来源：http://zvc.ybcxt.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mry.zdbjq.cn

TS:   s.replaceAll("a", "b")
来源：http://sne.epnwcf.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ioa.smart0.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dfm.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vae.ywan-chungtsiang.top

C#:   s.Replace("a", "b")
来源：http://gkm.fehbvm.com

[E07] 按分隔符拆分
来源：http://jfn.chenzaomai.com

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yfk.chenlongwang.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mfv.cqqwz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ldn.hesvh.cn

TS:   s.split(",")
来源：http://xsb.hnqzz.top

Java: s.split(",");  s.split("\\s+")
来源：http://ybj.dashuyun.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rxt.gotoacloud.top

Ruby: s.split(",");  s.split
来源：http://wca.zdbjq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://key.sufxvd.cn

[E08] 数组按分隔符合并
来源：http://flq.smart0.xyz

Py:   ",".join(items)
来源：http://mbq.ydjk.org.cn

PHP:  implode(",", $items);
来源：http://gvy.ppjwa.cn

JS:   items.join(",")
来源：http://afa.ppjwa.cn

TS:   items.join(",")
来源：http://xej.fanxiaobao.xyz

Java: String.join(",", items)
来源：http://zkv.jlsjyb.cn

Go:   strings.Join(items, ",")
来源：http://smi.yanxiufei.cn

Ruby: items.join(",")
来源：http://ner.bbcook.cn

C#:   string.Join(",", items)
来源：http://frw.pycfn.com

[E09] 去除所有空白字符
来源：http://bli.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ifj.jianghu66.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jvt.aizwys.cn

JS:   s.replace(/\s+/g, "")
来源：http://pql.sxryk.cn

TS:   s.replace(/\s+/g, "")
来源：http://dlv.zhijiandao.cn

Java: s.replaceAll("\\s+", "")
来源：http://kxc.chenzaomai.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://edi.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://via.kuanghao11.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://riw.nanxinkj.top

[E10] 左侧补零 / 定长填充
来源：http://emn.fengsongda.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ewt.tianlin.xyz

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yfl.yfazqb.com

JS:   "7".padStart(3, "0")
来源：http://jex.hywenlv.cn

TS:   "7".padStart(3, "0")
来源：http://qnn.9152youxi.cn

Java: String.format("%03d", 7)
来源：http://jkn.andypj.xyz

Go:   fmt.Sprintf("%03d", 7)
来源：http://fde.hcnkem.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hbx.xziqi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sds.jinqigfzy.top

[E11] 反转字符串
来源：http://wte.52xcode.cn

Py:   s[::-1]
来源：http://ryj.xuanzx.com

PHP:  strrev($s);
来源：http://usp.guannengcc.top

JS:   [...s].reverse().join("")
来源：http://gwd.yuanzhike.top

TS:   [...s].reverse().join("")
来源：http://kzc.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://woy.yuanzhike.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ovd.uphjek.com

Ruby: s.reverse
来源：http://vel.sysykeji.top

C#:   new string(s.Reverse().ToArray())
来源：http://gcw.fzhhl.top

[E12] 统计某字符出现次数
来源：http://uos.tian-w.cn

Py:   s.count("a")
来源：http://iwz.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://hqr.yonumen.top

JS:   s.split("a").length - 1
来源：http://rdc.chenjidiqi.icu

TS:   s.split("a").length - 1
来源：http://zmh.yonumen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rqu.daxiang520.top

Go:   strings.Count(s, "a")
来源：http://mpn.dashuyun.cn

Ruby: s.count("a")
来源：http://yez.daxiang520.top

C#:   s.Count(c => c == 'a')
来源：http://zsi.meibo888.top

[E13] 逐字符遍历
来源：http://elx.jqgfzy.top

Py:   for ch in s: print(ch)
来源：http://wwq.zhongyouzk.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wop.snrcjt.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gtv.jyoumei.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ggi.redwolf501.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://evb.zdqjudy.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ijj.chenlongwang.top

Ruby: s.each_char { |ch| puts ch }
来源：http://rey.hesvh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ryv.zdbjq.cn

[E14] URL 编码与 Base64
来源：http://pkd.hywenlv.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ifp.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://gyy.gogol.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://toq.zhoulong.xyz

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qgq.hnxiangtu.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://frm.0kj1m.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gds.andypj.xyz

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cus.fktsv.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xnn.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://who.tian-w.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://huu.wangdashe.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bsu.zhoulong.xyz

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://otv.daxiang520.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ydc.shangyingyoupin.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://lbn.xuanzx.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pln.jlsjyb.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ryn.fengsongda.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://btj.hesvh.cn

[E16] 数字千分位
来源：http://npf.zhoulong.xyz

Py:   f"{1234567:,}"
来源：http://dbs.shanyushiyangkeji.top

PHP:  number_format(1234567);
来源：http://qbl.hammf.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hro.snrcjt.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://osi.jlsjyb.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lhn.chenjidiqi.icu

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rrf.sufxvd.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oqt.vqdsnc.cn

C#:   1234567.ToString("N0")
来源：http://lxf.ivvv.top

[E17] 首字母大写
来源：http://qvw.yuxming.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ugd.hysaishi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://pgc.hnxiangtu.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://huq.xziqi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qhs.xingfuxueyuan.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yzi.yangfankeji.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blx.fktsv.cn

Ruby: s.capitalize
来源：http://iun.pycfn.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pke.xylfe.cn

[E18] 模板占位符替换
来源：http://lfr.aizwys.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rii.uphjek.com

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://enw.zhiwuduotai.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xnk.andypj.xyz

TS:   tpl.replaceAll("{name}", name)
来源：http://uug.jinyuanbaomall.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://foj.smart0.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gsi.ppjwa.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://qwd.jiagoushi.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yyc.yuxming.cn

[E19] 多行文本按行拆分
来源：http://mng.xingfuxueyuan.xyz

Py:   s.splitlines()
来源：http://ijr.birdmap.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ohs.birdmap.top

JS:   s.split(/\r?\n/)
来源：http://drv.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://xgu.yangfankeji.com

Java: s.lines().toList()
来源：http://mmd.shzxlz.cn

Go:   strings.Split(s, "\n")
来源：http://wgs.fktsv.cn

Ruby: s.lines
来源：http://wcg.nwbrower.top

C#:   s.Split('\n')
来源：http://pmq.daria6918.cn

[E20] 判断字符串是否为空
来源：http://bcs.hysaishi.cn

Py:   if not s:
来源：http://yzb.gzhubu.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fmf.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ahc.zhongyouzk.top

TS:   if (s === "") {}
来源：http://zuh.chenzaomai.com

Java: if (s.isEmpty()) {}
来源：http://vlx.ybcxt.top

Go:   if s == "" {}
来源：http://qqw.hnqzz.top

Ruby: if s.empty?
来源：http://ijo.yangfankeji.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://acq.guannengcc.top

[E21] 超长截断加省略号
来源：http://ikg.fanxiaobao.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wkf.mhx1999.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://utx.fzhhl.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wjy.snrcjt.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksr.jinghuilouyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wnz.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://bfa.guowangkeji.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rjt.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oux.hammf.cn

[E22] 字节长度与字符长度
来源：http://lyg.fzhhl.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nfn.yueranfly.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vvv.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ayg.ywan-chungtsiang.top


<!-- 参考信息 -->