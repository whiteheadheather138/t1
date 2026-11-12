代发 wailian999

TS:   [...new Set(arr)]
来源：http://phs.guannengcc.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zmz.9152youxi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ybb.hammf.cn

Ruby: arr.uniq
来源：http://nnq.yj202588.top

C#:   list.Distinct().ToList()
来源：http://xbn.kuanghao11.cn

[D16] 求和与平均值
来源：http://kto.hcnkem.com

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wwr.snrcjt.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yvr.52xcode.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fbq.iojbl.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fei.aibaodan.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wcr.quarkkingdee.top

Go:   // 手写循环累加
来源：http://reh.jinyuanbaomall.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vro.zhijiandao.cn

C#:   list.Sum();  list.Average()
来源：http://dkm.daria6918.cn

[D17] 最大值与最小值
来源：http://lph.hcnkem.com

Py:   max(arr);  min(arr)
来源：http://fbr.ctjpmb.com

PHP:  max($arr);  min($arr);
来源：http://yfq.52xcode.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pit.hfpthk.cn

TS:   Math.max(...arr);
来源：http://ttf.dianchejie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://khd.c1oappe.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mzl.zhengqikj.top

Ruby: arr.max;  arr.min
来源：http://les.zdbjq.cn

C#:   list.Max();  list.Min()
来源：http://hgf.zycfv.cn

[D18] 扁平化嵌套数组
来源：http://tfs.ydzc1.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jdw.xziqi.cn

PHP:  array_merge(...$nested);
来源：http://mrm.316326.xyz

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zff.sysykeji.top

TS:   nested.flat();
来源：http://lwu.zhoulong.xyz

Java: nested.stream().flatMap(List::stream).toList()
来源：http://noe.cdnleiting.top

Go:   // 手写双层循环
来源：http://cfe.hnqzz.top

Ruby: nested.flatten
来源：http://ryx.jinqigfzy.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://diu.sweek.top

[D19] 按字段分组
来源：http://hyc.tanke756.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nxh.havefunace.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vze.jinghuilouyu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fwe.gotoacloud.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://lzl.dianchejie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nyk.tianlin.xyz

Go:   // 手写 map[string][]T
来源：http://qtt.sweek.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://ldr.jlsjyb.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gon.gogol.net.cn

[D20] 统计每个元素出现次数
来源：http://pwb.birdmap.top

Py:   Counter(arr)
来源：http://wbk.xingfuxueyuan.xyz

PHP:  array_count_values($arr);
来源：http://til.ppjwa.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://avf.chenjidiqi.icu

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qhf.tianlin.xyz

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://qmj.zhengqikj.top

Go:   // 手写 map[T]int
来源：http://pqw.pengpengdd.cyou

Ruby: arr.tally
来源：http://fbx.zdbjq.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wsw.hongshengwenyu.top

[D21] 判断是否包含某元素
来源：http://mpb.vehdjk.com

Py:   x in arr
来源：http://pie.iojbl.cn

PHP:  in_array($x, $arr, true);
来源：http://qgd.andypj.xyz

JS:   arr.includes(x)
来源：http://bli.ivvv.top

TS:   arr.includes(x)
来源：http://wbx.fktsv.cn

Java: list.contains(x)
来源：http://irf.chenzaomai.com

Go:   slices.Contains(arr, x)
来源：http://jdw.fengsongda.top

Ruby: arr.include?(x)
来源：http://ugj.wangdashe.top

C#:   list.Contains(x)
来源：http://zbv.yanxiufei.cn

[D22] 复制数组（避免共享引用）
来源：http://lqg.tianlin.xyz

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wpz.zhengqikj.top

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ghm.daxiang520.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://rgx.daxiang520.top

TS:   [...arr];
来源：http://kcg.chenzaomai.com

Java: new ArrayList<>(list);
来源：http://frg.jinqigufen.top

Go:   copied := append([]int(nil), arr...)
来源：http://cjb.gzhubu.top

Ruby: arr.dup;  arr.clone
来源：http://qox.yongpay.top

C#:   new List<int>(list);
来源：http://hkz.zhixingplan.top

