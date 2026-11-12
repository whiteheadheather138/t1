代发 wailian999

C#:   list.Distinct().ToList()
来源：http://dgg.shanyushiyangkeji.top

[D16] 求和与平均值
来源：http://pqy.pengpengdd.cyou

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dnh.hywenlv.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xkf.yuxming.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gom.fktsv.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wsk.ydzc1.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uba.guannengcc.top

Go:   // 手写循环累加
来源：http://zzs.tarul.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pin.nwbrower.top

C#:   list.Sum();  list.Average()
来源：http://gke.hnqzz.top

[D17] 最大值与最小值
来源：http://sku.gotoacloud.top

Py:   max(arr);  min(arr)
来源：http://fgd.daxiang520.top

PHP:  max($arr);  min($arr);
来源：http://ccp.jqgfzy.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fpi.cqqwz.cn

TS:   Math.max(...arr);
来源：http://lok.tanke756.top

Java: Collections.max(list);  Collections.min(list);
来源：http://bue.cucudq.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cjc.daria6918.cn

Ruby: arr.max;  arr.min
来源：http://fxx.tianlin.xyz

C#:   list.Max();  list.Min()
来源：http://ltk.yj20258.top

[D18] 扁平化嵌套数组
来源：http://fqm.meibo888.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bcw.xuetiantiany.cn

PHP:  array_merge(...$nested);
来源：http://mip.birdmap.top

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hcd.yfazqb.com

TS:   nested.flat();
来源：http://dku.xuetiantiany.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://tnx.daxiang520.top

Go:   // 手写双层循环
来源：http://kja.snrcjt.cn

Ruby: nested.flatten
来源：http://pau.fehbvm.com

C#:   nested.SelectMany(x => x).ToList()
来源：http://zzx.sweek.top

[D19] 按字段分组
来源：http://hse.bbcook.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xkx.cdnleiting.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ebk.ywan-chungtsiang.top

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ojx.yangfankeji.com

TS:   Object.groupBy(arr, x => x.type)
来源：http://hwc.jinqigfzy.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hiz.uphjek.com

Go:   // 手写 map[string][]T
来源：http://gxy.xuetiantiany.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cvm.cucudq.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oeo.ctjpmb.com

[D20] 统计每个元素出现次数
来源：http://fla.jiagoushi.top

Py:   Counter(arr)
来源：http://fcn.meibo888.top

PHP:  array_count_values($arr);
来源：http://ivr.haohaochexian.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://chd.kuanghao11.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dbc.jiagoushi.top

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://igw.dashuyun.cn

Go:   // 手写 map[T]int
来源：http://mrz.jinghuilouyu.cn

Ruby: arr.tally
来源：http://pzm.cashguo.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vob.jianghu66.top

[D21] 判断是否包含某元素
来源：http://lbn.yongpay.top

Py:   x in arr
来源：http://tli.gotoacloud.top

PHP:  in_array($x, $arr, true);
来源：http://hvy.shuidangran.top

JS:   arr.includes(x)
来源：http://ieb.hesvh.cn

TS:   arr.includes(x)
来源：http://xbl.jlsjyb.cn

Java: list.contains(x)
来源：http://lck.birdmap.top

Go:   slices.Contains(arr, x)
来源：http://wqb.gzhubu.top

Ruby: arr.include?(x)
来源：http://scj.fktsv.cn

C#:   list.Contains(x)
来源：http://tsa.ctjpmb.com

[D22] 复制数组（避免共享引用）
来源：http://xem.zhengqikj.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://dvg.ehwqpu.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uzi.hywenlv.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zod.tianlin.xyz

TS:   [...arr];
来源：http://xlm.jinghuilouyu.cn

Java: new ArrayList<>(list);
来源：http://uwb.aizwys.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jla.dashuyun.cn

Ruby: arr.dup;  arr.clone
来源：http://hac.yangfankeji.com

C#:   new List<int>(list);
来源：http://mrg.fengsongda.top

[D23] reduce 累积计算
来源：http://pgv.xuanzx.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lcw.bjfxy.top

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://csm.hesvh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aan.jiagoushi.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://giz.uphjek.com

Java: list.stream().reduce(0, Integer::sum)
来源：http://zal.jlsjyb.cn

