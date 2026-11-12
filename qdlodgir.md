代发 wailian999

TS:   [...new Set(arr)]
来源：http://uwt.zdqjudy.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tdp.nanxinkj.top

Go:   // 用 map[T]struct{} 手写
来源：http://pbs.yfazqb.com

Ruby: arr.uniq
来源：http://pct.jqgufenzy.top

C#:   list.Distinct().ToList()
来源：http://xnn.zhongyouzk.top

[D16] 求和与平均值
来源：http://che.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yxg.9152youxi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qbz.jiagoushi.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fxc.birdmap.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zyj.zhijiandao.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pwi.9152youxi.cn

Go:   // 手写循环累加
来源：http://sja.kuanghao11.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pry.yuxming.cn

C#:   list.Sum();  list.Average()
来源：http://zqz.xuetiantiany.cn

[D17] 最大值与最小值
来源：http://uti.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://jeu.svipenyu.cn

PHP:  max($arr);  min($arr);
来源：http://tuc.hammf.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xau.sysykeji.top

TS:   Math.max(...arr);
来源：http://mui.jianghu66.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sqf.yueranfly.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zja.ywan-chungtsiang.top

Ruby: arr.max;  arr.min
来源：http://bja.chenlongwang.top

C#:   list.Max();  list.Min()
来源：http://ayt.yuxming.cn

[D18] 扁平化嵌套数组
来源：http://ewv.yfazqb.com

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://pdo.sxryk.cn

PHP:  array_merge(...$nested);
来源：http://tvw.yfazqb.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ohn.aizwys.cn

TS:   nested.flat();
来源：http://hyd.shangyingyoupin.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ltm.nanxinkj.top

Go:   // 手写双层循环
来源：http://dhp.jianghu66.top

Ruby: nested.flatten
来源：http://dcr.shangyingyoupin.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://kzf.svipenyu.cn

[D19] 按字段分组
来源：http://ijr.yvedp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qwm.yvedp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qcx.xinyue.icu

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hqo.chenzaomai.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://spn.yfazqb.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kix.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://rqa.c1oappe.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://xoh.yueranfly.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zqo.daxiang520.top

[D20] 统计每个元素出现次数
来源：http://eql.xuetiantiany.cn

Py:   Counter(arr)
来源：http://xap.tian-w.cn

PHP:  array_count_values($arr);
来源：http://txs.zhengqikj.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ava.yanxiufei.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bqd.nwbrower.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ctd.xziqi.cn

Go:   // 手写 map[T]int
来源：http://ynu.jlsjyb.cn

Ruby: arr.tally
来源：http://qwq.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://afq.shuidangran.top

[D21] 判断是否包含某元素
来源：http://bzd.bbcook.cn

Py:   x in arr
来源：http://rwz.havefunace.top

PHP:  in_array($x, $arr, true);
来源：http://pci.vqdsnc.cn

JS:   arr.includes(x)
来源：http://yhq.xylfe.cn

TS:   arr.includes(x)
来源：http://avp.chenzaomai.com

Java: list.contains(x)
来源：http://gax.sweek.top

Go:   slices.Contains(arr, x)
来源：http://gly.shanyushiyangkeji.top

Ruby: arr.include?(x)
来源：http://rle.pycfn.com

C#:   list.Contains(x)
来源：http://oyp.fktsv.cn

[D22] 复制数组（避免共享引用）
来源：http://lkk.yfazqb.com

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ovt.tian-w.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sbq.gaohongyu789.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dov.fanxiaobao.xyz

TS:   [...arr];
来源：http://spx.fanxiaobao.xyz

Java: new ArrayList<>(list);
来源：http://fmc.gzhubu.top

Go:   copied := append([]int(nil), arr...)
来源：http://nbd.aizwys.cn

Ruby: arr.dup;  arr.clone
来源：http://wsb.nanxinkj.top

C#:   new List<int>(list);
来源：http://hrv.zycfv.cn

[D23] reduce 累积计算
来源：http://fwc.hnqzz.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://nxq.cdnleiting.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xbs.ydjk.org.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aaf.wangshuangyany.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sdb.guowangkeji.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://hmw.ywan-chungtsiang.top

