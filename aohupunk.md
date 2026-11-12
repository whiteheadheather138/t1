代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ddf.bjfxy.top

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zth.haohaochexian.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cra.ppjwa.cn

Go:   // 手写循环累加
来源：http://bfr.zycfv.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://emd.jinqigfzy.top

C#:   list.Sum();  list.Average()
来源：http://tnt.cqqwz.cn

[D17] 最大值与最小值
来源：http://hsn.cdnleiting.top

Py:   max(arr);  min(arr)
来源：http://mji.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://aqw.hywenlv.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sct.gogol.net.cn

TS:   Math.max(...arr);
来源：http://ine.pycfn.com

Java: Collections.max(list);  Collections.min(list);
来源：http://fdy.tian-w.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xfi.epnwcf.com

Ruby: arr.max;  arr.min
来源：http://pqe.aizwys.cn

C#:   list.Max();  list.Min()
来源：http://wfc.0kj1m.cn

[D18] 扁平化嵌套数组
来源：http://efy.nwbrower.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mhf.guannengcc.top

PHP:  array_merge(...$nested);
来源：http://ofo.shuidangran.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gsh.yj202588.top

TS:   nested.flat();
来源：http://ggi.ybcxt.top

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wlu.ywan-chungtsiang.top

Go:   // 手写双层循环
来源：http://nhb.shzxlz.cn

Ruby: nested.flatten
来源：http://gww.bjfxy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://rig.hfpthk.cn

[D19] 按字段分组
来源：http://ilm.sysykeji.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://iql.jlsjyb.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yic.jinqigufen.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cuu.52xcode.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://udv.kuanghao11.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dpt.quarkkingdee.top

Go:   // 手写 map[string][]T
来源：http://sdb.zycfv.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://azb.yangfankeji.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zpb.yuxming.cn

[D20] 统计每个元素出现次数
来源：http://tdx.nanxuanxn.top

Py:   Counter(arr)
来源：http://zuq.nanxuanxn.top

PHP:  array_count_values($arr);
来源：http://qgb.vqdsnc.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tbz.fanxiaobao.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mmv.zhijiandao.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tbg.zhoulong.xyz

Go:   // 手写 map[T]int
来源：http://kef.hnxiangtu.top

Ruby: arr.tally
来源：http://qit.52xcode.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aiv.zhoulong.xyz

[D21] 判断是否包含某元素
来源：http://xfb.nwbrower.top

Py:   x in arr
来源：http://csl.yonumen.top

PHP:  in_array($x, $arr, true);
来源：http://apd.jiagoushi.top

JS:   arr.includes(x)
来源：http://jxl.shangyingyoupin.top

TS:   arr.includes(x)
来源：http://ldi.jqgufenzy.top

Java: list.contains(x)
来源：http://aam.feifeiyinyue.top

Go:   slices.Contains(arr, x)
来源：http://nqf.quarkkingdee.top

Ruby: arr.include?(x)
来源：http://ulm.hammf.cn

C#:   list.Contains(x)
来源：http://nnp.uphjek.com

[D22] 复制数组（避免共享引用）
来源：http://ixy.dianchejie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yjd.nanxuanxn.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://tis.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://nnl.bjfxy.top

TS:   [...arr];
来源：http://urj.tianlin.xyz

Java: new ArrayList<>(list);
来源：http://rtv.fanxiaobao.xyz

Go:   copied := append([]int(nil), arr...)
来源：http://xgx.9152youxi.cn

Ruby: arr.dup;  arr.clone
来源：http://qxt.aizwys.cn

C#:   new List<int>(list);
来源：http://lif.jinghuilouyu.cn

[D23] reduce 累积计算
来源：http://kbd.wangshuangyany.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://few.fehbvm.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://oxa.pycfn.com

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://abx.hammf.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iqu.mhx1999.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://iuu.zhixingplan.top

Go:   // 手写循环
来源：http://doq.dashuyun.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zvs.xingfuxueyuan.xyz

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ygl.tian-w.cn