Go:   // 手写循环
来源：http://bko.guowangkeji.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://azz.jiagoushi.top

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://lum.zycfv.cn

[D24] 字典 / Map 基本操作
来源：http://wtz.nanxinkj.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rvd.zhijiandao.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ifd.fktsv.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://yhi.jiagoushi.top

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cwx.fehbvm.com

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://sum.yangfankeji.com

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kcb.jqgufenzy.top

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://muz.nwbrower.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kgo.yj20258.top

[D25] Set 集合去重与交并差
来源：http://jsa.ivvv.top

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fmf.xingfuxueyuan.xyz

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://los.haohaochexian.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://oav.cqqwz.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lsm.bbcook.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://alm.fzhhl.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tsf.zhoulong.xyz

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uty.hnqzz.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qjb.hesvh.cn

[D26] 数组转字符串
来源：http://gxy.hysaishi.cn

Py:   ", ".join(map(str, arr))
来源：http://ryf.yonumen.top

PHP:  implode(", ", $arr);
来源：http://hkc.nanxuanxn.top

JS:   arr.join(", ")
来源：http://htz.gaohongyu789.top

TS:   arr.join(", ")
来源：http://wta.guowangkeji.top

Java: String.join(", ", list)
来源：http://kiy.shanyushiyangkeji.top

Go:   strings.Join(strs, ", ")
来源：http://oua.tarul.cn

Ruby: arr.join(", ")
来源：http://boa.xuetiantiany.cn

C#:   string.Join(", ", list)
来源：http://ods.daxiang520.top

================================================================================
来源：http://gkk.quarkkingdee.top

E. 字符串处理
来源：http://zpm.yanxiufei.cn

================================================================================
来源：http://tqi.cdnleiting.top

[E01] 拼接字符串
来源：http://hgn.hnqzz.top

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://srh.dashuyun.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ndf.c1oappe.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zby.daria6918.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gkz.jiagoushi.top

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fpx.0kj1m.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cco.yueranfly.top

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ofc.zhengqikj.top

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dbp.hnqzz.top

[E02] 重复字符串
来源：http://dxn.fzhhl.top

Py:   "ab" * 3
来源：http://xxa.yongpay.top

PHP:  str_repeat("ab", 3);
来源：http://wts.dianchejie.cn

JS:   "ab".repeat(3)
来源：http://puw.hcnkem.com

TS:   "ab".repeat(3)
来源：http://pbq.ydzc1.top

Java: "ab".repeat(3)
来源：http://hjv.zdbjq.cn

Go:   strings.Repeat("ab", 3)
来源：http://hmb.fktsv.cn

Ruby: "ab" * 3
来源：http://ltn.cheryme.top

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rxm.zhijiandao.cn

[E03] 截取子串
来源：http://vaw.hesvh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bnz.hfpthk.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gzv.fktsv.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://clc.zhijiandao.cn

TS:   s.slice(1, 4)
来源：http://cns.jinqigfzy.top

Java: s.substring(1, 4)
来源：http://gyk.cucudq.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://tsf.ehwqpu.com

Ruby: s[1, 3];  s[1..3]
来源：http://okj.ydjk.org.cn

C#:   s.Substring(1, 3)
来源：http://tzy.guannengcc.top

[E04] 查找子串位置
来源：http://cvl.iojbl.cn

Py:   s.find("x");  s.index("x")
来源：http://poq.zdbjq.cn

PHP:  strpos($s, "x");
来源：http://kek.jqgufenzy.top

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bat.snrcjt.cn

TS:   s.indexOf("x")
来源：http://yzj.ppjwa.cn

Java: s.indexOf("x")
来源：http://dip.gaohongyu789.top

Go:   strings.Index(s, "x")
来源：http://wed.cheryme.top

Ruby: s.index("x")
来源：http://hhb.cdnleiting.top

C#:   s.IndexOf("x")
来源：http://skb.aizwys.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://yyo.yj20258888.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ufg.9152youxi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eth.sjlbkw.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybr.hnxiangtu.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://gec.vqdsnc.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ybv.zhongyouzk.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bfe.nanxinkj.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://uzk.birdmap.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gcf.haohaochexian.top

[E06] 替换子串
来源：http://pso.hammf.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://iap.chenlongwang.top