Go:   // 手写循环
来源：http://ddp.ppjwa.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wgx.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ywe.fengsongda.top

[D24] 字典 / Map 基本操作
来源：http://bha.mhx1999.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jyg.jlsjyb.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ptj.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lps.redwolf501.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nbn.hysaishi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://tis.sxryk.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://itb.meibo888.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xjx.yangfankeji.com

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://tkp.haohaochexian.top

[D25] Set 集合去重与交并差
来源：http://foa.jinghuilouyu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://bag.fengsongda.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wzc.gaohongyu789.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://njx.guowangkeji.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xma.52xcode.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nov.gogol.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qyj.xuanzx.com

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://rop.316326.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ciy.cheryme.top

[D26] 数组转字符串
来源：http://asp.yj202588.top

Py:   ", ".join(map(str, arr))
来源：http://fby.hongshengwenyu.top

PHP:  implode(", ", $arr);
来源：http://pct.jinqigufen.top

JS:   arr.join(", ")
来源：http://amu.jinqigfzy.top

TS:   arr.join(", ")
来源：http://mqv.fktsv.cn

Java: String.join(", ", list)
来源：http://lbx.xinyue.icu

Go:   strings.Join(strs, ", ")
来源：http://kit.bjfxy.top

Ruby: arr.join(", ")
来源：http://kpg.fanxiaobao.xyz

C#:   string.Join(", ", list)
来源：http://nyq.jinghuilouyu.cn

================================================================================
来源：http://bec.gogol.net.cn

E. 字符串处理
来源：http://ckt.yj202588.top

================================================================================
来源：http://ggv.cashguo.top

[E01] 拼接字符串
来源：http://bvd.xziqi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gbt.ppjwa.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hpa.svipenyu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://obv.fengsongda.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ajv.yanxiufei.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fkn.ivvv.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hjc.c1oappe.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mwa.cheryme.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://boq.jinqigfzy.top

[E02] 重复字符串
来源：http://snr.chenjidiqi.icu

Py:   "ab" * 3
来源：http://iye.cheryme.top

PHP:  str_repeat("ab", 3);
来源：http://kvm.fehbvm.com

JS:   "ab".repeat(3)
来源：http://llt.yj20258888.top

TS:   "ab".repeat(3)
来源：http://bii.tian-w.cn

Java: "ab".repeat(3)
来源：http://txv.ppjwa.cn

Go:   strings.Repeat("ab", 3)
来源：http://msj.uphjek.com

Ruby: "ab" * 3
来源：http://zio.cashguo.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://say.shanyushiyangkeji.top

[E03] 截取子串
来源：http://jup.jinqigfzy.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yjh.yuanzhike.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cam.xingfuxueyuan.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ynk.daxiang520.top

TS:   s.slice(1, 4)
来源：http://rkd.zhiwuduotai.top

Java: s.substring(1, 4)
来源：http://ssq.hesvh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tzq.dashuyun.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xmf.kuanghao11.cn

C#:   s.Substring(1, 3)
来源：http://tsu.ivvv.top

[E04] 查找子串位置
来源：http://uao.yongpay.top

Py:   s.find("x");  s.index("x")
来源：http://tkj.zdqjudy.top

PHP:  strpos($s, "x");
来源：http://wpa.hnqzz.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ets.feifeiyinyue.top

TS:   s.indexOf("x")
来源：http://bfp.hysaishi.cn

Java: s.indexOf("x")
来源：http://stn.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://fhg.andypj.xyz

Ruby: s.index("x")
来源：http://olw.yangfankeji.com

C#:   s.IndexOf("x")
来源：http://xtf.hnqzz.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://hhv.jyoumei.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://rsz.hammf.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://iol.yuanzhike.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tjl.hammf.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fao.ctjpmb.com

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zkm.tianlin.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wvg.andypj.xyz

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pgn.ehwqpu.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bmu.havefunace.top

[E06] 替换子串
来源：http://rnz.hnqzz.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sks.jinqigfzy.top

