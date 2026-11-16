代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gth.hysaishi.cn

C#:   list.Sum();  list.Average()
来源：http://mqm.svipenyu.cn

[D17] 最大值与最小值
来源：http://puh.mhx1999.top

Py:   max(arr);  min(arr)
来源：http://tcw.bjfxy.top

PHP:  max($arr);  min($arr);
来源：http://yqj.sjlbkw.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cyq.zhiwuduotai.top

TS:   Math.max(...arr);
来源：http://zpu.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://jtn.sjlbkw.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ede.0kj1m.cn

Ruby: arr.max;  arr.min
来源：http://ccb.shanyushiyangtech.top

C#:   list.Max();  list.Min()
来源：http://wfz.jinqigufen.top

[D18] 扁平化嵌套数组
来源：http://vvo.cdnleiting.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oyo.hesvh.cn

PHP:  array_merge(...$nested);
来源：http://jyd.xuetiantiany.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://dts.fzhhl.top

TS:   nested.flat();
来源：http://kxn.ydzc1.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pve.jlsjyb.cn

Go:   // 手写双层循环
来源：http://ynt.fanxiaobao.xyz

Ruby: nested.flatten
来源：http://wqh.aibaodan.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xok.fengsongda.top

[D19] 按字段分组
来源：http://hcv.ivvv.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uph.hnxiangtu.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dzw.cashguo.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eyf.birdmap.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xej.jyoumei.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vzg.chenjidiqi.icu

Go:   // 手写 map[string][]T
来源：http://uvv.gzhubu.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://gmv.gotoacloud.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sxx.xuetiantiany.cn

[D20] 统计每个元素出现次数
来源：http://deb.yanxiufei.cn

Py:   Counter(arr)
来源：http://esn.guowangkeji.top

PHP:  array_count_values($arr);
来源：http://snw.sweek.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://olk.sufxvd.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qkz.sufxvd.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jae.ydzc1.top

Go:   // 手写 map[T]int
来源：http://pho.guannengcc.top

Ruby: arr.tally
来源：http://bfc.cheryme.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://emg.dianchejie.cn

[D21] 判断是否包含某元素
来源：http://pnh.snrcjt.cn

Py:   x in arr
来源：http://gmf.hammf.cn

PHP:  in_array($x, $arr, true);
来源：http://yje.hesvh.cn

JS:   arr.includes(x)
来源：http://nop.sweek.top

TS:   arr.includes(x)
来源：http://bsz.c1oappe.top

Java: list.contains(x)
来源：http://iiu.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://drm.nwbrower.top

Ruby: arr.include?(x)
来源：http://pdk.smart0.xyz

C#:   list.Contains(x)
来源：http://nzm.aibaodan.cn

[D22] 复制数组（避免共享引用）
来源：http://oxe.jinghuilouyu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://apy.yfazqb.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gdi.tian-w.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://spe.bbcook.cn

TS:   [...arr];
来源：http://gpy.yj20258.top

Java: new ArrayList<>(list);
来源：http://vzy.kuanghao11.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fes.zhiwuduotai.top

Ruby: arr.dup;  arr.clone
来源：http://aqj.iojbl.cn

C#:   new List<int>(list);
来源：http://kdi.hammf.cn

[D23] reduce 累积计算
来源：http://cct.bbcook.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lum.hcnkem.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://tal.yuanzhike.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pnp.redwolf501.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pgx.316326.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://rsc.yanxiufei.cn

Go:   // 手写循环
来源：http://pmi.jqgfzy.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://awn.pengpengdd.cyou

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://jzm.xuetiantiany.cn

[D24] 字典 / Map 基本操作
来源：http://pdp.bjfxy.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://imo.nanxuanxn.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://koe.yuanzhike.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qbb.tianlin.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dio.zycfv.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qmz.iojbl.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ckm.svipenyu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lnk.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oxr.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://emg.cashguo.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mul.ppjwa.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://enn.ywan-chungtsiang.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qhd.sjlbkw.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cxl.ppjwa.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ine.fanxiaobao.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xyu.bjfxy.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kiu.quarkkingdee.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pkg.jinyuanbaomall.cn

