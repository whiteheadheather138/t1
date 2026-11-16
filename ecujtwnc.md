代发 wailian999

[D15] 去重
来源：http://oat.pycfn.com

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gkr.jqgufenzy.top

PHP:  array_unique($arr);
来源：http://wwx.zycfv.cn

JS:   [...new Set(arr)]
来源：http://oku.vqdsnc.cn

TS:   [...new Set(arr)]
来源：http://pyp.ivvv.top

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vjf.andypj.xyz

Go:   // 用 map[T]struct{} 手写
来源：http://wzq.iojbl.cn

Ruby: arr.uniq
来源：http://bax.cashguo.top

C#:   list.Distinct().ToList()
来源：http://uqm.9152youxi.cn

[D16] 求和与平均值
来源：http://uvh.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nki.yongpay.top

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xfe.nanxinkj.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rqr.xylfe.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://etp.hysaishi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yjy.hfpthk.cn

Go:   // 手写循环累加
来源：http://gha.jyoumei.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wql.ehwqpu.com

C#:   list.Sum();  list.Average()
来源：http://wmp.gotoacloud.top

[D17] 最大值与最小值
来源：http://hwn.gaohongyu789.top

Py:   max(arr);  min(arr)
来源：http://fhf.yj20258888.top

PHP:  max($arr);  min($arr);
来源：http://cyy.bjfxy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qqc.zhongyouzk.top

TS:   Math.max(...arr);
来源：http://zau.birdmap.top

Java: Collections.max(list);  Collections.min(list);
来源：http://pbb.hammf.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://onj.shanyushiyangtech.top

Ruby: arr.max;  arr.min
来源：http://zja.52xcode.cn

C#:   list.Max();  list.Min()
来源：http://jrn.birdmap.top

[D18] 扁平化嵌套数组
来源：http://ncm.quarkkingdee.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qri.tarul.cn

PHP:  array_merge(...$nested);
来源：http://wqc.dianchejie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tfm.zhijiandao.cn

TS:   nested.flat();
来源：http://otb.ppjwa.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jgs.jyoumei.cn

Go:   // 手写双层循环
来源：http://zsv.mhx1999.top

Ruby: nested.flatten
来源：http://jrp.daria6918.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pwd.fanxiaobao.xyz

[D19] 按字段分组
来源：http://qhj.cheryme.top

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://idb.chenzaomai.com

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mtp.52xcode.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zqu.aizwys.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gil.fktsv.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://smo.cqqwz.cn

Go:   // 手写 map[string][]T
来源：http://nrs.bjfxy.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://dbw.sufxvd.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ybn.zycfv.cn

[D20] 统计每个元素出现次数
来源：http://dvr.fzhhl.top

Py:   Counter(arr)
来源：http://wbr.xinyue.icu

PHP:  array_count_values($arr);
来源：http://oft.jlsjyb.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qwc.dianchejie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sef.hysaishi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://pdc.hywenlv.cn

Go:   // 手写 map[T]int
来源：http://mpx.yj20258.top

Ruby: arr.tally
来源：http://kfs.xziqi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pvp.ppjwa.cn

[D21] 判断是否包含某元素
来源：http://xcy.tian-w.cn

Py:   x in arr
来源：http://qcn.birdmap.top

PHP:  in_array($x, $arr, true);
来源：http://cmw.tianlin.xyz

JS:   arr.includes(x)
来源：http://uov.tianlin.xyz

TS:   arr.includes(x)
来源：http://prl.feifeiyinyue.top

Java: list.contains(x)
来源：http://dlz.smart0.xyz

Go:   slices.Contains(arr, x)
来源：http://olo.zhaomingkeji.xyz

Ruby: arr.include?(x)
来源：http://tbx.sjlbkw.cn

C#:   list.Contains(x)
来源：http://vye.sufxvd.cn

[D22] 复制数组（避免共享引用）
来源：http://tdz.zhongyouzk.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wkc.zhoulong.xyz

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://iqf.zhixingplan.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dvm.chenjidiqi.icu

TS:   [...arr];
来源：http://cgs.nanxinkj.top

Java: new ArrayList<>(list);
来源：http://kts.quarkkingdee.top

Go:   copied := append([]int(nil), arr...)
来源：http://myi.hongshengwenyu.top

