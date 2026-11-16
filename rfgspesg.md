代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cim.zhaomingkeji.xyz

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://atm.chenlongwang.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yvb.zhongyouzk.top

Go:   // 手写循环累加
来源：http://vzz.vqdsnc.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rxd.jqgfzy.top

C#:   list.Sum();  list.Average()
来源：http://yct.hcnkem.com

[D17] 最大值与最小值
来源：http://yuo.chenzaomai.com

Py:   max(arr);  min(arr)
来源：http://bxf.aibaodan.cn

PHP:  max($arr);  min($arr);
来源：http://yae.zhengqikj.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hbr.yj20258.top

TS:   Math.max(...arr);
来源：http://tvm.sweek.top

Java: Collections.max(list);  Collections.min(list);
来源：http://gcp.zhoulong.xyz

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dmr.hywenlv.cn

Ruby: arr.max;  arr.min
来源：http://mui.jianghu66.top

C#:   list.Max();  list.Min()
来源：http://pdv.mhx1999.top

[D18] 扁平化嵌套数组
来源：http://ims.snrcjt.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://met.nanxuanxn.top

PHP:  array_merge(...$nested);
来源：http://ucc.zycfv.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rph.hfpthk.cn

TS:   nested.flat();
来源：http://urc.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://afz.yonumen.top

Go:   // 手写双层循环
来源：http://map.wangshuangyany.cn

Ruby: nested.flatten
来源：http://xja.yueranfly.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://sud.fanxiaobao.xyz

[D19] 按字段分组
来源：http://rgs.yuanzhike.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://afy.guowangkeji.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tfs.hongshengwenyu.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aji.ybcxt.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://qdp.xuanzx.com

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ssp.havefunace.top

Go:   // 手写 map[string][]T
来源：http://gul.yvedp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://zyg.ehwqpu.com

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fpx.epnwcf.com

[D20] 统计每个元素出现次数
来源：http://ttb.sufxvd.cn

Py:   Counter(arr)
来源：http://rzt.jqgufenzy.top

PHP:  array_count_values($arr);
来源：http://ilr.birdmap.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://klb.cashguo.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hie.shuidangran.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gem.yonumen.top

Go:   // 手写 map[T]int
来源：http://bqd.zhiwuduotai.top

Ruby: arr.tally
来源：http://rzt.guowangkeji.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://skl.wangdashe.top

[D21] 判断是否包含某元素
来源：http://nac.ehwqpu.com

Py:   x in arr
来源：http://zfj.hongshengwenyu.top

PHP:  in_array($x, $arr, true);
来源：http://lqs.pycfn.com

JS:   arr.includes(x)
来源：http://bhn.hnxiangtu.top

TS:   arr.includes(x)
来源：http://zvc.sxryk.cn

Java: list.contains(x)
来源：http://hgt.c1oappe.top

Go:   slices.Contains(arr, x)
来源：http://pvp.fzhhl.top

Ruby: arr.include?(x)
来源：http://ede.jlsjyb.cn

C#:   list.Contains(x)
来源：http://pmd.hnqzz.top

[D22] 复制数组（避免共享引用）
来源：http://rwf.gogol.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tar.hcnkem.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://rnp.nanxuanxn.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rmy.cqqwz.cn

TS:   [...arr];
来源：http://zjo.ydjk.org.cn

Java: new ArrayList<>(list);
来源：http://ibm.feifeiyinyue.top

Go:   copied := append([]int(nil), arr...)
来源：http://kjk.shangyingyoupin.top

Ruby: arr.dup;  arr.clone
来源：http://lqw.yfazqb.com

C#:   new List<int>(list);
来源：http://wmp.havefunace.top

[D23] reduce 累积计算
来源：http://yyb.smart0.xyz

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://uqu.fktsv.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jug.yj202588.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yfd.hysaishi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xhf.andypj.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://qta.mhx1999.top

Go:   // 手写循环
来源：http://zls.chenjidiqi.icu

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kyu.chenjidiqi.icu

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://dvs.jyoumei.cn

