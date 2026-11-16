代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://ewf.haohaochexian.top

Go:   // 手写循环
来源：http://wfb.jlsjyb.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wxb.feifeiyinyue.top

C#:   list.Select(x => x * 2).ToList()
来源：http://xwh.yanxiufei.cn

[D15] 去重
来源：http://oks.sweek.top

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yaw.kuanghao11.cn

PHP:  array_unique($arr);
来源：http://iso.cdnleiting.top

JS:   [...new Set(arr)]
来源：http://iwa.hcnkem.com

TS:   [...new Set(arr)]
来源：http://svz.hywenlv.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qve.ivvv.top

Go:   // 用 map[T]struct{} 手写
来源：http://vgl.fktsv.cn

Ruby: arr.uniq
来源：http://gby.jinqigfzy.top

C#:   list.Distinct().ToList()
来源：http://exy.ivvv.top

[D16] 求和与平均值
来源：http://eum.shuidangran.top

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dqo.fehbvm.com

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fba.jqgufenzy.top

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://uyq.shzxlz.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://axd.guowangkeji.top

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qiz.zycfv.cn

Go:   // 手写循环累加
来源：http://tgl.nwbrower.top

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mxv.jinyuanbaomall.cn

C#:   list.Sum();  list.Average()
来源：http://qsn.hnxiangtu.top

[D17] 最大值与最小值
来源：http://ent.ctjpmb.com

Py:   max(arr);  min(arr)
来源：http://yrh.guowangkeji.top

PHP:  max($arr);  min($arr);
来源：http://mdr.quarkkingdee.top

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lue.ehwqpu.com

TS:   Math.max(...arr);
来源：http://kes.yj202588.top

Java: Collections.max(list);  Collections.min(list);
来源：http://sls.hnqzz.top

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://utr.hfpthk.cn

Ruby: arr.max;  arr.min
来源：http://jrr.sweek.top

C#:   list.Max();  list.Min()
来源：http://wbp.xuanzx.com

[D18] 扁平化嵌套数组
来源：http://eyv.guannengcc.top

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hzf.ivvv.top

PHP:  array_merge(...$nested);
来源：http://wsh.hammf.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://anw.xuanzx.com

TS:   nested.flat();
来源：http://vub.xziqi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://izu.birdmap.top

Go:   // 手写双层循环
来源：http://zzn.cheryme.top

Ruby: nested.flatten
来源：http://xbf.ywan-chungtsiang.top

C#:   nested.SelectMany(x => x).ToList()
来源：http://hru.haohaochexian.top

[D19] 按字段分组
来源：http://jdh.pengpengdd.cyou

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qsh.zhongyouzk.top

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bhr.zdbjq.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jdo.bjfxy.top

TS:   Object.groupBy(arr, x => x.type)
来源：http://doa.yongpay.top

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qcq.vqdsnc.cn

Go:   // 手写 map[string][]T
来源：http://ict.ydzc1.top

Ruby: arr.group_by { |x| x[:type] }
来源：http://tom.sysykeji.top

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ssk.sysykeji.top

[D20] 统计每个元素出现次数
来源：http://uau.gogol.net.cn

Py:   Counter(arr)
来源：http://nuu.chenzaomai.com

PHP:  array_count_values($arr);
来源：http://oqq.jinqigufen.top

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kyf.zhaomingkeji.xyz

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wuf.bbcook.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tph.9152youxi.cn

Go:   // 手写 map[T]int
来源：http://uuf.zdqjudy.top

Ruby: arr.tally
来源：http://soi.yonumen.top

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cjp.xinyue.icu

[D21] 判断是否包含某元素
来源：http://rli.zdbjq.cn

Py:   x in arr
来源：http://vuf.jinyuanbaomall.cn

PHP:  in_array($x, $arr, true);
来源：http://qpn.aibaodan.cn

JS:   arr.includes(x)
来源：http://shx.xuanzx.com

TS:   arr.includes(x)
来源：http://ywg.gotoacloud.top

Java: list.contains(x)
来源：http://agf.nwbrower.top

Go:   slices.Contains(arr, x)
来源：http://ucl.cucudq.cn

Ruby: arr.include?(x)
来源：http://rnj.chenzaomai.com

C#:   list.Contains(x)
来源：http://dby.svipenyu.cn

[D22] 复制数组（避免共享引用）
来源：http://xkp.zhiwuduotai.top

Py:   arr.copy();  arr[:];  list(arr)
来源：http://orn.uphjek.com

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vmr.jinqigufen.top

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ezf.uphjek.com

