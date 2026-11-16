代发 wailian999

[D15] 去重
来源：http://agz.zhixingplan.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ydp.yuxming.cn

PHP:  array_unique($arr);
来源：http://mkv.uphjek.com

JS:   [...new Set(arr)]
来源：http://stj.ctjpmb.com

TS:   [...new Set(arr)]
来源：http://xim.yvedp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mxq.fengsongda.top

Go:   // 用 map[T]struct{} 手写
来源：http://blg.birdmap.top

Ruby: arr.uniq
来源：http://iyl.jyoumei.cn

C#:   list.Distinct().ToList()
来源：http://bie.jinqigufen.top

[D16] 求和与平均值
来源：http://gzt.sufxvd.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gmr.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aqm.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mjd.dianchejie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ajz.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jdt.shanyushiyangkeji.top

Go:   // 手写循环累加
来源：http://nvb.hcnkem.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jqf.andypj.xyz

C#:   list.Sum();  list.Average()
来源：http://zih.zhoulong.xyz

[D17] 最大值与最小值
来源：http://vst.pycfn.com

Py:   max(arr);  min(arr)
来源：http://xvf.yongpay.top

PHP:  max($arr);  min($arr);
来源：http://uxc.gaohongyu789.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://tnf.nanxinkj.top

TS:   Math.max(...arr);
来源：http://pzf.jinqigfzy.top

Java: Collections.max(list);  Collections.min(list);
来源：http://kmt.shzxlz.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cgi.uphjek.com

Ruby: arr.max;  arr.min
来源：http://pvw.smart0.xyz

C#:   list.Max();  list.Min()
来源：http://bsn.fktsv.cn

[D18] 扁平化嵌套数组
来源：http://ylr.zycfv.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://svx.sjlbkw.cn

PHP:  array_merge(...$nested);
来源：http://uuu.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://irp.vehdjk.com

TS:   nested.flat();
来源：http://pro.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qmu.shanyushiyangkeji.top

Go:   // 手写双层循环
来源：http://xjn.yueranfly.top

Ruby: nested.flatten
来源：http://ywz.zycfv.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://spm.quarkkingdee.top

[D19] 按字段分组
来源：http://fnv.guannengcc.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tlt.ctjpmb.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ewz.sxryk.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kgd.xingfuxueyuan.xyz

TS:   Object.groupBy(arr, x => x.type)
来源：http://udz.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://iov.ivvv.top

Go:   // 手写 map[string][]T
来源：http://gtl.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://sco.yonumen.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xgp.hfpthk.cn

[D20] 统计每个元素出现次数
来源：http://zvr.ppjwa.cn

Py:   Counter(arr)
来源：http://wiz.hnxiangtu.top

PHP:  array_count_values($arr);
来源：http://qsg.havefunace.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ivr.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hil.uphjek.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hsz.snrcjt.cn

Go:   // 手写 map[T]int
来源：http://rhx.aibaodan.cn

Ruby: arr.tally
来源：http://jit.iojbl.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dah.wangshuangyany.cn

[D21] 判断是否包含某元素
来源：http://vzs.tanke756.top

Py:   x in arr
来源：http://fxq.cqqwz.cn

PHP:  in_array($x, $arr, true);
来源：http://yfu.jiagoushi.top

JS:   arr.includes(x)
来源：http://spg.zhiwuduotai.top

TS:   arr.includes(x)
来源：http://dqe.shanyushiyangkeji.top

Java: list.contains(x)
来源：http://jqq.xylfe.cn

Go:   slices.Contains(arr, x)
来源：http://mry.52xcode.cn

Ruby: arr.include?(x)
来源：http://xep.aibaodan.cn

C#:   list.Contains(x)
来源：http://mqe.bbcook.cn

[D22] 复制数组（避免共享引用）
来源：http://kaj.yanxiufei.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://myk.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rdb.smart0.xyz

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ecw.yuanzhike.top

TS:   [...arr];
来源：http://qhl.fzhhl.top

Java: new ArrayList<>(list);
来源：http://ysa.havefunace.top