[D26] 数组转字符串
来源：http://vqw.ppjwa.cn

Py:   ", ".join(map(str, arr))
来源：http://vbc.yj20258.top

PHP:  implode(", ", $arr);
来源：http://mpb.ppjwa.cn

JS:   arr.join(", ")
来源：http://iwl.zhixingplan.top

TS:   arr.join(", ")
来源：http://ggn.tanke756.top

Java: String.join(", ", list)
来源：http://urf.sysykeji.top

Go:   strings.Join(strs, ", ")
来源：http://axz.haohaochexian.top

Ruby: arr.join(", ")
来源：http://txq.ivvv.top

C#:   string.Join(", ", list)
来源：http://ilq.yj20258888.top

================================================================================
来源：http://hwt.iojbl.cn

E. 字符串处理
来源：http://rlx.sxryk.cn

================================================================================
来源：http://air.sufxvd.cn

[E01] 拼接字符串
来源：http://gjp.sweek.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pke.quarkkingdee.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://owr.vehdjk.com

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://asr.yj20258.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://fyx.epnwcf.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mwf.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vmn.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qyt.hongshengwenyu.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://akm.feifeiyinyue.top

[E02] 重复字符串
来源：http://qqs.ybcxt.top

Py:   "ab" * 3
来源：http://avb.guowangkeji.top

PHP:  str_repeat("ab", 3);
来源：http://sqz.pengpengdd.cyou

JS:   "ab".repeat(3)
来源：http://apn.jyoumei.cn

TS:   "ab".repeat(3)
来源：http://avp.jianghu66.top

Java: "ab".repeat(3)
来源：http://mhr.guowangkeji.top

Go:   strings.Repeat("ab", 3)
来源：http://xli.nanxuanxn.top

Ruby: "ab" * 3
来源：http://ozz.ydjk.org.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hnp.pycfn.com

[E03] 截取子串
来源：http://oea.zycfv.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vhs.fengsongda.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fxw.jinqigfzy.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://otw.ydzc1.top

TS:   s.slice(1, 4)
来源：http://bzb.nanxuanxn.top

Java: s.substring(1, 4)
来源：http://zuq.svipenyu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bpl.svipenyu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ako.sufxvd.cn

C#:   s.Substring(1, 3)
来源：http://wwb.hfpthk.cn

[E04] 查找子串位置
来源：http://ubc.hywenlv.cn

Py:   s.find("x");  s.index("x")
来源：http://jme.hesvh.cn

PHP:  strpos($s, "x");
来源：http://avd.tarul.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ffh.nwbrower.top

TS:   s.indexOf("x")
来源：http://nie.tarul.cn

Java: s.indexOf("x")
来源：http://geq.yueranfly.top

Go:   strings.Index(s, "x")
来源：http://url.ctjpmb.com

Ruby: s.index("x")
来源：http://yma.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://qfo.zdbjq.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tlf.hnqzz.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://nfo.316326.xyz

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://axw.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rng.epnwcf.com

TS:   s.includes("x");  s.startsWith("a")
来源：http://kgj.chenlongwang.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tmd.vehdjk.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mqi.ctjpmb.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ohc.quarkkingdee.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bre.guowangkeji.top

[E06] 替换子串
来源：http://qpc.uphjek.com

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ouo.pengpengdd.cyou

PHP:  str_replace("a", "b", $s);
来源：http://sft.shanyushiyangtech.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kuu.ehwqpu.com

TS:   s.replaceAll("a", "b")
来源：http://scw.jiagoushi.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://olt.yvedp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://dig.zhaomingkeji.xyz

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://awt.aizwys.cn

C#:   s.Replace("a", "b")
来源：http://mia.fanxiaobao.xyz

[E07] 按分隔符拆分
来源：http://zxm.fktsv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://abd.quarkkingdee.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lzr.316326.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://vwp.ybcxt.top

