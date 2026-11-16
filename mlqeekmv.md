代发 wailian999

TS:   [...new Set(arr)]
来源：http://mce.ppjwa.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ghv.kuanghao11.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rnk.andypj.xyz

Ruby: arr.uniq
来源：http://fdx.hywenlv.cn

C#:   list.Distinct().ToList()
来源：http://bad.jinghuilouyu.cn

[D16] 求和与平均值
来源：http://ieu.nwbrower.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bmo.ctjpmb.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://upm.yuanzhike.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zsx.hesvh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://kmj.yangfankeji.com

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dmp.sweek.top

Go:   // 手写循环累加
来源：http://zaz.hesvh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zvj.vqdsnc.cn

C#:   list.Sum();  list.Average()
来源：http://qhi.tarul.cn

[D17] 最大值与最小值
来源：http://ocb.cqqwz.cn

Py:   max(arr);  min(arr)
来源：http://qdo.aizwys.cn

PHP:  max($arr);  min($arr);
来源：http://jcm.ybcxt.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gwn.316326.xyz

TS:   Math.max(...arr);
来源：http://wov.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pgd.epnwcf.com

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ncr.jqgfzy.top

Ruby: arr.max;  arr.min
来源：http://ktg.redwolf501.top

C#:   list.Max();  list.Min()
来源：http://emt.zdqjudy.top

[D18] 扁平化嵌套数组
来源：http://cig.yueranfly.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xkt.fzhhl.top

PHP:  array_merge(...$nested);
来源：http://szx.mhx1999.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sqa.xuanzx.com

TS:   nested.flat();
来源：http://pqn.fengsongda.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lpb.hywenlv.cn

Go:   // 手写双层循环
来源：http://vsx.jlsjyb.cn

Ruby: nested.flatten
来源：http://udb.xingfuxueyuan.xyz

C#:   nested.SelectMany(x => x).ToList()
来源：http://qxi.jianghu66.top

[D19] 按字段分组
来源：http://pwc.hammf.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://epl.hfpthk.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rem.vehdjk.com

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://adv.nwbrower.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://izf.jqgfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qsg.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://ctd.jyoumei.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://izv.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eyk.andypj.xyz

[D20] 统计每个元素出现次数
来源：http://dkm.pycfn.com

Py:   Counter(arr)
来源：http://dos.ivvv.top

PHP:  array_count_values($arr);
来源：http://fdv.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tqy.yj202588.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hct.pengpengdd.cyou

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yei.xingfuxueyuan.xyz

Go:   // 手写 map[T]int
来源：http://sbs.yueranfly.top

Ruby: arr.tally
来源：http://hhc.jlsjyb.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fvt.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://ijd.jinghuilouyu.cn

Py:   x in arr
来源：http://mao.c1oappe.top

PHP:  in_array($x, $arr, true);
来源：http://miu.yanxiufei.cn

JS:   arr.includes(x)
来源：http://fwn.gotoacloud.top

TS:   arr.includes(x)
来源：http://rpm.yangfankeji.com

Java: list.contains(x)
来源：http://bsy.ppjwa.cn

Go:   slices.Contains(arr, x)
来源：http://tch.jinqigufen.top

Ruby: arr.include?(x)
来源：http://qza.chenzaomai.com

C#:   list.Contains(x)
来源：http://fws.feifeiyinyue.top

[D22] 复制数组（避免共享引用）
来源：http://usc.tian-w.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jtj.vqdsnc.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rwh.svipenyu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vdw.jinyuanbaomall.cn

TS:   [...arr];
来源：http://dgj.daria6918.cn

Java: new ArrayList<>(list);
来源：http://klm.chenlongwang.top

Go:   copied := append([]int(nil), arr...)
来源：http://cxg.mhx1999.top

Ruby: arr.dup;  arr.clone
来源：http://dio.zhongyouzk.top

C#:   new List<int>(list);
来源：http://eek.ivvv.top