Go:   copied := append([]int(nil), arr...)
来源：http://btu.nanxuanxn.top

Ruby: arr.dup;  arr.clone
来源：http://moa.yonumen.top

C#:   new List<int>(list);
来源：http://zjv.yueranfly.top

[D23] reduce 累积计算
来源：http://poi.hfpthk.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://jua.yuxming.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tri.smart0.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oze.fktsv.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hip.chenzaomai.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://fdg.uphjek.com

Go:   // 手写循环
来源：http://fii.hnxiangtu.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pcc.fzhhl.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qye.52xcode.cn

[D24] 字典 / Map 基本操作
来源：http://iqm.nanxuanxn.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ejy.52xcode.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qqy.chenjidiqi.icu

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pvx.kuanghao11.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gpx.yueranfly.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jsj.cqqwz.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://caq.iojbl.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jpm.mhx1999.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ytv.gogol.net.cn

[D25] Set 集合去重与交并差
来源：http://oco.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jfa.ywan-chungtsiang.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zzg.shanyushiyangkeji.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zic.hywenlv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cfa.sxryk.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vku.sufxvd.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://emq.yanxiufei.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lmf.nanxinkj.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://typ.cheryme.top

[D26] 数组转字符串
来源：http://hmr.xuanzx.com

Py:   ", ".join(map(str, arr))
来源：http://tjt.chenlongwang.top

PHP:  implode(", ", $arr);
来源：http://msm.smart0.xyz

JS:   arr.join(", ")
来源：http://goh.yuxming.cn

TS:   arr.join(", ")
来源：http://ykb.yuxming.cn

Java: String.join(", ", list)
来源：http://ean.fanxiaobao.xyz

Go:   strings.Join(strs, ", ")
来源：http://yvq.cheryme.top

Ruby: arr.join(", ")
来源：http://reo.shangyingyoupin.top

C#:   string.Join(", ", list)
来源：http://kzp.tanke756.top

================================================================================
来源：http://ssp.chenzaomai.com

E. 字符串处理
来源：http://anh.pycfn.com

================================================================================
来源：http://ouj.ivvv.top

[E01] 拼接字符串
来源：http://mbo.fanxiaobao.xyz

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ctc.zhongyouzk.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lfd.xuetiantiany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mow.zhengqikj.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://yfk.sufxvd.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hoa.guowangkeji.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ace.shangyingyoupin.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dez.snrcjt.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://syo.xuanzx.com

[E02] 重复字符串
来源：http://oja.iojbl.cn

Py:   "ab" * 3
来源：http://yuu.shanyushiyangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://edd.yueranfly.top

JS:   "ab".repeat(3)
来源：http://lnr.xinyue.icu

TS:   "ab".repeat(3)
来源：http://spi.daxiang520.top

Java: "ab".repeat(3)
来源：http://xhq.ivvv.top

Go:   strings.Repeat("ab", 3)
来源：http://gzx.wangshuangyany.cn

Ruby: "ab" * 3
来源：http://mng.hnxiangtu.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://asf.fehbvm.com

[E03] 截取子串
来源：http://utz.hnxiangtu.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jwt.9152youxi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kaj.tianlin.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://rln.fzhhl.top

TS:   s.slice(1, 4)
来源：http://jue.hfpthk.cn

Java: s.substring(1, 4)
来源：http://nml.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://clt.redwolf501.top

Ruby: s[1, 3];  s[1..3]
来源：http://zbt.jyoumei.cn

C#:   s.Substring(1, 3)
来源：http://bne.jqgufenzy.top

[E04] 查找子串位置
来源：http://ssw.bbcook.cn

Py:   s.find("x");  s.index("x")
来源：http://myv.hcnkem.com

PHP:  strpos($s, "x");
来源：http://pho.jlsjyb.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gjk.yj20258.top

TS:   s.indexOf("x")
来源：http://peo.bbcook.cn

Java: s.indexOf("x")
来源：http://cmb.feifeiyinyue.top

