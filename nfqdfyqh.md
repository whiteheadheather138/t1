代发 wailian999

C#:   list.Distinct().ToList()
来源：http://nfj.gogol.net.cn

[D16] 求和与平均值
来源：http://xpa.fktsv.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cup.zhoulong.xyz

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ksr.hnxiangtu.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lxi.tianlin.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jmv.jiagoushi.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nil.sysykeji.top

Go:   // 手写循环累加
来源：http://ond.shuidangran.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wdh.vehdjk.com

C#:   list.Sum();  list.Average()
来源：http://vlh.nwbrower.top

[D17] 最大值与最小值
来源：http://pvi.smart0.xyz

Py:   max(arr);  min(arr)
来源：http://jww.hfpthk.cn

PHP:  max($arr);  min($arr);
来源：http://kaw.haohaochexian.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mjp.hysaishi.cn

TS:   Math.max(...arr);
来源：http://auc.cdnleiting.top

Java: Collections.max(list);  Collections.min(list);
来源：http://aud.guannengcc.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pbk.9152youxi.cn

Ruby: arr.max;  arr.min
来源：http://uam.jqgufenzy.top

C#:   list.Max();  list.Min()
来源：http://hxz.hysaishi.cn

[D18] 扁平化嵌套数组
来源：http://uqp.ctjpmb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://any.birdmap.top

PHP:  array_merge(...$nested);
来源：http://izw.havefunace.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://iiu.cdnleiting.top

TS:   nested.flat();
来源：http://dli.bjfxy.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://plo.wangshuangyany.cn

Go:   // 手写双层循环
来源：http://qxs.pengpengdd.cyou

Ruby: nested.flatten
来源：http://glc.hesvh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qtv.wangdashe.top

[D19] 按字段分组
来源：http://mos.sweek.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://uao.smart0.xyz

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://eyh.feifeiyinyue.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://koo.yanxiufei.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ynb.yj202588.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nhc.gotoacloud.top

Go:   // 手写 map[string][]T
来源：http://sec.nanxinkj.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://jfr.zhongyouzk.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vqb.wangshuangyany.cn

[D20] 统计每个元素出现次数
来源：http://znz.ehwqpu.com

Py:   Counter(arr)
来源：http://pqb.nanxinkj.top

PHP:  array_count_values($arr);
来源：http://moi.meibo888.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aak.daria6918.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sjv.nanxinkj.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sih.shanyushiyangtech.top

Go:   // 手写 map[T]int
来源：http://giq.dashuyun.cn

Ruby: arr.tally
来源：http://dnn.tianlin.xyz

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qhx.fanxiaobao.xyz

[D21] 判断是否包含某元素
来源：http://vxb.yuxming.cn

Py:   x in arr
来源：http://iwl.dianchejie.cn

PHP:  in_array($x, $arr, true);
来源：http://ngn.yfazqb.com

JS:   arr.includes(x)
来源：http://nyn.yuanzhike.top

TS:   arr.includes(x)
来源：http://ifd.vqdsnc.cn

Java: list.contains(x)
来源：http://yun.redwolf501.top

Go:   slices.Contains(arr, x)
来源：http://rjh.vqdsnc.cn

Ruby: arr.include?(x)
来源：http://dnr.yuanzhike.top

C#:   list.Contains(x)
来源：http://mlz.ywan-chungtsiang.top

[D22] 复制数组（避免共享引用）
来源：http://ttc.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nyv.cdnleiting.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://eon.cdnleiting.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hhx.shzxlz.cn

TS:   [...arr];
来源：http://juu.jinyuanbaomall.cn

Java: new ArrayList<>(list);
来源：http://hvd.vqdsnc.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oiy.haohaochexian.top

Ruby: arr.dup;  arr.clone
来源：http://dni.bjfxy.top

C#:   new List<int>(list);
来源：http://oaf.gzhubu.top

[D23] reduce 累积计算
来源：http://tlu.yj20258888.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hho.ivvv.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xgz.aibaodan.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eqm.shanyushiyangtech.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tmi.shzxlz.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zty.cheryme.top