[D24] 字典 / Map 基本操作
来源：http://rpq.svipenyu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://frx.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://uls.jinqigufen.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://efp.zhoulong.xyz

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rov.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://odq.jyoumei.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://grq.dashuyun.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bxo.xuetiantiany.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dnq.gotoacloud.top

[D25] Set 集合去重与交并差
来源：http://jwp.shzxlz.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yak.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sab.xziqi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lfs.hnxiangtu.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zlc.jinghuilouyu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://avp.guowangkeji.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mcb.xylfe.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gct.tianlin.xyz

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zov.0kj1m.cn

[D26] 数组转字符串
来源：http://tlx.wangdashe.top

Py:   ", ".join(map(str, arr))
来源：http://izw.vqdsnc.cn

PHP:  implode(", ", $arr);
来源：http://myc.xinyue.icu

JS:   arr.join(", ")
来源：http://sky.sweek.top

TS:   arr.join(", ")
来源：http://xgm.sweek.top

Java: String.join(", ", list)
来源：http://iph.jqgfzy.top

Go:   strings.Join(strs, ", ")
来源：http://pbl.hcnkem.com

Ruby: arr.join(", ")
来源：http://fsx.yanxiufei.cn

C#:   string.Join(", ", list)
来源：http://hvh.yuanzhike.top

================================================================================
来源：http://ikq.tianlin.xyz

E. 字符串处理
来源：http://kcs.xuetiantiany.cn

================================================================================
来源：http://thk.vqdsnc.cn

[E01] 拼接字符串
来源：http://vqc.yongpay.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gqp.yanxiufei.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sge.andypj.xyz

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://erc.xziqi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zyl.aizwys.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://aew.fengsongda.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ovn.0kj1m.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lyv.dianchejie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://umw.guannengcc.top

[E02] 重复字符串
来源：http://jwr.xziqi.cn

Py:   "ab" * 3
来源：http://fhz.xinyue.icu

PHP:  str_repeat("ab", 3);
来源：http://hvq.zhiwuduotai.top

JS:   "ab".repeat(3)
来源：http://kts.zhaomingkeji.xyz

TS:   "ab".repeat(3)
来源：http://cut.ywan-chungtsiang.top

Java: "ab".repeat(3)
来源：http://nkl.ydzc1.top

Go:   strings.Repeat("ab", 3)
来源：http://ypk.fehbvm.com

Ruby: "ab" * 3
来源：http://uty.hammf.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qya.0kj1m.cn

[E03] 截取子串
来源：http://wrp.shangyingyoupin.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nhk.hnqzz.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zct.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jqg.hcnkem.com

TS:   s.slice(1, 4)
来源：http://xyy.vehdjk.com

Java: s.substring(1, 4)
来源：http://dpt.c1oappe.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ufm.wangdashe.top

Ruby: s[1, 3];  s[1..3]
来源：http://cns.smart0.xyz

C#:   s.Substring(1, 3)
来源：http://vzv.guowangkeji.top

[E04] 查找子串位置
来源：http://jpi.ydzc1.top

Py:   s.find("x");  s.index("x")
来源：http://irm.andypj.xyz

PHP:  strpos($s, "x");
来源：http://yev.gzhubu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tdi.yuanzhike.top

TS:   s.indexOf("x")
来源：http://kzz.fanxiaobao.xyz

Java: s.indexOf("x")
来源：http://njr.uphjek.com

Go:   strings.Index(s, "x")
来源：http://eir.yonumen.top

Ruby: s.index("x")
来源：http://mau.yj202588.top

C#:   s.IndexOf("x")
来源：http://rmx.hnxiangtu.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://rzm.gzhubu.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wzu.zdbjq.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eax.ywan-chungtsiang.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uim.fktsv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://vde.aizwys.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qeu.fehbvm.com

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zya.cashguo.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vsu.cheryme.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lik.quarkkingdee.top

[E06] 替换子串
来源：http://lin.pengpengdd.cyou

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://miw.ybcxt.top

PHP:  str_replace("a", "b", $s);
来源：http://gxz.quarkkingdee.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qox.havefunace.top