[D23] reduce 累积计算
来源：http://nve.fehbvm.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hgy.ydzc1.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ikr.yj20258888.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uyr.smart0.xyz

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bza.pycfn.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://etx.chenzaomai.com

Go:   // 手写循环
来源：http://tky.xuetiantiany.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://onl.ydzc1.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://arc.yongpay.top

[D24] 字典 / Map 基本操作
来源：http://elj.daria6918.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fqx.zdqjudy.top

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://byt.gogol.net.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xjn.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oif.tianlin.xyz

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wrq.sysykeji.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qri.hnxiangtu.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cnz.nanxinkj.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://nci.shanyushiyangkeji.top

[D25] Set 集合去重与交并差
来源：http://bpr.yanxiufei.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dzn.zycfv.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xet.yj20258.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kjh.aibaodan.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fcc.chenzaomai.com

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://cvs.jiagoushi.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zgx.svipenyu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://iuc.cheryme.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sjo.havefunace.top

[D26] 数组转字符串
来源：http://eqy.ydzc1.top

Py:   ", ".join(map(str, arr))
来源：http://hkx.vehdjk.com

PHP:  implode(", ", $arr);
来源：http://qsk.ivvv.top

JS:   arr.join(", ")
来源：http://kkt.xinyue.icu

TS:   arr.join(", ")
来源：http://wzc.sxryk.cn

Java: String.join(", ", list)
来源：http://rml.nwbrower.top

Go:   strings.Join(strs, ", ")
来源：http://ysx.yj20258888.top

Ruby: arr.join(", ")
来源：http://uwq.guannengcc.top

C#:   string.Join(", ", list)
来源：http://wfl.gzhubu.top

================================================================================
来源：http://urb.ivvv.top

E. 字符串处理
来源：http://bng.ctjpmb.com

================================================================================
来源：http://dvj.zhixingplan.top

[E01] 拼接字符串
来源：http://icd.jinqigufen.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://loi.nanxuanxn.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bea.shzxlz.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cpp.ppjwa.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baq.sjlbkw.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jbc.svipenyu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://muz.dashuyun.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cur.quarkkingdee.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qhx.smart0.xyz

[E02] 重复字符串
来源：http://ytx.yonumen.top

Py:   "ab" * 3
来源：http://xlq.yuxming.cn

PHP:  str_repeat("ab", 3);
来源：http://eke.sysykeji.top

JS:   "ab".repeat(3)
来源：http://izg.ivvv.top

TS:   "ab".repeat(3)
来源：http://ocb.gotoacloud.top

Java: "ab".repeat(3)
来源：http://ixr.cqqwz.cn

Go:   strings.Repeat("ab", 3)
来源：http://sdr.52xcode.cn

Ruby: "ab" * 3
来源：http://chr.tarul.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://boc.iojbl.cn

[E03] 截取子串
来源：http://eur.guannengcc.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ogv.jinyuanbaomall.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jfk.guannengcc.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mxo.daria6918.cn

TS:   s.slice(1, 4)
来源：http://wgx.jqgfzy.top

Java: s.substring(1, 4)
来源：http://jci.zhiwuduotai.top

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bpj.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://ykj.chenjidiqi.icu

C#:   s.Substring(1, 3)
来源：http://hro.redwolf501.top

[E04] 查找子串位置
来源：http://ogy.daria6918.cn

Py:   s.find("x");  s.index("x")
来源：http://pvp.yuxming.cn

PHP:  strpos($s, "x");
来源：http://ehx.hcnkem.com

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vdg.pengpengdd.cyou

TS:   s.indexOf("x")
来源：http://kux.guowangkeji.top

Java: s.indexOf("x")
来源：http://cag.ywan-chungtsiang.top

Go:   strings.Index(s, "x")
来源：http://iya.epnwcf.com

Ruby: s.index("x")
来源：http://bvu.snrcjt.cn

C#:   s.IndexOf("x")
来源：http://esk.kuanghao11.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://uls.gogol.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ftp.xuetiantiany.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mwq.zhoulong.xyz

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mmv.mhx1999.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://bhi.sufxvd.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sxo.jinghuilouyu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fta.yangfankeji.com

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://cbq.pycfn.com

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wcy.birdmap.top