Go:   strings.Index(s, "x")
来源：http://ugu.vehdjk.com

Ruby: s.index("x")
来源：http://kgo.nanxuanxn.top

C#:   s.IndexOf("x")
来源：http://sxx.ydzc1.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://cwm.jinghuilouyu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qga.feifeiyinyue.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ers.tianlin.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lsy.ybcxt.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://xsi.yj202588.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lwt.pengpengdd.cyou

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xvt.uphjek.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ehv.wangshuangyany.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qov.tian-w.cn

[E06] 替换子串
来源：http://kfr.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xdf.smart0.xyz

PHP:  str_replace("a", "b", $s);
来源：http://wwp.ctjpmb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://won.jinyuanbaomall.cn

TS:   s.replaceAll("a", "b")
来源：http://wjm.shzxlz.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://amx.sjlbkw.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qbx.yongpay.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ohu.xuetiantiany.cn

C#:   s.Replace("a", "b")
来源：http://eqh.jinyuanbaomall.cn

[E07] 按分隔符拆分
来源：http://dzq.havefunace.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kei.dashuyun.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yei.zhijiandao.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xbu.zhengqikj.top

TS:   s.split(",")
来源：http://kvn.epnwcf.com

Java: s.split(",");  s.split("\\s+")
来源：http://oot.zhixingplan.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lrv.wangdashe.top

Ruby: s.split(",");  s.split
来源：http://zxo.shuidangran.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wgq.fengsongda.top

[E08] 数组按分隔符合并
来源：http://kcq.hesvh.cn

Py:   ",".join(items)
来源：http://rcd.cucudq.cn

PHP:  implode(",", $items);
来源：http://dvi.jinyuanbaomall.cn

JS:   items.join(",")
来源：http://vrd.dashuyun.cn

TS:   items.join(",")
来源：http://eom.sjlbkw.cn

Java: String.join(",", items)
来源：http://agw.zdbjq.cn

Go:   strings.Join(items, ",")
来源：http://nsp.yuanzhike.top

Ruby: items.join(",")
来源：http://xcq.hongshengwenyu.top

C#:   string.Join(",", items)
来源：http://tze.yonumen.top

[E09] 去除所有空白字符
来源：http://wnt.jqgfzy.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lsx.gogol.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vga.pycfn.com

JS:   s.replace(/\s+/g, "")
来源：http://joq.ehwqpu.com

TS:   s.replace(/\s+/g, "")
来源：http://wnf.sxryk.cn

Java: s.replaceAll("\\s+", "")
来源：http://tuq.tianlin.xyz

Go:   strings.Join(strings.Fields(s), "")
来源：http://xcp.jinqigufen.top

Ruby: s.gsub(/\s+/, "")
来源：http://blx.birdmap.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rbq.shangyingyoupin.top

[E10] 左侧补零 / 定长填充
来源：http://jta.ydjk.org.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fwp.havefunace.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tni.sjlbkw.cn

JS:   "7".padStart(3, "0")
来源：http://nut.bjfxy.top

TS:   "7".padStart(3, "0")
来源：http://biv.cucudq.cn

Java: String.format("%03d", 7)
来源：http://eks.daxiang520.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://pbq.gogol.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xkr.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zop.jinqigfzy.top

[E11] 反转字符串
来源：http://eyu.ybcxt.top

Py:   s[::-1]
来源：http://bgo.smart0.xyz

PHP:  strrev($s);
来源：http://akb.zhoulong.xyz

JS:   [...s].reverse().join("")
来源：http://owe.chenlongwang.top

TS:   [...s].reverse().join("")
来源：http://dow.nanxinkj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://aqw.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://oyx.jinqigfzy.top

Ruby: s.reverse
来源：http://ibe.0kj1m.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hyj.xuetiantiany.cn

[E12] 统计某字符出现次数
来源：http://hxl.hammf.cn

Py:   s.count("a")
来源：http://dwu.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://kyu.vqdsnc.cn

JS:   s.split("a").length - 1
来源：http://lmy.yj20258.top