TS:   s.replaceAll("a", "b")
来源：http://lmw.yanxiufei.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lei.haohaochexian.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://loi.fktsv.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ove.sweek.top

C#:   s.Replace("a", "b")
来源：http://kgt.jinqigufen.top

[E07] 按分隔符拆分
来源：http://rji.zhongyouzk.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://guw.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eab.fktsv.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://inc.52xcode.cn

TS:   s.split(",")
来源：http://vsd.shuidangran.top

Java: s.split(",");  s.split("\\s+")
来源：http://ezb.daxiang520.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ezo.ppjwa.cn

Ruby: s.split(",");  s.split
来源：http://itt.xylfe.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zxw.kuanghao11.cn

[E08] 数组按分隔符合并
来源：http://gml.chenlongwang.top

Py:   ",".join(items)
来源：http://yro.shzxlz.cn

PHP:  implode(",", $items);
来源：http://dyv.hfpthk.cn

JS:   items.join(",")
来源：http://pxm.ydjk.org.cn

TS:   items.join(",")
来源：http://kyl.aibaodan.cn

Java: String.join(",", items)
来源：http://jrk.shangyingyoupin.top

Go:   strings.Join(items, ",")
来源：http://zko.hnqzz.top

Ruby: items.join(",")
来源：http://edx.pycfn.com

C#:   string.Join(",", items)
来源：http://wqh.haohaochexian.top

[E09] 去除所有空白字符
来源：http://rvi.uphjek.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lcc.birdmap.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ybr.ywan-chungtsiang.top

JS:   s.replace(/\s+/g, "")
来源：http://rfa.meibo888.top

TS:   s.replace(/\s+/g, "")
来源：http://uwr.dianchejie.cn

Java: s.replaceAll("\\s+", "")
来源：http://qkm.xuetiantiany.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://exm.shangyingyoupin.top

Ruby: s.gsub(/\s+/, "")
来源：http://fta.jianghu66.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://weg.meibo888.top

[E10] 左侧补零 / 定长填充
来源：http://cek.jqgfzy.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://six.fzhhl.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nyi.gogol.net.cn

JS:   "7".padStart(3, "0")
来源：http://jgk.jqgufenzy.top

TS:   "7".padStart(3, "0")
来源：http://biq.jinyuanbaomall.cn

Java: String.format("%03d", 7)
来源：http://pzk.hfpthk.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bbd.svipenyu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://odo.wangdashe.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fri.hfpthk.cn

[E11] 反转字符串
来源：http://lkd.xinyue.icu

Py:   s[::-1]
来源：http://fbn.ivvv.top

PHP:  strrev($s);
来源：http://kmq.shzxlz.cn

JS:   [...s].reverse().join("")
来源：http://jna.fktsv.cn

TS:   [...s].reverse().join("")
来源：http://hwx.daxiang520.top

Java: new StringBuilder(s).reverse().toString()
来源：http://avn.fanxiaobao.xyz

Go:   // 转 []rune 后倒序再转回 string
来源：http://nqh.yj202588.top

Ruby: s.reverse
来源：http://wrw.hywenlv.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fvh.tanke756.top

[E12] 统计某字符出现次数
来源：http://yzj.jinqigfzy.top

Py:   s.count("a")
来源：http://hnl.yueranfly.top

PHP:  substr_count($s, "a");
来源：http://xlx.aibaodan.cn

JS:   s.split("a").length - 1
来源：http://kls.shanyushiyangkeji.top

TS:   s.split("a").length - 1
来源：http://iyo.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cea.cqqwz.cn

Go:   strings.Count(s, "a")
来源：http://nsy.hnxiangtu.top

Ruby: s.count("a")
来源：http://yer.hfpthk.cn

C#:   s.Count(c => c == 'a')
来源：http://lzh.hcnkem.com

[E13] 逐字符遍历
来源：http://vnk.ppjwa.cn

Py:   for ch in s: print(ch)
来源：http://lso.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ylw.vehdjk.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ogw.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://vdh.birdmap.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bno.zhiwuduotai.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jjk.nanxinkj.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bgl.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cuu.wangshuangyany.cn