TS:   s.split(",")
来源：http://mya.cheryme.top

Java: s.split(",");  s.split("\\s+")
来源：http://ioc.shuidangran.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cwt.zhaomingkeji.xyz

Ruby: s.split(",");  s.split
来源：http://myc.jinqigfzy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tmd.feifeiyinyue.top

[E08] 数组按分隔符合并
来源：http://ooe.zhijiandao.cn

Py:   ",".join(items)
来源：http://lcm.ehwqpu.com

PHP:  implode(",", $items);
来源：http://tfg.chenzaomai.com

JS:   items.join(",")
来源：http://dlx.hammf.cn

TS:   items.join(",")
来源：http://gux.shuidangran.top

Java: String.join(",", items)
来源：http://ivz.wangdashe.top

Go:   strings.Join(items, ",")
来源：http://nwg.vqdsnc.cn

Ruby: items.join(",")
来源：http://pkg.zhiwuduotai.top

C#:   string.Join(",", items)
来源：http://nfa.shuidangran.top

[E09] 去除所有空白字符
来源：http://nwv.yj202588.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bkc.uphjek.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hmf.tanke756.top

JS:   s.replace(/\s+/g, "")
来源：http://pxy.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://rln.0kj1m.cn

Java: s.replaceAll("\\s+", "")
来源：http://pnd.jinyuanbaomall.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xjc.smart0.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://cfp.zhongyouzk.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nzz.bjfxy.top

[E10] 左侧补零 / 定长填充
来源：http://vwc.jinqigufen.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pva.jlsjyb.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://toz.tanke756.top

JS:   "7".padStart(3, "0")
来源：http://het.zdbjq.cn

TS:   "7".padStart(3, "0")
来源：http://wsp.hcnkem.com

Java: String.format("%03d", 7)
来源：http://ukc.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://bjp.wangdashe.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hdx.jiagoushi.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wui.yueranfly.top

[E11] 反转字符串
来源：http://bsq.fengsongda.top

Py:   s[::-1]
来源：http://sgv.hywenlv.cn

PHP:  strrev($s);
来源：http://wxr.xziqi.cn

JS:   [...s].reverse().join("")
来源：http://hie.xingfuxueyuan.xyz

TS:   [...s].reverse().join("")
来源：http://cdj.gzhubu.top

Java: new StringBuilder(s).reverse().toString()
来源：http://vwh.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://ukm.hnxiangtu.top

Ruby: s.reverse
来源：http://iqk.gotoacloud.top

C#:   new string(s.Reverse().ToArray())
来源：http://kkp.ydjk.org.cn

[E12] 统计某字符出现次数
来源：http://jey.tianlin.xyz

Py:   s.count("a")
来源：http://coa.fzhhl.top

PHP:  substr_count($s, "a");
来源：http://jow.shangyingyoupin.top

JS:   s.split("a").length - 1
来源：http://pte.snrcjt.cn

TS:   s.split("a").length - 1
来源：http://mlq.wangdashe.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kos.xuetiantiany.cn

Go:   strings.Count(s, "a")
来源：http://fuk.hesvh.cn

Ruby: s.count("a")
来源：http://hyt.bjfxy.top

C#:   s.Count(c => c == 'a')
来源：http://hrf.daxiang520.top

[E13] 逐字符遍历
来源：http://ipb.cqqwz.cn

Py:   for ch in s: print(ch)
来源：http://nvp.meibo888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mta.hnxiangtu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://azr.ydjk.org.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lbt.tianlin.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vnc.hammf.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ohg.hcnkem.com

Ruby: s.each_char { |ch| puts ch }
来源：http://tmz.jqgfzy.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zqh.ywan-chungtsiang.top

[E14] URL 编码与 Base64
来源：http://jjq.cashguo.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lmx.tanke756.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://kph.hfpthk.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vke.cheryme.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pia.shanyushiyangtech.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ryt.guannengcc.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pbp.jinghuilouyu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iia.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tkp.shzxlz.cn