Go:   // 手写循环
来源：http://jue.daria6918.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fvp.zhongyouzk.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pml.zdbjq.cn

[D24] 字典 / Map 基本操作
来源：http://iam.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fqu.hywenlv.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lln.sufxvd.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dvq.yueranfly.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://feu.ywan-chungtsiang.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://obx.kuanghao11.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://udo.fktsv.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kas.hcnkem.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lsm.yj20258888.top

[D25] Set 集合去重与交并差
来源：http://bqy.fengsongda.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fei.tianlin.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wre.kuanghao11.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yjb.fktsv.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fst.jianghu66.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://rcq.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zzh.cqqwz.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ymm.ctjpmb.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ukf.redwolf501.top

[D26] 数组转字符串
来源：http://vju.tarul.cn

Py:   ", ".join(map(str, arr))
来源：http://yid.jlsjyb.cn

PHP:  implode(", ", $arr);
来源：http://dwv.guannengcc.top

JS:   arr.join(", ")
来源：http://lbm.yuanzhike.top

TS:   arr.join(", ")
来源：http://cwk.yuanzhike.top

Java: String.join(", ", list)
来源：http://yud.zhixingplan.top

Go:   strings.Join(strs, ", ")
来源：http://xjn.shanyushiyangtech.top

Ruby: arr.join(", ")
来源：http://gdd.xziqi.cn

C#:   string.Join(", ", list)
来源：http://vpm.hysaishi.cn

================================================================================
来源：http://nxq.birdmap.top

E. 字符串处理
来源：http://imb.c1oappe.top

================================================================================
来源：http://fwd.quarkkingdee.top

[E01] 拼接字符串
来源：http://fef.ivvv.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fjp.shangyingyoupin.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://xof.wangshuangyany.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nqm.fzhhl.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pkw.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sec.sweek.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://adt.svipenyu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://iwe.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://srp.ehwqpu.com

[E02] 重复字符串
来源：http://eed.c1oappe.top

Py:   "ab" * 3
来源：http://etg.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://luh.shangyingyoupin.top

JS:   "ab".repeat(3)
来源：http://tgp.pycfn.com

TS:   "ab".repeat(3)
来源：http://lno.sjlbkw.cn

Java: "ab".repeat(3)
来源：http://pgh.0kj1m.cn

Go:   strings.Repeat("ab", 3)
来源：http://ycu.cqqwz.cn

Ruby: "ab" * 3
来源：http://evw.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rfu.gotoacloud.top

[E03] 截取子串
来源：http://oyg.tarul.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://thc.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gnl.feifeiyinyue.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pdj.yueranfly.top

TS:   s.slice(1, 4)
来源：http://inv.dianchejie.cn

Java: s.substring(1, 4)
来源：http://kqy.cdnleiting.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zii.fengsongda.top

Ruby: s[1, 3];  s[1..3]
来源：http://shd.pengpengdd.cyou

C#:   s.Substring(1, 3)
来源：http://wha.wangshuangyany.cn

[E04] 查找子串位置
来源：http://jjg.aibaodan.cn

Py:   s.find("x");  s.index("x")
来源：http://ugu.dashuyun.cn

PHP:  strpos($s, "x");
来源：http://udn.epnwcf.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bop.jiagoushi.top

TS:   s.indexOf("x")
来源：http://utm.nanxuanxn.top

Java: s.indexOf("x")
来源：http://jup.gzhubu.top

Go:   strings.Index(s, "x")
来源：http://mzm.wangshuangyany.cn

Ruby: s.index("x")
来源：http://xnz.birdmap.top

C#:   s.IndexOf("x")
来源：http://wpv.jinyuanbaomall.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dac.pycfn.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jzm.0kj1m.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mam.sysykeji.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mag.yvedp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://feo.feifeiyinyue.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vpa.hcnkem.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hjn.sweek.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pue.hnxiangtu.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://zsi.smart0.xyz