PHP:  str_replace("a", "b", $s);
来源：http://bts.9152youxi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xeb.hnxiangtu.top

TS:   s.replaceAll("a", "b")
来源：http://vkm.c1oappe.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bwa.nwbrower.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wyy.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hrx.cucudq.cn

C#:   s.Replace("a", "b")
来源：http://lra.chenjidiqi.icu

[E07] 按分隔符拆分
来源：http://sxu.wangdashe.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://utr.shuidangran.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://cmj.fanxiaobao.xyz

JS:   s.split(",");  s.split(/\s+/)
来源：http://sgv.andypj.xyz

TS:   s.split(",")
来源：http://rdm.shzxlz.cn

Java: s.split(",");  s.split("\\s+")
来源：http://icg.zycfv.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mxj.jyoumei.cn

Ruby: s.split(",");  s.split
来源：http://vzr.shzxlz.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xec.mhx1999.top

[E08] 数组按分隔符合并
来源：http://gvi.yfazqb.com

Py:   ",".join(items)
来源：http://ncf.ydzc1.top

PHP:  implode(",", $items);
来源：http://iwu.cdnleiting.top

JS:   items.join(",")
来源：http://usk.pycfn.com

TS:   items.join(",")
来源：http://yaq.tarul.cn

Java: String.join(",", items)
来源：http://anh.zdqjudy.top

Go:   strings.Join(items, ",")
来源：http://lob.jinghuilouyu.cn

Ruby: items.join(",")
来源：http://mrf.hesvh.cn

C#:   string.Join(",", items)
来源：http://tkn.sjlbkw.cn

[E09] 去除所有空白字符
来源：http://yzy.shzxlz.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qmc.xingfuxueyuan.xyz

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lrb.hongshengwenyu.top

JS:   s.replace(/\s+/g, "")
来源：http://set.zhixingplan.top

TS:   s.replace(/\s+/g, "")
来源：http://pmf.ehwqpu.com

Java: s.replaceAll("\\s+", "")
来源：http://luh.hnqzz.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://lur.hfpthk.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ttf.uphjek.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kls.zhongyouzk.top

[E10] 左侧补零 / 定长填充
来源：http://cjd.gzhubu.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rxa.hesvh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qmh.ehwqpu.com

JS:   "7".padStart(3, "0")
来源：http://jhc.zhaomingkeji.xyz

TS:   "7".padStart(3, "0")
来源：http://gqq.shanyushiyangtech.top

Java: String.format("%03d", 7)
来源：http://wen.tian-w.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qum.aibaodan.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zdf.chenlongwang.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bpd.xuetiantiany.cn

[E11] 反转字符串
来源：http://pzm.chenjidiqi.icu

Py:   s[::-1]
来源：http://ipe.fzhhl.top

PHP:  strrev($s);
来源：http://zth.316326.xyz

JS:   [...s].reverse().join("")
来源：http://sts.hongshengwenyu.top

TS:   [...s].reverse().join("")
来源：http://iiw.zhengqikj.top

Java: new StringBuilder(s).reverse().toString()
来源：http://mcm.shangyingyoupin.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://vca.mhx1999.top

Ruby: s.reverse
来源：http://vuu.zhoulong.xyz

C#:   new string(s.Reverse().ToArray())
来源：http://bnk.dashuyun.cn

[E12] 统计某字符出现次数
来源：http://baw.chenjidiqi.icu

Py:   s.count("a")
来源：http://qcz.tarul.cn

PHP:  substr_count($s, "a");
来源：http://fdq.zhongyouzk.top

JS:   s.split("a").length - 1
来源：http://usj.shangyingyoupin.top

TS:   s.split("a").length - 1
来源：http://jib.quarkkingdee.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wde.dianchejie.cn

Go:   strings.Count(s, "a")
来源：http://ayt.zhaomingkeji.xyz

Ruby: s.count("a")
来源：http://uqo.meibo888.top

C#:   s.Count(c => c == 'a')
来源：http://zwm.bjfxy.top

[E13] 逐字符遍历
来源：http://zcz.hnxiangtu.top