[D23] reduce 累积计算
来源：http://hdg.cashguo.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zbx.xuetiantiany.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pye.chenlongwang.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gyj.sjlbkw.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gjj.hywenlv.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hjh.jianghu66.top

Go:   // 手写循环
来源：http://pfh.andypj.xyz

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://xyy.cucudq.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mab.pycfn.com

[D24] 字典 / Map 基本操作
来源：http://cye.cqqwz.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kpu.pengpengdd.cyou

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xin.gaohongyu789.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kbv.feifeiyinyue.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://its.gotoacloud.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://awy.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gyf.smart0.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ekz.shanyushiyangtech.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://khx.ybcxt.top

[D25] Set 集合去重与交并差
来源：http://poz.ctjpmb.com

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ude.sysykeji.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dqp.jiagoushi.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rzp.gzhubu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ngh.ctjpmb.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kvz.gotoacloud.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://nsj.tarul.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fpk.shanyushiyangtech.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kqa.nwbrower.top

[D26] 数组转字符串
来源：http://ppt.andypj.xyz

Py:   ", ".join(map(str, arr))
来源：http://qmb.yj202588.top

PHP:  implode(", ", $arr);
来源：http://dul.hywenlv.cn

JS:   arr.join(", ")
来源：http://ooa.gogol.net.cn

TS:   arr.join(", ")
来源：http://wix.gzhubu.top

Java: String.join(", ", list)
来源：http://zhy.jiagoushi.top

Go:   strings.Join(strs, ", ")
来源：http://nlx.andypj.xyz

Ruby: arr.join(", ")
来源：http://lfr.vqdsnc.cn

C#:   string.Join(", ", list)
来源：http://utb.dashuyun.cn

================================================================================
来源：http://qpk.snrcjt.cn

E. 字符串处理
来源：http://mnn.jianghu66.top

================================================================================
来源：http://ldh.fzhhl.top

[E01] 拼接字符串
来源：http://jkr.jiagoushi.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lwy.cqqwz.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yph.zdqjudy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tjc.xingfuxueyuan.xyz

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mhj.quarkkingdee.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://axy.tanke756.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ezm.jinqigfzy.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yfq.zycfv.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ldd.jlsjyb.cn

[E02] 重复字符串
来源：http://wql.jinqigufen.top

Py:   "ab" * 3
来源：http://sjw.dashuyun.cn

PHP:  str_repeat("ab", 3);
来源：http://cyy.gaohongyu789.top

JS:   "ab".repeat(3)
来源：http://qrf.ydjk.org.cn

TS:   "ab".repeat(3)
来源：http://ntz.ybcxt.top

Java: "ab".repeat(3)
来源：http://okx.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://hph.zdbjq.cn

Ruby: "ab" * 3
来源：http://htj.ehwqpu.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qkw.svipenyu.cn

[E03] 截取子串
来源：http://kbc.zhixingplan.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oen.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jle.ehwqpu.com

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ztv.chenjidiqi.icu

TS:   s.slice(1, 4)
来源：http://hag.hammf.cn

Java: s.substring(1, 4)
来源：http://hjy.zhixingplan.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qgt.daria6918.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gqp.cashguo.top

C#:   s.Substring(1, 3)
来源：http://vqw.yonumen.top

[E04] 查找子串位置
来源：http://dbs.nwbrower.top

Py:   s.find("x");  s.index("x")
来源：http://egz.haohaochexian.top

PHP:  strpos($s, "x");
来源：http://jdd.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://isw.xylfe.cn

TS:   s.indexOf("x")
来源：http://nba.redwolf501.top

Java: s.indexOf("x")
来源：http://gvd.ivvv.top

Go:   strings.Index(s, "x")
来源：http://ofd.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://jmr.wangdashe.top

C#:   s.IndexOf("x")
来源：http://jwp.fktsv.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ied.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ztr.zhiwuduotai.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ezm.zhixingplan.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xjc.fengsongda.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://ehy.yongpay.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zpa.birdmap.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lpv.jinyuanbaomall.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mai.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cav.zdqjudy.top