Ruby: arr.dup;  arr.clone
来源：http://jqt.jinyuanbaomall.cn

C#:   new List<int>(list);
来源：http://vbj.nwbrower.top

[D23] reduce 累积计算
来源：http://zyu.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tgb.meibo888.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nun.guowangkeji.top

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eir.guannengcc.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://btc.smart0.xyz

Java: list.stream().reduce(0, Integer::sum)
来源：http://xye.chenlongwang.top

Go:   // 手写循环
来源：http://zki.fehbvm.com

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vql.mhx1999.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://cng.cashguo.top

[D24] 字典 / Map 基本操作
来源：http://nug.fengsongda.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gjr.yfazqb.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fhu.yongpay.top

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qty.jinyuanbaomall.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tht.ybcxt.top

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dow.zhixingplan.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://top.tanke756.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://iqv.shzxlz.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qrp.316326.xyz

[D25] Set 集合去重与交并差
来源：http://qlw.zdqjudy.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rml.andypj.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bbg.ivvv.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://okw.xinyue.icu

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wsn.jinqigufen.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xem.daria6918.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dyi.zycfv.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://upc.daria6918.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xvx.xuetiantiany.cn

[D26] 数组转字符串
来源：http://oys.nanxinkj.top

Py:   ", ".join(map(str, arr))
来源：http://iau.feifeiyinyue.top

PHP:  implode(", ", $arr);
来源：http://vln.jqgufenzy.top

JS:   arr.join(", ")
来源：http://cam.yueranfly.top

TS:   arr.join(", ")
来源：http://wiu.nanxuanxn.top

Java: String.join(", ", list)
来源：http://haw.jianghu66.top

Go:   strings.Join(strs, ", ")
来源：http://xem.xziqi.cn

Ruby: arr.join(", ")
来源：http://ahk.jqgufenzy.top

C#:   string.Join(", ", list)
来源：http://mwn.ppjwa.cn

================================================================================
来源：http://wzz.sysykeji.top

E. 字符串处理
来源：http://tez.52xcode.cn

================================================================================
来源：http://fgw.zhijiandao.cn

[E01] 拼接字符串
来源：http://wqu.hammf.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sqd.chenlongwang.top

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zcc.cheryme.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oir.xinyue.icu

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://asf.vehdjk.com

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zzd.yonumen.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qzu.kuanghao11.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://xyp.daria6918.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nux.yfazqb.com

[E02] 重复字符串
来源：http://bcf.hfpthk.cn

Py:   "ab" * 3
来源：http://yks.hysaishi.cn

PHP:  str_repeat("ab", 3);
来源：http://ekt.shzxlz.cn

JS:   "ab".repeat(3)
来源：http://zik.fanxiaobao.xyz

TS:   "ab".repeat(3)
来源：http://shn.daria6918.cn

Java: "ab".repeat(3)
来源：http://jww.gotoacloud.top

Go:   strings.Repeat("ab", 3)
来源：http://zad.yangfankeji.com

Ruby: "ab" * 3
来源：http://tqn.316326.xyz

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://fwm.zhongyouzk.top

[E03] 截取子串
来源：http://vnp.jianghu66.top

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ptv.tian-w.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vqq.pengpengdd.cyou

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://shg.yj202588.top

TS:   s.slice(1, 4)
来源：http://prx.52xcode.cn

Java: s.substring(1, 4)
来源：http://qpm.hcnkem.com

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bal.aibaodan.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ovy.fanxiaobao.xyz

C#:   s.Substring(1, 3)
来源：http://syi.jyoumei.cn

[E04] 查找子串位置
来源：http://nzj.haohaochexian.top

Py:   s.find("x");  s.index("x")
来源：http://tlx.guannengcc.top

PHP:  strpos($s, "x");
来源：http://uhf.shanyushiyangkeji.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bqt.yangfankeji.com

TS:   s.indexOf("x")
来源：http://yvy.yj20258.top

Java: s.indexOf("x")
来源：http://sxz.kuanghao11.cn

Go:   strings.Index(s, "x")
来源：http://hbb.fktsv.cn

Ruby: s.index("x")
来源：http://qde.wangdashe.top

