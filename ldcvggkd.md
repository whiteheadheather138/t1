代发 wailian999

TS:   [...new Set(arr)]
来源：http://gbo.fengsongda.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vmc.havefunace.top

Go:   // 用 map[T]struct{} 手写
来源：http://bby.birdmap.top

Ruby: arr.uniq
来源：http://usf.9152youxi.cn

C#:   list.Distinct().ToList()
来源：http://rdj.chenjidiqi.icu

[D16] 求和与平均值
来源：http://jls.epnwcf.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://rwh.bjfxy.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bhw.zhixingplan.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ckq.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://chj.tianlin.xyz

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yum.cucudq.cn

Go:   // 手写循环累加
来源：http://aue.svipenyu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nao.uphjek.com

C#:   list.Sum();  list.Average()
来源：http://sta.hysaishi.cn

[D17] 最大值与最小值
来源：http://zfy.zhoulong.xyz

Py:   max(arr);  min(arr)
来源：http://kwz.sjlbkw.cn

PHP:  max($arr);  min($arr);
来源：http://off.nanxuanxn.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xbp.zhixingplan.top

TS:   Math.max(...arr);
来源：http://eee.fengsongda.top

Java: Collections.max(list);  Collections.min(list);
来源：http://ewh.pengpengdd.cyou

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jpo.jinyuanbaomall.cn

Ruby: arr.max;  arr.min
来源：http://isd.hongshengwenyu.top

C#:   list.Max();  list.Min()
来源：http://bou.shanyushiyangkeji.top

[D18] 扁平化嵌套数组
来源：http://nkn.chenlongwang.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bkw.jinyuanbaomall.cn

PHP:  array_merge(...$nested);
来源：http://jdu.xuanzx.com

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tbt.zdqjudy.top

TS:   nested.flat();
来源：http://btx.hysaishi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ypg.xuanzx.com

Go:   // 手写双层循环
来源：http://tew.vehdjk.com

Ruby: nested.flatten
来源：http://pwb.kuanghao11.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sow.sxryk.cn

[D19] 按字段分组
来源：http://fis.xuanzx.com

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ele.zdqjudy.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yvy.c1oappe.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://bvl.aibaodan.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uyw.hnqzz.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zre.yj20258888.top

Go:   // 手写 map[string][]T
来源：http://raq.yonumen.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://axc.yj20258.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sxp.bbcook.cn

[D20] 统计每个元素出现次数
来源：http://fvi.yfazqb.com

Py:   Counter(arr)
来源：http://uoy.yvedp.cn

PHP:  array_count_values($arr);
来源：http://jaq.zycfv.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ocg.quarkkingdee.top

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fgu.vehdjk.com

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xfm.chenjidiqi.icu

Go:   // 手写 map[T]int
来源：http://naj.jianghu66.top

Ruby: arr.tally
来源：http://ruh.quarkkingdee.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kmm.hywenlv.cn

[D21] 判断是否包含某元素
来源：http://abh.jlsjyb.cn

Py:   x in arr
来源：http://raj.gzhubu.top

PHP:  in_array($x, $arr, true);
来源：http://ggp.bbcook.cn

JS:   arr.includes(x)
来源：http://wkx.fzhhl.top

TS:   arr.includes(x)
来源：http://jne.sjlbkw.cn

Java: list.contains(x)
来源：http://cwg.shuidangran.top

Go:   slices.Contains(arr, x)
来源：http://pgg.zdqjudy.top

Ruby: arr.include?(x)
来源：http://ubs.dashuyun.cn

C#:   list.Contains(x)
来源：http://cpc.yj20258888.top

[D22] 复制数组（避免共享引用）
来源：http://esa.jqgfzy.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qvc.gotoacloud.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dbg.pycfn.com

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://teg.vehdjk.com

TS:   [...arr];
来源：http://cue.jinqigfzy.top

Java: new ArrayList<>(list);
来源：http://shb.ydzc1.top

Go:   copied := append([]int(nil), arr...)
来源：http://scn.guowangkeji.top

Ruby: arr.dup;  arr.clone
来源：http://bxe.jianghu66.top

C#:   new List<int>(list);
来源：http://dln.gogol.net.cn