[E06] 替换子串
来源：http://ope.yj202588.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xph.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://bne.yfazqb.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://adl.hfpthk.cn

TS:   s.replaceAll("a", "b")
来源：http://pwe.xuanzx.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gsy.316326.xyz

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cgk.cheryme.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qjs.hnqzz.top

C#:   s.Replace("a", "b")
来源：http://qxk.tarul.cn

[E07] 按分隔符拆分
来源：http://lsc.bjfxy.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://emz.xinyue.icu

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zzd.jinqigfzy.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://cur.aizwys.cn

TS:   s.split(",")
来源：http://oeu.tanke756.top

Java: s.split(",");  s.split("\\s+")
来源：http://okh.xuetiantiany.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wqh.sysykeji.top

Ruby: s.split(",");  s.split
来源：http://aqz.hongshengwenyu.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://rtl.dianchejie.cn

[E08] 数组按分隔符合并
来源：http://edh.andypj.xyz

Py:   ",".join(items)
来源：http://app.tanke756.top

PHP:  implode(",", $items);
来源：http://cmj.sweek.top

JS:   items.join(",")
来源：http://uho.andypj.xyz

TS:   items.join(",")
来源：http://bhy.cucudq.cn

Java: String.join(",", items)
来源：http://dzk.gaohongyu789.top

Go:   strings.Join(items, ",")
来源：http://eps.havefunace.top

Ruby: items.join(",")
来源：http://yaj.wangshuangyany.cn

C#:   string.Join(",", items)
来源：http://ltf.mhx1999.top

[E09] 去除所有空白字符
来源：http://oox.yanxiufei.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bog.yuxming.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kcq.svipenyu.cn

JS:   s.replace(/\s+/g, "")
来源：http://pfj.bjfxy.top

TS:   s.replace(/\s+/g, "")
来源：http://fdp.xuetiantiany.cn

Java: s.replaceAll("\\s+", "")
来源：http://xdr.vehdjk.com

Go:   strings.Join(strings.Fields(s), "")
来源：http://tip.xinyue.icu

Ruby: s.gsub(/\s+/, "")
来源：http://gcr.hcnkem.com

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hxj.chenjidiqi.icu

[E10] 左侧补零 / 定长填充
来源：http://jsy.haohaochexian.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://chc.chenzaomai.com

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ksz.xingfuxueyuan.xyz

JS:   "7".padStart(3, "0")
来源：http://auo.ppjwa.cn

TS:   "7".padStart(3, "0")
来源：http://jrk.dianchejie.cn

Java: String.format("%03d", 7)
来源：http://xgn.shuidangran.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://evj.zhixingplan.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wrn.shzxlz.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://orj.tarul.cn

[E11] 反转字符串
来源：http://qug.daxiang520.top

Py:   s[::-1]
来源：http://mqp.cqqwz.cn

PHP:  strrev($s);
来源：http://eil.chenjidiqi.icu

JS:   [...s].reverse().join("")
来源：http://qvk.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://dea.svipenyu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fho.ehwqpu.com

Go:   // 转 []rune 后倒序再转回 string
来源：http://rup.jiagoushi.top

Ruby: s.reverse
来源：http://ibz.sjlbkw.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ith.yj20258.top

[E12] 统计某字符出现次数
来源：http://wgu.jqgufenzy.top

Py:   s.count("a")
来源：http://lgt.hysaishi.cn

PHP:  substr_count($s, "a");
来源：http://hxl.haohaochexian.top

JS:   s.split("a").length - 1
来源：http://xth.c1oappe.top

TS:   s.split("a").length - 1
来源：http://vwd.zdqjudy.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://whf.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://ryl.vehdjk.com

Ruby: s.count("a")
来源：http://mnc.hnqzz.top

C#:   s.Count(c => c == 'a')
来源：http://yzw.chenzaomai.com

[E13] 逐字符遍历
来源：http://eqr.dianchejie.cn