TS:   [...arr];
来源：http://yxc.hammf.cn

Java: new ArrayList<>(list);
来源：http://rhh.yueranfly.top

Go:   copied := append([]int(nil), arr...)
来源：http://myg.316326.xyz

Ruby: arr.dup;  arr.clone
来源：http://alm.chenjidiqi.icu

C#:   new List<int>(list);
来源：http://tpf.aizwys.cn

[D23] reduce 累积计算
来源：http://tdf.yangfankeji.com

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xtg.uphjek.com

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://aup.tianlin.xyz

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jxx.quarkkingdee.top

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ecs.yueranfly.top

Java: list.stream().reduce(0, Integer::sum)
来源：http://tne.pengpengdd.cyou

Go:   // 手写循环
来源：http://xjz.sweek.top

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qse.svipenyu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://evf.chenlongwang.top

[D24] 字典 / Map 基本操作
来源：http://vhh.gotoacloud.top

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iox.yangfankeji.com

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vpj.0kj1m.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jee.yuxming.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cxo.cqqwz.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ojk.guannengcc.top

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ssm.tianlin.xyz

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lzt.yongpay.top

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://sei.jinqigfzy.top

[D25] Set 集合去重与交并差
来源：http://ojb.gogol.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://eto.yonumen.top

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cbh.zhixingplan.top

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://kif.iojbl.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kej.nwbrower.top

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ypq.ybcxt.top

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vsy.zhijiandao.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bwl.gzhubu.top

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ipz.ivvv.top

[D26] 数组转字符串
来源：http://iau.zhengqikj.top

Py:   ", ".join(map(str, arr))
来源：http://srm.ctjpmb.com

PHP:  implode(", ", $arr);
来源：http://lul.cdnleiting.top

JS:   arr.join(", ")
来源：http://wmb.nwbrower.top

TS:   arr.join(", ")
来源：http://whg.fehbvm.com

Java: String.join(", ", list)
来源：http://xiz.zhongyouzk.top

Go:   strings.Join(strs, ", ")
来源：http://gig.zdbjq.cn

Ruby: arr.join(", ")
来源：http://xxk.snrcjt.cn

C#:   string.Join(", ", list)
来源：http://evy.fanxiaobao.xyz

================================================================================
来源：http://wdp.smart0.xyz

E. 字符串处理
来源：http://dzd.svipenyu.cn

================================================================================
来源：http://lcc.svipenyu.cn

[E01] 拼接字符串
来源：http://sgw.fktsv.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jyv.fanxiaobao.xyz

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cjq.gotoacloud.top

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://gdp.mhx1999.top

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kiq.xingfuxueyuan.xyz

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hkh.bjfxy.top

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mpu.xziqi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://han.tian-w.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://for.chenzaomai.com

[E02] 重复字符串
来源：http://hxb.svipenyu.cn

Py:   "ab" * 3
来源：http://yiz.tianlin.xyz

PHP:  str_repeat("ab", 3);
来源：http://ioc.jianghu66.top

JS:   "ab".repeat(3)
来源：http://hqm.feifeiyinyue.top

TS:   "ab".repeat(3)
来源：http://eps.ydzc1.top

Java: "ab".repeat(3)
来源：http://xas.xuanzx.com

Go:   strings.Repeat("ab", 3)
来源：http://esz.zhongyouzk.top

Ruby: "ab" * 3
来源：http://ovw.ctjpmb.com

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gzl.feifeiyinyue.top

[E03] 截取子串
来源：http://jxe.xuanzx.com

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rzw.cdnleiting.top

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qtt.ywan-chungtsiang.top

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wrd.tanke756.top

TS:   s.slice(1, 4)
来源：http://svh.hysaishi.cn

Java: s.substring(1, 4)
来源：http://mbr.andypj.xyz

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nqs.birdmap.top

Ruby: s[1, 3];  s[1..3]
来源：http://fli.fengsongda.top

C#:   s.Substring(1, 3)
来源：http://ezu.meibo888.top

[E04] 查找子串位置
来源：http://iai.xuetiantiany.cn

Py:   s.find("x");  s.index("x")
来源：http://ams.cqqwz.cn

PHP:  strpos($s, "x");
来源：http://rts.xziqi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://til.bbcook.cn

TS:   s.indexOf("x")
来源：http://ljp.guowangkeji.top

Java: s.indexOf("x")
来源：http://pnx.zycfv.cn