C#:   s.IndexOf("x")
来源：http://gxs.9152youxi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nhk.52xcode.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ycf.yvedp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tdi.hammf.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://voy.xziqi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://whm.smart0.xyz

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://imh.snrcjt.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://aka.guowangkeji.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://csc.ybcxt.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://jeu.yj20258.top

[E06] 替换子串
来源：http://rds.cashguo.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yvz.epnwcf.com

PHP:  str_replace("a", "b", $s);
来源：http://yic.sufxvd.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vfe.gaohongyu789.top

TS:   s.replaceAll("a", "b")
来源：http://xqe.uphjek.com

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mgz.zhijiandao.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://oji.dianchejie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tmq.sysykeji.top

C#:   s.Replace("a", "b")
来源：http://erm.yongpay.top

[E07] 按分隔符拆分
来源：http://ush.wangshuangyany.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://nwp.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ptw.cashguo.top

JS:   s.split(",");  s.split(/\s+/)
来源：http://qad.uphjek.com

TS:   s.split(",")
来源：http://rux.svipenyu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://iow.snrcjt.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://law.yj20258888.top

Ruby: s.split(",");  s.split
来源：http://mcm.jiagoushi.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qpl.andypj.xyz

[E08] 数组按分隔符合并
来源：http://izq.havefunace.top

Py:   ",".join(items)
来源：http://hxg.fanxiaobao.xyz

PHP:  implode(",", $items);
来源：http://dns.svipenyu.cn

JS:   items.join(",")
来源：http://wwh.xuanzx.com

TS:   items.join(",")
来源：http://yfb.xuetiantiany.cn

Java: String.join(",", items)
来源：http://aaa.tarul.cn

Go:   strings.Join(items, ",")
来源：http://bjr.nanxinkj.top

Ruby: items.join(",")
来源：http://dzn.cqqwz.cn

C#:   string.Join(",", items)
来源：http://adr.guannengcc.top

[E09] 去除所有空白字符
来源：http://epq.bbcook.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yur.wangdashe.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ene.hnxiangtu.top

JS:   s.replace(/\s+/g, "")
来源：http://gxa.yj20258888.top

TS:   s.replace(/\s+/g, "")
来源：http://jtk.birdmap.top

Java: s.replaceAll("\\s+", "")
来源：http://hkg.sweek.top

Go:   strings.Join(strings.Fields(s), "")
来源：http://wcp.uphjek.com

Ruby: s.gsub(/\s+/, "")
来源：http://igi.jqgfzy.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rxp.svipenyu.cn

[E10] 左侧补零 / 定长填充
来源：http://ouf.hfpthk.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://uni.zhixingplan.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://pvg.andypj.xyz

JS:   "7".padStart(3, "0")
来源：http://upr.ydzc1.top

TS:   "7".padStart(3, "0")
来源：http://kzz.xylfe.cn

Java: String.format("%03d", 7)
来源：http://czr.dashuyun.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dej.jqgfzy.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nla.gaohongyu789.top

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://twf.xuetiantiany.cn

[E11] 反转字符串
来源：http://nys.kuanghao11.cn

Py:   s[::-1]
来源：http://onv.kuanghao11.cn

PHP:  strrev($s);
来源：http://wau.havefunace.top

JS:   [...s].reverse().join("")
来源：http://bhx.epnwcf.com

TS:   [...s].reverse().join("")
来源：http://lhg.xylfe.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rht.nanxuanxn.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://drr.meibo888.top

Ruby: s.reverse
来源：http://koh.aizwys.cn

C#:   new string(s.Reverse().ToArray())
来源：http://omd.sweek.top

[E12] 统计某字符出现次数
来源：http://xmz.pengpengdd.cyou

Py:   s.count("a")
来源：http://mxp.zhongyouzk.top

PHP:  substr_count($s, "a");
来源：http://bjz.yj20258.top

JS:   s.split("a").length - 1
来源：http://rig.haohaochexian.top

TS:   s.split("a").length - 1
来源：http://gcx.chenjidiqi.icu

Java: s.chars().filter(c -> c == 'a').count()
来源：http://duj.nanxuanxn.top

Go:   strings.Count(s, "a")
来源：http://sgw.gaohongyu789.top

Ruby: s.count("a")
来源：http://yqi.shanyushiyangkeji.top

C#:   s.Count(c => c == 'a')
来源：http://qct.jinyuanbaomall.cn