[D24] 字典 / Map 基本操作
来源：http://nej.xuanzx.com

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bjv.kuanghao11.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vxs.fehbvm.com

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://pty.aibaodan.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hnt.havefunace.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lpb.zhoulong.xyz

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gsn.yuanzhike.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wob.iojbl.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wrh.quarkkingdee.top

[D25] Set 集合去重与交并差
来源：http://wfs.jyoumei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xdx.tanke756.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lsq.zdbjq.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vrb.yj20258888.top

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vwo.tarul.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vxb.zhengqikj.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://acc.xinyue.icu

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tgh.vehdjk.com

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wqm.feifeiyinyue.top

[D26] 数组转字符串
来源：http://mxs.hesvh.cn

Py:   ", ".join(map(str, arr))
来源：http://plp.zhoulong.xyz

PHP:  implode(", ", $arr);
来源：http://ekh.hongshengwenyu.top

JS:   arr.join(", ")
来源：http://uww.meibo888.top

TS:   arr.join(", ")
来源：http://hiz.shzxlz.cn

Java: String.join(", ", list)
来源：http://rpn.snrcjt.cn

Go:   strings.Join(strs, ", ")
来源：http://edu.dashuyun.cn

Ruby: arr.join(", ")
来源：http://wjt.xylfe.cn

C#:   string.Join(", ", list)
来源：http://xim.gaohongyu789.top

================================================================================
来源：http://jkb.fengsongda.top

E. 字符串处理
来源：http://eri.ydzc1.top

================================================================================
来源：http://bel.shangyingyoupin.top

[E01] 拼接字符串
来源：http://zpz.gogol.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jdx.jqgufenzy.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fvg.dianchejie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://nwm.jiagoushi.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://duf.zhiwuduotai.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://iiu.fehbvm.com

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cuc.ywan-chungtsiang.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dmz.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://uid.tarul.cn

[E02] 重复字符串
来源：http://cpt.zdbjq.cn

Py:   "ab" * 3
来源：http://gdd.chenzaomai.com

PHP:  str_repeat("ab", 3);
来源：http://bew.ctjpmb.com

JS:   "ab".repeat(3)
来源：http://vin.guannengcc.top

TS:   "ab".repeat(3)
来源：http://hho.shanyushiyangkeji.top

Java: "ab".repeat(3)
来源：http://nlr.fzhhl.top

Go:   strings.Repeat("ab", 3)
来源：http://feu.yj20258888.top

Ruby: "ab" * 3
来源：http://cgz.nanxuanxn.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jmc.zhiwuduotai.top

[E03] 截取子串
来源：http://aip.ivvv.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dkp.yueranfly.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xyq.andypj.xyz

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nkk.yueranfly.top

TS:   s.slice(1, 4)
来源：http://ihh.feifeiyinyue.top

Java: s.substring(1, 4)
来源：http://sfo.haohaochexian.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tiy.ydjk.org.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xej.c1oappe.top

C#:   s.Substring(1, 3)
来源：http://tvb.wangshuangyany.cn

[E04] 查找子串位置
来源：http://zfr.ydjk.org.cn

Py:   s.find("x");  s.index("x")
来源：http://mmc.shanyushiyangtech.top

PHP:  strpos($s, "x");
来源：http://ioy.haohaochexian.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hzn.mhx1999.top

TS:   s.indexOf("x")
来源：http://tuj.yongpay.top

Java: s.indexOf("x")
来源：http://moo.zhaomingkeji.xyz

Go:   strings.Index(s, "x")
来源：http://ack.fanxiaobao.xyz

Ruby: s.index("x")
来源：http://ndz.hfpthk.cn

C#:   s.IndexOf("x")
来源：http://ozt.fzhhl.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://gjw.nanxuanxn.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gqq.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hhk.yj20258888.top

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nzb.zycfv.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://zpm.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qmz.shuidangran.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://efc.shangyingyoupin.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bnz.ydjk.org.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://iij.yonumen.top

[E06] 替换子串
来源：http://vqr.cucudq.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rba.cashguo.top

PHP:  str_replace("a", "b", $s);
来源：http://cae.fehbvm.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ndp.daxiang520.top

