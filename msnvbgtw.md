代发 wailian999

C#:   list.Distinct().ToList()
来源：http://tuv.gogol.net.cn

[D16] 求和与平均值
来源：http://wmn.jlsjyb.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xyz.jiagoushi.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nhr.meibo888.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://eye.xuanzx.com

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wnx.hammf.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nzs.nwbrower.top

Go:   // 手写循环累加
来源：http://jev.yfazqb.com

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zzr.sjlbkw.cn

C#:   list.Sum();  list.Average()
来源：http://lrc.zhoulong.xyz

[D17] 最大值与最小值
来源：http://ior.zdqjudy.top

Py:   max(arr);  min(arr)
来源：http://ile.birdmap.top

PHP:  max($arr);  min($arr);
来源：http://edo.nwbrower.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vmk.gotoacloud.top

TS:   Math.max(...arr);
来源：http://rgu.jiagoushi.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ril.fanxiaobao.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ymo.jinghuilouyu.cn

Ruby: arr.max;  arr.min
来源：http://qfj.bjfxy.top

C#:   list.Max();  list.Min()
来源：http://aqj.hesvh.cn

[D18] 扁平化嵌套数组
来源：http://pzr.yvedp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://faw.chenzaomai.com

PHP:  array_merge(...$nested);
来源：http://vnl.zhaomingkeji.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://czx.yueranfly.top

TS:   nested.flat();
来源：http://vkj.kuanghao11.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mvz.zhiwuduotai.top

Go:   // 手写双层循环
来源：http://cds.hnxiangtu.top

Ruby: nested.flatten
来源：http://chm.ehwqpu.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://jfk.zdqjudy.top

[D19] 按字段分组
来源：http://qjb.jyoumei.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iet.hywenlv.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dvm.aizwys.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yae.gzhubu.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://xnr.ywan-chungtsiang.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wse.jinqigfzy.top

Go:   // 手写 map[string][]T
来源：http://bsw.ppjwa.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qdc.fktsv.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://exa.fktsv.cn

[D20] 统计每个元素出现次数
来源：http://igl.daria6918.cn

Py:   Counter(arr)
来源：http://wyv.shanyushiyangkeji.top

PHP:  array_count_values($arr);
来源：http://mcr.jqgfzy.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://euw.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lec.aizwys.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ycy.gaohongyu789.top

Go:   // 手写 map[T]int
来源：http://xgx.zhiwuduotai.top

Ruby: arr.tally
来源：http://esl.nanxuanxn.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nii.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://tst.xylfe.cn

Py:   x in arr
来源：http://dte.smart0.xyz

PHP:  in_array($x, $arr, true);
来源：http://psc.shanyushiyangkeji.top

JS:   arr.includes(x)
来源：http://cxt.daria6918.cn

TS:   arr.includes(x)
来源：http://waz.chenlongwang.top

Java: list.contains(x)
来源：http://pcc.ehwqpu.com

Go:   slices.Contains(arr, x)
来源：http://ybd.jinghuilouyu.cn

Ruby: arr.include?(x)
来源：http://fbm.feifeiyinyue.top

C#:   list.Contains(x)
来源：http://gvp.yuxming.cn

[D22] 复制数组（避免共享引用）
来源：http://kqg.bjfxy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://trc.xinyue.icu

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lzj.birdmap.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://aou.jqgufenzy.top

TS:   [...arr];
来源：http://pyv.hysaishi.cn

Java: new ArrayList<>(list);
来源：http://lwp.yfazqb.com

Go:   copied := append([]int(nil), arr...)
来源：http://yxd.zdqjudy.top

Ruby: arr.dup;  arr.clone
来源：http://cqg.hnxiangtu.top

C#:   new List<int>(list);
来源：http://naz.tanke756.top

[D23] reduce 累积计算
来源：http://ulp.feifeiyinyue.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sbr.jinghuilouyu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cfv.hysaishi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kvy.vehdjk.com

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://heu.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hrm.zhiwuduotai.top