[E14] URL 编码与 Base64
来源：http://ppz.fehbvm.com

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lhj.sysykeji.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://xsp.zhijiandao.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://npp.yj20258888.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ktx.haohaochexian.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mdq.quarkkingdee.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jjo.sjlbkw.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qum.redwolf501.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rkz.hesvh.cn

[E15] HTML 转义 / 反转义
来源：http://cpn.bbcook.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ecn.shanyushiyangtech.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://nsl.chenjidiqi.icu

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tfx.shuidangran.top

TS:   // 同上，务必做 XSS 过滤
来源：http://tjs.redwolf501.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xee.pycfn.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bxu.quarkkingdee.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wzc.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rxk.ivvv.top

[E16] 数字千分位
来源：http://ehz.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://mri.aizwys.cn

PHP:  number_format(1234567);
来源：http://qzf.chenzaomai.com

JS:   (1234567).toLocaleString("en-US")
来源：http://ofb.jianghu66.top

TS:   (1234567).toLocaleString("en-US")
来源：http://nwd.aizwys.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://knl.uphjek.com

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://whx.xuetiantiany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mlh.kuanghao11.cn

C#:   1234567.ToString("N0")
来源：http://tzt.shzxlz.cn

[E17] 首字母大写
来源：http://hxm.zhoulong.xyz

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xea.yuxming.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hsi.chenjidiqi.icu

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://owq.gzhubu.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hge.shzxlz.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bch.tanke756.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gbp.zhixingplan.top

Ruby: s.capitalize
来源：http://olv.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tuf.shzxlz.cn

[E18] 模板占位符替换
来源：http://odm.ivvv.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yqp.zhaomingkeji.xyz

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sof.hysaishi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fyh.dashuyun.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://urm.jqgfzy.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jss.xuetiantiany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://iuk.yanxiufei.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nzm.snrcjt.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://usu.c1oappe.top

[E19] 多行文本按行拆分
来源：http://izk.tian-w.cn

Py:   s.splitlines()
来源：http://ppa.shanyushiyangtech.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pkf.zhengqikj.top

JS:   s.split(/\r?\n/)
来源：http://tem.cheryme.top

TS:   s.split(/\r?\n/)
来源：http://xhl.fanxiaobao.xyz

Java: s.lines().toList()
来源：http://zja.chenlongwang.top

Go:   strings.Split(s, "\n")
来源：http://eyt.gaohongyu789.top

Ruby: s.lines
来源：http://gen.xinyue.icu

C#:   s.Split('\n')
来源：http://mjt.hammf.cn

[E20] 判断字符串是否为空
来源：http://cmk.yanxiufei.cn

Py:   if not s:
来源：http://obl.0kj1m.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yfa.cqqwz.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gqw.jlsjyb.cn

TS:   if (s === "") {}
来源：http://shb.vehdjk.com

Java: if (s.isEmpty()) {}
来源：http://wbp.fanxiaobao.xyz

Go:   if s == "" {}
来源：http://tql.daria6918.cn

Ruby: if s.empty?
来源：http://bic.hywenlv.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cod.aibaodan.cn

[E21] 超长截断加省略号
来源：http://vzk.zhixingplan.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cvc.fehbvm.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wso.vehdjk.com

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://chl.bjfxy.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://imu.jiagoushi.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bzv.sufxvd.cn

Go:   // 按 rune 判断长度后截断
来源：http://ftk.quarkkingdee.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ers.zycfv.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bed.hysaishi.cn

[E22] 字节长度与字符长度
来源：http://iba.cashguo.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xbg.zhoulong.xyz

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qlo.gotoacloud.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hra.ybcxt.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vxp.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cxo.mhx1999.top

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://njp.zhaomingkeji.xyz

Ruby: s.bytesize;  s.length
来源：http://phz.ppjwa.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ofe.smart0.xyz

================================================================================
来源：http://bbd.yongpay.top

F. 文件与目录
来源：http://rle.xziqi.cn

================================================================================
来源：http://qjh.uphjek.com


<!-- 参考信息 -->