TS:   s.replaceAll("a", "b")
来源：http://hfv.fehbvm.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ibk.birdmap.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ndk.nwbrower.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://giq.xuanzx.com

C#:   s.Replace("a", "b")
来源：http://zwl.ivvv.top

[E07] 按分隔符拆分
来源：http://qgy.hywenlv.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://rle.kuanghao11.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://imq.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://umj.fanxiaobao.xyz

TS:   s.split(",")
来源：http://bpz.jianghu66.top

Java: s.split(",");  s.split("\\s+")
来源：http://wuh.ybcxt.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ext.zhiwuduotai.top

Ruby: s.split(",");  s.split
来源：http://wki.zhiwuduotai.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lol.jianghu66.top

[E08] 数组按分隔符合并
来源：http://dir.yonumen.top

Py:   ",".join(items)
来源：http://who.nanxuanxn.top

PHP:  implode(",", $items);
来源：http://ulh.zhongyouzk.top

JS:   items.join(",")
来源：http://gbb.nanxuanxn.top

TS:   items.join(",")
来源：http://vtw.shangyingyoupin.top

Java: String.join(",", items)
来源：http://ojs.sweek.top

Go:   strings.Join(items, ",")
来源：http://jdd.hammf.cn

Ruby: items.join(",")
来源：http://afg.yuxming.cn

C#:   string.Join(",", items)
来源：http://iox.0kj1m.cn

[E09] 去除所有空白字符
来源：http://uop.birdmap.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jgq.hcnkem.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fzf.yongpay.top

JS:   s.replace(/\s+/g, "")
来源：http://izs.zdbjq.cn

TS:   s.replace(/\s+/g, "")
来源：http://cie.shangyingyoupin.top

Java: s.replaceAll("\\s+", "")
来源：http://edf.zhixingplan.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://kco.tanke756.top

Ruby: s.gsub(/\s+/, "")
来源：http://jys.wangdashe.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oqu.hongshengwenyu.top

[E10] 左侧补零 / 定长填充
来源：http://nrh.yfazqb.com

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nby.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nge.zhiwuduotai.top

JS:   "7".padStart(3, "0")
来源：http://jxw.jlsjyb.cn

TS:   "7".padStart(3, "0")
来源：http://vko.uphjek.com

Java: String.format("%03d", 7)
来源：http://ujc.meibo888.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://sjb.jianghu66.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vkp.nanxuanxn.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ndo.andypj.xyz

[E11] 反转字符串
来源：http://rod.hfpthk.cn

Py:   s[::-1]
来源：http://npy.zhengqikj.top

PHP:  strrev($s);
来源：http://ltf.sxryk.cn

JS:   [...s].reverse().join("")
来源：http://ilq.ywan-chungtsiang.top

TS:   [...s].reverse().join("")
来源：http://jtn.jiagoushi.top

Java: new StringBuilder(s).reverse().toString()
来源：http://bpz.bjfxy.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://iqp.jinqigufen.top

Ruby: s.reverse
来源：http://fbl.cheryme.top

C#:   new string(s.Reverse().ToArray())
来源：http://akv.bjfxy.top

[E12] 统计某字符出现次数
来源：http://cys.vehdjk.com

Py:   s.count("a")
来源：http://gzf.smart0.xyz

PHP:  substr_count($s, "a");
来源：http://wxr.jiagoushi.top

JS:   s.split("a").length - 1
来源：http://khi.fzhhl.top

TS:   s.split("a").length - 1
来源：http://axx.tianlin.xyz

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gzh.cdnleiting.top

Go:   strings.Count(s, "a")
来源：http://egj.316326.xyz

Ruby: s.count("a")
来源：http://ali.cqqwz.cn

C#:   s.Count(c => c == 'a')
来源：http://fmt.hfpthk.cn

[E13] 逐字符遍历
来源：http://qzy.cucudq.cn

Py:   for ch in s: print(ch)
来源：http://nbz.xuanzx.com

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://esi.yangfankeji.com

JS:   for (const ch of s) { console.log(ch); }
来源：http://ksg.zhoulong.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://gve.ybcxt.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://awv.zhongyouzk.top

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wil.jqgufenzy.top