Go:   // 手写循环
来源：http://apu.yj20258888.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gos.ywan-chungtsiang.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oye.snrcjt.cn

[D24] 字典 / Map 基本操作
来源：http://mpa.guowangkeji.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zjb.yueranfly.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jeq.ywan-chungtsiang.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://edz.cashguo.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://xwg.daria6918.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kjl.haohaochexian.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lqc.tian-w.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lzp.bjfxy.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dmb.zhaomingkeji.xyz

[D25] Set 集合去重与交并差
来源：http://yfw.fehbvm.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kui.sxryk.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rgg.cucudq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hyx.zhiwuduotai.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kgf.daria6918.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://trm.ctjpmb.com

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dnn.quarkkingdee.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kzb.gotoacloud.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://msm.ehwqpu.com

[D26] 数组转字符串
来源：http://gds.zdqjudy.top

Py:   ", ".join(map(str, arr))
来源：http://hdw.jiagoushi.top

PHP:  implode(", ", $arr);
来源：http://nhy.gaohongyu789.top

JS:   arr.join(", ")
来源：http://gsn.yfazqb.com

TS:   arr.join(", ")
来源：http://lva.zdbjq.cn

Java: String.join(", ", list)
来源：http://ffs.xziqi.cn

Go:   strings.Join(strs, ", ")
来源：http://gvv.meibo888.top

Ruby: arr.join(", ")
来源：http://ikz.fengsongda.top

C#:   string.Join(", ", list)
来源：http://hvm.ydjk.org.cn

================================================================================
来源：http://qgx.tian-w.cn

E. 字符串处理
来源：http://fes.bjfxy.top

================================================================================
来源：http://nmd.svipenyu.cn

[E01] 拼接字符串
来源：http://kbc.yfazqb.com

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://obe.sjlbkw.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pcm.ywan-chungtsiang.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://izd.zhongyouzk.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://tms.yongpay.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://moe.feifeiyinyue.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sht.zhoulong.xyz

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hfz.ctjpmb.com

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://two.havefunace.top

[E02] 重复字符串
来源：http://ely.yonumen.top

Py:   "ab" * 3
来源：http://byd.316326.xyz

PHP:  str_repeat("ab", 3);
来源：http://cww.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://nnb.shuidangran.top

TS:   "ab".repeat(3)
来源：http://hlm.jyoumei.cn

Java: "ab".repeat(3)
来源：http://ykj.dashuyun.cn

Go:   strings.Repeat("ab", 3)
来源：http://hgx.jinqigufen.top

Ruby: "ab" * 3
来源：http://uqd.cucudq.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wjd.xingfuxueyuan.xyz

[E03] 截取子串
来源：http://brr.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kxk.jinghuilouyu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ebe.zhongyouzk.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dxm.cqqwz.cn

TS:   s.slice(1, 4)
来源：http://erg.hammf.cn

Java: s.substring(1, 4)
来源：http://bsa.fzhhl.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ttl.bjfxy.top

Ruby: s[1, 3];  s[1..3]
来源：http://gpo.zhixingplan.top

C#:   s.Substring(1, 3)
来源：http://bav.ivvv.top

[E04] 查找子串位置
来源：http://ddf.zdqjudy.top

Py:   s.find("x");  s.index("x")
来源：http://ccy.yj20258.top

PHP:  strpos($s, "x");
来源：http://mom.ydjk.org.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jlk.andypj.xyz

TS:   s.indexOf("x")
来源：http://hpm.yj20258888.top

Java: s.indexOf("x")
来源：http://vne.tarul.cn

Go:   strings.Index(s, "x")
来源：http://qfo.yonumen.top

Ruby: s.index("x")
来源：http://dwa.aizwys.cn

C#:   s.IndexOf("x")
来源：http://zxn.zhongyouzk.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://eix.daxiang520.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cbz.tarul.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://aar.hcnkem.com

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ppj.zhixingplan.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://lyx.hesvh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ozp.sxryk.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bie.jinghuilouyu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hlp.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iln.snrcjt.cn