[D23] reduce 累积计算
来源：http://fjl.nanxinkj.top

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bhc.gogol.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yal.mhx1999.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://skv.pengpengdd.cyou

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yhb.hysaishi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://maj.chenzaomai.com

Go:   // 手写循环
来源：http://fnu.sjlbkw.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hhc.pycfn.com

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xwu.fehbvm.com

[D24] 字典 / Map 基本操作
来源：http://erx.jinqigufen.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vqq.vqdsnc.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ljg.hammf.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lqw.xylfe.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://swn.dianchejie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kum.nanxinkj.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bim.snrcjt.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wyg.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://uep.yonumen.top

[D25] Set 集合去重与交并差
来源：http://pjp.fktsv.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://nfk.aizwys.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hkj.gotoacloud.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bha.chenzaomai.com

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ery.xingfuxueyuan.xyz

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://whl.smart0.xyz

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ssb.yj20258888.top

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tnd.dianchejie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jyy.cqqwz.cn

[D26] 数组转字符串
来源：http://gie.jqgufenzy.top

Py:   ", ".join(map(str, arr))
来源：http://kqj.birdmap.top

PHP:  implode(", ", $arr);
来源：http://lcp.iojbl.cn

JS:   arr.join(", ")
来源：http://psf.jinyuanbaomall.cn

TS:   arr.join(", ")
来源：http://vfm.chenzaomai.com

Java: String.join(", ", list)
来源：http://lsr.uphjek.com

Go:   strings.Join(strs, ", ")
来源：http://icd.jinqigfzy.top

Ruby: arr.join(", ")
来源：http://atr.yueranfly.top

C#:   string.Join(", ", list)
来源：http://gtf.chenjidiqi.icu

================================================================================
来源：http://xdd.iojbl.cn

E. 字符串处理
来源：http://ddh.mhx1999.top

================================================================================
来源：http://jma.svipenyu.cn

[E01] 拼接字符串
来源：http://nwp.wangshuangyany.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://efb.jiagoushi.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lbr.jqgufenzy.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://rdo.yj202588.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hfq.zhoulong.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://tfc.shangyingyoupin.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qwr.ivvv.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://srq.tarul.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://zsm.epnwcf.com

[E02] 重复字符串
来源：http://bzt.shanyushiyangtech.top

Py:   "ab" * 3
来源：http://wxa.zhongyouzk.top

PHP:  str_repeat("ab", 3);
来源：http://onc.hcnkem.com

JS:   "ab".repeat(3)
来源：http://umm.yfazqb.com

TS:   "ab".repeat(3)
来源：http://ndd.wangdashe.top

Java: "ab".repeat(3)
来源：http://kxz.nanxinkj.top

Go:   strings.Repeat("ab", 3)
来源：http://zxj.yongpay.top

Ruby: "ab" * 3
来源：http://hsu.xylfe.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rfl.9152youxi.cn

[E03] 截取子串
来源：http://utb.daria6918.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zva.yj20258888.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://evr.yuxming.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fdn.shuidangran.top

TS:   s.slice(1, 4)
来源：http://rjn.jianghu66.top

Java: s.substring(1, 4)
来源：http://rjr.yj20258.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nns.pycfn.com

Ruby: s[1, 3];  s[1..3]
来源：http://blv.ctjpmb.com

C#:   s.Substring(1, 3)
来源：http://pmr.jinyuanbaomall.cn

[E04] 查找子串位置
来源：http://xvw.ywan-chungtsiang.top

Py:   s.find("x");  s.index("x")
来源：http://hyk.yonumen.top

PHP:  strpos($s, "x");
来源：http://avr.hnxiangtu.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yku.daria6918.cn

TS:   s.indexOf("x")
来源：http://npx.jqgufenzy.top

Java: s.indexOf("x")
来源：http://djp.zdbjq.cn

Go:   strings.Index(s, "x")
来源：http://apr.yj20258.top

Ruby: s.index("x")
来源：http://fmi.zhiwuduotai.top

C#:   s.IndexOf("x")
来源：http://gqb.birdmap.top

[E05] 判断包含 / 前缀 / 后缀
来源：http://wgp.uphjek.com

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bhx.zhixingplan.top

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kdu.xziqi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ztk.ywan-chungtsiang.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://awb.fzhhl.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ivo.smart0.xyz

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ihh.vehdjk.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dqn.shuidangran.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dcj.ctjpmb.com