Go:   strings.Index(s, "x")
来源：http://xyy.bbcook.cn

Ruby: s.index("x")
来源：http://hui.zhengqikj.top

C#:   s.IndexOf("x")
来源：http://jin.0kj1m.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://amt.chenlongwang.top

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://vpp.dianchejie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sog.iojbl.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sux.bjfxy.top

TS:   s.includes("x");  s.startsWith("a")
来源：http://mdj.shuidangran.top

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nuf.havefunace.top

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://soz.yj20258.top

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mnu.jqgufenzy.top

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bxq.svipenyu.cn

[E06] 替换子串
来源：http://bbt.gaohongyu789.top

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mlp.zhiwuduotai.top

PHP:  str_replace("a", "b", $s);
来源：http://qkj.vehdjk.com

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sdk.yanxiufei.cn

TS:   s.replaceAll("a", "b")
来源：http://yvz.nwbrower.top

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nio.hcnkem.com

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://nax.yuanzhike.top

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vck.tian-w.cn

C#:   s.Replace("a", "b")
来源：http://hoz.xylfe.cn

[E07] 按分隔符拆分
来源：http://hor.gaohongyu789.top

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://dir.jiagoushi.top

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tmi.epnwcf.com

JS:   s.split(",");  s.split(/\s+/)
来源：http://gbk.dashuyun.cn

TS:   s.split(",")
来源：http://emv.haohaochexian.top

Java: s.split(",");  s.split("\\s+")
来源：http://mzq.hammf.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://woh.meibo888.top

Ruby: s.split(",");  s.split
来源：http://ecw.cashguo.top

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pmd.daxiang520.top

[E08] 数组按分隔符合并
来源：http://rgq.guowangkeji.top

Py:   ",".join(items)
来源：http://zfh.yj20258888.top

PHP:  implode(",", $items);
来源：http://vgo.vqdsnc.cn

JS:   items.join(",")
来源：http://pqu.fzhhl.top

TS:   items.join(",")
来源：http://qsy.nwbrower.top

Java: String.join(",", items)
来源：http://xob.yj20258.top

Go:   strings.Join(items, ",")
来源：http://udz.yuanzhike.top

Ruby: items.join(",")
来源：http://veu.redwolf501.top

C#:   string.Join(",", items)
来源：http://bex.epnwcf.com

[E09] 去除所有空白字符
来源：http://oip.nwbrower.top

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ikw.shuidangran.top

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rri.guowangkeji.top

JS:   s.replace(/\s+/g, "")
来源：http://fgn.hfpthk.cn

TS:   s.replace(/\s+/g, "")
来源：http://ral.hywenlv.cn

Java: s.replaceAll("\\s+", "")
来源：http://vwi.jinghuilouyu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://msb.sweek.top

Ruby: s.gsub(/\s+/, "")
来源：http://ktt.yuanzhike.top

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zrg.cucudq.cn

[E10] 左侧补零 / 定长填充
来源：http://ofi.quarkkingdee.top

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hxb.nwbrower.top

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://grq.yuanzhike.top

JS:   "7".padStart(3, "0")
来源：http://vki.fengsongda.top

TS:   "7".padStart(3, "0")
来源：http://qer.aizwys.cn

Java: String.format("%03d", 7)
来源：http://iid.zhixingplan.top

Go:   fmt.Sprintf("%03d", 7)
来源：http://slq.sweek.top

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://isl.tian-w.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jha.zdqjudy.top

[E11] 反转字符串
来源：http://bne.jqgufenzy.top

Py:   s[::-1]
来源：http://bbv.hesvh.cn

PHP:  strrev($s);
来源：http://lbr.pycfn.com

JS:   [...s].reverse().join("")
来源：http://due.c1oappe.top

TS:   [...s].reverse().join("")
来源：http://fvi.hysaishi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lhi.c1oappe.top

Go:   // 转 []rune 后倒序再转回 string
来源：http://sfe.shanyushiyangtech.top

Ruby: s.reverse
来源：http://bgg.hongshengwenyu.top

C#:   new string(s.Reverse().ToArray())
来源：http://chv.jqgfzy.top

[E12] 统计某字符出现次数
来源：http://egu.9152youxi.cn

Py:   s.count("a")
来源：http://cyr.chenlongwang.top

PHP:  substr_count($s, "a");
来源：http://pjt.feifeiyinyue.top

JS:   s.split("a").length - 1
来源：http://jsg.meibo888.top

TS:   s.split("a").length - 1
来源：http://lua.52xcode.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://cbr.cheryme.top