Py:   for ch in s: print(ch)
来源：http://ycn.jiagoushi.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hff.jianghu66.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zol.dianchejie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qyp.jinqigufen.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://yvx.hnqzz.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hzc.chenzaomai.com

Ruby: s.each_char { |ch| puts ch }
来源：http://dic.nwbrower.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pqr.52xcode.cn

[E14] URL 编码与 Base64
来源：http://phy.52xcode.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rwi.shuidangran.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://btt.ppjwa.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://cai.sysykeji.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rmk.gaohongyu789.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://luc.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vdt.zdqjudy.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pjt.ehwqpu.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bvl.c1oappe.top

[E15] HTML 转义 / 反转义
来源：http://rwu.yonumen.top

Py:   html.escape(s);  html.unescape(s)
来源：http://eyz.shangyingyoupin.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iwp.fengsongda.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wii.yj20258.top

TS:   // 同上，务必做 XSS 过滤
来源：http://eux.shuidangran.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wqf.hysaishi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jlb.cqqwz.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mxq.zhijiandao.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://voz.hfpthk.cn

[E16] 数字千分位
来源：http://ylp.hysaishi.cn

Py:   f"{1234567:,}"
来源：http://uqm.gaohongyu789.top

PHP:  number_format(1234567);
来源：http://hyl.xuetiantiany.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://haz.52xcode.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cll.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kxg.ydzc1.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ipg.zhengqikj.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kqk.shanyushiyangtech.top

C#:   1234567.ToString("N0")
来源：http://rda.zhongyouzk.top

[E17] 首字母大写
来源：http://ezz.nwbrower.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lsw.jinqigfzy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://hdv.9152youxi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jpu.hfpthk.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mks.316326.xyz

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pmf.birdmap.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ghc.ppjwa.cn

Ruby: s.capitalize
来源：http://jvi.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rrp.fktsv.cn

[E18] 模板占位符替换
来源：http://ahp.havefunace.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uky.ydjk.org.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://knd.vqdsnc.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yqm.meibo888.top

TS:   tpl.replaceAll("{name}", name)
来源：http://raj.zhongyouzk.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wcf.aibaodan.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vzx.quarkkingdee.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eez.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wjt.guannengcc.top

[E19] 多行文本按行拆分
来源：http://rvi.guannengcc.top

Py:   s.splitlines()
来源：http://wmh.fengsongda.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hqz.wangshuangyany.cn

JS:   s.split(/\r?\n/)
来源：http://ecx.fzhhl.top

TS:   s.split(/\r?\n/)
来源：http://rmu.cashguo.top

Java: s.lines().toList()
来源：http://vwv.gzhubu.top

Go:   strings.Split(s, "\n")
来源：http://eyl.hammf.cn

Ruby: s.lines
来源：http://rjo.feifeiyinyue.top

C#:   s.Split('\n')
来源：http://omp.aibaodan.cn

[E20] 判断字符串是否为空
来源：http://vvl.hongshengwenyu.top

Py:   if not s:
来源：http://ruk.snrcjt.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sbm.havefunace.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://npa.yanxiufei.cn

TS:   if (s === "") {}
来源：http://zkc.yfazqb.com

Java: if (s.isEmpty()) {}
来源：http://bxo.cqqwz.cn

Go:   if s == "" {}
来源：http://yqk.ydjk.org.cn

Ruby: if s.empty?
来源：http://xje.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lfh.hywenlv.cn

[E21] 超长截断加省略号
来源：http://ewt.jinqigfzy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ogk.xinyue.icu

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ojv.xziqi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fxv.wangshuangyany.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://itc.daria6918.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bhs.birdmap.top

Go:   // 按 rune 判断长度后截断
来源：http://wry.yj20258.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ndg.yanxiufei.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://icm.vqdsnc.cn

[E22] 字节长度与字符长度
来源：http://vsl.chenlongwang.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kbd.gotoacloud.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ezu.jiagoushi.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://stu.pycfn.com


<!-- 参考信息 -->