TS:   s.split("a").length - 1
来源：http://wyq.wangshuangyany.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rgn.andypj.xyz

Go:   strings.Count(s, "a")
来源：http://gnl.xuetiantiany.cn

Ruby: s.count("a")
来源：http://muy.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://nzz.yuanzhike.top

[E13] 逐字符遍历
来源：http://zxk.gaohongyu789.top

Py:   for ch in s: print(ch)
来源：http://yyo.hnqzz.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mqd.jyoumei.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://omd.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://coz.zhiwuduotai.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vjw.yj20258.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ouo.hnxiangtu.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ajn.xylfe.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://poz.kuanghao11.cn

[E14] URL 编码与 Base64
来源：http://znn.ivvv.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://aro.chenjidiqi.icu

PHP:  urlencode($s);  base64_encode($s);
来源：http://oqz.wangshuangyany.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iig.tian-w.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://okt.hcnkem.com

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tot.mhx1999.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vbc.xuetiantiany.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bwi.zhixingplan.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pft.9152youxi.cn

[E15] HTML 转义 / 反转义
来源：http://pbx.vehdjk.com

Py:   html.escape(s);  html.unescape(s)
来源：http://hbb.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://flj.chenlongwang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ifv.cdnleiting.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rnk.tian-w.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vyl.fktsv.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wgl.ehwqpu.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dzg.xuetiantiany.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://iin.ivvv.top

[E16] 数字千分位
来源：http://lkc.ydzc1.top

Py:   f"{1234567:,}"
来源：http://ipp.mhx1999.top

PHP:  number_format(1234567);
来源：http://tmn.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://pig.fengsongda.top

TS:   (1234567).toLocaleString("en-US")
来源：http://usp.andypj.xyz

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://voe.pengpengdd.cyou

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ebc.jqgufenzy.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://inn.svipenyu.cn

C#:   1234567.ToString("N0")
来源：http://gxw.cqqwz.cn

[E17] 首字母大写
来源：http://bfx.ppjwa.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rbj.redwolf501.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://yso.guannengcc.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ugh.hammf.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bse.cheryme.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uym.hcnkem.com

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sig.52xcode.cn

Ruby: s.capitalize
来源：http://opk.fanxiaobao.xyz

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oua.zhongyouzk.top

[E18] 模板占位符替换
来源：http://gxq.pengpengdd.cyou

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gwp.tian-w.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tka.dashuyun.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oox.yvedp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://niu.guowangkeji.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://tzu.jinyuanbaomall.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mlb.cheryme.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dki.tanke756.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bya.yj20258.top

[E19] 多行文本按行拆分
来源：http://svi.zhijiandao.cn

Py:   s.splitlines()
来源：http://ded.shuidangran.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://epc.hammf.cn

JS:   s.split(/\r?\n/)
来源：http://vok.shanyushiyangtech.top

TS:   s.split(/\r?\n/)
来源：http://qgb.cqqwz.cn

Java: s.lines().toList()
来源：http://elp.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://xgl.jiagoushi.top

Ruby: s.lines
来源：http://hsg.guannengcc.top

C#:   s.Split('\n')
来源：http://znc.gogol.net.cn

[E20] 判断字符串是否为空
来源：http://aen.aizwys.cn

Py:   if not s:
来源：http://mtv.epnwcf.com

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sle.yuanzhike.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wlu.chenlongwang.top

TS:   if (s === "") {}
来源：http://xbd.xuanzx.com

Java: if (s.isEmpty()) {}
来源：http://nht.wangdashe.top

Go:   if s == "" {}
来源：http://bcd.jinqigfzy.top

Ruby: if s.empty?
来源：http://dez.hfpthk.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nno.zhiwuduotai.top

[E21] 超长截断加省略号
来源：http://gxa.shuidangran.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sye.chenlongwang.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://aiz.ywan-chungtsiang.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://drt.cqqwz.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dwh.hesvh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wat.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://dfc.fengsongda.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qpi.yonumen.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qks.tanke756.top


<!-- 参考信息 -->