Go:   strings.Count(s, "a")
来源：http://wep.0kj1m.cn

Ruby: s.count("a")
来源：http://bll.andypj.xyz

C#:   s.Count(c => c == 'a')
来源：http://ogr.kuanghao11.cn

[E13] 逐字符遍历
来源：http://pjv.wangdashe.top

Py:   for ch in s: print(ch)
来源：http://xjk.yj20258.top

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cgs.hysaishi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sha.haohaochexian.top

TS:   for (const ch of s) { console.log(ch); }
来源：http://bio.yuxming.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fns.svipenyu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kmj.sweek.top

Ruby: s.each_char { |ch| puts ch }
来源：http://ydd.aizwys.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wfz.cqqwz.cn

[E14] URL 编码与 Base64
来源：http://abj.shanyushiyangkeji.top

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zbr.jinghuilouyu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rdw.xziqi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xke.yuanzhike.top

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zrt.iojbl.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dpm.jinqigfzy.top

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://njm.daxiang520.top

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pql.shzxlz.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hlr.yongpay.top

[E15] HTML 转义 / 反转义
来源：http://mdh.fehbvm.com

Py:   html.escape(s);  html.unescape(s)
来源：http://jru.ehwqpu.com

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vtc.ydzc1.top

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wbt.guannengcc.top

TS:   // 同上，务必做 XSS 过滤
来源：http://rhd.0kj1m.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://knb.zhiwuduotai.top

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://unq.zhixingplan.top

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://krx.xinyue.icu

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fqm.9152youxi.cn

[E16] 数字千分位
来源：http://mkq.52xcode.cn

Py:   f"{1234567:,}"
来源：http://jrw.yj20258.top

PHP:  number_format(1234567);
来源：http://nnz.jinqigfzy.top

JS:   (1234567).toLocaleString("en-US")
来源：http://lhg.zhengqikj.top

TS:   (1234567).toLocaleString("en-US")
来源：http://put.hongshengwenyu.top

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vjz.aizwys.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://opw.tanke756.top

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zhh.ivvv.top

C#:   1234567.ToString("N0")
来源：http://hcc.yuanzhike.top

[E17] 首字母大写
来源：http://akb.ybcxt.top

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fdi.cucudq.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ymz.svipenyu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dnq.shanyushiyangtech.top

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://omp.daria6918.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rei.kuanghao11.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uoa.shangyingyoupin.top

Ruby: s.capitalize
来源：http://sjl.zhongyouzk.top

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yws.gaohongyu789.top

[E18] 模板占位符替换
来源：http://axr.zhoulong.xyz

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nqu.yanxiufei.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eyn.epnwcf.com

JS:   tpl.replaceAll("{name}", name)
来源：http://rlc.gzhubu.top

TS:   tpl.replaceAll("{name}", name)
来源：http://upg.yuanzhike.top

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fmb.daxiang520.top

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://poc.yj20258.top

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ynm.zhixingplan.top

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hou.aibaodan.cn

[E19] 多行文本按行拆分
来源：http://jov.yj20258.top

Py:   s.splitlines()
来源：http://ztm.pengpengdd.cyou

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zmd.vqdsnc.cn

JS:   s.split(/\r?\n/)
来源：http://bda.bbcook.cn

TS:   s.split(/\r?\n/)
来源：http://vcf.zhengqikj.top

Java: s.lines().toList()
来源：http://oqb.cucudq.cn

Go:   strings.Split(s, "\n")
来源：http://msb.yvedp.cn

Ruby: s.lines
来源：http://kqh.smart0.xyz

C#:   s.Split('\n')
来源：http://tsk.vqdsnc.cn

[E20] 判断字符串是否为空
来源：http://zvm.hammf.cn

Py:   if not s:
来源：http://vvr.aibaodan.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yfo.yongpay.top

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mwj.vqdsnc.cn

TS:   if (s === "") {}
来源：http://svu.fengsongda.top

Java: if (s.isEmpty()) {}
来源：http://eah.yueranfly.top

Go:   if s == "" {}
来源：http://bmr.sjlbkw.cn

Ruby: if s.empty?
来源：http://drk.xingfuxueyuan.xyz

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fny.316326.xyz

[E21] 超长截断加省略号
来源：http://jbu.yuanzhike.top

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yqq.sweek.top

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nsw.redwolf501.top

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://drn.zhixingplan.top

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ksh.chenzaomai.com


<!-- 参考信息 -->