[E06] 替换子串
来源：http://dqm.zhaomingkeji.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bcc.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://rdp.smart0.xyz

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tsq.xinyue.icu

TS:   s.replaceAll("a", "b")
来源：http://hov.quarkkingdee.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qyy.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://jhh.daria6918.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tvo.ctjpmb.com

C#:   s.Replace("a", "b")
来源：http://yfl.c1oappe.top

[E07] 按分隔符拆分
来源：http://taj.shanyushiyangkeji.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wch.zhongyouzk.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wra.ywan-chungtsiang.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://tvg.shuidangran.top

TS:   s.split(",")
来源：http://bdb.nwbrower.top

Java: s.split(",");  s.split("\\s+")
来源：http://nvu.guowangkeji.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lgk.feifeiyinyue.top

Ruby: s.split(",");  s.split
来源：http://lsy.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sik.havefunace.top

[E08] 数组按分隔符合并
来源：http://zht.uphjek.com

Py:   ",".join(items)
来源：http://nsz.zycfv.cn

PHP:  implode(",", $items);
来源：http://abj.pengpengdd.cyou

JS:   items.join(",")
来源：http://pnv.yongpay.top

TS:   items.join(",")
来源：http://amv.bjfxy.top

Java: String.join(",", items)
来源：http://dsf.ehwqpu.com

Go:   strings.Join(items, ",")
来源：http://twg.dashuyun.cn

Ruby: items.join(",")
来源：http://kko.cashguo.top

C#:   string.Join(",", items)
来源：http://pqg.hywenlv.cn

[E09] 去除所有空白字符
来源：http://asd.feifeiyinyue.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lvp.gotoacloud.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xac.cdnleiting.top

JS:   s.replace(/\s+/g, "")
来源：http://gig.yvedp.cn

TS:   s.replace(/\s+/g, "")
来源：http://sss.nanxinkj.top

Java: s.replaceAll("\\s+", "")
来源：http://qyn.yueranfly.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ngp.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://hbz.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fdl.zhiwuduotai.top

[E10] 左侧补零 / 定长填充
来源：http://jjc.guowangkeji.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://izp.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nwl.jinyuanbaomall.cn

JS:   "7".padStart(3, "0")
来源：http://ztu.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://ikd.meibo888.top

Java: String.format("%03d", 7)
来源：http://uey.iojbl.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gfw.jyoumei.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jqc.yangfankeji.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qme.birdmap.top

[E11] 反转字符串
来源：http://mca.316326.xyz

Py:   s[::-1]
来源：http://jmg.haohaochexian.top

PHP:  strrev($s);
来源：http://wtg.9152youxi.cn

JS:   [...s].reverse().join("")
来源：http://kes.jinqigfzy.top

TS:   [...s].reverse().join("")
来源：http://mwb.tarul.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xyr.aibaodan.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lik.gaohongyu789.top

Ruby: s.reverse
来源：http://xtz.yj20258.top

C#:   new string(s.Reverse().ToArray())
来源：http://kfw.mhx1999.top

[E12] 统计某字符出现次数
来源：http://tno.jinqigfzy.top

Py:   s.count("a")
来源：http://bhb.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://vtn.yonumen.top

JS:   s.split("a").length - 1
来源：http://ilf.0kj1m.cn

TS:   s.split("a").length - 1
来源：http://dqk.zhaomingkeji.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ofs.tarul.cn

Go:   strings.Count(s, "a")
来源：http://frp.vqdsnc.cn

Ruby: s.count("a")
来源：http://yma.jinqigfzy.top

C#:   s.Count(c => c == 'a')
来源：http://tcq.meibo888.top

[E13] 逐字符遍历
来源：http://cio.jinyuanbaomall.cn

Py:   for ch in s: print(ch)
来源：http://yij.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://huv.quarkkingdee.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vfn.yj20258.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://odq.jqgufenzy.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://brw.smart0.xyz

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zkq.smart0.xyz

Ruby: s.each_char { |ch| puts ch }
来源：http://mja.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jer.birdmap.top