Ruby: s.each_char { |ch| puts ch }
来源：http://bqy.sufxvd.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jvf.svipenyu.cn

[E14] URL 编码与 Base64
来源：http://zpj.yj20258888.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gdy.yj20258888.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://tet.havefunace.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yay.hammf.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vot.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yng.yvedp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gjv.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fea.sxryk.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bht.zhixingplan.top

[E15] HTML 转义 / 反转义
来源：http://drv.havefunace.top

Py:   html.escape(s);  html.unescape(s)
来源：http://mhe.jianghu66.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uzn.cdnleiting.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vfx.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://vvf.zdqjudy.top

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mtd.fanxiaobao.xyz

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://dqw.epnwcf.com

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tmx.zhengqikj.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gyr.gotoacloud.top

[E16] 数字千分位
来源：http://yic.gotoacloud.top

Py:   f"{1234567:,}"
来源：http://suv.yonumen.top

PHP:  number_format(1234567);
来源：http://nmv.9152youxi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vfd.sufxvd.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xox.52xcode.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cos.tarul.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wgo.yanxiufei.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zen.shanyushiyangkeji.top

C#:   1234567.ToString("N0")
来源：http://iho.jqgufenzy.top

[E17] 首字母大写
来源：http://wdy.hnqzz.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hmb.gaohongyu789.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://xsg.daria6918.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xgs.haohaochexian.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://onj.kuanghao11.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vxj.fzhhl.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ycg.yvedp.cn

Ruby: s.capitalize
来源：http://tvw.gotoacloud.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zte.guowangkeji.top

[E18] 模板占位符替换
来源：http://owx.svipenyu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wbq.svipenyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cvw.tarul.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hqv.xuetiantiany.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jqo.c1oappe.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dmu.wangshuangyany.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hnd.cashguo.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lbp.shuidangran.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://iop.chenjidiqi.icu

[E19] 多行文本按行拆分
来源：http://jlz.ivvv.top

Py:   s.splitlines()
来源：http://ykm.ppjwa.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dws.yfazqb.com

JS:   s.split(/\r?\n/)
来源：http://bkp.guannengcc.top

TS:   s.split(/\r?\n/)
来源：http://ldv.shzxlz.cn

Java: s.lines().toList()
来源：http://hag.jinghuilouyu.cn

Go:   strings.Split(s, "\n")
来源：http://iuk.cucudq.cn

Ruby: s.lines
来源：http://hya.pengpengdd.cyou

C#:   s.Split('\n')
来源：http://kao.cucudq.cn

[E20] 判断字符串是否为空
来源：http://ddj.ppjwa.cn

Py:   if not s:
来源：http://xck.guowangkeji.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eql.jinqigfzy.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://oxy.jianghu66.top

TS:   if (s === "") {}
来源：http://pjm.cqqwz.cn

Java: if (s.isEmpty()) {}
来源：http://rjp.hnqzz.top

Go:   if s == "" {}
来源：http://ybb.52xcode.cn

Ruby: if s.empty?
来源：http://oac.cheryme.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ejv.gaohongyu789.top

[E21] 超长截断加省略号
来源：http://nmd.nanxuanxn.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://zjg.shanyushiyangkeji.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zpk.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dhy.gotoacloud.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zdj.9152youxi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://njk.ivvv.top

Go:   // 按 rune 判断长度后截断
来源：http://ile.yuxming.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://itj.hesvh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jbh.xinyue.icu

[E22] 字节长度与字符长度
来源：http://vzt.ydzc1.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hpz.birdmap.top

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sua.gzhubu.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jsw.xylfe.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bss.hnxiangtu.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hiw.316326.xyz

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qlk.hfpthk.cn

Ruby: s.bytesize;  s.length
来源：http://rfh.cdnleiting.top

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ryr.fanxiaobao.xyz

================================================================================
来源：http://xnd.chenlongwang.top

F. 文件与目录
来源：http://vkq.jyoumei.cn

================================================================================
来源：http://ote.yvedp.cn


<!-- 参考信息 -->