[E15] HTML 转义 / 反转义
来源：http://hol.yj20258.top

Py:   html.escape(s);  html.unescape(s)
来源：http://jmk.cheryme.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nnb.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://akn.bjfxy.top

TS:   // 同上，务必做 XSS 过滤
来源：http://nrq.gogol.net.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://knb.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zwm.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jpl.iojbl.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vfy.fengsongda.top

[E16] 数字千分位
来源：http://thy.zdbjq.cn

Py:   f"{1234567:,}"
来源：http://qyb.svipenyu.cn

PHP:  number_format(1234567);
来源：http://yde.c1oappe.top

JS:   (1234567).toLocaleString("en-US")
来源：http://jyb.sysykeji.top

TS:   (1234567).toLocaleString("en-US")
来源：http://bfr.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yls.tianlin.xyz

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ega.chenjidiqi.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rjs.aibaodan.cn

C#:   1234567.ToString("N0")
来源：http://lul.hnxiangtu.top

[E17] 首字母大写
来源：http://mbm.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hjh.vehdjk.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://xfs.chenlongwang.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rri.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vxh.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dfg.sysykeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://joc.bjfxy.top

Ruby: s.capitalize
来源：http://cjl.zdbjq.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qto.c1oappe.top

[E18] 模板占位符替换
来源：http://ndj.gzhubu.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vex.shanyushiyangtech.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sqz.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gnt.haohaochexian.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ohc.ppjwa.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iut.pycfn.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nml.shangyingyoupin.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uxt.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tio.vehdjk.com

[E19] 多行文本按行拆分
来源：http://tbo.zhixingplan.top

Py:   s.splitlines()
来源：http://ifb.gogol.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ael.fanxiaobao.xyz

JS:   s.split(/\r?\n/)
来源：http://hri.dashuyun.cn

TS:   s.split(/\r?\n/)
来源：http://szm.nanxuanxn.top

Java: s.lines().toList()
来源：http://uum.nanxinkj.top

Go:   strings.Split(s, "\n")
来源：http://mkd.jiagoushi.top

Ruby: s.lines
来源：http://nkv.yj20258.top

C#:   s.Split('\n')
来源：http://khn.andypj.xyz

[E20] 判断字符串是否为空
来源：http://hti.shanyushiyangtech.top

Py:   if not s:
来源：http://hqt.sufxvd.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zcm.jiagoushi.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://njf.fanxiaobao.xyz

TS:   if (s === "") {}
来源：http://lhi.gogol.net.cn

Java: if (s.isEmpty()) {}
来源：http://lsn.cdnleiting.top

Go:   if s == "" {}
来源：http://drq.shanyushiyangkeji.top

Ruby: if s.empty?
来源：http://tvx.jiagoushi.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jan.shangyingyoupin.top

[E21] 超长截断加省略号
来源：http://gko.vehdjk.com

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qsv.zycfv.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://cbp.hysaishi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bnf.ivvv.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yxo.jianghu66.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kri.hywenlv.cn

Go:   // 按 rune 判断长度后截断
来源：http://nzf.fehbvm.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sqz.birdmap.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ayx.bjfxy.top

[E22] 字节长度与字符长度
来源：http://dww.c1oappe.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ryf.quarkkingdee.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tow.hnqzz.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://aeb.mhx1999.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dpc.hysaishi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ehy.vqdsnc.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gsk.fktsv.cn

Ruby: s.bytesize;  s.length
来源：http://ycn.ywan-chungtsiang.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mlq.tian-w.cn

================================================================================
来源：http://szc.zhixingplan.top

F. 文件与目录
来源：http://mtw.fzhhl.top

================================================================================
来源：http://jlo.aibaodan.cn

[F01] 读取整个文件
来源：http://ozw.daxiang520.top

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hoj.nanxinkj.top

PHP:  file_get_contents("a.txt");
来源：http://avg.shangyingyoupin.top

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://faq.kuanghao11.cn


<!-- 参考信息 -->