[E06] 替换子串
来源：http://psh.andypj.xyz

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://enn.sufxvd.cn

PHP:  str_replace("a", "b", $s);
来源：http://sdc.jiagoushi.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mav.jianghu66.top

TS:   s.replaceAll("a", "b")
来源：http://eaf.ydzc1.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wno.uphjek.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mqu.pycfn.com

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bdr.cqqwz.cn

C#:   s.Replace("a", "b")
来源：http://pnm.xuetiantiany.cn

[E07] 按分隔符拆分
来源：http://mbn.cheryme.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://clb.yongpay.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hzu.zhixingplan.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://mfn.epnwcf.com

TS:   s.split(",")
来源：http://odn.chenlongwang.top

Java: s.split(",");  s.split("\\s+")
来源：http://dig.0kj1m.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://brb.chenzaomai.com

Ruby: s.split(",");  s.split
来源：http://lsj.ybcxt.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mwv.zhaomingkeji.xyz

[E08] 数组按分隔符合并
来源：http://dqx.hongshengwenyu.top

Py:   ",".join(items)
来源：http://hdn.shzxlz.cn

PHP:  implode(",", $items);
来源：http://kli.tanke756.top

JS:   items.join(",")
来源：http://dgy.wangshuangyany.cn

TS:   items.join(",")
来源：http://kat.yueranfly.top

Java: String.join(",", items)
来源：http://uxv.jinqigfzy.top

Go:   strings.Join(items, ",")
来源：http://ucz.shuidangran.top

Ruby: items.join(",")
来源：http://ciz.tianlin.xyz

C#:   string.Join(",", items)
来源：http://mgl.pycfn.com

[E09] 去除所有空白字符
来源：http://ufg.fehbvm.com

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vou.vehdjk.com

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zls.sxryk.cn

JS:   s.replace(/\s+/g, "")
来源：http://mna.sysykeji.top

TS:   s.replace(/\s+/g, "")
来源：http://cks.9152youxi.cn

Java: s.replaceAll("\\s+", "")
来源：http://mbv.zdqjudy.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://ucq.shanyushiyangtech.top

Ruby: s.gsub(/\s+/, "")
来源：http://kqm.fengsongda.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://usc.tian-w.cn

[E10] 左侧补零 / 定长填充
来源：http://zop.xingfuxueyuan.xyz

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xzb.yvedp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pbh.yangfankeji.com

JS:   "7".padStart(3, "0")
来源：http://mlj.haohaochexian.top

TS:   "7".padStart(3, "0")
来源：http://mqq.havefunace.top

Java: String.format("%03d", 7)
来源：http://upf.aibaodan.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sfh.yfazqb.com

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kxh.xuanzx.com

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rib.chenjidiqi.icu

[E11] 反转字符串
来源：http://lzh.fehbvm.com

Py:   s[::-1]
来源：http://hqs.nanxinkj.top

PHP:  strrev($s);
来源：http://yqd.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://jhq.zycfv.cn

TS:   [...s].reverse().join("")
来源：http://wha.ctjpmb.com

Java: new StringBuilder(s).reverse().toString()
来源：http://fmz.chenjidiqi.icu

Go:   // 转 []rune 后倒序再转回 string
来源：http://pgg.kuanghao11.cn

Ruby: s.reverse
来源：http://mko.hcnkem.com

C#:   new string(s.Reverse().ToArray())
来源：http://xic.bjfxy.top

[E12] 统计某字符出现次数
来源：http://wbq.iojbl.cn

Py:   s.count("a")
来源：http://jxs.xylfe.cn

PHP:  substr_count($s, "a");
来源：http://kfj.bbcook.cn

JS:   s.split("a").length - 1
来源：http://xda.ydzc1.top

TS:   s.split("a").length - 1
来源：http://jnw.jinqigufen.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://erk.hongshengwenyu.top

Go:   strings.Count(s, "a")
来源：http://deh.yvedp.cn

Ruby: s.count("a")
来源：http://hvn.snrcjt.cn