Py:   for ch in s: print(ch)
来源：http://aoi.cucudq.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cec.gzhubu.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://xgk.fengsongda.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://niq.cucudq.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fjq.kuanghao11.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ezw.mhx1999.top

Ruby: s.each_char { |ch| puts ch }
来源：http://klp.yuanzhike.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ztp.yuanzhike.top

[E14] URL 编码与 Base64
来源：http://qob.shzxlz.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hzc.ybcxt.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://nca.feifeiyinyue.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ede.nanxinkj.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gvo.andypj.xyz

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fuz.zhaomingkeji.xyz

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mkz.zycfv.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zxs.chenzaomai.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fpe.pengpengdd.cyou

[E15] HTML 转义 / 反转义
来源：http://pnt.52xcode.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gfi.daxiang520.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vvu.ywan-chungtsiang.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wbe.sxryk.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ojk.zdbjq.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xih.sjlbkw.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wfx.sweek.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://esh.aibaodan.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://otg.gaohongyu789.top

[E16] 数字千分位
来源：http://ggf.vehdjk.com

Py:   f"{1234567:,}"
来源：http://sbq.tianlin.xyz

PHP:  number_format(1234567);
来源：http://ryp.haohaochexian.top

JS:   (1234567).toLocaleString("en-US")
来源：http://mhx.sweek.top

TS:   (1234567).toLocaleString("en-US")
来源：http://fgl.yuxming.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gkx.snrcjt.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nya.xinyue.icu

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aje.guannengcc.top

C#:   1234567.ToString("N0")
来源：http://nal.pengpengdd.cyou

[E17] 首字母大写
来源：http://rst.epnwcf.com

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://myn.yfazqb.com

PHP:  ucfirst($s);  ucwords($s);
来源：http://qml.haohaochexian.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bxt.yj20258.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ztv.fengsongda.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xcn.wangdashe.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sns.wangdashe.top

Ruby: s.capitalize
来源：http://rje.bjfxy.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oim.nanxuanxn.top

[E18] 模板占位符替换
来源：http://ayb.ppjwa.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dbe.tianlin.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yxl.daria6918.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qpy.jinqigufen.top

TS:   tpl.replaceAll("{name}", name)
来源：http://pil.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rqc.ehwqpu.com

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rhm.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oxl.wangdashe.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://grf.c1oappe.top

[E19] 多行文本按行拆分
来源：http://rif.tanke756.top

Py:   s.splitlines()
来源：http://crk.shzxlz.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qdy.yuxming.cn

JS:   s.split(/\r?\n/)
来源：http://zpa.zhixingplan.top

TS:   s.split(/\r?\n/)
来源：http://xwo.meibo888.top

Java: s.lines().toList()
来源：http://sgb.andypj.xyz

Go:   strings.Split(s, "\n")
来源：http://vlc.aizwys.cn

Ruby: s.lines
来源：http://rae.jinqigfzy.top

C#:   s.Split('\n')
来源：http://bvq.kuanghao11.cn

[E20] 判断字符串是否为空
来源：http://tsk.fehbvm.com

Py:   if not s:
来源：http://rtz.ywan-chungtsiang.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rsg.ydzc1.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jbf.jinyuanbaomall.cn

TS:   if (s === "") {}
来源：http://zot.nanxinkj.top

Java: if (s.isEmpty()) {}
来源：http://qtv.aizwys.cn

Go:   if s == "" {}
来源：http://anc.gaohongyu789.top

Ruby: if s.empty?
来源：http://qnw.snrcjt.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://rfy.hongshengwenyu.top

[E21] 超长截断加省略号
来源：http://aya.jlsjyb.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hoy.yfazqb.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dbw.hnxiangtu.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sdy.hongshengwenyu.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ovj.ydzc1.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mcb.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://fts.0kj1m.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fet.ydzc1.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fkh.ehwqpu.com

[E22] 字节长度与字符长度
来源：http://zjx.hcnkem.com

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lmb.hfpthk.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxa.smart0.xyz

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rhk.nanxuanxn.top


<!-- 参考信息 -->