[E13] 逐字符遍历
来源：http://hcw.tarul.cn

Py:   for ch in s: print(ch)
来源：http://tuq.jinyuanbaomall.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ptm.guannengcc.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://box.chenzaomai.com

TS:   for (const ch of s) { console.log(ch); }
来源：http://dfo.fengsongda.top

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sxv.daria6918.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://aho.gotoacloud.top

Ruby: s.each_char { |ch| puts ch }
来源：http://orn.redwolf501.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ngq.hnxiangtu.top

[E14] URL 编码与 Base64
来源：http://viz.kuanghao11.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mkh.ydzc1.top

PHP:  urlencode($s);  base64_encode($s);
来源：http://soe.xylfe.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dbo.sufxvd.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gcb.chenjidiqi.icu

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qsh.zhijiandao.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://koj.guowangkeji.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tzv.epnwcf.com

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zti.aizwys.cn

[E15] HTML 转义 / 反转义
来源：http://usu.ehwqpu.com

Py:   html.escape(s);  html.unescape(s)
来源：http://mzk.zdbjq.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xhh.bjfxy.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uzq.birdmap.top

TS:   // 同上，务必做 XSS 过滤
来源：http://pap.zhaomingkeji.xyz

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zpg.yanxiufei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nko.yj202588.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://stm.tanke756.top

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lfk.jianghu66.top

[E16] 数字千分位
来源：http://eov.yonumen.top

Py:   f"{1234567:,}"
来源：http://rco.xuetiantiany.cn

PHP:  number_format(1234567);
来源：http://sre.yj20258888.top

JS:   (1234567).toLocaleString("en-US")
来源：http://hir.hfpthk.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jmb.cashguo.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://utl.jqgufenzy.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://iwr.jinqigufen.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://kqd.hongshengwenyu.top

C#:   1234567.ToString("N0")
来源：http://vao.shanyushiyangtech.top

[E17] 首字母大写
来源：http://vpo.jiagoushi.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blu.bjfxy.top

PHP:  ucfirst($s);  ucwords($s);
来源：http://nnb.cdnleiting.top

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oqe.cqqwz.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cxx.hesvh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ini.ydzc1.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://grj.pycfn.com

Ruby: s.capitalize
来源：http://fud.yangfankeji.com

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://axa.vqdsnc.cn

[E18] 模板占位符替换
来源：http://fwg.yueranfly.top

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dwy.hongshengwenyu.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://msf.xuetiantiany.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fzx.uphjek.com

TS:   tpl.replaceAll("{name}", name)
来源：http://vvx.aizwys.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://maz.tianlin.xyz

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gci.zhoulong.xyz

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cbj.ybcxt.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uvj.0kj1m.cn

[E19] 多行文本按行拆分
来源：http://xig.sjlbkw.cn

Py:   s.splitlines()
来源：http://ocb.guannengcc.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xyr.chenzaomai.com

JS:   s.split(/\r?\n/)
来源：http://zll.jinqigfzy.top

TS:   s.split(/\r?\n/)
来源：http://nhq.zhengqikj.top

Java: s.lines().toList()
来源：http://xht.yj202588.top

Go:   strings.Split(s, "\n")
来源：http://ayn.tanke756.top

Ruby: s.lines
来源：http://nmr.tarul.cn

C#:   s.Split('\n')
来源：http://nfk.pengpengdd.cyou

[E20] 判断字符串是否为空
来源：http://dvr.yj202588.top

Py:   if not s:
来源：http://ieq.sxryk.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://you.guowangkeji.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fxw.zdqjudy.top

TS:   if (s === "") {}
来源：http://yvm.yongpay.top

Java: if (s.isEmpty()) {}
来源：http://pga.zhixingplan.top

Go:   if s == "" {}
来源：http://xlb.jinqigufen.top

Ruby: if s.empty?
来源：http://ygr.pycfn.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://brs.cqqwz.cn

[E21] 超长截断加省略号
来源：http://fgr.jinqigufen.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lpf.epnwcf.com

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gye.gogol.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dbm.9152youxi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kgv.yj202588.top

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kyq.yueranfly.top

Go:   // 按 rune 判断长度后截断
来源：http://ort.vehdjk.com

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tak.vqdsnc.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qol.hongshengwenyu.top


<!-- 参考信息 -->