[E06] 替换子串
来源：http://tdj.zhoulong.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jle.52xcode.cn

PHP:  str_replace("a", "b", $s);
来源：http://tzm.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lnb.zycfv.cn

TS:   s.replaceAll("a", "b")
来源：http://ygw.316326.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ivp.wangshuangyany.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://igp.jqgufenzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ogw.kuanghao11.cn

C#:   s.Replace("a", "b")
来源：http://pgc.xuanzx.com

[E07] 按分隔符拆分
来源：http://jko.bbcook.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kqt.bbcook.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ikf.yangfankeji.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://auv.epnwcf.com

TS:   s.split(",")
来源：http://fjy.hesvh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pnj.cqqwz.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://int.yanxiufei.cn

Ruby: s.split(",");  s.split
来源：http://kpr.bjfxy.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://biu.316326.xyz

[E08] 数组按分隔符合并
来源：http://ixb.jinghuilouyu.cn

Py:   ",".join(items)
来源：http://hsr.9152youxi.cn

PHP:  implode(",", $items);
来源：http://uln.jqgfzy.top

JS:   items.join(",")
来源：http://hcz.hammf.cn

TS:   items.join(",")
来源：http://sin.jyoumei.cn

Java: String.join(",", items)
来源：http://jzq.ydjk.org.cn

Go:   strings.Join(items, ",")
来源：http://cmd.daria6918.cn

Ruby: items.join(",")
来源：http://hrb.yuanzhike.top

C#:   string.Join(",", items)
来源：http://vlm.gogol.net.cn

[E09] 去除所有空白字符
来源：http://zjl.nanxinkj.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uaz.sjlbkw.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mbh.aibaodan.cn

JS:   s.replace(/\s+/g, "")
来源：http://ppt.jqgfzy.top

TS:   s.replace(/\s+/g, "")
来源：http://hcp.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://fnr.fehbvm.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://wbo.zhoulong.xyz

Ruby: s.gsub(/\s+/, "")
来源：http://spk.vehdjk.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oqd.jqgufenzy.top

[E10] 左侧补零 / 定长填充
来源：http://rol.xuetiantiany.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bhg.cashguo.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://iqv.nwbrower.top

JS:   "7".padStart(3, "0")
来源：http://prv.jianghu66.top

TS:   "7".padStart(3, "0")
来源：http://qwu.fengsongda.top

Java: String.format("%03d", 7)
来源：http://uya.xylfe.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lvl.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dwt.vqdsnc.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ceg.sjlbkw.cn

[E11] 反转字符串
来源：http://ncz.wangdashe.top

Py:   s[::-1]
来源：http://qbz.andypj.xyz

PHP:  strrev($s);
来源：http://pdm.hcnkem.com

JS:   [...s].reverse().join("")
来源：http://wey.gaohongyu789.top

TS:   [...s].reverse().join("")
来源：http://uaz.epnwcf.com

Java: new StringBuilder(s).reverse().toString()
来源：http://fcs.daxiang520.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://wwi.xuetiantiany.cn

Ruby: s.reverse
来源：http://lrs.jinghuilouyu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gaw.vqdsnc.cn

[E12] 统计某字符出现次数
来源：http://kba.quarkkingdee.top

Py:   s.count("a")
来源：http://pnu.sysykeji.top

PHP:  substr_count($s, "a");
来源：http://jqs.yvedp.cn

JS:   s.split("a").length - 1
来源：http://hvv.yj20258888.top

TS:   s.split("a").length - 1
来源：http://kps.ehwqpu.com

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lnc.xylfe.cn

Go:   strings.Count(s, "a")
来源：http://vzn.yonumen.top

Ruby: s.count("a")
来源：http://qrl.iojbl.cn

C#:   s.Count(c => c == 'a')
来源：http://mkg.bbcook.cn

[E13] 逐字符遍历
来源：http://gbj.iojbl.cn