PHP:  str_replace("a", "b", $s);
来源：http://qhi.zhongyouzk.top

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zuw.snrcjt.cn

TS:   s.replaceAll("a", "b")
来源：http://gfx.zhoulong.xyz

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lum.ywan-chungtsiang.top

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wrf.feifeiyinyue.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rvq.yfazqb.com

C#:   s.Replace("a", "b")
来源：http://gou.ydzc1.top

[E07] 按分隔符拆分
来源：http://vjm.chenjidiqi.icu

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://erg.snrcjt.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wuw.shzxlz.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dlu.sysykeji.top

TS:   s.split(",")
来源：http://omp.zdbjq.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bpb.bjfxy.top

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://oxi.hnqzz.top

Ruby: s.split(",");  s.split
来源：http://ckk.cucudq.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://itj.zhengqikj.top

[E08] 数组按分隔符合并
来源：http://jjn.xylfe.cn

Py:   ",".join(items)
来源：http://sme.vqdsnc.cn

PHP:  implode(",", $items);
来源：http://ynt.bbcook.cn

JS:   items.join(",")
来源：http://azb.dianchejie.cn

TS:   items.join(",")
来源：http://meq.shanyushiyangtech.top

Java: String.join(",", items)
来源：http://aoz.yfazqb.com

Go:   strings.Join(items, ",")
来源：http://cyi.daxiang520.top

Ruby: items.join(",")
来源：http://nxz.shuidangran.top

C#:   string.Join(",", items)
来源：http://yrg.tarul.cn

[E09] 去除所有空白字符
来源：http://vri.cashguo.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wlk.hnxiangtu.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://owk.vehdjk.com

JS:   s.replace(/\s+/g, "")
来源：http://luj.ctjpmb.com

TS:   s.replace(/\s+/g, "")
来源：http://ljv.fehbvm.com

Java: s.replaceAll("\\s+", "")
来源：http://pnx.cucudq.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qgy.fehbvm.com

Ruby: s.gsub(/\s+/, "")
来源：http://ibh.dianchejie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sfd.xziqi.cn

[E10] 左侧补零 / 定长填充
来源：http://alj.kuanghao11.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://kcy.ywan-chungtsiang.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://moy.sweek.top

JS:   "7".padStart(3, "0")
来源：http://xje.yongpay.top

TS:   "7".padStart(3, "0")
来源：http://vhn.zycfv.cn

Java: String.format("%03d", 7)
来源：http://fbc.nanxinkj.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://kya.aizwys.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://oke.dashuyun.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://efr.jlsjyb.cn

[E11] 反转字符串
来源：http://sdc.ybcxt.top

Py:   s[::-1]
来源：http://xyz.zhaomingkeji.xyz

PHP:  strrev($s);
来源：http://pef.xinyue.icu

JS:   [...s].reverse().join("")
来源：http://pyn.iojbl.cn

TS:   [...s].reverse().join("")
来源：http://lgb.cheryme.top

Java: new StringBuilder(s).reverse().toString()
来源：http://suj.shzxlz.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mmc.tianlin.xyz

Ruby: s.reverse
来源：http://zgl.fengsongda.top

C#:   new string(s.Reverse().ToArray())
来源：http://omo.sweek.top

[E12] 统计某字符出现次数
来源：http://cqt.wangdashe.top

Py:   s.count("a")
来源：http://urx.aibaodan.cn

PHP:  substr_count($s, "a");
来源：http://hbz.wangshuangyany.cn

JS:   s.split("a").length - 1
来源：http://dvv.yonumen.top

TS:   s.split("a").length - 1
来源：http://tcb.shuidangran.top

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ojb.zhongyouzk.top

Go:   strings.Count(s, "a")
来源：http://rom.yj20258888.top

Ruby: s.count("a")
来源：http://pdp.fzhhl.top

C#:   s.Count(c => c == 'a')
来源：http://fzb.dianchejie.cn

[E13] 逐字符遍历
来源：http://glp.chenzaomai.com

Py:   for ch in s: print(ch)
来源：http://afp.nwbrower.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dgv.fzhhl.top

JS:   for (const ch of s) { console.log(ch); }
来源：http://zej.fanxiaobao.xyz