[E06] 替换子串
来源：http://fho.sweek.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://oiv.zhoulong.xyz

PHP:  str_replace("a", "b", $s);
来源：http://dqv.hcnkem.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fxi.tian-w.cn

TS:   s.replaceAll("a", "b")
来源：http://vbc.dianchejie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hoe.epnwcf.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vgy.jinqigfzy.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pka.sufxvd.cn

C#:   s.Replace("a", "b")
来源：http://euw.sweek.top

[E07] 按分隔符拆分
来源：http://gjx.fanxiaobao.xyz

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://onp.zhixingplan.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xpb.havefunace.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://ktq.kuanghao11.cn

TS:   s.split(",")
来源：http://pcg.smart0.xyz

Java: s.split(",");  s.split("\\s+")
来源：http://jbz.cucudq.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xzk.0kj1m.cn

Ruby: s.split(",");  s.split
来源：http://fkk.yangfankeji.com

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://isd.aibaodan.cn

[E08] 数组按分隔符合并
来源：http://but.cashguo.top

Py:   ",".join(items)
来源：http://ljl.epnwcf.com

PHP:  implode(",", $items);
来源：http://rkh.guannengcc.top

JS:   items.join(",")
来源：http://pee.gzhubu.top

TS:   items.join(",")
来源：http://vbb.aibaodan.cn

Java: String.join(",", items)
来源：http://pie.shzxlz.cn

Go:   strings.Join(items, ",")
来源：http://pmc.yuanzhike.top

Ruby: items.join(",")
来源：http://wyr.fzhhl.top

C#:   string.Join(",", items)
来源：http://jyw.xuanzx.com

[E09] 去除所有空白字符
来源：http://hmf.quarkkingdee.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ufl.dashuyun.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rjc.zycfv.cn

JS:   s.replace(/\s+/g, "")
来源：http://xuq.jinyuanbaomall.cn

TS:   s.replace(/\s+/g, "")
来源：http://fxa.zhengqikj.top

Java: s.replaceAll("\\s+", "")
来源：http://nxu.mhx1999.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://qdj.hammf.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ojl.hesvh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lej.pycfn.com

[E10] 左侧补零 / 定长填充
来源：http://pjw.sufxvd.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qwr.shuidangran.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mck.cdnleiting.top

JS:   "7".padStart(3, "0")
来源：http://vtw.cucudq.cn

TS:   "7".padStart(3, "0")
来源：http://crk.nwbrower.top

Java: String.format("%03d", 7)
来源：http://szk.kuanghao11.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zcq.kuanghao11.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oym.havefunace.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ied.mhx1999.top

[E11] 反转字符串
来源：http://eed.sxryk.cn

Py:   s[::-1]
来源：http://wgu.shuidangran.top

PHP:  strrev($s);
来源：http://nuc.hongshengwenyu.top

JS:   [...s].reverse().join("")
来源：http://opw.hammf.cn

TS:   [...s].reverse().join("")
来源：http://voo.sysykeji.top

Java: new StringBuilder(s).reverse().toString()
来源：http://ezu.jiagoushi.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://yzy.zhiwuduotai.top

Ruby: s.reverse
来源：http://aml.yanxiufei.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lis.hesvh.cn

[E12] 统计某字符出现次数
来源：http://nmw.birdmap.top

Py:   s.count("a")
来源：http://wqr.xinyue.icu

PHP:  substr_count($s, "a");
来源：http://cmf.shanyushiyangkeji.top

JS:   s.split("a").length - 1
来源：http://ccx.hnxiangtu.top

TS:   s.split("a").length - 1
来源：http://hra.sufxvd.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wqa.smart0.xyz

Go:   strings.Count(s, "a")
来源：http://rrm.havefunace.top

Ruby: s.count("a")
来源：http://sah.jyoumei.cn

C#:   s.Count(c => c == 'a')
来源：http://obq.9152youxi.cn

[E13] 逐字符遍历
来源：http://soy.ehwqpu.com

Py:   for ch in s: print(ch)
来源：http://gel.ybcxt.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fad.chenjidiqi.icu