C#:   s.Count(c => c == 'a')
来源：http://kcb.sufxvd.cn

[E13] 逐字符遍历
来源：http://oeh.epnwcf.com

Py:   for ch in s: print(ch)
来源：http://lce.yj20258888.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://vor.birdmap.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://vyc.yj20258888.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://qau.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://amw.sjlbkw.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kxz.hnqzz.top

Ruby: s.each_char { |ch| puts ch }
来源：http://iff.chenjidiqi.icu

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gkb.yueranfly.top

[E14] URL 编码与 Base64
来源：http://qwk.dianchejie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://djn.pengpengdd.cyou

PHP:  urlencode($s);  base64_encode($s);
来源：http://qbz.jinqigufen.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ppx.vehdjk.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mtr.nwbrower.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yar.zhixingplan.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yhf.ehwqpu.com

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lge.yj20258888.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ovc.52xcode.cn

[E15] HTML 转义 / 反转义
来源：http://vjm.sweek.top

Py:   html.escape(s);  html.unescape(s)
来源：http://oyp.shuidangran.top

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hfj.yangfankeji.com

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pnh.hywenlv.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vbk.52xcode.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://kte.chenzaomai.com

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bst.cdnleiting.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://asu.hesvh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qay.jinqigfzy.top

[E16] 数字千分位
来源：http://wqo.zycfv.cn

Py:   f"{1234567:,}"
来源：http://jsr.zdbjq.cn

PHP:  number_format(1234567);
来源：http://wle.sxryk.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jwx.xylfe.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xda.havefunace.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iue.cdnleiting.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iru.wangshuangyany.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qlq.yvedp.cn

C#:   1234567.ToString("N0")
来源：http://uqb.hfpthk.cn

[E17] 首字母大写
来源：http://nkp.xuetiantiany.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tcj.zhijiandao.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fni.jlsjyb.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ajq.pycfn.com

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zsq.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dma.ydjk.org.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xka.jinqigfzy.top

Ruby: s.capitalize
来源：http://zmf.jinghuilouyu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lte.yanxiufei.cn

[E18] 模板占位符替换
来源：http://gui.cheryme.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aiy.0kj1m.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nmv.snrcjt.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sml.yuxming.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dyg.kuanghao11.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xyv.daria6918.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kjo.wangdashe.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fhh.mhx1999.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://odn.yongpay.top

[E19] 多行文本按行拆分
来源：http://iba.daria6918.cn

Py:   s.splitlines()
来源：http://smd.andypj.xyz

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fsy.yonumen.top

JS:   s.split(/\r?\n/)
来源：http://mgy.xylfe.cn

TS:   s.split(/\r?\n/)
来源：http://nck.smart0.xyz

Java: s.lines().toList()
来源：http://zen.xingfuxueyuan.xyz

Go:   strings.Split(s, "\n")
来源：http://gti.ivvv.top

Ruby: s.lines
来源：http://fjh.zdqjudy.top

C#:   s.Split('\n')
来源：http://gsr.hfpthk.cn

[E20] 判断字符串是否为空
来源：http://mkg.ybcxt.top

Py:   if not s:
来源：http://jcz.meibo888.top

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://peh.fanxiaobao.xyz

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jwr.fehbvm.com

TS:   if (s === "") {}
来源：http://zma.tianlin.xyz

Java: if (s.isEmpty()) {}
来源：http://uem.chenzaomai.com

Go:   if s == "" {}
来源：http://enk.sxryk.cn

Ruby: if s.empty?
来源：http://olm.ydzc1.top

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kox.c1oappe.top

[E21] 超长截断加省略号
来源：http://mfw.shanyushiyangkeji.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dsk.yj20258.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bbx.daxiang520.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eci.yongpay.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pgi.cdnleiting.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://emz.jqgufenzy.top

Go:   // 按 rune 判断长度后截断
来源：http://zhi.zhoulong.xyz

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://utq.yuanzhike.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gbx.hfpthk.cn

[E22] 字节长度与字符长度
来源：http://dim.shanyushiyangkeji.top

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zkk.aibaodan.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgx.cashguo.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://vzu.sweek.top


<!-- 参考信息 -->