Py:   for ch in s: print(ch)
来源：http://ohl.hongshengwenyu.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jwl.xziqi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cxq.yuxming.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tef.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jol.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xgy.guowangkeji.top

Ruby: s.each_char { |ch| puts ch }
来源：http://zwg.shanyushiyangtech.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bgb.jlsjyb.cn

[E14] URL 编码与 Base64
来源：http://mrl.gotoacloud.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cjg.zhijiandao.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tjs.jqgfzy.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mmy.cdnleiting.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nni.xingfuxueyuan.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://crf.xuanzx.com

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rfn.cdnleiting.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://spk.hongshengwenyu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://znp.wangdashe.top

[E15] HTML 转义 / 反转义
来源：http://zme.zycfv.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://otg.uphjek.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://byu.quarkkingdee.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://drn.feifeiyinyue.top

TS:   // 同上，务必做 XSS 过滤
来源：http://zvh.xingfuxueyuan.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kzm.aibaodan.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ovk.tarul.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tgq.fanxiaobao.xyz

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pth.hesvh.cn

[E16] 数字千分位
来源：http://cpr.yuxming.cn

Py:   f"{1234567:,}"
来源：http://eqx.ydjk.org.cn

PHP:  number_format(1234567);
来源：http://swy.smart0.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://kyg.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://yek.ydjk.org.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qvz.svipenyu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qhp.haohaochexian.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nql.gaohongyu789.top

C#:   1234567.ToString("N0")
来源：http://bso.haohaochexian.top

[E17] 首字母大写
来源：http://kjr.316326.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://odp.hfpthk.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://owb.shangyingyoupin.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vwd.zdqjudy.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tlg.dashuyun.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ieq.yj202588.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jnz.yvedp.cn

Ruby: s.capitalize
来源：http://til.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://byj.nanxuanxn.top

[E18] 模板占位符替换
来源：http://ica.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cfp.jyoumei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fkj.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://twl.zdbjq.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ito.hongshengwenyu.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ijf.0kj1m.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nmv.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vma.birdmap.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ujj.52xcode.cn

[E19] 多行文本按行拆分
来源：http://gly.yj20258.top

Py:   s.splitlines()
来源：http://wru.aizwys.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yce.havefunace.top

JS:   s.split(/\r?\n/)
来源：http://jgl.shzxlz.cn

TS:   s.split(/\r?\n/)
来源：http://fue.0kj1m.cn

Java: s.lines().toList()
来源：http://srj.chenzaomai.com

Go:   strings.Split(s, "\n")
来源：http://gkr.fzhhl.top

Ruby: s.lines
来源：http://rup.cucudq.cn

C#:   s.Split('\n')
来源：http://eml.yueranfly.top

[E20] 判断字符串是否为空
来源：http://kre.zdqjudy.top

Py:   if not s:
来源：http://pyq.nanxinkj.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ger.dashuyun.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vqz.zhaomingkeji.xyz

TS:   if (s === "") {}
来源：http://tjq.uphjek.com

Java: if (s.isEmpty()) {}
来源：http://mkz.jqgfzy.top

Go:   if s == "" {}
来源：http://sje.zdbjq.cn

Ruby: if s.empty?
来源：http://zxc.jinqigufen.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dtr.havefunace.top

[E21] 超长截断加省略号
来源：http://rac.smart0.xyz

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iby.fanxiaobao.xyz

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://duu.yj20258888.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bih.birdmap.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gel.mhx1999.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://clw.mhx1999.top

Go:   // 按 rune 判断长度后截断
来源：http://jpe.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sbd.ctjpmb.com

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ulk.zhengqikj.top

[E22] 字节长度与字符长度
来源：http://hdg.xylfe.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kbo.yonumen.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwb.tarul.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fph.yonumen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://svt.yongpay.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pwx.zhiwuduotai.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://amy.meibo888.top

Ruby: s.bytesize;  s.length
来源：http://umd.shanyushiyangtech.top


<!-- 参考信息 -->