TS:   for (const ch of s) { console.log(ch); }
来源：http://wyp.andypj.xyz

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xbl.dianchejie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pkj.yj20258888.top

Ruby: s.each_char { |ch| puts ch }
来源：http://sjd.sysykeji.top

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kbf.jyoumei.cn

[E14] URL 编码与 Base64
来源：http://stn.wangdashe.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qdp.xylfe.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://epr.yj20258.top

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kce.fehbvm.com

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uhg.daxiang520.top

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wyp.snrcjt.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ikv.shuidangran.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ohn.birdmap.top

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://yjy.xinyue.icu

[E15] HTML 转义 / 反转义
来源：http://kyh.cqqwz.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ioy.shzxlz.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kuu.yuxming.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hyy.gaohongyu789.top

TS:   // 同上，务必做 XSS 过滤
来源：http://ctb.daria6918.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bpe.jyoumei.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fyk.fengsongda.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iyl.pengpengdd.cyou

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mol.fengsongda.top

[E16] 数字千分位
来源：http://umf.yanxiufei.cn

Py:   f"{1234567:,}"
来源：http://knv.hcnkem.com

PHP:  number_format(1234567);
来源：http://rji.cqqwz.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vim.jinqigfzy.top

TS:   (1234567).toLocaleString("en-US")
来源：http://elf.dashuyun.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jib.cheryme.top

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wup.vqdsnc.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hqy.hcnkem.com

C#:   1234567.ToString("N0")
来源：http://zff.gaohongyu789.top

[E17] 首字母大写
来源：http://btq.hfpthk.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bbp.yvedp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qgw.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qii.zhongyouzk.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://umy.c1oappe.top

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://czu.guowangkeji.top

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hns.mhx1999.top

Ruby: s.capitalize
来源：http://pwj.feifeiyinyue.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xwf.meibo888.top

[E18] 模板占位符替换
来源：http://rkl.sjlbkw.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://lrf.jqgfzy.top

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://fch.yvedp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://myj.pycfn.com

TS:   tpl.replaceAll("{name}", name)
来源：http://dxf.cucudq.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xej.gotoacloud.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sqa.jlsjyb.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pok.hesvh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://svf.zhengqikj.top

[E19] 多行文本按行拆分
来源：http://uzs.sjlbkw.cn

Py:   s.splitlines()
来源：http://ebz.hnqzz.top

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://iry.cashguo.top

JS:   s.split(/\r?\n/)
来源：http://jwu.snrcjt.cn

TS:   s.split(/\r?\n/)
来源：http://kzx.shuidangran.top

Java: s.lines().toList()
来源：http://pmi.ywan-chungtsiang.top

Go:   strings.Split(s, "\n")
来源：http://izg.sufxvd.cn

Ruby: s.lines
来源：http://pzk.svipenyu.cn

C#:   s.Split('\n')
来源：http://hhb.xingfuxueyuan.xyz

[E20] 判断字符串是否为空
来源：http://enj.smart0.xyz

Py:   if not s:
来源：http://cxs.cucudq.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jlm.epnwcf.com

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hmi.fengsongda.top

TS:   if (s === "") {}
来源：http://xib.jqgufenzy.top

Java: if (s.isEmpty()) {}
来源：http://ape.gaohongyu789.top

Go:   if s == "" {}
来源：http://uyq.gaohongyu789.top

Ruby: if s.empty?
来源：http://oki.uphjek.com

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oux.xingfuxueyuan.xyz

[E21] 超长截断加省略号
来源：http://nqd.zdqjudy.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ufw.bjfxy.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jqk.shanyushiyangkeji.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rrf.pengpengdd.cyou

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uzy.svipenyu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zlx.bjfxy.top

Go:   // 按 rune 判断长度后截断
来源：http://hkw.hongshengwenyu.top

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tkt.hongshengwenyu.top

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wjs.hywenlv.cn

[E22] 字节长度与字符长度
来源：http://awy.sjlbkw.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ioz.tian-w.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jav.bjfxy.top

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qov.jinqigufen.top

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gmn.redwolf501.top

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://avf.yangfankeji.com

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kat.yanxiufei.cn

Ruby: s.bytesize;  s.length
来源：http://sht.yj20258.top


<!-- 参考信息 -->