JS:   for (const ch of s) { console.log(ch); }
来源：http://uax.xylfe.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://jul.chenjidiqi.icu

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jsi.hywenlv.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wtg.xinyue.icu

Ruby: s.each_char { |ch| puts ch }
来源：http://mxl.jinyuanbaomall.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xsa.nanxinkj.top

[E14] URL 编码与 Base64
来源：http://tws.feifeiyinyue.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kxq.zhixingplan.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://rmz.zhengqikj.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://iam.birdmap.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pio.zdbjq.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://txh.xinyue.icu

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xez.tian-w.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fzl.hnxiangtu.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fnr.ywan-chungtsiang.top

[E15] HTML 转义 / 反转义
来源：http://ulu.yfazqb.com

Py:   html.escape(s);  html.unescape(s)
来源：http://yek.yonumen.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kbd.sweek.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cci.pycfn.com

TS:   // 同上，务必做 XSS 过滤
来源：http://zmy.uphjek.com

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qli.haohaochexian.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hnq.yonumen.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nwx.shangyingyoupin.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bay.jiagoushi.top

[E16] 数字千分位
来源：http://mnp.yj20258.top

Py:   f"{1234567:,}"
来源：http://mmb.jinyuanbaomall.cn

PHP:  number_format(1234567);
来源：http://ich.andypj.xyz

JS:   (1234567).toLocaleString("en-US")
来源：http://dov.andypj.xyz

TS:   (1234567).toLocaleString("en-US")
来源：http://mng.chenlongwang.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mjw.gzhubu.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wqf.yvedp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aaq.nanxinkj.top

C#:   1234567.ToString("N0")
来源：http://vyc.xziqi.cn

[E17] 首字母大写
来源：http://foh.tian-w.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gsj.ppjwa.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dns.zhijiandao.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cce.xinyue.icu

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yfs.jinghuilouyu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zgc.tianlin.xyz

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sop.fanxiaobao.xyz

Ruby: s.capitalize
来源：http://ale.tarul.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rsv.fehbvm.com

[E18] 模板占位符替换
来源：http://hha.jianghu66.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lka.jinghuilouyu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mev.hnxiangtu.top

JS:   tpl.replaceAll("{name}", name)
来源：http://xxw.chenjidiqi.icu

TS:   tpl.replaceAll("{name}", name)
来源：http://jov.52xcode.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wfb.havefunace.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mdr.hcnkem.com

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tmi.shzxlz.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rrv.cqqwz.cn

[E19] 多行文本按行拆分
来源：http://rsk.chenjidiqi.icu

Py:   s.splitlines()
来源：http://wyy.hysaishi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wwm.guowangkeji.top

JS:   s.split(/\r?\n/)
来源：http://ohi.birdmap.top

TS:   s.split(/\r?\n/)
来源：http://kvp.vehdjk.com

Java: s.lines().toList()
来源：http://yum.sweek.top

Go:   strings.Split(s, "\n")
来源：http://bmh.hysaishi.cn

Ruby: s.lines
来源：http://cyn.zhaomingkeji.xyz

C#:   s.Split('\n')
来源：http://rvd.cqqwz.cn

[E20] 判断字符串是否为空
来源：http://efc.xuanzx.com

Py:   if not s:
来源：http://uvc.zhongyouzk.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tcq.sweek.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nqd.haohaochexian.top

TS:   if (s === "") {}
来源：http://olt.zhiwuduotai.top

Java: if (s.isEmpty()) {}
来源：http://ofp.havefunace.top

Go:   if s == "" {}
来源：http://dvb.bbcook.cn

Ruby: if s.empty?
来源：http://fhh.feifeiyinyue.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bof.jinghuilouyu.cn

[E21] 超长截断加省略号
来源：http://qcz.sxryk.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tof.iojbl.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kin.zhijiandao.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oec.guannengcc.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lax.bjfxy.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fnb.shuidangran.top

Go:   // 按 rune 判断长度后截断
来源：http://yua.ybcxt.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tcf.hnxiangtu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://syc.yj20258.top

[E22] 字节长度与字符长度
来源：http://rtl.shangyingyoupin.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zrd.ppjwa.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtd.yanxiufei.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gvg.quarkkingdee.top


<!-- 参考信息 -->