[E14] URL 编码与 Base64
来源：http://zvf.nanxinkj.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ljt.vehdjk.com

PHP:  urlencode($s);  base64_encode($s);
来源：http://jyy.ctjpmb.com

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fos.havefunace.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://jxe.0kj1m.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rda.jiagoushi.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iwl.yvedp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://man.svipenyu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wfc.bjfxy.top

[E15] HTML 转义 / 反转义
来源：http://kgk.jianghu66.top

Py:   html.escape(s);  html.unescape(s)
来源：http://dxq.fktsv.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://edi.tanke756.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fhz.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fyc.sjlbkw.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sqk.zdqjudy.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kkt.bjfxy.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://loe.shanyushiyangkeji.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mra.fktsv.cn

[E16] 数字千分位
来源：http://jip.52xcode.cn

Py:   f"{1234567:,}"
来源：http://jwd.gotoacloud.top

PHP:  number_format(1234567);
来源：http://nyj.xinyue.icu

JS:   (1234567).toLocaleString("en-US")
来源：http://dul.pycfn.com

TS:   (1234567).toLocaleString("en-US")
来源：http://hac.cheryme.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dip.hammf.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lkg.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vmd.tianlin.xyz

C#:   1234567.ToString("N0")
来源：http://tlq.hfpthk.cn

[E17] 首字母大写
来源：http://wrp.andypj.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ywl.fanxiaobao.xyz

PHP:  ucfirst($s);  ucwords($s);
来源：http://nvk.zycfv.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hyy.ppjwa.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dcs.yanxiufei.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://avv.guannengcc.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wnn.tianlin.xyz

Ruby: s.capitalize
来源：http://mnk.zdqjudy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hdh.hongshengwenyu.top

[E18] 模板占位符替换
来源：http://eav.quarkkingdee.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gxc.chenlongwang.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bdk.sjlbkw.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vnh.cashguo.top

TS:   tpl.replaceAll("{name}", name)
来源：http://ciy.andypj.xyz

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kbp.hnxiangtu.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iye.fengsongda.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://jdz.guannengcc.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vtm.svipenyu.cn

[E19] 多行文本按行拆分
来源：http://laz.tian-w.cn

Py:   s.splitlines()
来源：http://vug.gzhubu.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zqu.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://wag.hammf.cn

TS:   s.split(/\r?\n/)
来源：http://xmh.svipenyu.cn

Java: s.lines().toList()
来源：http://len.xinyue.icu

Go:   strings.Split(s, "\n")
来源：http://znz.gaohongyu789.top

Ruby: s.lines
来源：http://pyg.aizwys.cn

C#:   s.Split('\n')
来源：http://dug.cashguo.top

[E20] 判断字符串是否为空
来源：http://zxj.vehdjk.com

Py:   if not s:
来源：http://sxq.vqdsnc.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pnv.wangdashe.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hak.hnqzz.top

TS:   if (s === "") {}
来源：http://mck.kuanghao11.cn

Java: if (s.isEmpty()) {}
来源：http://dcb.vqdsnc.cn

Go:   if s == "" {}
来源：http://fid.xziqi.cn

Ruby: if s.empty?
来源：http://rgi.birdmap.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vyx.quarkkingdee.top

[E21] 超长截断加省略号
来源：http://mle.vqdsnc.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ede.c1oappe.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iki.chenzaomai.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zqv.quarkkingdee.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dnr.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yjj.zhengqikj.top

Go:   // 按 rune 判断长度后截断
来源：http://wvx.tarul.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jwk.tanke756.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rxg.mhx1999.top

[E22] 字节长度与字符长度
来源：http://nlx.yangfankeji.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qkn.zhongyouzk.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gfi.chenjidiqi.icu

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rsg.feifeiyinyue.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vcd.feifeiyinyue.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fib.xinyue.icu

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wim.yuanzhike.top

Ruby: s.bytesize;  s.length
来源：http://tfp.smart0.xyz


<!-- 参考信息 -->